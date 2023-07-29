# Comparing `tmp/multilogue-0.0.3.tar.gz` & `tmp/multilogue-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multilogue-0.0.3.tar", last modified: Wed Jul 26 21:11:56 2023, max compression
+gzip compressed data, was "multilogue-0.0.5.tar", last modified: Sat Jul 29 19:44:18 2023, max compression
```

## Comparing `multilogue-0.0.3.tar` & `multilogue-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 21:11:56.796677 multilogue-0.0.3/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.3/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      555 2023-07-26 21:11:56.796677 multilogue-0.0.3/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       55 2023-07-02 15:37:04.000000 multilogue-0.0.3/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      581 2023-07-26 21:10:22.000000 multilogue-0.0.3/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-26 21:11:56.796677 multilogue-0.0.3/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 21:11:56.792677 multilogue-0.0.3/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 21:11:56.796677 multilogue-0.0.3/src/multilogue/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       91 2023-07-26 20:35:34.000000 multilogue-0.0.3/src/multilogue/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1206 2023-07-26 21:10:22.000000 multilogue-0.0.3/src/multilogue/entities.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 21:11:56.796677 multilogue-0.0.3/src/multilogue.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      555 2023-07-26 21:11:56.000000 multilogue-0.0.3/src/multilogue.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      238 2023-07-26 21:11:56.000000 multilogue-0.0.3/src/multilogue.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-26 21:11:56.000000 multilogue-0.0.3/src/multilogue.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-07-26 21:11:56.000000 multilogue-0.0.3/src/multilogue.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.5/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-07-29 19:44:18.175396 multilogue-0.0.5/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       55 2023-07-02 15:37:04.000000 multilogue-0.0.5/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      689 2023-07-29 19:11:37.000000 multilogue-0.0.5/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-29 19:44:18.175396 multilogue-0.0.5/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/src/multilogue/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-07-29 19:20:27.000000 multilogue-0.0.5/src/multilogue/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1244 2023-07-27 12:09:50.000000 multilogue-0.0.5/src/multilogue/entities.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-07-27 00:36:41.000000 multilogue-0.0.5/src/multilogue/participants.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/src/multilogue/utilities/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      246 2023-07-29 19:42:30.000000 multilogue-0.0.5/src/multilogue/utilities/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1336 2023-07-29 19:42:30.000000 multilogue-0.0.5/src/multilogue/utilities/chatgpt.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/src/multilogue.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-07-29 19:44:18.000000 multilogue-0.0.5/src/multilogue.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      402 2023-07-29 19:44:18.000000 multilogue-0.0.5/src/multilogue.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-29 19:44:18.000000 multilogue-0.0.5/src/multilogue.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       17 2023-07-29 19:44:18.000000 multilogue-0.0.5/src/multilogue.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-07-29 19:44:18.000000 multilogue-0.0.5/src/multilogue.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/tests/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      345 2023-07-27 12:09:50.000000 multilogue-0.0.5/tests/test_entities.py
```

### Comparing `multilogue-0.0.3/LICENSE` & `multilogue-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.3/PKG-INFO` & `multilogue-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: multilogue
-Version: 0.0.3
+Version: 0.0.5
 Summary: Multilogue
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/multilogue
 Project-URL: Bug Tracker, https://github.com/multilogue/multilogue/issues
+Keywords: multilogue,multilectic,conversation,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `multilogue-0.0.3/pyproject.toml` & `multilogue-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "multilogue"
-version = "0.0.3"
+version = "0.0.5"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Multilogue"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
 ]
+keywords = ["multilogue", "multilectic", "conversation", "ai"]
+dependencies = [
+    "requests >= 2.30.0",
+]
 [project.urls]
 "Homepage" = "https://github.com/multilogue/multilogue"
 "Bug Tracker" = "https://github.com/multilogue/multilogue/issues"
```

### Comparing `multilogue-0.0.3/src/multilogue/entities.py` & `multilogue-0.0.5/src/multilogue/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 # Python
 
 """Copyright (c) Alexander Fedotov.
 This source code is licensed under the license found in the
 LICENSE file in the root directory of this source tree.
 """
+from typing import List, Dict
 
 
 class Entity(object):
     """ Human or other entity, participating in the multilogue """
 
     name:           str = ''
     role:           str = ''
     instructions:   str = ''
-    functions:      str = ''
+    functions:      str = List[Dict]
     python_code:    str = ''
 
     def __init__(self, *args, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
         super(Entity, self).__init__()
```

### Comparing `multilogue-0.0.3/src/multilogue.egg-info/PKG-INFO` & `multilogue-0.0.5/src/multilogue.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: multilogue
-Version: 0.0.3
+Version: 0.0.5
 Summary: Multilogue
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/multilogue
 Project-URL: Bug Tracker, https://github.com/multilogue/multilogue/issues
+Keywords: multilogue,multilectic,conversation,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

