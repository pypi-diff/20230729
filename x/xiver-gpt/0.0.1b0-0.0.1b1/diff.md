# Comparing `tmp/xiver_gpt-0.0.1b0.tar.gz` & `tmp/xiver_gpt-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiver_gpt-0.0.1b0.tar", last modified: Fri Jul 28 19:10:51 2023, max compression
+gzip compressed data, was "xiver_gpt-0.0.1b1.tar", last modified: Fri Jul 28 20:40:10 2023, max compression
```

## Comparing `xiver_gpt-0.0.1b0.tar` & `xiver_gpt-0.0.1b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-07-28 19:10:51.031726 xiver_gpt-0.0.1b0/
--rw-r--r--   0 q         (1000) q         (1000)      677 2023-07-27 11:44:15.000000 xiver_gpt-0.0.1b0/LICENSE
--rw-r--r--   0 q         (1000) q         (1000)     1758 2023-07-28 19:10:51.031726 xiver_gpt-0.0.1b0/PKG-INFO
--rw-r--r--   0 q         (1000) q         (1000)     1258 2023-07-28 18:48:14.000000 xiver_gpt-0.0.1b0/README.rst
--rw-r--r--   0 q         (1000) q         (1000)      964 2023-07-28 18:23:34.000000 xiver_gpt-0.0.1b0/pyproject.toml
--rw-r--r--   0 q         (1000) q         (1000)       38 2023-07-28 19:10:51.031726 xiver_gpt-0.0.1b0/setup.cfg
--rw-r--r--   0 q         (1000) q         (1000)     1381 2023-07-28 19:06:01.000000 xiver_gpt-0.0.1b0/setup.py
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-07-28 19:10:51.028726 xiver_gpt-0.0.1b0/xiver_gpt/
--rw-r--r--   0 q         (1000) q         (1000)     3240 2023-07-28 18:16:51.000000 xiver_gpt-0.0.1b0/xiver_gpt/XiverGPT.py
--rw-r--r--   0 q         (1000) q         (1000)       31 2023-07-27 12:36:16.000000 xiver_gpt-0.0.1b0/xiver_gpt/__init__.py
--rw-r--r--   0 q         (1000) q         (1000)     1852 2023-07-28 18:19:03.000000 xiver_gpt-0.0.1b0/xiver_gpt/the_s_of_idea.py
-drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-07-28 19:10:51.030727 xiver_gpt-0.0.1b0/xiver_gpt.egg-info/
--rw-r--r--   0 q         (1000) q         (1000)     1758 2023-07-28 19:10:50.000000 xiver_gpt-0.0.1b0/xiver_gpt.egg-info/PKG-INFO
--rw-r--r--   0 q         (1000) q         (1000)      277 2023-07-28 19:10:50.000000 xiver_gpt-0.0.1b0/xiver_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 q         (1000) q         (1000)        1 2023-07-28 19:10:50.000000 xiver_gpt-0.0.1b0/xiver_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 q         (1000) q         (1000)       13 2023-07-28 19:10:50.000000 xiver_gpt-0.0.1b0/xiver_gpt.egg-info/requires.txt
--rw-r--r--   0 q         (1000) q         (1000)       10 2023-07-28 19:10:50.000000 xiver_gpt-0.0.1b0/xiver_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-07-28 20:40:10.786779 xiver_gpt-0.0.1b1/
+-rw-r--r--   0 q         (1000) q         (1000)      677 2023-07-27 11:44:15.000000 xiver_gpt-0.0.1b1/LICENSE
+-rw-r--r--   0 q         (1000) q         (1000)     1758 2023-07-28 20:40:10.786779 xiver_gpt-0.0.1b1/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)     1258 2023-07-28 18:48:14.000000 xiver_gpt-0.0.1b1/README.rst
+-rw-r--r--   0 q         (1000) q         (1000)      965 2023-07-28 20:39:45.000000 xiver_gpt-0.0.1b1/pyproject.toml
+-rw-r--r--   0 q         (1000) q         (1000)       38 2023-07-28 20:40:10.786779 xiver_gpt-0.0.1b1/setup.cfg
+-rw-r--r--   0 q         (1000) q         (1000)     1381 2023-07-28 19:06:01.000000 xiver_gpt-0.0.1b1/setup.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-07-28 20:40:10.783779 xiver_gpt-0.0.1b1/xiver_gpt/
+-rw-r--r--   0 q         (1000) q         (1000)     3239 2023-07-28 20:39:35.000000 xiver_gpt-0.0.1b1/xiver_gpt/XiverGPT.py
+-rw-r--r--   0 q         (1000) q         (1000)       31 2023-07-27 12:36:16.000000 xiver_gpt-0.0.1b1/xiver_gpt/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     1852 2023-07-28 18:19:03.000000 xiver_gpt-0.0.1b1/xiver_gpt/the_s_of_idea.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-07-28 20:40:10.785779 xiver_gpt-0.0.1b1/xiver_gpt.egg-info/
+-rw-r--r--   0 q         (1000) q         (1000)     1758 2023-07-28 20:40:10.000000 xiver_gpt-0.0.1b1/xiver_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)      277 2023-07-28 20:40:10.000000 xiver_gpt-0.0.1b1/xiver_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 q         (1000) q         (1000)        1 2023-07-28 20:40:10.000000 xiver_gpt-0.0.1b1/xiver_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 q         (1000) q         (1000)       13 2023-07-28 20:40:10.000000 xiver_gpt-0.0.1b1/xiver_gpt.egg-info/requires.txt
+-rw-r--r--   0 q         (1000) q         (1000)       10 2023-07-28 20:40:10.000000 xiver_gpt-0.0.1b1/xiver_gpt.egg-info/top_level.txt
```

### Comparing `xiver_gpt-0.0.1b0/LICENSE` & `xiver_gpt-0.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `xiver_gpt-0.0.1b0/PKG-INFO` & `xiver_gpt-0.0.1b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiver_gpt
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: The module Xiver team use to work with gpt.
 Home-page: https://github.com/xiver/xiver-gpt
 Download-URL: https://github.com/xiver/xiver-gpt/archive/master.zip
 Author: GigantPro
 Author-email: gigantpro2000@gmail.ru
 License: The GPLv3 License (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `xiver_gpt-0.0.1b0/README.rst` & `xiver_gpt-0.0.1b1/README.rst`

 * *Files identical despite different names*

### Comparing `xiver_gpt-0.0.1b0/pyproject.toml` & `xiver_gpt-0.0.1b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xiver_gpt"
-version = "0.0.1b"
+version = "0.0.1b1"
 description = "The module Xiver team use to work with gpt."
 
 authors = [
     "GigantPro <gigantpro2000@gmail.com>"
 ]
 maintainers = [
     "GigantPro <gigantpro2000@gmail.com>"
```

### Comparing `xiver_gpt-0.0.1b0/setup.py` & `xiver_gpt-0.0.1b1/setup.py`

 * *Files identical despite different names*

### Comparing `xiver_gpt-0.0.1b0/xiver_gpt/XiverGPT.py` & `xiver_gpt-0.0.1b1/xiver_gpt/XiverGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 import inspect
 
 import g4f
 
-from .exceptions import NoProvider
+from exceptions import NoProvider
 
 __all__ = ("XiverGPT",)
 
 
 providers_blacklist = (
     g4f.Provider.DfeHub,
 )
```

### Comparing `xiver_gpt-0.0.1b0/xiver_gpt/the_s_of_idea.py` & `xiver_gpt-0.0.1b1/xiver_gpt/the_s_of_idea.py`

 * *Files identical despite different names*

### Comparing `xiver_gpt-0.0.1b0/xiver_gpt.egg-info/PKG-INFO` & `xiver_gpt-0.0.1b1/xiver_gpt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiver-gpt
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: The module Xiver team use to work with gpt.
 Home-page: https://github.com/xiver/xiver-gpt
 Download-URL: https://github.com/xiver/xiver-gpt/archive/master.zip
 Author: GigantPro
 Author-email: gigantpro2000@gmail.ru
 License: The GPLv3 License (GPLv3)
 Classifier: Operating System :: OS Independent
```

