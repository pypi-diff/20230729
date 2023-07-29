# Comparing `tmp/apixdev-0.3.2.tar.gz` & `tmp/apixdev-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apixdev-0.3.2.tar", last modified: Thu Jul 27 22:01:48 2023, max compression
+gzip compressed data, was "apixdev-0.3.4.tar", last modified: Sat Jul 29 11:26:03 2023, max compression
```

## Comparing `apixdev-0.3.2.tar` & `apixdev-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-27 22:01:48.675858 apixdev-0.3.2/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-23 16:27:29.000000 apixdev-0.3.2/LICENSE
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-27 22:01:48.675858 apixdev-0.3.2/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      864 2023-07-23 16:50:50.000000 apixdev-0.3.2/README.md
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-27 22:01:48.675858 apixdev-0.3.2/apixdev/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/__init__.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-27 22:01:48.675858 apixdev-0.3.2/apixdev/cli/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2022-08-11 15:34:34.000000 apixdev-0.3.2/apixdev/cli/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      630 2023-07-23 16:32:30.000000 apixdev-0.3.2/apixdev/cli/config.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      287 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/cli/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1265 2023-07-24 19:52:26.000000 apixdev-0.3.2/apixdev/cli/main.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     6928 2023-07-24 19:03:21.000000 apixdev-0.3.2/apixdev/cli/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      598 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/cli/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      760 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/cli/tools.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-27 22:01:48.675858 apixdev-0.3.2/apixdev/core/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/core/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/core/common.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1457 2023-07-24 19:09:56.000000 apixdev-0.3.2/apixdev/core/compose.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5198 2023-07-24 19:48:50.000000 apixdev-0.3.2/apixdev/core/docker.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      908 2023-07-24 19:31:49.000000 apixdev-0.3.2/apixdev/core/exceptions.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      649 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/core/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2706 2023-07-27 22:01:15.000000 apixdev-0.3.2/apixdev/core/odoo.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4656 2023-07-24 18:55:18.000000 apixdev-0.3.2/apixdev/core/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      561 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/core/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1232 2023-07-23 16:27:29.000000 apixdev-0.3.2/apixdev/core/repository.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     6045 2023-07-27 21:57:47.000000 apixdev-0.3.2/apixdev/core/settings.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3036 2023-07-24 19:52:26.000000 apixdev-0.3.2/apixdev/core/tools.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1296 2023-07-27 21:52:46.000000 apixdev-0.3.2/apixdev/vars.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-27 22:01:48.675858 apixdev-0.3.2/apixdev.egg-info/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      695 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/SOURCES.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/dependency_links.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/entry_points.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      136 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/requires.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-27 22:01:48.000000 apixdev-0.3.2/apixdev.egg-info/top_level.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-27 22:01:48.675858 apixdev-0.3.2/setup.cfg
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1575 2023-07-27 21:50:09.000000 apixdev-0.3.2/setup.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:26:03.162209 apixdev-0.3.4/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-23 16:27:29.000000 apixdev-0.3.4/LICENSE
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-29 11:26:03.162209 apixdev-0.3.4/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      825 2023-07-29 10:46:23.000000 apixdev-0.3.4/README.md
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:26:03.158209 apixdev-0.3.4/apixdev/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/__init__.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:26:03.162209 apixdev-0.3.4/apixdev/cli/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2022-08-11 15:34:34.000000 apixdev-0.3.4/apixdev/cli/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      716 2023-07-29 11:19:37.000000 apixdev-0.3.4/apixdev/cli/config.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      205 2023-07-29 11:19:20.000000 apixdev-0.3.4/apixdev/cli/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1854 2023-07-29 11:19:52.000000 apixdev-0.3.4/apixdev/cli/main.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     9654 2023-07-29 11:08:25.000000 apixdev-0.3.4/apixdev/cli/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      551 2023-07-29 11:09:52.000000 apixdev-0.3.4/apixdev/cli/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      760 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/cli/tools.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:26:03.162209 apixdev-0.3.4/apixdev/core/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/core/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/core/common.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1661 2023-07-29 08:12:20.000000 apixdev-0.3.4/apixdev/core/compose.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5317 2023-07-29 07:18:44.000000 apixdev-0.3.4/apixdev/core/docker.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1123 2023-07-29 10:53:37.000000 apixdev-0.3.4/apixdev/core/exceptions.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      649 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/core/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2709 2023-07-28 18:39:39.000000 apixdev-0.3.4/apixdev/core/odoo.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4656 2023-07-27 22:05:53.000000 apixdev-0.3.4/apixdev/core/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      561 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/core/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1232 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/core/repository.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     6049 2023-07-28 20:16:17.000000 apixdev-0.3.4/apixdev/core/settings.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3216 2023-07-29 08:12:20.000000 apixdev-0.3.4/apixdev/core/tools.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1395 2023-07-29 07:15:48.000000 apixdev-0.3.4/apixdev/vars.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:26:03.158209 apixdev-0.3.4/apixdev.egg-info/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      695 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/entry_points.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      136 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/requires.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/top_level.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-29 11:26:03.162209 apixdev-0.3.4/setup.cfg
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1575 2023-07-29 11:09:11.000000 apixdev-0.3.4/setup.py
```

### Comparing `apixdev-0.3.2/LICENSE` & `apixdev-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.2/PKG-INFO` & `apixdev-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.3.2
+Version: 0.3.4
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.3.2/apixdev/cli/config.py` & `apixdev-0.3.4/apixdev/cli/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import click
 
 from apixdev.cli.tools import print_dict
