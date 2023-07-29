# Comparing `tmp/pypus-1.2.0.tar.gz` & `tmp/pypus-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypus-1.2.0.tar", max compression
+gzip compressed data, was "pypus-1.3.0.tar", max compression
```

## Comparing `pypus-1.2.0.tar` & `pypus-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.2.0/LICENSE
--rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.2.0/README.md
--rw-r--r--   0        0        0      511 2023-05-08 16:57:22.101016 pypus-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.2.0/src/pypus/__init__.py
--rw-r--r--   0        0        0    23328 2023-05-08 16:55:48.132893 pypus-1.2.0/src/pypus/cli.py
--rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 pypus-1.2.0/setup.py
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 pypus-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.3.0/LICENSE
+-rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.3.0/README.md
+-rw-r--r--   0        0        0      569 2023-07-29 16:34:00.874249 pypus-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.3.0/src/pypus/__init__.py
+-rw-r--r--   0        0        0    24713 2023-07-29 16:33:09.561695 pypus-1.3.0/src/pypus/cli.py
+-rw-r--r--   0        0        0      392 2023-07-28 22:05:17.330425 pypus-1.3.0/src/pypus/shelf.py
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypus-1.3.0/PKG-INFO
```

### Comparing `pypus-1.2.0/LICENSE` & `pypus-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypus-1.2.0/src/pypus/cli.py` & `pypus-1.3.0/src/pypus/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Core module with cli """
 import click
 import json
 import os
 import requests
+from pypus import shelf
 from termcolor import cprint
 from pprint import pprint
 from requests.api import get, head
 from urllib3.exceptions import InsecureRequestWarning
 # Suppress only the single warning from urllib3 needed.
 requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
 # Set `verify=False` on `requests.post`.
@@ -19,14 +20,23 @@
     """
     Pypus is a cli tool for making changes to Octopus Deploy\n
     Set the following environment variables\n
     OCTOPUS_API_KEY = 'API-YOURAPIKEY'\n
     OCTOPUS_SERVER_URI = 'https://my-octopus-server.com/api'
 
     Example Usage: pypus get-projects Default
+
+    Variable set examples \n
+    Example with scope: \n
+    pypus set-var SQLDBA SSIS_BONDDB test test1 \\
+            '{"Environment":["Environments-90"]}'
+
+    Example without scope: \n
+    pypus set-var SQLDBA SSIS_BONDDB test1 test2 '{}'
+
     """
 
 @main.command('check-env', short_help='Check required environment variables')
 def check_env():
     """ Prints out the current necessary environment variables """
     octopus_api_key = os.getenv('OCTOPUS_API_KEY')
     octopus_server_uri = os.getenv('OCTOPUS_SERVER_URI')
@@ -69,14 +79,15 @@
     space = get_by_name('{0}/spaces/all'.format(octopus_server_uri), space_name)
     machines = get_octopus_resource('{0}/{1}/machines/all'.format(octopus_server_uri, space['Id']))
     print(f"The space {space_name} has these machines in it")
     for i in machines:
         print(f"Machine {i['Name']} has an ID of {i['Id']} and is assigned to these {i['Roles']} roles.")
     return machines
 
+
 @main.command('get-spaces', short_help='Get a list of spaces for server')
 def get_spaces():
     octopus_api_key = os.getenv('OCTOPUS_API_KEY')
     octopus_server_uri = os.getenv('OCTOPUS_SERVER_URI')
     headers = {'X-Octopus-ApiKey': octopus_api_key}
     def get_octopus_resource(uri, headers, skip_count = 0):
         """ Gets a resource from the API
@@ -104,14 +115,25 @@
     uri = '{0}/spaces'.format(octopus_server_uri)
     spaces = get_octopus_resource(uri, headers)
     for i in spaces:
         print(f"Space {i['Name']} has an ID of {i['Id']}")
     return spaces
 
 
