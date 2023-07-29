# Comparing `tmp/localstack-client-2.2.tar.gz` & `tmp/localstack-client-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-client-2.2.tar", last modified: Fri Jun  9 17:42:46 2023, max compression
+gzip compressed data, was "localstack-client-2.3.tar", last modified: Sat Jul 29 19:19:47 2023, max compression
```

## Comparing `localstack-client-2.2.tar` & `localstack-client-2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-06-09 17:42:46.952392 localstack-client-2.2/
--rw-r--r--   0 whummer    (501) staff       (20)    11357 2022-06-14 05:51:42.000000 localstack-client-2.2/LICENSE
--rw-r--r--   0 whummer    (501) staff       (20)      673 2023-06-09 17:42:46.952485 localstack-client-2.2/PKG-INFO
--rw-r--r--   0 whummer    (501) staff       (20)     4303 2023-05-18 20:09:36.000000 localstack-client-2.2/README.md
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-06-09 17:42:46.950719 localstack-client-2.2/localstack_client/
--rw-r--r--   0 whummer    (501) staff       (20)        0 2022-06-14 05:51:43.000000 localstack-client-2.2/localstack_client/__init__.py
--rw-r--r--   0 whummer    (501) staff       (20)     5377 2023-06-09 17:29:45.000000 localstack-client-2.2/localstack_client/config.py
--rw-r--r--   0 whummer    (501) staff       (20)     4637 2022-08-31 16:04:05.000000 localstack-client-2.2/localstack_client/patch.py
--rw-r--r--   0 whummer    (501) staff       (20)     3471 2022-08-31 16:04:05.000000 localstack-client-2.2/localstack_client/session.py
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-06-09 17:42:46.952278 localstack-client-2.2/localstack_client.egg-info/
--rw-r--r--   0 whummer    (501) staff       (20)      673 2023-06-09 17:42:46.000000 localstack-client-2.2/localstack_client.egg-info/PKG-INFO
--rw-r--r--   0 whummer    (501) staff       (20)      354 2023-06-09 17:42:46.000000 localstack-client-2.2/localstack_client.egg-info/SOURCES.txt
--rw-r--r--   0 whummer    (501) staff       (20)        1 2023-06-09 17:42:46.000000 localstack-client-2.2/localstack_client.egg-info/dependency_links.txt
--rw-r--r--   0 whummer    (501) staff       (20)       60 2023-06-09 17:42:46.000000 localstack-client-2.2/localstack_client.egg-info/requires.txt
--rw-r--r--   0 whummer    (501) staff       (20)       18 2023-06-09 17:42:46.000000 localstack-client-2.2/localstack_client.egg-info/top_level.txt
--rw-r--r--   0 whummer    (501) staff       (20)      756 2023-06-09 17:42:46.953063 localstack-client-2.2/setup.cfg
--rwxr-xr-x   0 whummer    (501) staff       (20)       60 2022-06-14 05:51:43.000000 localstack-client-2.2/setup.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-07-29 19:19:47.726802 localstack-client-2.3/
+-rw-r--r--   0 whummer    (501) staff       (20)    11357 2022-06-14 05:51:42.000000 localstack-client-2.3/LICENSE
+-rw-r--r--   0 whummer    (501) staff       (20)      673 2023-07-29 19:19:47.726873 localstack-client-2.3/PKG-INFO
+-rw-r--r--   0 whummer    (501) staff       (20)     4303 2023-05-18 20:09:36.000000 localstack-client-2.3/README.md
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-07-29 19:19:47.725728 localstack-client-2.3/localstack_client/
+-rw-r--r--   0 whummer    (501) staff       (20)        0 2022-06-14 05:51:43.000000 localstack-client-2.3/localstack_client/__init__.py
+-rw-r--r--   0 whummer    (501) staff       (20)     5400 2023-07-29 19:19:32.000000 localstack-client-2.3/localstack_client/config.py
+-rw-r--r--   0 whummer    (501) staff       (20)     4637 2022-08-31 16:04:05.000000 localstack-client-2.3/localstack_client/patch.py
+-rw-r--r--   0 whummer    (501) staff       (20)     3471 2022-08-31 16:04:05.000000 localstack-client-2.3/localstack_client/session.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-07-29 19:19:47.726698 localstack-client-2.3/localstack_client.egg-info/
+-rw-r--r--   0 whummer    (501) staff       (20)      673 2023-07-29 19:19:47.000000 localstack-client-2.3/localstack_client.egg-info/PKG-INFO
+-rw-r--r--   0 whummer    (501) staff       (20)      354 2023-07-29 19:19:47.000000 localstack-client-2.3/localstack_client.egg-info/SOURCES.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        1 2023-07-29 19:19:47.000000 localstack-client-2.3/localstack_client.egg-info/dependency_links.txt
+-rw-r--r--   0 whummer    (501) staff       (20)       60 2023-07-29 19:19:47.000000 localstack-client-2.3/localstack_client.egg-info/requires.txt
+-rw-r--r--   0 whummer    (501) staff       (20)       18 2023-07-29 19:19:47.000000 localstack-client-2.3/localstack_client.egg-info/top_level.txt
+-rw-r--r--   0 whummer    (501) staff       (20)      756 2023-07-29 19:19:47.727169 localstack-client-2.3/setup.cfg
+-rwxr-xr-x   0 whummer    (501) staff       (20)       60 2022-06-14 05:51:43.000000 localstack-client-2.3/setup.py
```

### Comparing `localstack-client-2.2/LICENSE` & `localstack-client-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `localstack-client-2.2/PKG-INFO` & `localstack-client-2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-client
-Version: 2.2
+Version: 2.3
 Summary: A lightweight Python client for LocalStack.
 Home-page: https://github.com/localstack/localstack-python-client
 Author: LocalStack Team
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `localstack-client-2.2/README.md` & `localstack-client-2.3/README.md`

 * *Files identical despite different names*

### Comparing `localstack-client-2.2/localstack_client/config.py` & `localstack-client-2.3/localstack_client/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
     "meteringmarketplace": 4644,
     "transcribe": 4566,
     "mq": 4566,
     "emr-serverless": 4566,
     "appflow": 4566,
     "route53domains": 4566,
     "keyspaces": 4566,
+    "scheduler": 4566,
 }
 
 # TODO remove service port mapping above entirely
 if os.environ.get("USE_LEGACY_PORTS") not in ["1", "true"]:
     for key, value in _service_ports.items():
         if key not in ["dashboard", "elasticsearch"]:
             _service_ports[key] = DEFAULT_EDGE_PORT
```

### Comparing `localstack-client-2.2/localstack_client/patch.py` & `localstack-client-2.3/localstack_client/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-client-2.2/localstack_client/session.py` & `localstack-client-2.3/localstack_client/session.py`

 * *Files identical despite different names*

### Comparing `localstack-client-2.2/localstack_client.egg-info/PKG-INFO` & `localstack-client-2.3/localstack_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-client
-Version: 2.2
+Version: 2.3
 Summary: A lightweight Python client for LocalStack.
 Home-page: https://github.com/localstack/localstack-python-client
 Author: LocalStack Team
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `localstack-client-2.2/setup.cfg` & `localstack-client-2.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = localstack-client
-version = 2.2
+version = 2.3
 url = https://github.com/localstack/localstack-python-client
 author = LocalStack Team
 author_email = info@localstack.cloud
 description = A lightweight Python client for LocalStack.
 license = Apache License 2.0
 classifiers = 
 	Programming Language :: Python :: 3
```