-from apixdev.core.settings import Settings
-
-settings = Settings()
-
-
-@click.group()
-def config():
-    """View and edit configuration"""
+from apixdev.core.exceptions import CommandNotImplemented
+from apixdev.core.settings import settings
 
 
 @click.command()
 def view():
     """Resume configuration"""
 
     vals = settings.get_vars()
     print_dict(vals, False)
 
 
 @click.command()
 @click.argument("key")
 @click.argument("value")
-def set(key, value):
+def set_value(key, value):
     """Set a value"""
     settings.set_vars({key: value})
 
 
 @click.command()
 def clear():
     """Clear all parameters"""
-    raise NotImplementedError()
+    raise CommandNotImplemented("clear")
 
 
-config.add_command(view)
-config.add_command(clear)
-config.add_command(set)
+@click.command()
+def edit():
+    """
+    Edit config.ini.
+    """
+    _ = click.edit(
+        require_save=True,
+        extension="ini",
+        filename=settings.filepath,
+    )
```

### Comparing `apixdev-0.3.2/apixdev/cli/main.py` & `apixdev-0.3.4/apixdev/cli/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,13 @@
 import click
 
-from apixdev.cli.config import config
-from apixdev.cli.images import images
-from apixdev.cli.project import (
-    bash,
-    clear,
-    delete,
-    install_modules,
-    logs,
-    merge,
-    new,
-    pull,
-    run,
-    search,
-    shell,
-    show,
-    stop,
-    update,
-    update_modules,
-)
-from apixdev.cli.projects import projects
+import apixdev.cli.config as config_cmd
+import apixdev.cli.images as images_cmd
+import apixdev.cli.project as project_cmd
+import apixdev.cli.projects as projects_cmd
 from apixdev.core.settings import settings
 
 # try:
 #     settings.check()
 # except ExternalDependenciesMissing as error:
 #     click.echo(error)
 #     sys.exit(1)
@@ -36,31 +20,58 @@
 @click.group()
 def cli():
     """ApiX command line tool."""
 
 
 @click.group()
 def project():