+@main.command('add-vars-toshelf', short_help='Parse json object and store variables')
+@click.argument('json-file', type=click.Path(exists=True))
+def add_vars_toshelf(json_file):
+    filename = str(json_file)
+    filename = filename.split('.', 1)[0]
+    with open(json_file) as f:
+        data = json.load(f)
+        shelf.shelf_add_item(filename, 'Variables', data['Variables'])
+        shelf.shelf_add_item(filename, 'ScopeValues', data['ScopeValues'])
+
+
 @main.command('get-vars', short_help='Get a list of vars for a project in a space')
 @click.argument("space")
 @click.argument("project")
 def get_vars(space, project):
     """ Get a list of vars for a project within a space
 
     Arguments:
@@ -165,26 +187,30 @@
 
 
 @main.command('set-var', short_help='Set a variable for a project in a space')
 @click.argument("space")
 @click.argument("project")
 @click.argument("variable-name")
 @click.argument("variable-value")
+@click.argument("variable-scope")
 @click.option('--sensitive', is_flag=True)
-def set_var(space, project, variable_name, variable_value, sensitive):
+def set_var(space, project, variable_name, variable_value, variable_scope, sensitive):
     """ Set a variable for a project in a space
 
     Arguments:
         space: The space where the project resides
         project: The project where the variable is created
         variable-name: The name of the variable
         variable-value: The value to set for the variable
+        scope-values: A list of key value pairs
         sensitive: Set this flag for passwords
 
         note: Only string variable types are currently supported
+
+        Example: pypus set-var SQLDBA SSIS_BONDDB test test1 '{"Environment":["Environments-90"]}'
     """
     def get_octopus_resource(uri, headers, skip_count = 0):
         """ Gets a resource from the API
 
         Arguments:
             uri: The base url of the Octopus Deploy API
         """
@@ -207,40 +233,46 @@
         # return results
         return items
     octopus_api_key = os.getenv('OCTOPUS_API_KEY')
     octopus_server_uri = os.getenv('OCTOPUS_SERVER_URI')
     headers = {'X-Octopus-ApiKey': octopus_api_key}
     project_name = project
     space_name = space
+    variable_scope = json.loads(variable_scope)
     variable = {
             'Name': variable_name,
             'Value': variable_value,
             'Type': 'String',
+            'Scope': variable_scope,
             'IsSensitive': sensitive
     }
     uri = '{0}/spaces'.format(octopus_server_uri)
     spaces = get_octopus_resource(uri, headers)
     space = next((x for x in spaces if x['Name'] == space_name), None)
     uri = '{0}/{1}/projects'.format(octopus_server_uri, space['Id'])
     projects = get_octopus_resource(uri, headers)
     project = next((x for x in projects if x['Name'] == project_name), None)
     if project != None:
         uri = '{0}/{1}/variables/{2}'.format(octopus_server_uri, space['Id'], project['VariableSetId'])
         project_variables = get_octopus_resource(uri, headers)
-        project_variable = next((x for x in project_variables['Variables'] if x['Name'] == variable['Name']), None)
+        project_variable = next((x for x in project_variables['Variables'] if (x['Name'] == variable['Name']) and
+            (x['Scope'] == variable['Scope'])), None)
 
         if project_variable == None:
             project_variables['Variables'].append(variable)
         else:
             project_variable['Value'] = variable['Value']
             project_variable['Type'] = variable['Type']
+            project_variable['Scope'] = variable['Scope']
             project_variable['IsSensitive'] = variable ['IsSensitive']
 
+        print(f"The json looks like {project_variables}")
         response = requests.put(uri, headers=headers, json=project_variables, verify=False)
         response.raise_for_status
+        print(response)
 
 
 @main.command('get-projects', short_help='Get a list of projects for space')
 @click.argument("space")
 def get_projects(space):
     """ Get a list of Projects for the defined URI
 
@@ -556,7 +588,11 @@
                 publish_object = create_publish_object(project_id, runbook_id, info['next_name'])
                 print(f" This is the publish_object {publish_object}")
                 publish_result = post_octopus_resource('{0}/{1}/runbookSnapshots?publish=true'.format(octopus_server_uri, space['Id']), publish_object)
                 print(publish_result)
             else:
                 cprint('No publishing needed', 'green')
 
+@main.command("list-shelf-data", short_help="Print data in a shelf")
+@click.argument("shelf_name")
+def list_shelf_data(shelf_name):
+    contents = shelf.shelf_list_contents(shelf_name)
```

### Comparing `pypus-1.2.0/PKG-INFO` & `pypus-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pypus
-Version: 1.2.0
+Version: 1.3.0
 Summary: Octopus cli toolkit
 License: MIT
 Author: Michael MacKenna
 Author-email: mmackenna@unitedfiregroup.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
```

