# Comparing `tmp/impose-cli-0.3.8.tar.gz` & `tmp/impose-cli-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.3.8.tar", last modified: Sun Jul 16 17:53:02 2023, max compression
+gzip compressed data, was "impose-cli-0.3.9.tar", last modified: Sat Jul 29 15:28:14 2023, max compression
```

## Comparing `impose-cli-0.3.8.tar` & `impose-cli-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:53:02.219831 impose-cli-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 17:52:42.000000 impose-cli-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 17:53:02.219831 impose-cli-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-16 17:52:42.000000 impose-cli-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:53:02.219831 impose-cli-0.3.8/impose_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:52:42.000000 impose-cli-0.3.8/impose_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-07-16 17:52:42.000000 impose-cli-0.3.8/impose_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-16 17:52:42.000000 impose-cli-0.3.8/impose_cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-16 17:52:42.000000 impose-cli-0.3.8/impose_cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-16 17:52:42.000000 impose-cli-0.3.8/impose_cli/impose_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:53:02.219831 impose-cli-0.3.8/impose_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 17:53:01.000000 impose-cli-0.3.8/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-16 17:53:02.000000 impose-cli-0.3.8/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:53:01.000000 impose-cli-0.3.8/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-16 17:53:01.000000 impose-cli-0.3.8/impose_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 17:53:01.000000 impose-cli-0.3.8/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:53:02.219831 impose-cli-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-16 17:52:42.000000 impose-cli-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:53:02.219831 impose-cli-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:52:42.000000 impose-cli-0.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-16 17:52:42.000000 impose-cli-0.3.8/tests/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:28:14.856801 impose-cli-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 15:27:53.000000 impose-cli-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-29 15:28:14.856801 impose-cli-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-29 15:27:53.000000 impose-cli-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:28:14.852801 impose-cli-0.3.9/impose_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 15:27:53.000000 impose-cli-0.3.9/impose_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-29 15:27:53.000000 impose-cli-0.3.9/impose_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-29 15:27:53.000000 impose-cli-0.3.9/impose_cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-29 15:27:53.000000 impose-cli-0.3.9/impose_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-29 15:27:53.000000 impose-cli-0.3.9/impose_cli/impose_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:28:14.856801 impose-cli-0.3.9/impose_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-29 15:28:14.000000 impose-cli-0.3.9/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-29 15:28:14.000000 impose-cli-0.3.9/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:28:14.000000 impose-cli-0.3.9/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 15:28:14.000000 impose-cli-0.3.9/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 15:28:14.000000 impose-cli-0.3.9/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 15:28:14.856801 impose-cli-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-29 15:27:53.000000 impose-cli-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:28:14.856801 impose-cli-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 15:27:53.000000 impose-cli-0.3.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-29 15:27:53.000000 impose-cli-0.3.9/tests/simple.py
```

### Comparing `impose-cli-0.3.8/LICENSE` & `impose-cli-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.8/README.md` & `impose-cli-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.8/impose_cli/_utils.py` & `impose-cli-0.3.9/impose_cli/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,16 +236,20 @@
                 config["default"] = meta["default"]
             if "type" in meta and meta["type"] != "Any":
                 config["type"] = getattr(builtins, meta["type"])
             if "default" not in meta and "require_flags" in function.decorators:
                 config["required"] = True
             if "description" in meta and "default" in meta or "require_flags" in function.decorators:
                 config["help"] = meta["description"]
+
+            # This change was made in version 0.3.9, where argument names did not have - instead of _
+            arg = arg.replace("_", "-")
             command.params.append(
-                click.Option((f"--{arg}",), **config) if "default" in meta or "require_flags" in function.decorators else click.Argument((arg,), **config)
+                click.Option((f"--{arg}",), **config) if "default" in meta or "require_flags" in function.decorators
+                else click.Argument((arg,), **config)
             )
         node.external_object.add_command(command)
 
     @staticmethod
     def handle_edge(node, parent):
         node.external_object = click.Group(name=node.name)
         parent.external_object.add_command(node.external_object)
```

### Comparing `impose-cli-0.3.8/impose_cli/impose_cli.py` & `impose-cli-0.3.9/impose_cli/impose_cli.py`

 * *Files identical despite different names*

