# Comparing `tmp/rescan-1.0.2.tar.gz` & `tmp/rescan-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rescan-1.0.2.tar", last modified: Sat Jul 29 13:29:02 2023, max compression
+gzip compressed data, was "rescan-1.0.3.tar", last modified: Sat Jul 29 20:28:26 2023, max compression
```

## Comparing `rescan-1.0.2.tar` & `rescan-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:29:02.256668 rescan-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-29 13:28:48.000000 rescan-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-29 13:29:02.256668 rescan-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-29 13:28:48.000000 rescan-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-29 13:28:48.000000 rescan-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 13:29:02.256668 rescan-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-29 13:28:48.000000 rescan-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:29:02.252668 rescan-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:29:02.252668 rescan-1.0.2/src/rescan/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 13:28:48.000000 rescan-1.0.2/src/rescan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 13:28:48.000000 rescan-1.0.2/src/rescan/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-29 13:28:48.000000 rescan-1.0.2/src/rescan/rescan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:29:02.256668 rescan-1.0.2/src/rescan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:29:02.256668 rescan-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:28:48.000000 rescan-1.0.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:28:26.239985 rescan-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-29 20:28:11.000000 rescan-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-29 20:28:26.239985 rescan-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-29 20:28:11.000000 rescan-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-29 20:28:11.000000 rescan-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:28:26.239985 rescan-1.0.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-29 20:28:11.000000 rescan-1.0.3/scripts/rescan
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 20:28:26.239985 rescan-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-29 20:28:11.000000 rescan-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:28:26.239985 rescan-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:28:26.239985 rescan-1.0.3/src/rescan/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 20:28:11.000000 rescan-1.0.3/src/rescan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 20:28:11.000000 rescan-1.0.3/src/rescan/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-29 20:28:11.000000 rescan-1.0.3/src/rescan/rescan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:28:26.239985 rescan-1.0.3/src/rescan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-29 20:28:26.000000 rescan-1.0.3/src/rescan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-29 20:28:26.000000 rescan-1.0.3/src/rescan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 20:28:26.000000 rescan-1.0.3/src/rescan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-29 20:28:26.000000 rescan-1.0.3/src/rescan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 20:28:26.000000 rescan-1.0.3/src/rescan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 20:28:26.000000 rescan-1.0.3/src/rescan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:28:26.239985 rescan-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:28:11.000000 rescan-1.0.3/tests/test.py
```

### Comparing `rescan-1.0.2/LICENSE` & `rescan-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rescan-1.0.2/PKG-INFO` & `rescan-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rescan
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Modern Port scanner in python
 Home-page: https://github.com/snowkluster/rescan
 Author: SnowKluster
 Project-URL: Homepage, https://github.com/snowkluster/rescan
 Project-URL: Bug Tracker, https://github.com/snowkluster/rescan/issues
 Project-URL: Changelog, https://github.com/snowkluster/rescan/blob/master/CHANGELOG.md
 Keywords: Port Scanner,Modern
```

### Comparing `rescan-1.0.2/README.md` & `rescan-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rescan-1.0.2/pyproject.toml` & `rescan-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rescan"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="SnowKluster"},
 ]
 description = "A Modern Port scanner in python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `rescan-1.0.2/setup.py` & `rescan-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup
 
 setup(
     name = 'rescan',
-    version = '1.0.2',
+    version = '1.0.3',
     description = 'A modern port scanner for recon written in python',
     py_modules = ["rescan"],
+    scripts=['./scripts/rescan'],
     packages = ["rescan"],
     entry_points = {
         "console_scripts": ['rescan = rescan.rescan:main']
         },
     package_dir = {'':'src'},
     author = 'SnowKluster',
     long_description = open('README.md').read(),
```

### Comparing `rescan-1.0.2/src/rescan/rescan.py` & `rescan-1.0.3/src/rescan/rescan.py`

 * *Files identical despite different names*

### Comparing `rescan-1.0.2/src/rescan.egg-info/PKG-INFO` & `rescan-1.0.3/src/rescan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rescan
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Modern Port scanner in python
 Home-page: https://github.com/snowkluster/rescan
 Author: SnowKluster
 Project-URL: Homepage, https://github.com/snowkluster/rescan
 Project-URL: Bug Tracker, https://github.com/snowkluster/rescan/issues
 Project-URL: Changelog, https://github.com/snowkluster/rescan/blob/master/CHANGELOG.md
 Keywords: Port Scanner,Modern
```

