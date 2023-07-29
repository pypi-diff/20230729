# Comparing `tmp/apixdev-0.3.4.tar.gz` & `tmp/apixdev-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apixdev-0.3.4.tar", last modified: Sat Jul 29 11:26:03 2023, max compression
+gzip compressed data, was "apixdev-0.3.5.tar", last modified: Sat Jul 29 13:20:12 2023, max compression
```

## Comparing `apixdev-0.3.4.tar` & `apixdev-0.3.5.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:26:03.162209 apixdev-0.3.4/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-23 16:27:29.000000 apixdev-0.3.4/LICENSE
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-29 11:26:03.162209 apixdev-0.3.4/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      825 2023-07-29 10:46:23.000000 apixdev-0.3.4/README.md
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:26:03.158209 apixdev-0.3.4/apixdev/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/__init__.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:26:03.162209 apixdev-0.3.4/apixdev/cli/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2022-08-11 15:34:34.000000 apixdev-0.3.4/apixdev/cli/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      716 2023-07-29 11:19:37.000000 apixdev-0.3.4/apixdev/cli/config.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      205 2023-07-29 11:19:20.000000 apixdev-0.3.4/apixdev/cli/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1854 2023-07-29 11:19:52.000000 apixdev-0.3.4/apixdev/cli/main.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     9654 2023-07-29 11:08:25.000000 apixdev-0.3.4/apixdev/cli/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      551 2023-07-29 11:09:52.000000 apixdev-0.3.4/apixdev/cli/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      760 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/cli/tools.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:26:03.162209 apixdev-0.3.4/apixdev/core/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/core/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/core/common.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1661 2023-07-29 08:12:20.000000 apixdev-0.3.4/apixdev/core/compose.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5317 2023-07-29 07:18:44.000000 apixdev-0.3.4/apixdev/core/docker.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1123 2023-07-29 10:53:37.000000 apixdev-0.3.4/apixdev/core/exceptions.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      649 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/core/images.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2709 2023-07-28 18:39:39.000000 apixdev-0.3.4/apixdev/core/odoo.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4656 2023-07-27 22:05:53.000000 apixdev-0.3.4/apixdev/core/project.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      561 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/core/projects.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1232 2023-07-23 16:27:29.000000 apixdev-0.3.4/apixdev/core/repository.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     6049 2023-07-28 20:16:17.000000 apixdev-0.3.4/apixdev/core/settings.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3216 2023-07-29 08:12:20.000000 apixdev-0.3.4/apixdev/core/tools.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1395 2023-07-29 07:15:48.000000 apixdev-0.3.4/apixdev/vars.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:26:03.158209 apixdev-0.3.4/apixdev.egg-info/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      695 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/SOURCES.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/dependency_links.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/entry_points.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      136 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/requires.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-29 11:26:03.000000 apixdev-0.3.4/apixdev.egg-info/top_level.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-29 11:26:03.162209 apixdev-0.3.4/setup.cfg
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1575 2023-07-29 11:09:11.000000 apixdev-0.3.4/setup.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:20:12.009798 apixdev-0.3.5/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1074 2023-07-29 11:31:48.000000 apixdev-0.3.5/LICENSE
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-29 13:20:12.009798 apixdev-0.3.5/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      826 2023-07-29 11:31:48.000000 apixdev-0.3.5/README.md
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:20:12.009798 apixdev-0.3.5/apixdev/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       71 2023-07-29 11:31:48.000000 apixdev-0.3.5/apixdev/__init__.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:20:12.009798 apixdev-0.3.5/apixdev/cli/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:31:48.000000 apixdev-0.3.5/apixdev/cli/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      716 2023-07-29 12:42:21.000000 apixdev-0.3.5/apixdev/cli/config.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      230 2023-07-29 12:44:08.000000 apixdev-0.3.5/apixdev/cli/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1856 2023-07-29 12:39:31.000000 apixdev-0.3.5/apixdev/cli/main.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     9736 2023-07-29 13:09:17.000000 apixdev-0.3.5/apixdev/cli/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      576 2023-07-29 13:11:10.000000 apixdev-0.3.5/apixdev/cli/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      707 2023-07-29 13:16:12.000000 apixdev-0.3.5/apixdev/cli/tools.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:20:12.009798 apixdev-0.3.5/apixdev/core/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-07-29 11:31:48.000000 apixdev-0.3.5/apixdev/core/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      627 2023-07-29 11:31:48.000000 apixdev-0.3.5/apixdev/core/common.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2134 2023-07-29 13:06:38.000000 apixdev-0.3.5/apixdev/core/compose.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5443 2023-07-29 13:07:48.000000 apixdev-0.3.5/apixdev/core/docker.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1123 2023-07-29 11:31:48.000000 apixdev-0.3.5/apixdev/core/exceptions.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      716 2023-07-29 12:42:21.000000 apixdev-0.3.5/apixdev/core/images.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2953 2023-07-29 12:56:45.000000 apixdev-0.3.5/apixdev/core/odoo.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4815 2023-07-29 12:13:36.000000 apixdev-0.3.5/apixdev/core/project.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      631 2023-07-29 13:10:26.000000 apixdev-0.3.5/apixdev/core/projects.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5599 2023-07-29 12:55:03.000000 apixdev-0.3.5/apixdev/core/settings.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5116 2023-07-29 13:17:11.000000 apixdev-0.3.5/apixdev/core/tools.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1539 2023-07-29 12:35:44.000000 apixdev-0.3.5/apixdev/vars.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-07-29 13:20:12.009798 apixdev-0.3.5/apixdev.egg-info/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      662 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      668 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       46 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/entry_points.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      136 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/requires.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        8 2023-07-29 13:20:12.000000 apixdev-0.3.5/apixdev.egg-info/top_level.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-07-29 13:20:12.009798 apixdev-0.3.5/setup.cfg
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1575 2023-07-29 12:42:00.000000 apixdev-0.3.5/setup.py
```

### Comparing `apixdev-0.3.4/LICENSE` & `apixdev-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.4/PKG-INFO` & `apixdev-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.3.4
+Version: 0.3.5
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.3.4/README.md` & `apixdev-0.3.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 
 # apix
 
 _**ApiX** Command Line Tool_