-    """Manage apix project"""
+    """Manage project"""
 
 
-project.add_command(new)
-project.add_command(update)
-project.add_command(search)
-project.add_command(delete)
-project.add_command(merge)
-project.add_command(pull)
-project.add_command(run)
-project.add_command(stop)
-project.add_command(clear)
-project.add_command(show)
-project.add_command(logs)
-project.add_command(bash)
-project.add_command(shell)
-project.add_command(install_modules)
-project.add_command(update_modules)
+@click.group()
+def projects():
+    """Manage projects"""
+
+
+@click.group()
+def images():
+    """Manage Docker images"""
+
+
+@click.group()
+def config():
+    """View and edit configuration"""
+
 
+project.add_command(project_cmd.new)
+project.add_command(project_cmd.update)
+project.add_command(project_cmd.search)
+project.add_command(project_cmd.delete)
+project.add_command(project_cmd.merge)
+project.add_command(project_cmd.pull)
+project.add_command(project_cmd.run)
+project.add_command(project_cmd.restart)
+project.add_command(project_cmd.stop)
+project.add_command(project_cmd.clear)
+project.add_command(project_cmd.show)
+project.add_command(project_cmd.logs)
+project.add_command(project_cmd.locate)
+project.add_command(project_cmd.bash)
+project.add_command(project_cmd.shell)
+project.add_command(project_cmd.install_modules)
+project.add_command(project_cmd.update_modules)
+project.add_command(project_cmd.last_backup)
+
+projects.add_command(projects_cmd.ls)
+projects.add_command(projects_cmd.stop)
+
+images.add_command(images_cmd.ls)
+
+config.add_command(config_cmd.view)
+config.add_command(config_cmd.clear)
+config.add_command(config_cmd.set_value)
+config.add_command(config_cmd.edit)
 
 cli.add_command(project)
 cli.add_command(projects)
 cli.add_command(images)
 cli.add_command(config)
```

### Comparing `apixdev-0.3.2/apixdev/cli/tools.py` & `apixdev-0.3.4/apixdev/cli/tools.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.2/apixdev/core/common.py` & `apixdev-0.3.4/apixdev/core/common.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.2/apixdev/core/compose.py` & `apixdev-0.3.4/apixdev/core/compose.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 import os
 
 import requests
 import yaml
 
 from apixdev.core.tools import dict_merge, nested_set
 
+_logger = logging.getLogger(__name__)
+
 
 class Compose:
     _name = "docker-compose.yaml"
 
     def __init__(self, content, name=None):
         self._content = content
 
@@ -39,17 +42,23 @@
     def update(self, chain, value):
         keys = chain.split("/")
         vals = {}
 
         nested_set(vals, keys, value)
         dict_merge(self._content, vals)
 
+        print(self._content)
+
     def save(self, filepath):
         assert self._content, "No content to save."
 
+        if os.path.exists(filepath):
+            _logger.info("Remove '%s'", filepath)
+            os.remove(filepath)
+
         with open(filepath, mode="wb") as file:
             yaml.dump(self._content, file, encoding="utf-8")
 
     def extract(self, chain):
         keys = chain.split("/")
 
         def dive(vals, keys):
```

### Comparing `apixdev-0.3.2/apixdev/core/docker.py` & `apixdev-0.3.4/apixdev/core/docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,23 @@
         states = map(lambda item: item.get("state", False), services)
 
         if not all(map(lambda item: bool(item in ["running"]), states)):
             return False
 
         return True
 
-    def run(self, run_on_background=False):
+    def run(self, run_on_background=False, auto_reload=False):
         """Run docker-compose stack."""
         if run_on_background:
             cmd = vars.DOCKER_COMPOSE_RUN_BACKGROUND
         else:
-            cmd = vars.DOCKER_COMPOSE_RUN
+            if auto_reload:
+                cmd = vars.DOCKER_COMPOSE_RUN_DEV
+            else:
+                cmd = vars.DOCKER_COMPOSE_RUN
 
         subprocess.call(cmd.split(" "), cwd=self.path)
 
     def stop(self, clear=False):
         """Stop docker-compose stack."""
         cmd = vars.DOCKER_COMPOSE_DOWN.split(" ")
