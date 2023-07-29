# Comparing `tmp/awyes-10.0.8.tar.gz` & `tmp/awyes-10.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awyes-10.0.8.tar", last modified: Fri Jul 28 05:56:42 2023, max compression
+gzip compressed data, was "awyes-10.0.9.tar", last modified: Fri Jul 28 06:01:26 2023, max compression
```

## Comparing `awyes-10.0.8.tar` & `awyes-10.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:56:42.528987 awyes-10.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 05:56:42.532987 awyes-10.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 05:56:20.000000 awyes-10.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 05:56:40.000000 awyes-10.0.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:56:42.528987 awyes-10.0.8/awyes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:56:20.000000 awyes-10.0.8/awyes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-28 05:56:20.000000 awyes-10.0.8/awyes/awyes.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-28 05:56:20.000000 awyes-10.0.8/awyes/awyes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-28 05:56:20.000000 awyes-10.0.8/awyes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:56:42.528987 awyes-10.0.8/awyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 05:56:42.000000 awyes-10.0.8/awyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 05:56:42.000000 awyes-10.0.8/awyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 05:56:42.000000 awyes-10.0.8/awyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 05:56:42.000000 awyes-10.0.8/awyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 05:56:42.000000 awyes-10.0.8/awyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 05:56:42.000000 awyes-10.0.8/awyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 05:56:42.532987 awyes-10.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 05:56:20.000000 awyes-10.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:01:26.781810 awyes-10.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 06:01:26.781810 awyes-10.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 06:01:04.000000 awyes-10.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 06:01:25.000000 awyes-10.0.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:01:26.781810 awyes-10.0.9/awyes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:01:04.000000 awyes-10.0.9/awyes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-28 06:01:04.000000 awyes-10.0.9/awyes/awyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-28 06:01:04.000000 awyes-10.0.9/awyes/awyes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-28 06:01:04.000000 awyes-10.0.9/awyes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:01:26.781810 awyes-10.0.9/awyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 06:01:26.000000 awyes-10.0.9/awyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 06:01:26.781810 awyes-10.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 06:01:04.000000 awyes-10.0.9/setup.py
```

### Comparing `awyes-10.0.8/PKG-INFO` & `awyes-10.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.0.8
+Version: 10.0.9
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.0.8/awyes/awyes.py` & `awyes-10.0.9/awyes/awyes.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from os.path import normpath
 
 from .utils import rgetattr, rsetattr
 
 
 class Deployment:
     def __init__(self, path="", verbose=False):
-        # Initialize paths and shared dictionary
-        self.path = path if path else "./awyes.yml"
+        # Initialize paths and log settings
+        self.path = path
         self.verbose = verbose
 
         # Load the config and docker images
         with open(normpath(self.path)) as config:
             self.config = yaml.safe_load(config)
             self.clients = {
                 "os": os,
@@ -103,14 +103,15 @@
                     value=value,
                 )
             except Exception as e:
                 print("err: ", e)
 
 
 def main():
-    _, path = argv
+    _, *path = argv
+    path = path[0] if path else "./awyes"
 
     Deployment(path=path).deploy()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `awyes-10.0.8/awyes/awyes_test.py` & `awyes-10.0.9/awyes/awyes_test.py`

 * *Files identical despite different names*

### Comparing `awyes-10.0.8/awyes/utils.py` & `awyes-10.0.9/awyes/utils.py`

 * *Files identical despite different names*

### Comparing `awyes-10.0.8/awyes.egg-info/PKG-INFO` & `awyes-10.0.9/awyes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.0.8
+Version: 10.0.9
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.0.8/setup.py` & `awyes-10.0.9/setup.py`

 * *Files identical despite different names*

