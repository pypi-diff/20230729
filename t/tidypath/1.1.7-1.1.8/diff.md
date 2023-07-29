# Comparing `tmp/tidypath-1.1.7.tar.gz` & `tmp/tidypath-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.1.7.tar", last modified: Sat Jul  1 08:07:41 2023, max compression
+gzip compressed data, was "tidypath-1.1.8.tar", last modified: Sat Jul 29 08:55:02 2023, max compression
```

## Comparing `tidypath-1.1.7.tar` & `tidypath-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-07-01 08:07:41.514871 tidypath-1.1.7/
--rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.1.7/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-07-01 08:07:41.514871 tidypath-1.1.7/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.1.7/README.md
--rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2023-07-01 08:07:41.518204 tidypath-1.1.7/setup.cfg
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2023-07-01 08:07:09.000000 tidypath-1.1.7/setup.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-07-01 08:07:41.514871 tidypath-1.1.7/tidypath/
--rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2023-06-08 21:46:44.000000 tidypath-1.1.7/tidypath/__init__.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.1.7/tidypath/_helper.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     5054 2023-06-08 21:46:44.000000 tidypath-1.1.7/tidypath/config.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    11950 2023-07-01 08:06:21.000000 tidypath-1.1.7/tidypath/decorators.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     6165 2023-07-01 08:06:57.000000 tidypath-1.1.7/tidypath/fmt.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.1.7/tidypath/inspection.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    13171 2023-06-30 17:40:49.000000 tidypath-1.1.7/tidypath/paths.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.1.7/tidypath/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-07-01 08:07:41.514871 tidypath-1.1.7/tidypath.egg-info/
--rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2023-07-01 08:07:41.000000 tidypath-1.1.7/tidypath.egg-info/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2023-07-01 08:07:41.000000 tidypath-1.1.7/tidypath.egg-info/SOURCES.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2023-07-01 08:07:41.000000 tidypath-1.1.7/tidypath.egg-info/dependency_links.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2023-07-01 08:07:41.000000 tidypath-1.1.7/tidypath.egg-info/requires.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2023-07-01 08:07:41.000000 tidypath-1.1.7/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-07-29 08:55:02.864940 tidypath-1.1.8/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.1.8/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-07-29 08:55:02.864940 tidypath-1.1.8/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.1.8/README.md
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2023-07-29 08:55:02.868273 tidypath-1.1.8/setup.cfg
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2023-07-29 08:54:52.000000 tidypath-1.1.8/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-07-29 08:55:02.864940 tidypath-1.1.8/tidypath/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2023-06-08 21:46:44.000000 tidypath-1.1.8/tidypath/__init__.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.1.8/tidypath/_helper.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     5054 2023-06-08 21:46:44.000000 tidypath-1.1.8/tidypath/config.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    11990 2023-07-29 08:54:37.000000 tidypath-1.1.8/tidypath/decorators.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     6165 2023-07-01 08:06:57.000000 tidypath-1.1.8/tidypath/fmt.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.1.8/tidypath/inspection.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    13697 2023-07-14 09:49:41.000000 tidypath-1.1.8/tidypath/paths.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.1.8/tidypath/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-07-29 08:55:02.864940 tidypath-1.1.8/tidypath.egg-info/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2023-07-29 08:55:02.000000 tidypath-1.1.8/tidypath.egg-info/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2023-07-29 08:55:02.000000 tidypath-1.1.8/tidypath.egg-info/SOURCES.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2023-07-29 08:55:02.000000 tidypath-1.1.8/tidypath.egg-info/dependency_links.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2023-07-29 08:55:02.000000 tidypath-1.1.8/tidypath.egg-info/requires.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2023-07-29 08:55:02.000000 tidypath-1.1.8/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.1.7/LICENSE.md` & `tidypath-1.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.7/PKG-INFO` & `tidypath-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.7
+Version: 1.1.8
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.1.7/README.md` & `tidypath-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.7/setup.py` & `tidypath-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.1.7',
+    version='1.1.8',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.1.7/tidypath/_helper.py` & `tidypath-1.1.8/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.7/tidypath/config.py` & `tidypath-1.1.8/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.7/tidypath/decorators.py` & `tidypath-1.1.8/tidypath/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import warnings
 import os
 from pathlib import Path
 from functools import wraps
 from collections.abc import Iterable
 from importlib.util import find_spec
 from ._helper import NoFigure
+from lzma import LZMAError
 if find_spec("plotly") is None:
     plotly_figure = NoFigure
 else:
     from plotly.graph_objs._figure import Figure as plotly_figure
 if find_spec("matplotlib") is None:
     mpl_figure = NoFigure
 else:
@@ -93,15 +94,15 @@
             filename_too_long = len(saving_path) > max_str_length
             if filename_too_long:
                 saving_path = hash_path(saving_path)
 
             if Path(saving_path).exists() and not overwrite:
                 try:
                     result = getattr(storage, f"load_{ext}")(saving_path, **load_opts)
-                except EOFError:
+                except EOFError or LZMAError:
                     warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
                     result = func(*args, **kwargs)
                     getattr(storage, f"save_{ext}")(result, saving_path, **save_opts)
             else:
                 if filename_too_long:
                     warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
                 result = func(*args, **kwargs)
```

### Comparing `tidypath-1.1.7/tidypath/fmt.py` & `tidypath-1.1.8/tidypath/fmt.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.7/tidypath/inspection.py` & `tidypath-1.1.8/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.7/tidypath/paths.py` & `tidypath-1.1.8/tidypath/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,38 @@
 (1) is the most appropiate.
 """
 import os
 import sys
 import inspect
 import warnings
 import numpy as np
+import pandas as pd
+import datetime
 from copy import deepcopy
 from collections.abc import Iterable
 from pathlib import Path
 from .fmt import dict_to_id, encoder, hash_string
 from .inspection import get_class_that_defined_method
 
 dataDir = "data"
 figDir = "figs"
 
+def time_since_last_update(parent_dir, ext='lzma'):
+    """
+    Returns a pandas Series with the time since last update of each file in parent_dir.
+    """
+    t = {}
+    today = datetime.datetime.now()
+    for f in os.listdir(parent_dir):
+        if ext is None or f.endswith(ext):
+            path = os.path.join(parent_dir, f)
+            last_update = today - pd.to_datetime(Path(path).stat().st_mtime, unit='s')
+            t[path] = last_update
+    return pd.Series(t).sort_values()
+
 def hash_path(path):
     """
     Hashes the filename (keeping the extension and parentDir) of a path.
     """
     parentDir = os.path.dirname(path)
     filename = os.path.basename(path)
     filename, ext = os.path.splitext(filename)
```

### Comparing `tidypath-1.1.7/tidypath/storage.py` & `tidypath-1.1.8/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.7/tidypath.egg-info/PKG-INFO` & `tidypath-1.1.8/tidypath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.7
+Version: 1.1.8
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

