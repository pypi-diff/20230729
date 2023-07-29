# Comparing `tmp/cloca-1.1.0.tar.gz` & `tmp/cloca-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloca-1.1.0.tar", last modified: Sat Jul 29 15:32:06 2023, max compression
+gzip compressed data, was "cloca-1.1.1.tar", last modified: Sat Jul 29 15:37:05 2023, max compression
```

## Comparing `cloca-1.1.0.tar` & `cloca-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:32:06.071926 cloca-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 15:31:55.000000 cloca-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-29 15:32:06.071926 cloca-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-29 15:31:55.000000 cloca-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:32:06.071926 cloca-1.1.0/cloca/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-29 15:31:55.000000 cloca-1.1.0/cloca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-29 15:31:55.000000 cloca-1.1.0/cloca/cloca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:32:06.071926 cloca-1.1.0/cloca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-29 15:32:06.000000 cloca-1.1.0/cloca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-29 15:32:06.000000 cloca-1.1.0/cloca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:32:06.000000 cloca-1.1.0/cloca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 15:32:06.000000 cloca-1.1.0/cloca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 15:32:06.071926 cloca-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-29 15:31:55.000000 cloca-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:37:05.008877 cloca-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 15:36:55.000000 cloca-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-29 15:37:05.008877 cloca-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-29 15:36:55.000000 cloca-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:37:05.008877 cloca-1.1.1/cloca/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-29 15:36:55.000000 cloca-1.1.1/cloca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-29 15:36:55.000000 cloca-1.1.1/cloca/cloca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:37:05.008877 cloca-1.1.1/cloca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-29 15:37:04.000000 cloca-1.1.1/cloca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-29 15:37:04.000000 cloca-1.1.1/cloca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:37:04.000000 cloca-1.1.1/cloca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 15:37:04.000000 cloca-1.1.1/cloca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 15:37:05.012877 cloca-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-29 15:36:55.000000 cloca-1.1.1/setup.py
```

### Comparing `cloca-1.1.0/LICENSE` & `cloca-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloca-1.1.0/PKG-INFO` & `cloca-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloca
-Version: 1.1.0
+Version: 1.1.1
 Summary: Global Clock Python Library
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cloca-1.1.0/README.md` & `cloca-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cloca-1.1.0/cloca/cloca.py` & `cloca-1.1.1/cloca/cloca.py`

 * *Files identical despite different names*

### Comparing `cloca-1.1.0/cloca.egg-info/PKG-INFO` & `cloca-1.1.1/cloca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloca
-Version: 1.1.0
+Version: 1.1.1
 Summary: Global Clock Python Library
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cloca-1.1.0/setup.py` & `cloca-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cloca',
-    version='1.1.0',
+    version='1.1.1',
     description='Global Clock Python Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ahmad Siavashi',
     author_email='siavashi@aut.ac.ir',
     packages=find_packages(),
     install_requires=[],
```

