# Comparing `tmp/baam-0.0.2.tar.gz` & `tmp/baam-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baam-0.0.2.tar", last modified: Tue Jul 25 15:16:54 2023, max compression
+gzip compressed data, was "baam-0.0.3.tar", last modified: Sat Jul 29 13:13:49 2023, max compression
```

## Comparing `baam-0.0.2.tar` & `baam-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:16:54.195754 baam-0.0.2/
--rw-r--r--   0 pedro      (503) staff       (20)      906 2023-07-25 15:16:54.195645 baam-0.0.2/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      325 2023-07-25 15:15:02.000000 baam-0.0.2/README.md
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:16:54.194436 baam-0.0.2/baam/
--rw-r--r--   0 pedro      (503) staff       (20)       18 2023-07-25 15:15:59.000000 baam-0.0.2/baam/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)      101 2023-07-25 15:00:06.000000 baam-0.0.2/baam/cli.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:16:54.195332 baam-0.0.2/baam.egg-info/
--rw-r--r--   0 pedro      (503) staff       (20)      906 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      234 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (503) staff       (20)        1 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (503) staff       (20)       39 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/entry_points.txt
--rw-r--r--   0 pedro      (503) staff       (20)        7 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/requires.txt
--rw-r--r--   0 pedro      (503) staff       (20)        5 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/top_level.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-07-25 15:16:54.195796 baam-0.0.2/setup.cfg
--rw-r--r--   0 pedro      (503) staff       (20)      999 2023-07-25 15:16:15.000000 baam-0.0.2/setup.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:16:54.195466 baam-0.0.2/test/
--rw-r--r--   0 pedro      (503) staff       (20)       73 2023-07-25 15:00:02.000000 baam-0.0.2/test/test_cli.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-29 13:13:49.309713 baam-0.0.3/
+-rw-r--r--   0 pedro      (503) staff       (20)      989 2023-07-29 13:13:49.309560 baam-0.0.3/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      408 2023-07-29 13:13:22.000000 baam-0.0.3/README.md
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-29 13:13:49.307894 baam-0.0.3/baam/
+-rw-r--r--   0 pedro      (503) staff       (20)       18 2023-07-29 13:13:24.000000 baam-0.0.3/baam/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)      101 2023-07-29 13:09:01.000000 baam-0.0.3/baam/cli.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-29 13:13:49.308991 baam-0.0.3/baam.egg-info/
+-rw-r--r--   0 pedro      (503) staff       (20)      989 2023-07-29 13:13:49.000000 baam-0.0.3/baam.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      234 2023-07-29 13:13:49.000000 baam-0.0.3/baam.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        1 2023-07-29 13:13:49.000000 baam-0.0.3/baam.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       39 2023-07-29 13:13:49.000000 baam-0.0.3/baam.egg-info/entry_points.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        7 2023-07-29 13:13:49.000000 baam-0.0.3/baam.egg-info/requires.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        5 2023-07-29 13:13:49.000000 baam-0.0.3/baam.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-07-29 13:13:49.309770 baam-0.0.3/setup.cfg
+-rw-r--r--   0 pedro      (503) staff       (20)      999 2023-07-25 15:16:15.000000 baam-0.0.3/setup.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-29 13:13:49.309161 baam-0.0.3/test/
+-rw-r--r--   0 pedro      (503) staff       (20)       73 2023-07-25 15:00:02.000000 baam-0.0.3/test/test_cli.py
```

### Comparing `baam-0.0.2/PKG-INFO` & `baam-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baam
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deploys docker apps
 Home-page: https://github.com/jpedro/baam
 Download-URL: https://github.com/jpedro/baam/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: deploy docker apps
@@ -15,17 +15,21 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # Baam
 
 [![PyPI version](https://badge.fury.io/py/baam.svg)](https://badge.fury.io/py/baam)
-[![Unstable package](https://img.shields.io/badge/_Unstable_package_-_This_code_is_a_work_in_progress_-red)](https://semver.org)
+[![Unstable package](https://img.shields.io/badge/_Unstable_package_-_This_shit_will_be_amazing_-red)](https://semver.org)
 
 Builds and deploys docker apps.
 
 
-## Inspired by
+## What people are saying
 
 > "Bang, baam, thank you ma'am."
 >
 > — Dean Martin
+
+> "This is the most important software of the decade!"
+>
+> — Bernie Madoff
```

### Comparing `baam-0.0.2/baam.egg-info/PKG-INFO` & `baam-0.0.3/baam.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baam
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deploys docker apps
 Home-page: https://github.com/jpedro/baam
 Download-URL: https://github.com/jpedro/baam/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: deploy docker apps
@@ -15,17 +15,21 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # Baam
 
 [![PyPI version](https://badge.fury.io/py/baam.svg)](https://badge.fury.io/py/baam)
-[![Unstable package](https://img.shields.io/badge/_Unstable_package_-_This_code_is_a_work_in_progress_-red)](https://semver.org)
+[![Unstable package](https://img.shields.io/badge/_Unstable_package_-_This_shit_will_be_amazing_-red)](https://semver.org)
 
 Builds and deploys docker apps.
 
 
-## Inspired by
+## What people are saying
 
 > "Bang, baam, thank you ma'am."
 >
 > — Dean Martin
+
+> "This is the most important software of the decade!"
+>
+> — Bernie Madoff
```

### Comparing `baam-0.0.2/setup.py` & `baam-0.0.3/setup.py`

 * *Files identical despite different names*

