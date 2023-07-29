# Comparing `tmp/awyes-10.1.0.tar.gz` & `tmp/awyes-10.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awyes-10.1.0.tar", last modified: Sat Jul 29 21:29:58 2023, max compression
+gzip compressed data, was "awyes-10.1.1.tar", last modified: Sat Jul 29 21:54:09 2023, max compression
```

## Comparing `awyes-10.1.0.tar` & `awyes-10.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:29:58.014737 awyes-10.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 21:29:58.014737 awyes-10.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-29 21:29:35.000000 awyes-10.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:29:58.010737 awyes-10.1.0/awyes/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 21:29:56.000000 awyes-10.1.0/awyes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-29 21:29:35.000000 awyes-10.1.0/awyes/awyes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-29 21:29:35.000000 awyes-10.1.0/awyes/awyes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 21:29:35.000000 awyes-10.1.0/awyes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:29:58.014737 awyes-10.1.0/awyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 21:29:57.000000 awyes-10.1.0/awyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 21:29:58.014737 awyes-10.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 21:29:35.000000 awyes-10.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:54:09.720784 awyes-10.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 21:54:09.720784 awyes-10.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-29 21:53:48.000000 awyes-10.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:54:09.716783 awyes-10.1.1/awyes/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 21:54:08.000000 awyes-10.1.1/awyes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-29 21:53:48.000000 awyes-10.1.1/awyes/awyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-29 21:53:48.000000 awyes-10.1.1/awyes/awyes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 21:53:48.000000 awyes-10.1.1/awyes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:54:09.716783 awyes-10.1.1/awyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 21:54:09.000000 awyes-10.1.1/awyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 21:54:09.720784 awyes-10.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 21:53:48.000000 awyes-10.1.1/setup.py
```

### Comparing `awyes-10.1.0/PKG-INFO` & `awyes-10.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.1.0
+Version: 10.1.1
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.1.0/awyes/awyes.py` & `awyes-10.1.1/awyes/awyes.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from sys import argv
 from os.path import normpath
 
 from .utils import rgetattr, rsetattr
 
 
 class Deployment:
-    def __init__(self, path="", verbose=False):
+    def __init__(self, path=""):
         # Initialize paths and log settings
         self.path = path
-        self.verbose = verbose
 
         # Load the clients and config
         with open(normpath(path)) as config:
             self.config = yaml.safe_load(config)
             self.clients = {
                 "os": os,
                 "s3": boto3.client("s3"),
@@ -90,16 +89,16 @@
 
             resource_name, action_name = node_name.split(".")
 
             try:
                 action = rgetattr(node_client, action_name)
                 value = action(**self.shared_lookup(node_args))
 
-                if self.verbose:
-                    print(f"setting value {value} for {node_name}")
+                print(f"executing: {node_name}")
+                print(f"setting value {value}")
 
                 rsetattr(
                     context=self.config,
                     accessor=f"{resource_name}.{action_name}",
                     value=value,
                 )
             except Exception as e:
```

### Comparing `awyes-10.1.0/awyes/awyes_test.py` & `awyes-10.1.1/awyes/awyes_test.py`

 * *Files identical despite different names*

### Comparing `awyes-10.1.0/awyes/utils.py` & `awyes-10.1.1/awyes/utils.py`

 * *Files identical despite different names*

### Comparing `awyes-10.1.0/awyes.egg-info/PKG-INFO` & `awyes-10.1.1/awyes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.1.0
+Version: 10.1.1
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.1.0/setup.py` & `awyes-10.1.1/setup.py`

 * *Files identical despite different names*

