# Comparing `tmp/py-helper-mod-0.0.49.tar.gz` & `tmp/py-helper-mod-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-helper-mod-0.0.49.tar", last modified: Fri Jul 21 15:00:41 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.50.tar", last modified: Sat Jul 29 18:58:42 2023, max compression
```

## Comparing `py-helper-mod-0.0.49.tar` & `py-helper-mod-0.0.50.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-21 15:00:41.802273 py-helper-mod-0.0.49/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.49/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-21 15:00:41.802273 py-helper-mod-0.0.49/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.49/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    91349 2023-07-21 14:58:42.000000 py-helper-mod-0.0.49/py_helper.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-21 15:00:41.798273 py-helper-mod-0.0.49/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-21 15:00:41.000000 py-helper-mod-0.0.49/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-21 15:00:41.000000 py-helper-mod-0.0.49/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-21 15:00:41.000000 py-helper-mod-0.0.49/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-21 15:00:41.000000 py-helper-mod-0.0.49/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.49/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-21 15:00:41.802273 py-helper-mod-0.0.49/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.49/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-29 18:58:42.348514 py-helper-mod-0.0.50/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.50/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-29 18:58:42.348514 py-helper-mod-0.0.50/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.50/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    91802 2023-07-29 18:56:58.000000 py-helper-mod-0.0.50/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-29 18:58:42.348514 py-helper-mod-0.0.50/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-29 18:58:42.000000 py-helper-mod-0.0.50/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-29 18:58:42.000000 py-helper-mod-0.0.50/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-29 18:58:42.000000 py-helper-mod-0.0.50/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-29 18:58:42.000000 py-helper-mod-0.0.50/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.50/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-29 18:58:42.348514 py-helper-mod-0.0.50/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.50/setup.py
```

### Comparing `py-helper-mod-0.0.49/LICENSE` & `py-helper-mod-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.49/PKG-INFO` & `py-helper-mod-0.0.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.49
+Version: 0.0.50
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.49/py_helper.py` & `py-helper-mod-0.0.50/py_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # The Usual Suspects
 # import keyser_soze
 import os, sys, io, platform
 import shutil, subprocess, getpass
 import random
 import math
 
+# For some decorator action
+import functools
+
 # Reg Exprs... I have the POWER!!!!!!!!!
 import re
 
 # For Viewing Stoof
 import pydoc
 
 # For Shell Stoof
@@ -1181,15 +1184,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,49)
+VERSION=(0,0,50)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1439,15 +1442,15 @@
 def IsDebugLabelEnabled(dbglabel):
 	"""Check if Debug Label is Enabled"""
 
 	global DebugLabels, DebugLabelExists
 
 	enabled = not DebugLabelExists
 
-	dbglb = None
+	dbglb = dbglabel
 
 	if DebugLabels is not None and dbglabel is not None:
 		if type(dbglabel) is str and dbglabel in DebugLabels:
 			enabled = DebugLabels[dbglabel]
 			dbglb = dbglabel
 		elif type(dbglabel) is list:
 			for lbl in dbglabel:
@@ -1542,14 +1545,35 @@
 	message = f"Entering {msg}"
 
 	if callerframe == None:
 		callerframe = inspect.currentframe().f_back
 
 	return DbgMsg(message,func=func,prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,interval_stamp=interval_stamp,dbglabel=dbglabel)
 
+# Get Debug Names (Block, Label) Lambda
+DbgNames = lambda object: [ object.__qualname__, object.__name__ ]
+
+# DebugMe Decorator
+def DebugMe(func):
+	"""Debug Decorator For Enter/Exit Messages"""
+
+	@functools.wraps(func)
+	def wrapper(*args,**kwargs):
+		dbgblk, dbglb = DbgNames(func)
+
+		DbgEnter(dbgblk,dbglb)
+
+		results = func(*args,**kwargs)
+
+		DbgExit(dbgblk,dbglb)
+
+		return results
+
+	return wrapper
+
 # Block Exit Debug Messages
 def DbgExit(msg,dbglabel=None,func=None,prefix="<--",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None):
 	"""DbgMsg Helper Function Output a message when exitting a code block"""
 
 	message = f"Exitting {msg}"
 
 	if callerframe == None:
```

### Comparing `py-helper-mod-0.0.49/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.50/py_helper_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.49
+Version: 0.0.50
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.49/setup.cfg` & `py-helper-mod-0.0.50/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.49
+version = 0.0.50
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

