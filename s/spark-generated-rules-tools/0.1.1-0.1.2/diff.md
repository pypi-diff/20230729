# Comparing `tmp/spark_generated_rules_tools-0.1.1.tar.gz` & `tmp/spark_generated_rules_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_generated_rules_tools-0.1.1.tar", last modified: Sat Jul 29 05:46:06 2023, max compression
+gzip compressed data, was "spark_generated_rules_tools-0.1.2.tar", last modified: Sat Jul 29 12:22:56 2023, max compression
```

## Comparing `spark_generated_rules_tools-0.1.1.tar` & `spark_generated_rules_tools-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.993401 spark_generated_rules_tools-0.1.1/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       52 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2411 2023-07-29 05:46:06.993401 spark_generated_rules_tools-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1604 2023-07-18 06:35:00.000000 spark_generated_rules_tools-0.1.1/README.md
--rw-rw-rw-   0        0        0      689 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-29 05:46:06.994401 spark_generated_rules_tools-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1218 2023-07-29 05:45:56.000000 spark_generated_rules_tools-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.968556 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/
--rw-rw-rw-   0        0        0     1101 2023-07-29 05:44:29.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.990408 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    24417 2023-07-29 05:42:33.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.992400 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.992400 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0    26115 2023-07-29 02:06:11.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0      501 2023-07-29 03:39:01.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/utilitty.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:46:06.989396 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     2411 2023-07-29 05:46:06.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2023-07-29 05:46:06.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 05:46:06.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-29 05:46:06.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-29 05:46:06.000000 spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.780182 spark_generated_rules_tools-0.1.2/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       52 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2411 2023-07-29 12:22:56.780182 spark_generated_rules_tools-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1604 2023-07-18 06:35:00.000000 spark_generated_rules_tools-0.1.2/README.md
+-rw-rw-rw-   0        0        0      689 2023-07-18 06:18:04.000000 spark_generated_rules_tools-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-29 12:22:56.785185 spark_generated_rules_tools-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2023-07-29 12:22:34.000000 spark_generated_rules_tools-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.758257 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/
+-rw-rw-rw-   0        0        0     1101 2023-07-29 05:44:29.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.777334 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    24415 2023-07-29 12:21:38.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.779334 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.779334 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0    26115 2023-07-29 02:06:11.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0      501 2023-07-29 03:39:01.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/utilitty.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:22:56.773356 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     2411 2023-07-29 12:22:56.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2023-07-29 12:22:56.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 12:22:56.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-29 12:22:56.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-29 12:22:56.000000 spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_generated_rules_tools-0.1.1/LICENSE` & `spark_generated_rules_tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.1/PKG-INFO` & `spark_generated_rules_tools-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_generated_rules_tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: spark_generated_rules_tools
 Home-page: https://github.com/jonaqp/spark_generated_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_generated_rules_tools-0.1.1/README.md` & `spark_generated_rules_tools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.1/pyproject.toml` & `spark_generated_rules_tools-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.1/setup.py` & `spark_generated_rules_tools-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_generated_rules_tools',
     packages=find_packages(),
-    version='0.1.1',
+    version='0.1.2',
     description='spark_generated_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_generated_rules_tools/',
     download_url='https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip',
```

### Comparing `spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/__init__.py` & `spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/functions/generator.py` & `spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
     import os
     import requests
     import json
     from spark_generated_rules_tools.utils.utilitty import extract_only_column_text
     from spark_generated_rules_tools.utils.utilitty import extract_only_parenthesis
 
     dir_schema_name = os.getenv('pj_dq_dir_schema_name')
-    uuaa_name = str(table_name.split("_")[2]).lower()
+    uuaa_name = str(table_name.split("_")[1]).lower()
     uuaa_tag = "".join(table_name.split("_")[2:])
     table_name_extract = "_".join(table_name.split("_")[2:])
 
     uuaa_tag_table = table_name
     if is_uuaa_tag:
         uuaa_tag_table = uuaa_tag
 
@@ -313,26 +313,25 @@
                  f"schemas/pe/{uuaa_name}/master/" \
                  f"{uuaa_tag_table}/latest/" \
                  f"{uuaa_tag_table}.output.schema"
     url_raw_filename = str(url_raw.split("/")[-1])
     dir_raw_schema_filename = os.path.join(dir_schema_name, f"{table_name}", f"{url_raw_filename}")
     url_master_filename = str(url_master.split("/")[-1])
     dir_master_schema_filename = os.path.join(dir_schema_name, f"{table_name}", f"{url_master_filename}")
+    os.makedirs(os.path.dirname(dir_raw_schema_filename), exist_ok=True)
+    os.makedirs(os.path.dirname(dir_master_schema_filename), exist_ok=True)
 
     path = requests.get(url_raw)
     with open(dir_raw_schema_filename, 'wb') as f:
         f.write(path.content)
 
     path = requests.get(url_master)
     with open(dir_master_schema_filename, 'wb') as f:
         f.write(path.content)
 
-    os.makedirs(os.path.dirname(dir_raw_schema_filename), exist_ok=True)
-    os.makedirs(os.path.dirname(dir_master_schema_filename), exist_ok=True)
-
     with open(dir_raw_schema_filename) as f:
         artifactory_json = json.load(f)
 
     table_name = artifactory_json.get("name")
     namespace = artifactory_json.get("namespace")
     table_name_path = artifactory_json.get("physicalPath")
     zone = artifactory_json.get("database").lower()
```

### Comparing `spark_generated_rules_tools-0.1.1/spark_generated_rules_tools/utils/resource/rules.json` & `spark_generated_rules_tools-0.1.2/spark_generated_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/PKG-INFO` & `spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-generated-rules-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: spark_generated_rules_tools
 Home-page: https://github.com/jonaqp/spark_generated_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_generated_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_generated_rules_tools-0.1.1/spark_generated_rules_tools.egg-info/SOURCES.txt` & `spark_generated_rules_tools-0.1.2/spark_generated_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