```

### Comparing `apixdev-0.3.2/apixdev/core/exceptions.py` & `apixdev-0.3.4/apixdev/core/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,7 +23,14 @@
 class ExternalDependenciesMissing(Exception):
     """Exception raised for system package missing ."""
 
     def __init__(self, name):
         self.name = name
         self.message = f"System package missing, please install {name} first."
         super().__init__(self.message)
+
+
+class CommandNotImplemented(NotImplementedError):
+    def __init__(self, name):
+        self.name = name
+        self.message = f"The {name} command is not yet implemented."
+        super().__init__(self.message)
```

### Comparing `apixdev-0.3.2/apixdev/core/images.py` & `apixdev-0.3.4/apixdev/core/images.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.2/apixdev/core/odoo.py` & `apixdev-0.3.4/apixdev/core/odoo.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 
         self._cr = self._connect()
 
     @classmethod
     def new(cls):
         return cls(*settings.odoo_credentials, **settings.odoo_options)
 
+    @property
+    def saas_database(self):
+        return self._cr.env["saas.database"]
+
     def get_params(self):
         return {k: v for k, v in self.__dict__.items() if k in vars.ODOORPC_OPTIONS}
 
     def _connect(self):
         options = self.get_params()
         _logger.info("Odoorpc %s with %s", self._url, options)
 
@@ -57,40 +61,36 @@
             obj.login(self._db, self._user, self._password)
         except odoorpc.error.RPCError as e:
             _logger.error(e)
             obj = None
 
         return obj
 
-    @property
-    def databases(self):
-        return self._cr.env["saas.database"]
-
     def get_databases(self, name, **kwargs):
-        Databases = self._cr.env["saas.database"]
-
         strict = kwargs.get("strict", True)
         options = {k: v for k, v in kwargs.items() if k in ["limit"]}
 
         operator = "=" if strict else "ilike"
         domain = [("name", operator, name)]
-        ids = Databases.search(domain, **options)
+        ids = self.saas_database.search(domain, **options)
 
         if ids:
-            return Databases.browse(ids)
+            return self.saas_database.browse(ids)
         return False
 
     def get_database_from_uuid(self, uuid):
-        Databases = self._cr.env["saas.database"]
         domain = [("uuid", "=", uuid)]
-        id = Databases.search(domain, limit=1)
-        if id:
-            return Databases.browse(id)
+        ids = self.saas_database.search(domain, limit=1)
+        if ids:
+            return self.saas_database.browse(ids)
         return False
 
     def get_last_backup_url(self, uuid):
-        database = self._cr.env["saas.database"].search([("uuid", "=", uuid)], limit=1)
+        ids = self.saas_database.search([("uuid", "=", uuid)], limit=1)
 
-        if not database:
+        if not ids:
             return False
 
-        return database.action_get_last_backup().res["url"]
+        database = self.saas_database.browse(ids)
+        action = database.action_get_last_backup()
+
+        return action.get("url", False)
```

### Comparing `apixdev-0.3.2/apixdev/core/project.py` & `apixdev-0.3.4/apixdev/core/project.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.2/apixdev/core/projects.py` & `apixdev-0.3.4/apixdev/core/projects.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.2/apixdev/core/repository.py` & `apixdev-0.3.4/apixdev/core/repository.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.2/apixdev/core/settings.py` & `apixdev-0.3.4/apixdev/core/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,37 +112,37 @@
         return section, key
 
     def _add_separator(self, items, separator="."):
         return separator.join(items)
 
     def merge_sections(self, vals):
         # [section][key] ==> [section.key]
-        _logger.info("merge sections (before): %s", vals)
+        _logger.debug("merge sections (before): %s", vals)
         tmp = dict()
         for section in vals.keys():
             tmp.update({self._add_separator([section, k]): v for k, v in vals[section]})
 
