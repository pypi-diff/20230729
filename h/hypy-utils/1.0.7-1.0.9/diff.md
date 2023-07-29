# Comparing `tmp/hypy_utils-1.0.7.tar.gz` & `tmp/hypy_utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypy_utils-1.0.7.tar", last modified: Mon Apr 11 05:43:31 2022, max compression
+gzip compressed data, was "hypy_utils-1.0.9.tar", last modified: Sun Jul  3 06:24:17 2022, max compression
```

## Comparing `hypy_utils-1.0.7.tar` & `hypy_utils-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2022-04-11 05:43:31.800288 hypy_utils-1.0.7/
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1069 2022-04-09 04:12:55.000000 hypy_utils-1.0.7/LICENSE
--rw-r--r--   0 azalea    (1000) azalea    (1000)      629 2022-04-11 05:43:31.800288 hypy_utils-1.0.7/PKG-INFO
--rw-r--r--   0 azalea    (1000) azalea    (1000)       36 2022-04-09 04:12:55.000000 hypy_utils-1.0.7/README.md
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2022-04-11 05:43:31.800288 hypy_utils-1.0.7/hypy_utils/
--rw-r--r--   0 azalea    (1000) azalea    (1000)     5470 2022-04-11 05:40:28.000000 hypy_utils-1.0.7/hypy_utils/__init__.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      107 2022-04-11 02:11:07.000000 hypy_utils-1.0.7/hypy_utils/__main__.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      527 2022-04-11 05:42:57.000000 hypy_utils-1.0.7/hypy_utils/serializer.py
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2022-04-11 05:43:31.800288 hypy_utils-1.0.7/hypy_utils.egg-info/
--rw-r--r--   0 azalea    (1000) azalea    (1000)      629 2022-04-11 05:43:31.000000 hypy_utils-1.0.7/hypy_utils.egg-info/PKG-INFO
--rw-r--r--   0 azalea    (1000) azalea    (1000)      270 2022-04-11 05:43:31.000000 hypy_utils-1.0.7/hypy_utils.egg-info/SOURCES.txt
--rw-r--r--   0 azalea    (1000) azalea    (1000)        1 2022-04-11 05:43:31.000000 hypy_utils-1.0.7/hypy_utils.egg-info/dependency_links.txt
--rw-r--r--   0 azalea    (1000) azalea    (1000)       57 2022-04-11 05:43:31.000000 hypy_utils-1.0.7/hypy_utils.egg-info/entry_points.txt
--rw-r--r--   0 azalea    (1000) azalea    (1000)       11 2022-04-11 05:43:31.000000 hypy_utils-1.0.7/hypy_utils.egg-info/top_level.txt
--rw-r--r--   0 azalea    (1000) azalea    (1000)       38 2022-04-11 05:43:31.800288 hypy_utils-1.0.7/setup.cfg
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1138 2022-04-11 02:14:23.000000 hypy_utils-1.0.7/setup.py
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2022-07-03 06:24:17.374337 hypy_utils-1.0.9/
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)     1069 2022-04-09 04:12:55.000000 hypy_utils-1.0.9/LICENSE
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      629 2022-07-03 06:24:17.374337 hypy_utils-1.0.9/PKG-INFO
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)       36 2022-04-09 04:12:55.000000 hypy_utils-1.0.9/README.md
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2022-07-03 06:24:17.374337 hypy_utils-1.0.9/hypy_utils/
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)     5876 2022-07-03 06:24:16.000000 hypy_utils-1.0.9/hypy_utils/__init__.py
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)      107 2022-04-11 02:11:07.000000 hypy_utils-1.0.9/hypy_utils/__main__.py
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)     1734 2022-07-03 06:17:12.000000 hypy_utils-1.0.9/hypy_utils/scientific_utils.py
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)      684 2022-04-11 06:15:43.000000 hypy_utils-1.0.9/hypy_utils/serializer.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1352 2022-07-03 06:22:21.000000 hypy_utils-1.0.9/hypy_utils/tqdm_utils.py
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2022-07-03 06:24:17.374337 hypy_utils-1.0.9/hypy_utils.egg-info/
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)      629 2022-07-03 06:24:17.000000 hypy_utils-1.0.9/hypy_utils.egg-info/PKG-INFO
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)      326 2022-07-03 06:24:17.000000 hypy_utils-1.0.9/hypy_utils.egg-info/SOURCES.txt
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)        1 2022-07-03 06:24:17.000000 hypy_utils-1.0.9/hypy_utils.egg-info/dependency_links.txt
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)       57 2022-07-03 06:24:17.000000 hypy_utils-1.0.9/hypy_utils.egg-info/entry_points.txt
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)       11 2022-07-03 06:24:17.000000 hypy_utils-1.0.9/hypy_utils.egg-info/top_level.txt
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       38 2022-07-03 06:24:17.374337 hypy_utils-1.0.9/setup.cfg
+-rwxrwxr-x   0 azalea    (1000) azalea    (1000)     1138 2022-04-11 02:14:23.000000 hypy_utils-1.0.9/setup.py
```

### Comparing `hypy_utils-1.0.7/LICENSE` & `hypy_utils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hypy_utils-1.0.7/PKG-INFO` & `hypy_utils-1.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypy_utils
-Version: 1.0.7
+Version: 1.0.9
 Summary: Python utility functions for HyDEV
 Home-page: https://github.com/hykilpikonna/HyPyUtils
 Author: Azalea Gui
 Author-email: me@hydev.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hypy_utils-1.0.7/hypy_utils/__init__.py` & `hypy_utils-1.0.9/hypy_utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
-__version__ = "1.0.7"
+__version__ = "1.0.9"
 
 import dataclasses
 import hashlib
 import json
 import time
 from datetime import datetime, date
 from pathlib import Path
-from typing import Union
+from typing import Union, Callable
 
 
 def ansi_rgb(r: int, g: int, b: int, foreground: bool = True) -> str:
     """
     Convert rgb color into ANSI escape code format
 
     :param r:
@@ -198,7 +198,20 @@
         return t
 
     def log(self, *args):
         print(f'{self.elapsed():.0f}ms', *args)
 
     def reset(self):
         self.start = time.time_ns()
+
+
+def mem(var: str):
+    print(f'Memory usage for {var}: {eval(f"sys.getsizeof({var})") / 1024:.1f}KB')
+
+
+def run_time(func: Callable, *args, **kwargs):
+    name = getattr(func, '__name__', 'function')
+    start = time.time_ns()
+    iter = kwargs.pop('iter', 10)
+    _ = [func(*args, **kwargs) for _ in range(iter)]
+    ms = (time.time_ns() - start) / 1e6
+    print(f'RT {name:30} {ms:6.1f} ms')
```

### Comparing `hypy_utils-1.0.7/hypy_utils.egg-info/PKG-INFO` & `hypy_utils-1.0.9/hypy_utils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypy-utils
-Version: 1.0.7
+Version: 1.0.9
 Summary: Python utility functions for HyDEV
 Home-page: https://github.com/hykilpikonna/HyPyUtils
 Author: Azalea Gui
 Author-email: me@hydev.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hypy_utils-1.0.7/setup.py` & `hypy_utils-1.0.9/setup.py`

 * *Files identical despite different names*

