# Comparing `tmp/evenity-0.0.2.tar.gz` & `tmp/evenity-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evenity-0.0.2.tar", last modified: Fri Jul 28 23:23:39 2023, max compression
+gzip compressed data, was "evenity-0.0.3.tar", last modified: Sat Jul 29 11:50:24 2023, max compression
```

## Comparing `evenity-0.0.2.tar` & `evenity-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:23:39.308453 evenity-0.0.2/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 21:02:20.000000 evenity-0.0.2/LICENSE
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1463 2023-07-28 23:23:39.305119 evenity-0.0.2/PKG-INFO
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1008 2023-07-28 23:22:35.000000 evenity-0.0.2/README.md
--rw-r--r--   0 localghost  (1000) localghost  (1000)      531 2023-07-28 23:23:10.000000 evenity-0.0.2/pyproject.toml
--rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-07-28 23:23:39.308453 evenity-0.0.2/setup.cfg
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:23:39.305119 evenity-0.0.2/src/
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:23:39.305119 evenity-0.0.2/src/evenity/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/__init__.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      404 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/observable.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      446 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/observer.py
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:23:39.305119 evenity-0.0.2/src/evenity/plugins/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/plugins/__init__.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1327 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/plugins/ftp.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      714 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/plugins/kafka.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      632 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/plugins/shell.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      617 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/plugins/telegram.py
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:23:39.305119 evenity-0.0.2/src/evenity.egg-info/
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1463 2023-07-28 23:23:39.000000 evenity-0.0.2/src/evenity.egg-info/PKG-INFO
--rw-r--r--   0 localghost  (1000) localghost  (1000)      395 2023-07-28 23:23:39.000000 evenity-0.0.2/src/evenity.egg-info/SOURCES.txt
--rw-r--r--   0 localghost  (1000) localghost  (1000)        1 2023-07-28 23:23:39.000000 evenity-0.0.2/src/evenity.egg-info/dependency_links.txt
--rw-r--r--   0 localghost  (1000) localghost  (1000)        8 2023-07-28 23:23:39.000000 evenity-0.0.2/src/evenity.egg-info/top_level.txt
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-29 11:50:24.810745 evenity-0.0.3/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 21:02:20.000000 evenity-0.0.3/LICENSE
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1545 2023-07-29 11:50:24.810745 evenity-0.0.3/PKG-INFO
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1090 2023-07-29 11:49:18.000000 evenity-0.0.3/README.md
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      531 2023-07-29 11:50:13.000000 evenity-0.0.3/pyproject.toml
+-rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-07-29 11:50:24.810745 evenity-0.0.3/setup.cfg
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-29 11:50:24.810745 evenity-0.0.3/src/
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-29 11:50:24.810745 evenity-0.0.3/src/evenity/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.3/src/evenity/__init__.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      404 2023-07-28 23:22:35.000000 evenity-0.0.3/src/evenity/observable.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      594 2023-07-29 11:49:18.000000 evenity-0.0.3/src/evenity/observer.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-29 11:50:24.810745 evenity-0.0.3/src/evenity/plugins/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.3/src/evenity/plugins/__init__.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1327 2023-07-28 23:22:35.000000 evenity-0.0.3/src/evenity/plugins/ftp.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      714 2023-07-28 23:22:35.000000 evenity-0.0.3/src/evenity/plugins/kafka.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      632 2023-07-28 23:22:35.000000 evenity-0.0.3/src/evenity/plugins/shell.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      617 2023-07-28 23:22:35.000000 evenity-0.0.3/src/evenity/plugins/telegram.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-29 11:50:24.810745 evenity-0.0.3/src/evenity.egg-info/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1545 2023-07-29 11:50:24.000000 evenity-0.0.3/src/evenity.egg-info/PKG-INFO
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      395 2023-07-29 11:50:24.000000 evenity-0.0.3/src/evenity.egg-info/SOURCES.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        1 2023-07-29 11:50:24.000000 evenity-0.0.3/src/evenity.egg-info/dependency_links.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        8 2023-07-29 11:50:24.000000 evenity-0.0.3/src/evenity.egg-info/top_level.txt
```

### Comparing `evenity-0.0.2/PKG-INFO` & `evenity-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evenity
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pluggable event hooks library
 Author-email: Mario Baldi <mariobaldi.py@gmail.com>
 Project-URL: Homepage, https://github.com/baldimario/evenity
 Project-URL: Bug Tracker, https://github.com/baldimario/evenity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -15,15 +15,15 @@
 
 ## Installation
 ```sh
 pip install evenity
 ```
 
 ## Usage
-See examples folder
+See examples folder at [https://github.com/baldimario/evenity](https://github.com/baldimario/evenity)
 
 ### simple.py 
 This file contains an implementation of observers and observable
 It shows how simple is to implement your own observable and register all the observers as you want
 
 ## kafka.py
 This script contains an implementations of some listeners (observers) for the kafka plugin
```

### Comparing `evenity-0.0.2/pyproject.toml` & `evenity-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=42"]
 
 [project]
 name = "evenity"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Mario Baldi", email="mariobaldi.py@gmail.com" },
 ]
 description = "Pluggable event hooks library"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `evenity-0.0.2/src/evenity/plugins/ftp.py` & `evenity-0.0.3/src/evenity/plugins/ftp.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.2/src/evenity/plugins/kafka.py` & `evenity-0.0.3/src/evenity/plugins/kafka.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.2/src/evenity/plugins/shell.py` & `evenity-0.0.3/src/evenity/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.2/src/evenity/plugins/telegram.py` & `evenity-0.0.3/src/evenity/plugins/telegram.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.2/src/evenity.egg-info/PKG-INFO` & `evenity-0.0.3/src/evenity.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evenity
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pluggable event hooks library
 Author-email: Mario Baldi <mariobaldi.py@gmail.com>
 Project-URL: Homepage, https://github.com/baldimario/evenity
 Project-URL: Bug Tracker, https://github.com/baldimario/evenity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -15,15 +15,15 @@
 
 ## Installation
 ```sh
 pip install evenity
 ```
 
 ## Usage
-See examples folder
+See examples folder at [https://github.com/baldimario/evenity](https://github.com/baldimario/evenity)
 
 ### simple.py 
 This file contains an implementation of observers and observable
 It shows how simple is to implement your own observable and register all the observers as you want
 
 ## kafka.py
 This script contains an implementations of some listeners (observers) for the kafka plugin
```

