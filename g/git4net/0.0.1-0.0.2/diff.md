# Comparing `tmp/git4net-0.0.1.tar.gz` & `tmp/git4net-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git4net-0.0.1.tar", last modified: Sat May 27 04:02:14 2023, max compression
+gzip compressed data, was "git4net-0.0.2.tar", last modified: Fri Jul 28 22:49:27 2023, max compression
```

## Comparing `git4net-0.0.1.tar` & `git4net-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:02:14.111338 git4net-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-27 04:02:01.000000 git4net-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-05-27 04:02:14.111338 git4net-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-27 04:02:01.000000 git4net-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:02:14.111338 git4net-0.0.1/git4net/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/disambiguation.py
--rw-r--r--   0 runner    (1001) docker     (123)    81642 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:02:14.111338 git4net-0.0.1/git4net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-27 04:02:01.000000 git4net-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-27 04:02:14.111338 git4net-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-27 04:02:01.000000 git4net-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:02:14.111338 git4net-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-05-27 04:02:01.000000 git4net-0.0.1/tests/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:49:27.206180 git4net-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-28 22:49:15.000000 git4net-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-28 22:49:27.206180 git4net-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-28 22:49:15.000000 git4net-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:49:27.202180 git4net-0.0.2/git4net/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-28 22:49:15.000000 git4net-0.0.2/git4net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-07-28 22:49:15.000000 git4net-0.0.2/git4net/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19668 2023-07-28 22:49:15.000000 git4net-0.0.2/git4net/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-28 22:49:15.000000 git4net-0.0.2/git4net/disambiguation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81651 2023-07-28 22:49:15.000000 git4net-0.0.2/git4net/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-07-28 22:49:15.000000 git4net-0.0.2/git4net/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:49:27.206180 git4net-0.0.2/git4net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-28 22:49:27.000000 git4net-0.0.2/git4net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-28 22:49:27.000000 git4net-0.0.2/git4net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:49:27.000000 git4net-0.0.2/git4net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-28 22:49:27.000000 git4net-0.0.2/git4net.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 22:49:27.000000 git4net-0.0.2/git4net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 22:49:27.000000 git4net-0.0.2/git4net.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 22:49:15.000000 git4net-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-28 22:49:27.206180 git4net-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-28 22:49:15.000000 git4net-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:49:27.206180 git4net-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-07-28 22:49:15.000000 git4net-0.0.2/tests/test_functions.py
```

### Comparing `git4net-0.0.1/LICENSE.txt` & `git4net-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git4net-0.0.1/PKG-INFO` & `git4net-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git4net
-Version: 0.0.1
+Version: 0.0.2
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/git4net
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: AGPL-3.0+
 Keywords: co-editing,networks,repository,mining,network,analysis
 Classifier: Programming Language :: Python
```

### Comparing `git4net-0.0.1/README.md` & `git4net-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `git4net-0.0.1/git4net/__init__.py` & `git4net-0.0.2/git4net/__init__.py`

 * *Files identical despite different names*

### Comparing `git4net-0.0.1/git4net/command_line.py` & `git4net-0.0.2/git4net/command_line.py`

 * *Files identical despite different names*

### Comparing `git4net-0.0.1/git4net/complexity.py` & `git4net-0.0.2/git4net/complexity.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,14 +124,25 @@
 
                 return custom_metric
             ```
     
     :return:
         **_compute_complexity_measures** (*func*) – The main function that
             computes the complexity measurements for a given commit/file combination.
+
+    example:
+    class FileContents(GRepo_Seed_Metric[str]):
+        def name(self):
+            return "FileContents"
+
+        def metric(self, filename: str, source_code: str):
+            return mystring.string(source_code).tobase64()
+
+        def diff(self, latest, previous):
+            return None
     """
 
     def _compute_complexity_measures(args):
         """
         Computes a set of complexity measures for a given commit/file combination.
         
         :param dict args: dictionary with the following key/value pairs:
```

### Comparing `git4net-0.0.1/git4net/disambiguation.py` & `git4net-0.0.2/git4net/disambiguation.py`

 * *Files identical despite different names*

### Comparing `git4net-0.0.1/git4net/extraction.py` & `git4net-0.0.2/git4net/extraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import pathpy as pp
 import re
 import lizard
 import collections
 import git
 from git.exc import GitCommandError
 
-from git4net import __version__
-
+__version__ = "0.0.0"
+import pandas as pd
 import time
 import sys
 
 import json
 
 import contextlib
 import io
```

### Comparing `git4net-0.0.1/git4net/visualisation.py` & `git4net-0.0.2/git4net/visualisation.py`

 * *Files identical despite different names*

### Comparing `git4net-0.0.1/git4net.egg-info/PKG-INFO` & `git4net-0.0.2/git4net.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git4net
-Version: 0.0.1
+Version: 0.0.2
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/git4net
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: AGPL-3.0+
 Keywords: co-editing,networks,repository,mining,network,analysis
 Classifier: Programming Language :: Python
```

### Comparing `git4net-0.0.1/setup.cfg` & `git4net-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `git4net-0.0.1/setup.py` & `git4net-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"git4net"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

### Comparing `git4net-0.0.1/tests/test_functions.py` & `git4net-0.0.2/tests/test_functions.py`

 * *Files identical despite different names*

