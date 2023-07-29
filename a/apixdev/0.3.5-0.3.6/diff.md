# Comparing `tmp/apixdev-0.3.5.tar.gz` & `tmp/apixdev-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apixdev-0.3.5.tar", last modified: Sat Jul 29 13:20:12 2023, max compression
+gzip compressed data, was "apixdev-0.3.6.tar", last modified: Sat Jul 29 13:36:43 2023, max compression
```

## Comparing `apixdev-0.3.5.tar` & `apixdev-0.3.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:20:12.009798 apixdev-0.3.5/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-29 11:31:48.000000 apixdev-0.3.5/LICENSE
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-29 13:20:12.009798 apixdev-0.3.5/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      826 2023-07-29 11:31:48.000000 apixdev-0.3.5/README.md
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:20:12.009798 apixdev-0.3.5/apixdev/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-29 11:31:48.000000 apixdev-0.3.5/apixdev/__init__.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:20:12.009798 apixdev-0.3.5/apixdev/cli/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:31:48.000000 apixdev-0.3.5/apixdev/cli/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      716 2023-07-29 12:42:21.000000 apixdev-0.3.5/apixdev/cli/config.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      230 2023-07-29 12:44:08.000000 apixdev-0.3.5/apixdev/cli/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1856 2023-07-29 12:39:31.000000 apixdev-0.3.5/apixdev/cli/main.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     9736 2023-07-29 13:09:17.000000 apixdev-0.3.5/apixdev/cli/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      576 2023-07-29 13:11:10.000000 apixdev-0.3.5/apixdev/cli/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      707 2023-07-29 13:16:12.000000 apixdev-0.3.5/apixdev/cli/tools.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:20:12.009798 apixdev-0.3.5/apixdev/core/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:31:48.000000 apixdev-0.3.5/apixdev/core/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-29 11:31:48.000000 apixdev-0.3.5/apixdev/core/common.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2134 2023-07-29 13:06:38.000000 apixdev-0.3.5/apixdev/core/compose.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5443 2023-07-29 13:07:48.000000 apixdev-0.3.5/apixdev/core/docker.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1123 2023-07-29 11:31:48.000000 apixdev-0.3.5/apixdev/core/exceptions.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      716 2023-07-29 12:42:21.000000 apixdev-0.3.5/apixdev/core/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2953 2023-07-29 12:56:45.000000 apixdev-0.3.5/apixdev/core/odoo.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4815 2023-07-29 12:13:36.000000 apixdev-0.3.5/apixdev/core/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      631 2023-07-29 13:10:26.000000 apixdev-0.3.5/apixdev/core/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5599 2023-07-29 12:55:03.000000 apixdev-0.3.5/apixdev/core/settings.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5116 2023-07-29 13:17:11.000000 apixdev-0.3.5/apixdev/core/tools.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1539 2023-07-29 12:35:44.000000 apixdev-0.3.5/apixdev/vars.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:20:12.009798 apixdev-0.3.5/apixdev.egg-info/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      668 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/SOURCES.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/dependency_links.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/entry_points.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      136 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/requires.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/top_level.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-29 13:20:12.009798 apixdev-0.3.5/setup.cfg
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1575 2023-07-29 12:42:00.000000 apixdev-0.3.5/setup.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:36:43.846349 apixdev-0.3.6/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-29 11:31:48.000000 apixdev-0.3.6/LICENSE
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-29 13:36:43.846349 apixdev-0.3.6/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      826 2023-07-29 11:31:48.000000 apixdev-0.3.6/README.md
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:36:43.846349 apixdev-0.3.6/apixdev/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-29 11:31:48.000000 apixdev-0.3.6/apixdev/__init__.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:36:43.846349 apixdev-0.3.6/apixdev/cli/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:31:48.000000 apixdev-0.3.6/apixdev/cli/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      716 2023-07-29 12:42:21.000000 apixdev-0.3.6/apixdev/cli/config.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      230 2023-07-29 12:44:08.000000 apixdev-0.3.6/apixdev/cli/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1894 2023-07-29 13:26:47.000000 apixdev-0.3.6/apixdev/cli/main.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)    10113 2023-07-29 13:35:38.000000 apixdev-0.3.6/apixdev/cli/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      576 2023-07-29 13:11:10.000000 apixdev-0.3.6/apixdev/cli/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      707 2023-07-29 13:16:12.000000 apixdev-0.3.6/apixdev/cli/tools.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:36:43.846349 apixdev-0.3.6/apixdev/core/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:31:48.000000 apixdev-0.3.6/apixdev/core/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-29 11:31:48.000000 apixdev-0.3.6/apixdev/core/common.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2104 2023-07-29 13:23:17.000000 apixdev-0.3.6/apixdev/core/compose.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5443 2023-07-29 13:07:48.000000 apixdev-0.3.6/apixdev/core/docker.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1123 2023-07-29 11:31:48.000000 apixdev-0.3.6/apixdev/core/exceptions.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      716 2023-07-29 12:42:21.000000 apixdev-0.3.6/apixdev/core/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2953 2023-07-29 12:56:45.000000 apixdev-0.3.6/apixdev/core/odoo.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5124 2023-07-29 13:33:41.000000 apixdev-0.3.6/apixdev/core/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      631 2023-07-29 13:10:26.000000 apixdev-0.3.6/apixdev/core/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5599 2023-07-29 12:55:03.000000 apixdev-0.3.6/apixdev/core/settings.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5116 2023-07-29 13:17:11.000000 apixdev-0.3.6/apixdev/core/tools.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1539 2023-07-29 12:35:44.000000 apixdev-0.3.6/apixdev/vars.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:36:43.846349 apixdev-0.3.6/apixdev.egg-info/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-29 13:36:43.000000 apixdev-0.3.6/apixdev.egg-info/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      668 2023-07-29 13:36:43.000000 apixdev-0.3.6/apixdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-29 13:36:43.000000 apixdev-0.3.6/apixdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-29 13:36:43.000000 apixdev-0.3.6/apixdev.egg-info/entry_points.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      136 2023-07-29 13:36:43.000000 apixdev-0.3.6/apixdev.egg-info/requires.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-29 13:36:43.000000 apixdev-0.3.6/apixdev.egg-info/top_level.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-29 13:36:43.846349 apixdev-0.3.6/setup.cfg
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1575 2023-07-29 13:35:52.000000 apixdev-0.3.6/setup.py
```

### Comparing `apixdev-0.3.5/LICENSE` & `apixdev-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/PKG-INFO` & `apixdev-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.3.5
+Version: 0.3.6
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.3.5/README.md` & `apixdev-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/cli/config.py` & `apixdev-0.3.6/apixdev/cli/config.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/cli/main.py` & `apixdev-0.3.6/apixdev/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 project.add_command(project_cmd.logs)
 project.add_command(project_cmd.locate)
 project.add_command(project_cmd.bash)
 project.add_command(project_cmd.shell)
 project.add_command(project_cmd.install_modules)
 project.add_command(project_cmd.update_modules)
 project.add_command(project_cmd.last_backup)
