# Comparing `tmp/rescan-1.0.1.tar.gz` & `tmp/rescan-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rescan-1.0.1.tar", last modified: Sat Jul 29 12:29:34 2023, max compression
+gzip compressed data, was "rescan-1.0.2.tar", last modified: Sat Jul 29 13:29:02 2023, max compression
```

## Comparing `rescan-1.0.1.tar` & `rescan-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:34.565325 rescan-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-29 12:29:19.000000 rescan-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-29 12:29:34.565325 rescan-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-29 12:29:19.000000 rescan-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-29 12:29:19.000000 rescan-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:29:34.565325 rescan-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-29 12:29:19.000000 rescan-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:34.565325 rescan-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:34.565325 rescan-1.0.1/src/rescan/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 12:29:19.000000 rescan-1.0.1/src/rescan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 12:29:19.000000 rescan-1.0.1/src/rescan/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-29 12:29:19.000000 rescan-1.0.1/src/rescan/rescan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:34.565325 rescan-1.0.1/src/rescan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:34.565325 rescan-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:19.000000 rescan-1.0.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:29:02.256668 rescan-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-29 13:28:48.000000 rescan-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-29 13:29:02.256668 rescan-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-29 13:28:48.000000 rescan-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-29 13:28:48.000000 rescan-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 13:29:02.256668 rescan-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-29 13:28:48.000000 rescan-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:29:02.252668 rescan-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:29:02.252668 rescan-1.0.2/src/rescan/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 13:28:48.000000 rescan-1.0.2/src/rescan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 13:28:48.000000 rescan-1.0.2/src/rescan/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-29 13:28:48.000000 rescan-1.0.2/src/rescan/rescan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:29:02.256668 rescan-1.0.2/src/rescan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 13:29:02.000000 rescan-1.0.2/src/rescan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:29:02.256668 rescan-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:28:48.000000 rescan-1.0.2/tests/test.py
```

### Comparing `rescan-1.0.1/LICENSE` & `rescan-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rescan-1.0.1/pyproject.toml` & `rescan-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rescan"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="SnowKluster"},
 ]
 description = "A Modern Port scanner in python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -12,8 +12,8 @@
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/snowkluster/rescan"
 "Bug Tracker" = "https://github.com/snowkluster/rescan/issues"
-Changelog = "https://github.com/snowkluster/rescan/blob/master/CHANGELOG.md"
+Changelog = "https://github.com/snowkluster/rescan/blob/master/CHANGELOG.md"
```

### Comparing `rescan-1.0.1/setup.py` & `rescan-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name = 'rescan',
-    version = '1.0.1',
+    version = '1.0.2',
     description = 'A modern port scanner for recon written in python',
     py_modules = ["rescan"],
     packages = ["rescan"],
     entry_points = {
         "console_scripts": ['rescan = rescan.rescan:main']
         },
     package_dir = {'':'src'},
@@ -27,8 +27,8 @@
         'Operating System :: OS Independent',
     ],
     install_requires = [
         'rich~=13.4.2',
         'typer~=0.9.0'
     ],
     keywords = ['Port Scanner', 'Modern'],
-)
+)
```

### Comparing `rescan-1.0.1/src/rescan/rescan.py` & `rescan-1.0.2/src/rescan/rescan.py`

 * *Files identical despite different names*

