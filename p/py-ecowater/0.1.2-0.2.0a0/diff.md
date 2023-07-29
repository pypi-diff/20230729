# Comparing `tmp/py_ecowater-0.1.2.tar.gz` & `tmp/py_ecowater-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ecowater-0.1.2.tar", last modified: Sat Jul 29 20:37:06 2023, max compression
+gzip compressed data, was "py_ecowater-0.2.0a0.tar", last modified: Sat Jul 29 20:20:12 2023, max compression
```

## Comparing `py_ecowater-0.1.2.tar` & `py_ecowater-0.2.0a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:37:06.456256 py_ecowater-0.1.2/
--rw-r--r--   0 dbunker    (501) staff       (20)     1071 2023-07-29 15:30:43.000000 py_ecowater-0.1.2/LICENSE
--rw-r--r--   0 dbunker    (501) staff       (20)     6757 2023-07-29 20:37:06.456308 py_ecowater-0.1.2/PKG-INFO
--rw-r--r--   0 dbunker    (501) staff       (20)     6233 2023-07-29 20:29:59.000000 py_ecowater-0.1.2/README.md
--rw-r--r--   0 dbunker    (501) staff       (20)        5 2023-07-29 20:29:59.000000 py_ecowater-0.1.2/VERSION.txt
--rw-r--r--   0 dbunker    (501) staff       (20)       85 2022-05-29 21:43:28.000000 py_ecowater-0.1.2/pyproject.toml
--rw-r--r--   0 dbunker    (501) staff       (20)      661 2023-07-29 20:37:06.456553 py_ecowater-0.1.2/setup.cfg
-drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:37:06.453473 py_ecowater-0.1.2/src/
-drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:37:06.455413 py_ecowater-0.1.2/src/py_ecowater/
--rw-r--r--   0 dbunker    (501) staff       (20)      101 2023-07-29 20:29:59.000000 py_ecowater-0.1.2/src/py_ecowater/__init__.py
--rw-r--r--   0 dbunker    (501) staff       (20)      875 2022-06-05 22:39:36.000000 py_ecowater-0.1.2/src/py_ecowater/constants.py
--rw-r--r--   0 dbunker    (501) staff       (20)     4641 2023-07-29 20:29:59.000000 py_ecowater-0.1.2/src/py_ecowater/ecowater_client.py
--rw-r--r--   0 dbunker    (501) staff       (20)        0 2022-06-03 02:53:26.000000 py_ecowater-0.1.2/src/py_ecowater/exception.py
--rw-r--r--   0 dbunker    (501) staff       (20)    27962 2023-07-29 20:29:59.000000 py_ecowater-0.1.2/src/py_ecowater/model.py
-drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:37:06.456135 py_ecowater-0.1.2/src/py_ecowater.egg-info/
--rw-r--r--   0 dbunker    (501) staff       (20)     6757 2023-07-29 20:37:06.000000 py_ecowater-0.1.2/src/py_ecowater.egg-info/PKG-INFO
--rw-r--r--   0 dbunker    (501) staff       (20)      356 2023-07-29 20:37:06.000000 py_ecowater-0.1.2/src/py_ecowater.egg-info/SOURCES.txt
--rw-r--r--   0 dbunker    (501) staff       (20)        1 2023-07-29 20:37:06.000000 py_ecowater-0.1.2/src/py_ecowater.egg-info/dependency_links.txt
--rw-r--r--   0 dbunker    (501) staff       (20)       12 2023-07-29 20:37:06.000000 py_ecowater-0.1.2/src/py_ecowater.egg-info/top_level.txt
+drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:20:12.773542 py_ecowater-0.2.0a0/
+-rw-r--r--   0 dbunker    (501) staff       (20)     1071 2023-07-29 15:30:43.000000 py_ecowater-0.2.0a0/LICENSE
+-rw-r--r--   0 dbunker    (501) staff       (20)     6760 2023-07-29 20:20:12.773600 py_ecowater-0.2.0a0/PKG-INFO
+-rw-r--r--   0 dbunker    (501) staff       (20)     6234 2023-07-29 19:44:33.000000 py_ecowater-0.2.0a0/README.md
+-rw-r--r--   0 dbunker    (501) staff       (20)        6 2023-07-29 19:44:33.000000 py_ecowater-0.2.0a0/VERSION.txt
+-rw-r--r--   0 dbunker    (501) staff       (20)       85 2022-05-29 21:43:28.000000 py_ecowater-0.2.0a0/pyproject.toml
+-rw-r--r--   0 dbunker    (501) staff       (20)      661 2023-07-29 20:20:12.773852 py_ecowater-0.2.0a0/setup.cfg
+drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:20:12.771825 py_ecowater-0.2.0a0/src/
+drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:20:12.772968 py_ecowater-0.2.0a0/src/py_ecowater/
+-rw-r--r--   0 dbunker    (501) staff       (20)      101 2023-07-29 20:14:27.000000 py_ecowater-0.2.0a0/src/py_ecowater/__init__.py
+-rw-r--r--   0 dbunker    (501) staff       (20)      875 2022-06-05 22:39:36.000000 py_ecowater-0.2.0a0/src/py_ecowater/constants.py
+-rw-r--r--   0 dbunker    (501) staff       (20)     4641 2023-07-29 20:13:59.000000 py_ecowater-0.2.0a0/src/py_ecowater/ecowater_client.py
+-rw-r--r--   0 dbunker    (501) staff       (20)        0 2022-06-03 02:53:26.000000 py_ecowater-0.2.0a0/src/py_ecowater/exception.py
+-rw-r--r--   0 dbunker    (501) staff       (20)    27962 2023-07-29 20:13:37.000000 py_ecowater-0.2.0a0/src/py_ecowater/model.py
+drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:20:12.773443 py_ecowater-0.2.0a0/src/py_ecowater.egg-info/
+-rw-r--r--   0 dbunker    (501) staff       (20)     6760 2023-07-29 20:20:12.000000 py_ecowater-0.2.0a0/src/py_ecowater.egg-info/PKG-INFO
+-rw-r--r--   0 dbunker    (501) staff       (20)      356 2023-07-29 20:20:12.000000 py_ecowater-0.2.0a0/src/py_ecowater.egg-info/SOURCES.txt
+-rw-r--r--   0 dbunker    (501) staff       (20)        1 2023-07-29 20:20:12.000000 py_ecowater-0.2.0a0/src/py_ecowater.egg-info/dependency_links.txt
+-rw-r--r--   0 dbunker    (501) staff       (20)       12 2023-07-29 20:20:12.000000 py_ecowater-0.2.0a0/src/py_ecowater.egg-info/top_level.txt
```

### Comparing `py_ecowater-0.1.2/LICENSE` & `py_ecowater-0.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ecowater-0.1.2/PKG-INFO` & `py_ecowater-0.2.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: py_ecowater
-Version: 0.1.2
+Version: 0.2.0a0
 Summary: A python package for interacting with the Ecowater API
 Home-page: https://github.com/ejsuncy/py_ecowater
 Author: Dan Bunker
 Author-email: dbunked@gmail.com
 Project-URL: Bug Tracker, https://github.com/ejsuncy/py_ecowater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py_ecowater