-        _logger.info("merge sections: %s", tmp)
+        _logger.debug("merge sections: %s", tmp)
         return tmp
 
         # {self._add_dot(section, k):v for k,v in vals[section].items()}
 
     def unmerge_sections(self, vals):
         # [section.key] ==> [section][key]
         tmp = dict()
         for k, v in vals.items():
             section, key = self.split_var(k)
             curr = tmp.setdefault(section, dict())
             curr[key] = v
 
-        _logger.info("unmerge_sections: %s", tmp)
+        _logger.debug("unmerge_sections: %s", tmp)
         return tmp
 
     def set_vars(self, vals):
-        _logger.info("set vars: %s", vals)
+        _logger.debug("set vars: %s", vals)
         vals = self.unmerge_sections(vals)
         self._config.read_dict(vals)
 
         self.save()
 
     def get_vars(self):
         return {section: self._config[section].items() for section in self._config}
```

### Comparing `apixdev-0.3.2/apixdev/core/tools.py` & `apixdev-0.3.4/apixdev/core/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
+import logging
 import os
 import subprocess
 
 import requirements as req_tool
 from packaging.specifiers import SpecifierSet
 
+_logger = logging.getLogger(__name__)
+
 
 def check_system_dependencies(cmd):
     try:
         res = subprocess.check_output(cmd)
     except FileNotFoundError:
         return False
 
@@ -32,14 +35,15 @@
     for r, d, f in os.walk(path):
         for file in f:
             if file == "requirements.txt":
                 with open(os.path.join(r, file)) as tmp:
                     requirements += tmp.readlines()
 
     requirements = list({e.strip() for e in requirements})
+    _logger.info("Read requirements from path: %s", requirements)
 
     return requirements
 
 
 def filter_requirements(items):
     """Cleans and eliminates duplicate requirements"""
     requirements = "\n".join(deduplicate(items))
@@ -61,14 +65,15 @@
             continue
 
         # Sort specifiers and keep only last one
         # FIXME: Not perfect IMHO, errors possible, fix it !
         specs = sorted({*specs}, key=str)
         res.append("".join([name, str(specs[-1])]))
 
+    _logger.info("Filtered requirements: %s", requirements)
     return res
 
 
 def list_to_text(items):
     return "\n\n".join(items) if items else ""
```

### Comparing `apixdev-0.3.2/apixdev/vars.py` & `apixdev-0.3.4/apixdev/vars.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 
 EXTERNAL_DEPENDENCIES = {
     "docker": "docker --version",
     "docker-compose": "docker-compose --version",
 }
 
 DOCKER_COMPOSE_RUN_BACKGROUND = "docker-compose up -d"
+DOCKER_COMPOSE_RUN_DEV = (
+    "docker-compose run --rm --service-ports odoo odoo --dev=reload"
+)
 DOCKER_COMPOSE_RUN = "docker-compose run --rm --service-ports odoo bash"
+
 DOCKER_COMPOSE_DOWN = "docker-compose down"
 DOCKER_LOGS = "docker logs -f {}"
 DOCKER_EXEC = "docker exec -it {} {}"
 
 ODOO_MODULES = "odoo -d {} --stop-after-init {} {}"
 ODOO_SHELL = "odoo shell -d {}"
```

### Comparing `apixdev-0.3.2/apixdev.egg-info/PKG-INFO` & `apixdev-0.3.4/apixdev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.3.2
+Version: 0.3.4
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.3.2/apixdev.egg-info/SOURCES.txt` & `apixdev-0.3.4/apixdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.2/setup.py` & `apixdev-0.3.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="apixdev",
-    version="0.3.2",
+    version="0.3.4",
     description="ApiX CLI",
     keywords="docker odoo development",
     url="https://github.com/apikcloud/apix-cli",
     author="Aurelien ROY",
     author_email="roy.aurelien@gmail.com",
     license="MIT",
     classifiers=[
```

