# Comparing `tmp/cudagrad-0.0.31.tar.gz` & `tmp/cudagrad-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.31.tar", last modified: Sat Jul 29 19:25:39 2023, max compression
+gzip compressed data, was "cudagrad-0.0.33.tar", last modified: Sat Jul 29 20:03:05 2023, max compression
```

## Comparing `cudagrad-0.0.31.tar` & `cudagrad-0.0.33.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 19:25:39.223912 cudagrad-0.0.31/
--rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.31/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3660 2023-07-29 19:25:39.223796 cudagrad-0.0.31/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3157 2023-07-28 03:27:33.000000 cudagrad-0.0.31/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 19:25:39.221685 cudagrad-0.0.31/cudagrad/
--rw-r--r--   0 ryan       (501) staff       (20)      107 2023-07-27 03:25:50.000000 cudagrad-0.0.31/cudagrad/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     5925 2023-07-27 03:50:10.000000 cudagrad-0.0.31/cudagrad/mlp.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 19:25:39.222728 cudagrad-0.0.31/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3660 2023-07-29 19:25:39.000000 cudagrad-0.0.31/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      331 2023-07-29 19:25:39.000000 cudagrad-0.0.31/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-29 19:25:39.000000 cudagrad-0.0.31/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.31/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-29 19:25:39.000000 cudagrad-0.0.31/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-29 19:25:39.000000 cudagrad-0.0.31/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)      984 2023-07-29 19:17:46.000000 cudagrad-0.0.31/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-29 19:25:39.223950 cudagrad-0.0.31/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1659 2023-07-27 00:49:51.000000 cudagrad-0.0.31/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 19:25:39.223131 cudagrad-0.0.31/src/
--rw-r--r--   0 ryan       (501) staff       (20)     2910 2023-07-29 19:18:45.000000 cudagrad-0.0.31/src/bindings.cpp
--rw-r--r--   0 ryan       (501) staff       (20)    20457 2023-07-29 19:17:36.000000 cudagrad-0.0.31/src/cudagrad.hpp
--rw-r--r--   0 ryan       (501) staff       (20)      254 2023-07-29 18:53:13.000000 cudagrad-0.0.31/src/ops.cu
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 19:25:39.223508 cudagrad-0.0.31/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1083 2023-07-29 16:33:01.000000 cudagrad-0.0.31/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 20:03:05.302396 cudagrad-0.0.33/
+-rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-29 19:31:23.000000 cudagrad-0.0.33/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3660 2023-07-29 20:03:05.302240 cudagrad-0.0.33/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     3157 2023-07-28 03:27:33.000000 cudagrad-0.0.33/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 20:03:05.299239 cudagrad-0.0.33/cudagrad/
+-rw-r--r--   0 ryan       (501) staff       (20)      131 2023-07-29 20:02:43.000000 cudagrad-0.0.33/cudagrad/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5925 2023-07-27 03:50:10.000000 cudagrad-0.0.33/cudagrad/mlp.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 20:03:05.300230 cudagrad-0.0.33/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3660 2023-07-29 20:03:05.000000 cudagrad-0.0.33/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      331 2023-07-29 20:03:05.000000 cudagrad-0.0.33/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-29 20:03:05.000000 cudagrad-0.0.33/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.33/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-29 20:03:05.000000 cudagrad-0.0.33/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-29 20:03:05.000000 cudagrad-0.0.33/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      984 2023-07-29 20:02:43.000000 cudagrad-0.0.33/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-29 20:03:05.302499 cudagrad-0.0.33/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1659 2023-07-27 00:49:51.000000 cudagrad-0.0.33/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 20:03:05.301491 cudagrad-0.0.33/src/
+-rw-r--r--   0 ryan       (501) staff       (20)     2910 2023-07-29 19:18:45.000000 cudagrad-0.0.33/src/bindings.cpp
+-rw-r--r--   0 ryan       (501) staff       (20)    20457 2023-07-29 19:17:36.000000 cudagrad-0.0.33/src/cudagrad.hpp
+-rw-r--r--   0 ryan       (501) staff       (20)      254 2023-07-29 18:53:13.000000 cudagrad-0.0.33/src/ops.cu
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 20:03:05.301797 cudagrad-0.0.33/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)     1083 2023-07-29 16:33:01.000000 cudagrad-0.0.33/tests/test.py
```

### Comparing `cudagrad-0.0.31/PKG-INFO` & `cudagrad-0.0.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.31
+Version: 0.0.33
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <ryanm.inbox@gmail.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cudagrad-0.0.31/README.md` & `cudagrad-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.31/cudagrad/mlp.py` & `cudagrad-0.0.33/cudagrad/mlp.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.31/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.33/cudagrad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.31
+Version: 0.0.33
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <ryanm.inbox@gmail.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cudagrad-0.0.31/pyproject.toml` & `cudagrad-0.0.33/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=40.8.0", "wheel", "pybind11>=2.10.1", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.31"
+version = "0.0.33"
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 # TEMP while we implement mlp
 dependencies = [ "micrograd",]
 [[project.authors]]
```

### Comparing `cudagrad-0.0.31/setup.py` & `cudagrad-0.0.33/setup.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.31/src/bindings.cpp` & `cudagrad-0.0.33/src/bindings.cpp`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.31/src/cudagrad.hpp` & `cudagrad-0.0.33/src/cudagrad.hpp`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.31/tests/test.py` & `cudagrad-0.0.33/tests/test.py`

 * *Files identical despite different names*