-![PyPI](https://img.shields.io/pypi/v/apixdev) ![PyPI](https://img.shields.io/pypi/pyversions/apixdev) ![GitHub last commit (by committer)](https://img.shields.io/github/last-commit/apikcloud/apix-cli)
+
+![PyPI](https://img.shields.io/pypi/v/apixdev)
+![PyPI](https://img.shields.io/pypi/pyversions/apixdev)
+![GitHub last commit (by committer)](https://img.shields.io/github/last-commit/apikcloud/apix-cli)
 
 
 ## Installation
 
 Install from PyPI:
 
 ```bash
```

### Comparing `apixdev-0.3.4/apixdev/cli/config.py` & `apixdev-0.3.5/apixdev/cli/config.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.4/apixdev/cli/main.py` & `apixdev-0.3.5/apixdev/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 project.add_command(project_cmd.delete)
 project.add_command(project_cmd.merge)
 project.add_command(project_cmd.pull)
 project.add_command(project_cmd.run)
 project.add_command(project_cmd.restart)
 project.add_command(project_cmd.stop)
 project.add_command(project_cmd.clear)
-project.add_command(project_cmd.show)
+project.add_command(project_cmd.status)
 project.add_command(project_cmd.logs)
 project.add_command(project_cmd.locate)
 project.add_command(project_cmd.bash)
 project.add_command(project_cmd.shell)
 project.add_command(project_cmd.install_modules)
 project.add_command(project_cmd.update_modules)
 project.add_command(project_cmd.last_backup)
```

### Comparing `apixdev-0.3.4/apixdev/cli/project.py` & `apixdev-0.3.5/apixdev/cli/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 
         urls = [
             ("manifest.yaml", database.manifest_url),
             ("repositories.yaml", database.repositories_url),
             ("docker-compose.yaml", database.compose_url),
         ]
 
-        for name, url in urls:
+        for filename, url in urls:
             try:
-                project.download(name, url)
+                project.download(filename, url)
             except DownloadError as error:
                 click.echo(error)
                 sys.exit(1)
 
         project.pull_repositories()
         project.merge_requirements()
 
@@ -54,15 +54,15 @@
     "--yes",
     is_flag=True,
     callback=abort_if_false,
     expose_value=False,
     prompt="Are you sure you want to overwrite project ?",
 )
 @click.argument("name")
-def update(name, help="update project"):
+def update(name):
     """Update the local project based on the manifest.
 
     `NAME` is the name of the local project.
 
     Note: Repositorie and requirements are updated.
     """
 
@@ -356,28 +356,33 @@
     stack = project.get_stack()
     container = stack.get_odoo_container()
     container.install_modules(database, modules, install=False)
 
 
 @click.command()
 @click.argument("name")
-def show(name):
+def status(name):
     """Show project containers and states.
 
     `NAME` is the name of the local project.
     """
 
     project = Project(name)
 
     if not project.is_ready:
         click.echo(f"No '{project}' project found locally.")
         sys.exit(1)
 
     stack = project.get_stack()
     containers = stack.get_containers()
+
+    if not containers:
+        click.echo(f"'{project}' stack is down.")
+        sys.exit(1)
+
     print_list(containers)
 
 
 @click.command()
 @click.argument("name")
 def locate(name):
     """Locate project on disk.
```

### Comparing `apixdev-0.3.4/apixdev/cli/projects.py` & `apixdev-0.3.5/apixdev/cli/projects.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from apixdev.cli.tools import abort_if_false, print_list
 from apixdev.core.exceptions import CommandNotImplemented
 from apixdev.core.projects import Projects
 
 
 @click.command()
-def ls():
+def ls():  # pylint: disable=C0103
     """List local projects"""
 
     projects = Projects.from_path()
     print_list(projects)
 
 
 @click.command()
```

### Comparing `apixdev-0.3.4/apixdev/core/common.py` & `apixdev-0.3.5/apixdev/core/common.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.4/apixdev/core/docker.py` & `apixdev-0.3.5/apixdev/core/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import subprocess
-
 from apixdev.core.exceptions import NoContainerFound
 from apixdev.core.settings import vars
-from apixdev.core.tools import convert_stdout_to_json
+from apixdev.core.tools import convert_stdout_to_json, run_external_command
 
 
 class Stack:
     def __init__(self, name, path):
         self.name = name
         self.path = path
         self.service_count = 3
@@ -32,54 +30,52 @@
             cmd = vars.DOCKER_COMPOSE_RUN_BACKGROUND
         else:
             if auto_reload:
                 cmd = vars.DOCKER_COMPOSE_RUN_DEV
             else:
                 cmd = vars.DOCKER_COMPOSE_RUN
 
-        subprocess.call(cmd.split(" "), cwd=self.path)
+        run_external_command(cmd, result=False, cwd=self.path)
 
     def stop(self, clear=False):
         """Stop docker-compose stack."""
         cmd = vars.DOCKER_COMPOSE_DOWN.split(" ")
 
         if clear:
             cmd.append("-v")
 
-        subprocess.call(cmd, cwd=self.path)
+        run_external_command(cmd, result=False, cwd=self.path)
 
     def clear(self):
         """Stop and clear docker-compose stack."""
         self.stop(True)
 
-    def _convert_container_info(self, vals_list):
+    def _convert_container_info(self, vals_list):  # pylint: disable=R0201
         def apply(vals):
             name = vals.get("Name", vals.get("Names", ""))
             return {
                 "name": name,
                 "state": vals.get("State", ""),
             }
 
         return list(map(apply, vals_list))
 
     def _inspect_services(self):
         # Method 1 : docker compose ps
-        cmd = ["docker", "compose", "ps", "--format", "json"]
-        res = subprocess.check_output(cmd, cwd=self.path)
+        res = run_external_command(vars.DOCKER_COMPOSE_PS, cwd=self.path)
         data = convert_stdout_to_json(res)
 
         if len(data) == vars.DOCKER_SERVICES_COUNT:
             return self._convert_container_info(data)
 
         # When the stack is not running in background,
         # the odoo container does not appear with the first ps command
 
         # Method 2 : docker ps + filtering on project name
-        cmd = ["docker", "ps", "--format", "json"]
-        res = subprocess.check_output(cmd, cwd=self.path)
+        res = run_external_command(vars.DOCKER_PS, cwd=self.path)
         data = convert_stdout_to_json(res)
 
         data = list(
             filter(lambda item: item.get("Names", "").startswith(self.name), data)
         )
 
         return self._convert_container_info(data)
@@ -137,23 +133,27 @@
 
     def logs(self):
         """Show container logs"""
         if not self.is_running:
             return False
 
         cmd = vars.DOCKER_LOGS.format(self.name).split(" ")
-        subprocess.call(cmd, cwd=self.path)
+        run_external_command(cmd, result=False, cwd=self.path)
+
+        return True
 
     def bash(self):
         """Attach to container bash"""
         if not self.is_running:
             return False
 
         cmd = vars.DOCKER_EXEC.format(self.name, "bash").split(" ")
-        subprocess.call(cmd, cwd=self.path)
+        run_external_command(cmd, result=False, cwd=self.path)
+
+        return True
 
 
 class OdooContainer(Container):
     def __init__(self, stack, name):
         super().__init__(stack, "odoo", name)
 
     def install_modules(self, database, modules, **kwargs):
@@ -161,18 +161,22 @@
         if not self.is_running:
             return False
 
         odoo_arg = "-u" if not kwargs.get("install", False) else "-i"
         odoo_cmd = vars.ODOO_MODULES.format(database, odoo_arg, modules)
         cmd = vars.DOCKER_EXEC.format(self.name, odoo_cmd).split()
 
-        subprocess.call(cmd, cwd=self.path)
+        run_external_command(cmd, result=False, cwd=self.path)
+
+        return True
 
     def shell(self, database):
         """Attach to Odoo Shell"""
         if not self.is_running:
             return False
 
         cmd = vars.DOCKER_EXEC.format(
             self.name, vars.ODOO_SHELL.format(database)
         ).split(" ")
-        subprocess.call(cmd, cwd=self.path)
+        run_external_command(cmd, result=False, cwd=self.path)
+
+        return True
```

### Comparing `apixdev-0.3.4/apixdev/core/exceptions.py` & `apixdev-0.3.5/apixdev/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `apixdev-0.3.4/apixdev/core/odoo.py` & `apixdev-0.3.5/apixdev/core/odoo.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,39 +13,44 @@
 class Odoo(metaclass=SingletonMeta):
     _cr = None
     _url = ""
     _db = ""
     _user = ""
     _password = ""
 
-    def __init__(self, url, db, user, password, **kwargs):
+    def __init__(self, url, dbname, user, password, **kwargs):
         self._url = url
-        self._db = db
+        self._db = dbname
         self._user = user
         self._password = password
 
-        for k, v in kwargs.items():
-            self.__dict__[k] = v
+        for key, value in kwargs.items():
+            self.__dict__[key] = value
 
         self._cr = self._connect()
 
     @classmethod
     def new(cls):
+        """Return Odoo object with credentials and options."""
         return cls(*settings.odoo_credentials, **settings.odoo_options)
 
     @property
     def saas_database(self):
+        """Return SaaS Database object."""
+
         return self._cr.env["saas.database"]
 
     def get_params(self):
+        """Return Odoo options."""
+
         return {k: v for k, v in self.__dict__.items() if k in vars.ODOORPC_OPTIONS}
 
     def _connect(self):
         options = self.get_params()
-        _logger.info("Odoorpc %s with %s", self._url, options)
+        _logger.debug("Odoorpc %s with %s", self._url, options)
 
         # urlopen error [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate
         # FIXME: definitely not the best solution...
         if settings.no_verify:
             myssl = ssl.create_default_context()
             myssl.check_hostname = False
             myssl.verify_mode = ssl.CERT_NONE
@@ -55,42 +60,47 @@
             )
             options["opener"] = opener_selfsigned
 
         obj = odoorpc.ODOO(self._url, **options)
 
         try:
             obj.login(self._db, self._user, self._password)
-        except odoorpc.error.RPCError as e:
-            _logger.error(e)
+        except odoorpc.error.RPCError as error:
+            _logger.error(error)
             obj = None
 
         return obj
 
     def get_databases(self, name, **kwargs):
+        """Search on ApiX databases."""
+
         strict = kwargs.get("strict", True)
         options = {k: v for k, v in kwargs.items() if k in ["limit"]}
 
         operator = "=" if strict else "ilike"
         domain = [("name", operator, name)]
         ids = self.saas_database.search(domain, **options)
 
         if ids:
             return self.saas_database.browse(ids)
         return False
 
-    def get_database_from_uuid(self, uuid):
+    def get_database_by_uuid(self, uuid):
+        """Get database object by UUID."""
+
         domain = [("uuid", "=", uuid)]
         ids = self.saas_database.search(domain, limit=1)
         if ids:
             return self.saas_database.browse(ids)
         return False
 
     def get_last_backup_url(self, uuid):
-        ids = self.saas_database.search([("uuid", "=", uuid)], limit=1)
+        """Get last backup url from ApiX database."""
+
+        database = self.get_database_by_uuid(uuid)
 
-        if not ids:
+        if not database:
             return False
 
-        database = self.saas_database.browse(ids)
         action = database.action_get_last_backup()
 
         return action.get("url", False)
```

### Comparing `apixdev-0.3.4/apixdev/core/project.py` & `apixdev-0.3.5/apixdev/core/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,63 +33,72 @@
         return f"Project({self.name})"
 
     def __str__(self) -> str:
         return self.name
 
     @classmethod
     def from_path(cls, path):
-        """Load project from path"""
+        """Load project from path."""
+
         name = os.path.basename(path)
         instance = cls(name, path)
 
         return instance
 
     @property
     def compose_file(self):
-        """Complete filepath to docker-compose.yaml"""
+        """Complete filepath to docker-compose.yaml."""
+
         return os.path.join(self.path, "docker-compose.yaml")
 
     @property
     def repositories_file(self):
-        """Complete filepath to repositories.yaml"""
+        """Complete filepath to repositories.yaml."""
+
         return os.path.join(self.path, "repositories.yaml")
 
     @property
     def manifest_file(self):
-        """Complete filepath to manifest.yaml"""
+        """Complete filepath to manifest.yaml."""
+
         return os.path.join(self.path, "manifest.yaml")
 
     @property
     def env_file(self):
-        """Complete filepath to .env file"""
+        """Complete filepath to .env file."""
+
         return os.path.join(self.path, ".env")
 
     @property
     def repositories_path(self):
-        """Complete path to repositories"""
+        """Complete path to repositories."""
+
         return os.path.join(self.path, "repositories")
 
     @property
     def is_ready(self):
-        """A project is considered ready if all 3 manifests are present"""
+        """A project is considered ready if all 3 manifests are present."""
+
         files = [
             self.compose_file,
             self.repositories_file,
             self.manifest_file,
         ]
         return bool(all(map(os.path.exists, files)))
 
     def download(self, filename, url, force=False):
+        """Generic method to download file from ApiX database."""
+
         filepath = os.path.join(self.path, filename)
         headers = {
             "X-Api-Token": settings.get_var("apix.token"),
         }
 
         if force and os.path.exists(filepath):
-            _logger.info("Remove %s file", filepath)
+            _logger.debug("Remove %s file", filepath)
             os.remove(filepath)
 
         try:
             response = requests.get(
                 url,
                 headers=headers,
                 allow_redirects=False,
@@ -118,47 +127,51 @@
             "repositories.yaml",
             "--expand-env",
             "--env-file",
             env_file,
         ]
         subprocess.call(args, cwd=self.path)
 
+        return True
+
     def merge_requirements(self):
+        """Merge all requirements from manifest and repositories."""
+
         compose = Compose.from_path(self.compose_file)
 
         requirements = get_requirements_from_path(self.repositories_path)
         requirements += text_to_list(
             compose.extract("services/odoo/environment/CUSTOM_REQUIREMENTS")
         )
         requirements = filter_requirements(requirements)
 
         text = list_to_text(requirements)
         compose.update("services/odoo/environment/CUSTOM_REQUIREMENTS", text)
         compose.save(self.compose_file)
 
     def load_manifest(self):
+        """Load YAML manifest and download files related."""
+
         manifest = Compose.from_path(self.manifest_file)
         self.uuid = manifest.extract("uuid")
 
         keys = [
             (self.compose_file, "docker_compose_url"),
             (self.repositories_file, "repositories_url"),
         ]
 
         for filename, key in keys:
             url = manifest.extract(key)
             self.download(filename, url, True)
 
     def get_stack(self):
-        return Stack(self.name, self.path)
+        """Return Stack object."""
 
-    # def __del__(self):
-    #     rmtree(self.path, ignore_errors=True)
-    #     self.root_path = None
-    #     self.path = None
-    #     self.name = None
+        return Stack(self.name, self.path)
 
     def delete(self):
+        """Delete project and remove files."""
+
         rmtree(self.path, ignore_errors=True)
         self.root_path = None
         self.path = None
         self.name = None
```

### Comparing `apixdev-0.3.4/apixdev/core/projects.py` & `apixdev-0.3.5/apixdev/core/projects.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 
 from apixdev.core.project import Project
-from apixdev.core.settings import Settings
+from apixdev.core.settings import settings
 
 
 class Projects:
     def __init__(self, path):
         self.path = path
 
     @classmethod
     def from_path(cls, path=None):
+        """Return Projects object from path."""
         if not path:
-            settings = Settings()
             path = settings.workdir
         instance = cls(path)
         return instance.get_all()
 
     def get_all(self):
+        """Return all projects find in workdir path."""
         projects = list(map(Project, os.listdir(self.path)))
         projects = list(filter(lambda project: project.is_ready, projects))
 
         return projects
```

### Comparing `apixdev-0.3.4/apixdev/core/settings.py` & `apixdev-0.3.5/apixdev/core/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,214 +1,193 @@
 import configparser
 import getpass
 import logging
 import os
-import subprocess
 
 import apixdev.vars as vars
 from apixdev.core.exceptions import ExternalDependenciesMissing
+from apixdev.core.tools import (
+    merge_sections,
+    run_external_command,
+    split_var,
+    unmerge_sections,
+)
 
 config_dir = os.path.join(vars.HOME_PATH, vars.CONFIG_PATH)
-filename = os.path.join(config_dir, vars.LOGGING_FILE)
 
 if not os.path.isdir(config_dir):
     os.makedirs(config_dir)
 
-logging.basicConfig(filename=filename, level=vars.LOGGING_LEVEL)
+logging.basicConfig(level=vars.LOGGING_LEVEL)
 
 _logger = logging.getLogger(__name__)
 
-from apixdev.core.common import SingletonMeta  # noqa: E402
-
-
-def check_system_dependencies(cmd):
-    try:
-        res = subprocess.check_output(cmd.split(" "))
-        res = res.decode("utf8").strip()
-    except FileNotFoundError:
-        return False
-
-    return res
+from apixdev.core.common import SingletonMeta  # noqa: E402, pylint: disable=C0413
 
 
 class Settings(metaclass=SingletonMeta):
     def __init__(self, path, name="config.ini"):
         self._path = path
         self._name = name
         self._config = None
 
         self.docker_version = None
         self.docker_compose_version = None
 
         self._load()
 
-    def check(self, raise_if_not_found=True):
-        for name, cmd in vars.EXTERNAL_DEPENDENCIES.items():
-            res = check_system_dependencies(cmd)
-            if not res and raise_if_not_found:
-                raise ExternalDependenciesMissing(name)
-            _logger.error("Check failed: %s not found.", name)
-
     @property
     def filepath(self):
+        """Configuration filepath."""
         return os.path.join(self._path, self._name)
 
-    def _load(self):
-        self._config = configparser.ConfigParser()
-        if not os.path.isdir(self._path):
-            os.makedirs(self._path)
-
-        if not os.path.isfile(self.filepath):
-            _logger.info("New configuration file.")
-
-            vals = self._prepare_config()
-            vals.update(self._get_default_values())
-
-            self.set_vars(vals)
+    @property
+    def odoo_credentials(self):
+        """Odoo credentials property."""
+        return [
+            self.get_var("apix.url"),
+            self.get_var("apix.database"),
+            self.get_var("apix.user"),
+            self.get_var("apix.password"),
+        ]
 
-        else:
-            _logger.info("Load configuration from %s.", self.filepath)
-            self._config.read(self.filepath)
+    @property
+    def odoo_options(self):
+        """Odoo options property."""
+        return {key: self.get_var(f"apix.{key}") for key in vars.ODOORPC_OPTIONS}
 
-    def logout(self):
-        values = self._config["apix"]
-        self._config["apix"] = {
-            k: v for k, v in values.items() if k not in vars.MANDATORY_VALUES
-        }
-        self.save()
+    @property
+    def is_ready(self):
+        """IS Ready property."""
+        return bool(len(self._get_missing_values()) == 0)
 
-    def reload(self):
-        self._config = None
-        self._load()
+    @property
+    def workdir(self):
+        """Workdir path property."""
+        return self.get_var("local.workdir")
 
-    def save(self):
-        _logger.info("Save configuration to %s.", self.filepath)
+    @property
+    def env_file(self):
+        """ENV file property."""
+        return os.path.join(self._path, ".env")
 
-        with open(self.filepath, "w") as configfile:
-            self._config.write(configfile)
+    @property
+    def no_verify(self):
+        """No verify property."""
+        return self.get_boolean("apix.no_verify", False)
 
-    def _get_default_values(self):
+    def _get_default_values(self):  # pylint: disable=R0201
         return {
             "apix.port": vars.DEFAULT_PORT,
             "apix.protocol": vars.DEFAULT_PROTOCOL,
             "apix.timeout": vars.DEFAULT_TIMEOUT,
             "apix.no_verify": vars.DEFAULT_NO_VERIFY,
             "local.default_password": vars.DEFAULT_PASSWORD,
         }
 
-    def _prepare_config(self):
+    def _prepare_config(self):  # pylint: disable=R0201
         return {
             "apix.url": "",
             "apix.port": "",
             "apix.protocol": "",
             "apix.timeout": "",
             "apix.no_verify": "",
             "apix.database": "",
             "apix.user": "",
             "apix.password": "",
         }
 
-    def split_var(self, key, separator="."):
-        section, key = key.split(separator)
-        return section, key
-
-    def _add_separator(self, items, separator="."):
-        return separator.join(items)
-
-    def merge_sections(self, vals):
-        # [section][key] ==> [section.key]
-        _logger.debug("merge sections (before): %s", vals)
-        tmp = dict()
-        for section in vals.keys():
-            tmp.update({self._add_separator([section, k]): v for k, v in vals[section]})
-
-        _logger.debug("merge sections: %s", tmp)
-        return tmp
-
-        # {self._add_dot(section, k):v for k,v in vals[section].items()}
-
-    def unmerge_sections(self, vals):
-        # [section.key] ==> [section][key]
-        tmp = dict()
-        for k, v in vals.items():
-            section, key = self.split_var(k)
-            curr = tmp.setdefault(section, dict())
-            curr[key] = v
+    def _load(self):
+        self._config = configparser.ConfigParser()
+        if not os.path.isdir(self._path):
+            os.makedirs(self._path)
+
+        if not os.path.isfile(self.filepath):
+            _logger.debug("New configuration file.")
 
-        _logger.debug("unmerge_sections: %s", tmp)
-        return tmp
+            vals = self._prepare_config()
+            vals.update(self._get_default_values())
+
+            self.set_vars(vals)
+
+        else:
+            _logger.debug("Load configuration from %s.", self.filepath)
+            self._config.read(self.filepath)
 
     def set_vars(self, vals):
+        """Set values."""
         _logger.debug("set vars: %s", vals)
-        vals = self.unmerge_sections(vals)
+        vals = unmerge_sections(vals)
         self._config.read_dict(vals)
 
         self.save()
 
     def get_vars(self):
+        """Return values."""
         return {section: self._config[section].items() for section in self._config}
 
     def get_var(self, name):
-        section, key = self.split_var(name)
+        """Return value."""
+        section, key = split_var(name)
         return self._config.get(section, key)
 
     def get_boolean(self, name, default=False):
-        section, key = self.split_var(name)
+        """Return boolean value."""
+        section, key = split_var(name)
         return self._config.getboolean(section, key) or default
 
-    def get_missing_values(self):
-        _logger.error("missing values")
+    def _get_missing_values(self):
+        _logger.debug("missing values")
 
-        missing_values = dict()
+        missing_values = {}
 
         vals = self.get_vars()
-        vals = self.merge_sections(vals)
+        vals = merge_sections(vals)
 
         missing_values = {
             k: ""
             for k in vars.MANDATORY_VALUES
             if k not in vals or not vals.get(k, False)
         }
 
         return missing_values.items()
 
-    @property
-    def odoo_credentials(self):
-        return [
-            self.get_var("apix.url"),
-            self.get_var("apix.database"),
-            self.get_var("apix.user"),
-            self.get_var("apix.password"),
-        ]
+    def reload(self):
+        """Reload configuration from file."""
+        self._config = None
+        self._load()
 
-    @property
-    def odoo_options(self):
-        return {k: self.get_var("apix.%s" % k) for k in vars.ODOORPC_OPTIONS}
+    def save(self):
+        """Save current configuration to file."""
+        _logger.debug("Save configuration to %s.", self.filepath)
+
+        with open(self.filepath, "w", encoding="utf8") as configfile:
+            self._config.write(configfile)
+
+    def check(self, raise_if_not_found=True):  # pylint: disable=R0201
+        """Check external dependencies."""
+        for name, cmd in vars.EXTERNAL_DEPENDENCIES.items():
+            res = run_external_command(cmd)
+            if not res and raise_if_not_found:
+                raise ExternalDependenciesMissing(name)
+            _logger.error("Check external dependencies failed: %s not found.", name)
 
     def set_config(self):
+        """Prepare configuration and ask user to complete if necessary."""
         while not self.is_ready:
-            vals = dict()
-            for key, _ in self.get_missing_values():
+            vals = {}
+            for key, _ in self._get_missing_values():
                 if "password" in key:
                     vals[key] = getpass.getpass(f"{key.capitalize()}: ")
                 else:
                     vals[key] = input(f"{key.capitalize()}: ")
             self.set_vars(vals)
 
-    @property
-    def is_ready(self):
-        return True if len(self.get_missing_values()) == 0 else False
-
-    @property
-    def workdir(self):
-        return self.get_var("local.workdir")
-
-    @property
-    def env_file(self):
-        return os.path.join(self._path, ".env")
-
-    @property
-    def no_verify(self):
-        return self.get_boolean("apix.no_verify", False)
+    # def logout(self):
+    #     values = self._config["apix"]
+    #     self._config["apix"] = {
+    #         k: v for k, v in values.items() if k not in vars.MANDATORY_VALUES
+    #     }
+    #     self.save()
 
 
 settings = Settings(config_dir)
```

### Comparing `apixdev-0.3.4/apixdev.egg-info/PKG-INFO` & `apixdev-0.3.5/apixdev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apixdev
-Version: 0.3.4
+Version: 0.3.5
 Summary: ApiX CLI
 Home-page: https://github.com/apikcloud/apix-cli
 Author: Aurelien ROY
 Author-email: roy.aurelien@gmail.com
 License: MIT
 Keywords: docker odoo development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `apixdev-0.3.4/apixdev.egg-info/SOURCES.txt` & `apixdev-0.3.5/apixdev.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -21,10 +21,9 @@
 apixdev/core/compose.py
 apixdev/core/docker.py
 apixdev/core/exceptions.py
 apixdev/core/images.py
 apixdev/core/odoo.py
 apixdev/core/project.py
 apixdev/core/projects.py
-apixdev/core/repository.py
 apixdev/core/settings.py
 apixdev/core/tools.py
```

### Comparing `apixdev-0.3.4/setup.py` & `apixdev-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="apixdev",
-    version="0.3.4",
+    version="0.3.5",
     description="ApiX CLI",
     keywords="docker odoo development",
     url="https://github.com/apikcloud/apix-cli",
     author="Aurelien ROY",
     author_email="roy.aurelien@gmail.com",
     license="MIT",
     classifiers=[
```