-![Current Version](https://img.shields.io/badge/Version-0.1.2-brightgreen)
+![Current Version](https://img.shields.io/badge/Version-0.2.0a-brightgreen)
 
 A python library for getting device data from Ecowater API for devices such as the Rheem RHW42 water softener, which 
 provides WI-FI connectivity via the iQua app.
 
 ## Installation
 
 ```bash
```

### Comparing `py_ecowater-0.1.2/README.md` & `py_ecowater-0.2.0a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # py_ecowater
-![Current Version](https://img.shields.io/badge/Version-0.1.2-brightgreen)
+![Current Version](https://img.shields.io/badge/Version-0.2.0a-brightgreen)
 
 A python library for getting device data from Ecowater API for devices such as the Rheem RHW42 water softener, which 
 provides WI-FI connectivity via the iQua app.
 
 ## Installation
 
 ```bash
```

### Comparing `py_ecowater-0.1.2/setup.cfg` & `py_ecowater-0.2.0a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `py_ecowater-0.1.2/src/py_ecowater/constants.py` & `py_ecowater-0.2.0a0/src/py_ecowater/constants.py`

 * *Files identical despite different names*

### Comparing `py_ecowater-0.1.2/src/py_ecowater/ecowater_client.py` & `py_ecowater-0.2.0a0/src/py_ecowater/ecowater_client.py`

 * *Files identical despite different names*

### Comparing `py_ecowater-0.1.2/src/py_ecowater/model.py` & `py_ecowater-0.2.0a0/src/py_ecowater/model.py`

 * *Files identical despite different names*

### Comparing `py_ecowater-0.1.2/src/py_ecowater.egg-info/PKG-INFO` & `py_ecowater-0.2.0a0/src/py_ecowater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: py-ecowater
-Version: 0.1.2
+Version: 0.2.0a0
 Summary: A python package for interacting with the Ecowater API
 Home-page: https://github.com/ejsuncy/py_ecowater
 Author: Dan Bunker
 Author-email: dbunked@gmail.com
 Project-URL: Bug Tracker, https://github.com/ejsuncy/py_ecowater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py_ecowater
-![Current Version](https://img.shields.io/badge/Version-0.1.2-brightgreen)
+![Current Version](https://img.shields.io/badge/Version-0.2.0a-brightgreen)
 
 A python library for getting device data from Ecowater API for devices such as the Rheem RHW42 water softener, which 
 provides WI-FI connectivity via the iQua app.
 
 ## Installation
 
 ```bash
```

