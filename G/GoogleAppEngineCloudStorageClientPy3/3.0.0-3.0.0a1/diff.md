# Comparing `tmp/GoogleAppEngineCloudStorageClientPy3-3.0.0.tar.gz` & `tmp/GoogleAppEngineCloudStorageClientPy3-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleAppEngineCloudStorageClientPy3-3.0.0.tar", last modified: Sat Jul 29 20:04:48 2023, max compression
+gzip compressed data, was "GoogleAppEngineCloudStorageClientPy3-3.0.0a1.tar", last modified: Tue Jul 25 21:31:34 2023, max compression
```

## Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0.tar` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 20:04:48.472228 GoogleAppEngineCloudStorageClientPy3-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-07-29 20:04:48.472228 GoogleAppEngineCloudStorageClientPy3-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-29 20:04:48.476228 GoogleAppEngineCloudStorageClientPy3-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 20:04:48.468228 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 20:04:48.472228 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/GoogleAppEngineCloudStorageClientPy3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-07-29 20:04:48.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/GoogleAppEngineCloudStorageClientPy3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-07-29 20:04:48.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/GoogleAppEngineCloudStorageClientPy3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-29 20:04:48.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/GoogleAppEngineCloudStorageClientPy3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-29 20:04:48.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/GoogleAppEngineCloudStorageClientPy3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-29 20:04:48.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/GoogleAppEngineCloudStorageClientPy3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 20:04:48.472228 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12068 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    23653 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/cloudstorage_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12530 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 20:04:48.472228 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/port/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18778 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/port/cloudstorage_stub.py
--rw-r--r--   0 runner    (1001) docker     (122)    14692 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/port/stub_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/port/testbed.py
--rw-r--r--   0 runner    (1001) docker     (122)     9120 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    28792 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/storage_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-07-29 20:04:38.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/test_utils.py
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-25 21:31:34.667059 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/
+-rw-r--r--   0 kamilturek   (501) staff       (20)    11324 2023-07-21 17:10:13.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/LICENSE
+-rw-r--r--   0 kamilturek   (501) staff       (20)     1303 2023-07-25 21:31:34.666902 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/PKG-INFO
+-rw-r--r--   0 kamilturek   (501) staff       (20)      461 2023-07-25 21:27:45.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/README.md
+-rw-r--r--   0 kamilturek   (501) staff       (20)     1279 2023-07-25 21:25:44.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/pyproject.toml
+-rw-r--r--   0 kamilturek   (501) staff       (20)       38 2023-07-25 21:31:34.667097 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/setup.cfg
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-25 21:31:34.663346 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-25 21:31:34.664566 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/GoogleAppEngineCloudStorageClientPy3.egg-info/
+-rw-r--r--   0 kamilturek   (501) staff       (20)     1303 2023-07-25 21:31:34.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/GoogleAppEngineCloudStorageClientPy3.egg-info/PKG-INFO
+-rw-r--r--   0 kamilturek   (501) staff       (20)      744 2023-07-25 21:31:34.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/GoogleAppEngineCloudStorageClientPy3.egg-info/SOURCES.txt
+-rw-r--r--   0 kamilturek   (501) staff       (20)        1 2023-07-25 21:31:34.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/GoogleAppEngineCloudStorageClientPy3.egg-info/dependency_links.txt
+-rw-r--r--   0 kamilturek   (501) staff       (20)       40 2023-07-25 21:31:34.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/GoogleAppEngineCloudStorageClientPy3.egg-info/requires.txt
+-rw-r--r--   0 kamilturek   (501) staff       (20)       13 2023-07-25 21:31:34.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/GoogleAppEngineCloudStorageClientPy3.egg-info/top_level.txt
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-25 21:31:34.666027 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/
+-rw-r--r--   0 kamilturek   (501) staff       (20)      995 2023-07-23 11:50:32.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/__init__.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)    12068 2023-07-23 12:22:39.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/api_utils.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)    23653 2023-07-24 21:20:49.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/cloudstorage_api.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)    12530 2023-07-24 21:23:45.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/common.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)     3989 2023-07-23 11:51:09.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/errors.py
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-25 21:31:34.666638 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/port/
+-rw-r--r--   0 kamilturek   (501) staff       (20)        0 2023-07-23 12:01:53.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/port/__init__.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)    18778 2023-07-24 21:12:07.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/port/cloudstorage_stub.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)    14692 2023-07-24 21:20:15.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/port/stub_dispatcher.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)     1296 2023-07-24 21:12:04.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/port/testbed.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)     9120 2023-07-23 12:21:44.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/rest_api.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)    28792 2023-07-24 21:29:50.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/storage_api.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)      849 2023-07-22 20:24:52.000000 GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/test_utils.py
```

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/LICENSE` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/PKG-INFO` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 Metadata-Version: 2.1
 Name: GoogleAppEngineCloudStorageClientPy3
-Version: 3.0.0
+Version: 3.0.0a1
 Summary: This library is the preferred way of accessing Google
 Author-email: Kamil Turek <kamil.turek@hotmail.com>
 License: Apache-2.0
 Keywords: google,app engine,cloud storage
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Google App Engine Cloud Storage Client for Python 3
 
-[![PyPi version](https://img.shields.io/pypi/v/GoogleAppEngineCloudStorageClientPy3.svg)](https://pypi.python.org/pypi/GoogleAppEngineCloudStorageClientPy3/)
-[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
 [![Test](https://github.com/kamilturek/appengine-gcs-client-py3/actions/workflows/test.yaml/badge.svg)](https://github.com/kamilturek/appengine-gcs-client-py3/actions/workflows/test.yaml)
 
 This is a port of the [GoogleAppEngineCloudStorageClient](https://pypi.org/project/GoogleAppEngineCloudStorageClient/)
 package to Python 3.
 
 ## Installation
 
 ```sh
 pip install GoogleAppEngineCloudStorageClientPy3
 ```
-
-## Demo
-
-See the [demo](./demo/) application for sample usage.
```

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/pyproject.toml` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "GoogleAppEngineCloudStorageClientPy3"
-version = "3.0.0"
+version = "3.0.0a1"
 authors = [{name = "Kamil Turek", email = "kamil.turek@hotmail.com"}]
 description = """
 This library is the preferred way of accessing Google
 Cloud Storage from App Engine. It was designed to
 replace the Files API. As a result it contains much
 of the same functionality (streaming reads and writes but
 not the complete set of GCS APIs). It also provides key
@@ -16,22 +16,26 @@
 keywords = ["google", "app engine", "cloud storage"]
 license = {text = "Apache-2.0"}
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Topic :: Internet",
 ]
 dependencies = [
     "appengine-python-standard"
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
+
+[project.optional-dependencies]
+dev = [
+    "pytest"
+]
```

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/GoogleAppEngineCloudStorageClientPy3.egg-info/PKG-INFO` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/GoogleAppEngineCloudStorageClientPy3.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 Metadata-Version: 2.1
 Name: GoogleAppEngineCloudStorageClientPy3
-Version: 3.0.0
+Version: 3.0.0a1
 Summary: This library is the preferred way of accessing Google
 Author-email: Kamil Turek <kamil.turek@hotmail.com>
 License: Apache-2.0
 Keywords: google,app engine,cloud storage
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Google App Engine Cloud Storage Client for Python 3
 
-[![PyPi version](https://img.shields.io/pypi/v/GoogleAppEngineCloudStorageClientPy3.svg)](https://pypi.python.org/pypi/GoogleAppEngineCloudStorageClientPy3/)
-[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
 [![Test](https://github.com/kamilturek/appengine-gcs-client-py3/actions/workflows/test.yaml/badge.svg)](https://github.com/kamilturek/appengine-gcs-client-py3/actions/workflows/test.yaml)
 
 This is a port of the [GoogleAppEngineCloudStorageClient](https://pypi.org/project/GoogleAppEngineCloudStorageClient/)
 package to Python 3.
 
 ## Installation
 
 ```sh
 pip install GoogleAppEngineCloudStorageClientPy3
 ```
-
-## Demo
-
-See the [demo](./demo/) application for sample usage.
```

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/GoogleAppEngineCloudStorageClientPy3.egg-info/SOURCES.txt` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/GoogleAppEngineCloudStorageClientPy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/__init__.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/__init__.py`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/api_utils.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/api_utils.py`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/cloudstorage_api.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/cloudstorage_api.py`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/common.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/common.py`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/errors.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/errors.py`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/port/cloudstorage_stub.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/port/cloudstorage_stub.py`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/port/stub_dispatcher.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/port/stub_dispatcher.py`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/port/testbed.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/port/testbed.py`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/rest_api.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/rest_api.py`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/storage_api.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/storage_api.py`

 * *Files identical despite different names*

### Comparing `GoogleAppEngineCloudStorageClientPy3-3.0.0/src/cloudstorage/test_utils.py` & `GoogleAppEngineCloudStorageClientPy3-3.0.0a1/src/cloudstorage/test_utils.py`

 * *Files identical despite different names*

