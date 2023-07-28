# Comparing `tmp/evenity-0.0.1.tar.gz` & `tmp/evenity-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evenity-0.0.1.tar", last modified: Fri Jul 28 23:10:17 2023, max compression
+gzip compressed data, was "evenity-0.0.2.tar", last modified: Fri Jul 28 23:23:39 2023, max compression
```

## Comparing `evenity-0.0.1.tar` & `evenity-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:10:17.835056 evenity-0.0.1/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 21:02:20.000000 evenity-0.0.1/LICENSE
--rw-r--r--   0 localghost  (1000) localghost  (1000)      494 2023-07-28 23:10:17.835056 evenity-0.0.1/PKG-INFO
--rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-07-28 23:03:45.000000 evenity-0.0.1/README.md
--rw-r--r--   0 localghost  (1000) localghost  (1000)      531 2023-07-28 23:09:01.000000 evenity-0.0.1/pyproject.toml
--rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-07-28 23:10:17.835056 evenity-0.0.1/setup.cfg
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:10:17.835056 evenity-0.0.1/src/
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:10:17.835056 evenity-0.0.1/src/evenity/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 20:46:23.000000 evenity-0.0.1/src/evenity/__init__.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      404 2023-07-28 20:48:05.000000 evenity-0.0.1/src/evenity/observable.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      446 2023-07-28 20:52:50.000000 evenity-0.0.1/src/evenity/observer.py
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:10:17.835056 evenity-0.0.1/src/evenity/plugins/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 20:53:47.000000 evenity-0.0.1/src/evenity/plugins/__init__.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1327 2023-07-28 20:56:54.000000 evenity-0.0.1/src/evenity/plugins/ftp.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      714 2023-07-28 20:56:18.000000 evenity-0.0.1/src/evenity/plugins/kafka.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      632 2023-07-28 20:54:49.000000 evenity-0.0.1/src/evenity/plugins/shell.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      617 2023-07-28 20:57:09.000000 evenity-0.0.1/src/evenity/plugins/telegram.py
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:10:17.835056 evenity-0.0.1/src/evenity.egg-info/
--rw-r--r--   0 localghost  (1000) localghost  (1000)      494 2023-07-28 23:10:17.000000 evenity-0.0.1/src/evenity.egg-info/PKG-INFO
--rw-r--r--   0 localghost  (1000) localghost  (1000)      395 2023-07-28 23:10:17.000000 evenity-0.0.1/src/evenity.egg-info/SOURCES.txt
--rw-r--r--   0 localghost  (1000) localghost  (1000)        1 2023-07-28 23:10:17.000000 evenity-0.0.1/src/evenity.egg-info/dependency_links.txt
--rw-r--r--   0 localghost  (1000) localghost  (1000)        8 2023-07-28 23:10:17.000000 evenity-0.0.1/src/evenity.egg-info/top_level.txt
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:23:39.308453 evenity-0.0.2/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 21:02:20.000000 evenity-0.0.2/LICENSE
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1463 2023-07-28 23:23:39.305119 evenity-0.0.2/PKG-INFO
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1008 2023-07-28 23:22:35.000000 evenity-0.0.2/README.md
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      531 2023-07-28 23:23:10.000000 evenity-0.0.2/pyproject.toml
+-rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-07-28 23:23:39.308453 evenity-0.0.2/setup.cfg
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:23:39.305119 evenity-0.0.2/src/
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:23:39.305119 evenity-0.0.2/src/evenity/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/__init__.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      404 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/observable.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      446 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/observer.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:23:39.305119 evenity-0.0.2/src/evenity/plugins/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/plugins/__init__.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1327 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/plugins/ftp.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      714 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/plugins/kafka.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      632 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/plugins/shell.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      617 2023-07-28 23:22:35.000000 evenity-0.0.2/src/evenity/plugins/telegram.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:23:39.305119 evenity-0.0.2/src/evenity.egg-info/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1463 2023-07-28 23:23:39.000000 evenity-0.0.2/src/evenity.egg-info/PKG-INFO
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      395 2023-07-28 23:23:39.000000 evenity-0.0.2/src/evenity.egg-info/SOURCES.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        1 2023-07-28 23:23:39.000000 evenity-0.0.2/src/evenity.egg-info/dependency_links.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        8 2023-07-28 23:23:39.000000 evenity-0.0.2/src/evenity.egg-info/top_level.txt
```

### Comparing `evenity-0.0.1/pyproject.toml` & `evenity-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=42"]
 
 [project]
 name = "evenity"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mario Baldi", email="mariobaldi.py@gmail.com" },
 ]
 description = "Pluggable event hooks library"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `evenity-0.0.1/src/evenity/plugins/ftp.py` & `evenity-0.0.2/src/evenity/plugins/ftp.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.1/src/evenity/plugins/kafka.py` & `evenity-0.0.2/src/evenity/plugins/kafka.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.1/src/evenity/plugins/shell.py` & `evenity-0.0.2/src/evenity/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.1/src/evenity/plugins/telegram.py` & `evenity-0.0.2/src/evenity/plugins/telegram.py`

 * *Files identical despite different names*