+project.add_command(project_cmd.repo)
 
 projects.add_command(projects_cmd.ls)
 projects.add_command(projects_cmd.stop)
 
 images.add_command(images_cmd.ls)
 
 config.add_command(config_cmd.view)
```

### Comparing `apixdev-0.3.5/apixdev/cli/project.py` & `apixdev-0.3.6/apixdev/cli/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 import click
 
-from apixdev.cli.tools import abort_if_false, print_list
+from apixdev.cli.tools import abort_if_false, print_dict, print_list
 from apixdev.core.exceptions import DownloadError, NoContainerFound
 from apixdev.core.odoo import Odoo
 from apixdev.core.project import Project
 
 
 @click.command()
 @click.argument("name")
@@ -418,7 +418,25 @@
 
     odoo = Odoo.new()
     url = odoo.get_last_backup_url(project.uuid)
     print_list([url])
 
     if url:
         click.launch(url)
+
+
+@click.command()
+@click.argument("name")
+def repo(name):
+    """Get repositories list with branches.
+
+    `NAME` is the name of the local project.
+    """
+
+    project = Project(name)
+
+    if not project.is_ready:
+        click.echo(f"No '{project}' project found locally.")
+        sys.exit(1)
+
+    repositories = project.get_repo()
+    print_dict(repositories)
```

### Comparing `apixdev-0.3.5/apixdev/cli/projects.py` & `apixdev-0.3.6/apixdev/cli/projects.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/cli/tools.py` & `apixdev-0.3.6/apixdev/cli/tools.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/core/common.py` & `apixdev-0.3.6/apixdev/core/common.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/core/compose.py` & `apixdev-0.3.6/apixdev/core/compose.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,14 @@
 
         keys = chain.split("/")
         vals = {}
 
         nested_set(vals, keys, value)
         dict_merge(self._content, vals)
 
-        print(self._content)
-
     def save(self, filepath):
         """Save compose object to filepath."""
 
         assert self._content, "No content to save."
 
         if os.path.exists(filepath):
             _logger.debug("Remove '%s'", filepath)
```

### Comparing `apixdev-0.3.5/apixdev/core/docker.py` & `apixdev-0.3.6/apixdev/core/docker.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/core/exceptions.py` & `apixdev-0.3.6/apixdev/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/core/images.py` & `apixdev-0.3.6/apixdev/core/images.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/core/odoo.py` & `apixdev-0.3.6/apixdev/core/odoo.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/core/project.py` & `apixdev-0.3.6/apixdev/core/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,14 +164,26 @@
             self.download(filename, url, True)
 
     def get_stack(self):
         """Return Stack object."""
 
         return Stack(self.name, self.path)
 
+    def get_repo(self):
+        """Return repositories and branches from YAML manifest."""
+
+        compose = Compose.from_path(self.repositories_file)
+
+        res = {
+            k.split("/")[-1]: v["merges"][0].split(" ")[-1]
+            for k, v in compose._content.items()
+        }
+
+        return res
+
     def delete(self):
         """Delete project and remove files."""
 
         rmtree(self.path, ignore_errors=True)
         self.root_path = None
         self.path = None
         self.name = None
```

### Comparing `apixdev-0.3.5/apixdev/core/projects.py` & `apixdev-0.3.6/apixdev/core/projects.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/core/settings.py` & `apixdev-0.3.6/apixdev/core/settings.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/core/tools.py` & `apixdev-0.3.6/apixdev/core/tools.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev/vars.py` & `apixdev-0.3.6/apixdev/vars.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/apixdev.egg-info/PKG-INFO` & `apixdev-0.3.6/apixdev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.3.5
+Version: 0.3.6
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.3.5/apixdev.egg-info/SOURCES.txt` & `apixdev-0.3.6/apixdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.5/setup.py` & `apixdev-0.3.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="apixdev",
-    version="0.3.5",
+    version="0.3.6",
     description="ApiX CLI",
     keywords="docker odoo development",
     url="https://github.com/apikcloud/apix-cli",
     author="Aurelien ROY",
     author_email="roy.aurelien@gmail.com",
     license="MIT",
     classifiers=[
```

