# Comparing `tmp/rescan-1.0.0.tar.gz` & `tmp/rescan-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rescan-1.0.0.tar", last modified: Fri Jul 28 20:12:31 2023, max compression
+gzip compressed data, was "rescan-1.0.1.tar", last modified: Sat Jul 29 12:29:34 2023, max compression
```

## Comparing `rescan-1.0.0.tar` & `rescan-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:12:31.907328 rescan-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-28 20:12:19.000000 rescan-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 20:12:31.907328 rescan-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 20:12:19.000000 rescan-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-28 20:12:19.000000 rescan-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:12:31.907328 rescan-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-28 20:12:19.000000 rescan-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:12:31.903329 rescan-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:12:31.907328 rescan-1.0.0/src/rescan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 20:12:31.000000 rescan-1.0.0/src/rescan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 20:12:31.000000 rescan-1.0.0/src/rescan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:12:31.000000 rescan-1.0.0/src/rescan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:12:31.000000 rescan-1.0.0/src/rescan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 20:12:31.000000 rescan-1.0.0/src/rescan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:12:31.907328 rescan-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:12:19.000000 rescan-1.0.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:34.565325 rescan-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-29 12:29:19.000000 rescan-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-29 12:29:34.565325 rescan-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-29 12:29:19.000000 rescan-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-29 12:29:19.000000 rescan-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:29:34.565325 rescan-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-29 12:29:19.000000 rescan-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:34.565325 rescan-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:34.565325 rescan-1.0.1/src/rescan/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 12:29:19.000000 rescan-1.0.1/src/rescan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 12:29:19.000000 rescan-1.0.1/src/rescan/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-29 12:29:19.000000 rescan-1.0.1/src/rescan/rescan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:34.565325 rescan-1.0.1/src/rescan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 12:29:34.000000 rescan-1.0.1/src/rescan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:34.565325 rescan-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:29:19.000000 rescan-1.0.1/tests/test.py
```

### Comparing `rescan-1.0.0/LICENSE` & `rescan-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rescan-1.0.0/PKG-INFO` & `rescan-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: rescan
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Modern Port scanner in python
 Home-page: https://github.com/snowkluster/rescan
 Author: SnowKluster
 Project-URL: Homepage, https://github.com/snowkluster/rescan
 Project-URL: Bug Tracker, https://github.com/snowkluster/rescan/issues
+Project-URL: Changelog, https://github.com/snowkluster/rescan/blob/master/CHANGELOG.md
 Keywords: Port Scanner,Modern
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rescan-1.0.0/src/rescan.egg-info/PKG-INFO` & `rescan-1.0.1/src/rescan.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: rescan
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Modern Port scanner in python
 Home-page: https://github.com/snowkluster/rescan
 Author: SnowKluster
 Project-URL: Homepage, https://github.com/snowkluster/rescan
 Project-URL: Bug Tracker, https://github.com/snowkluster/rescan/issues
+Project-URL: Changelog, https://github.com/snowkluster/rescan/blob/master/CHANGELOG.md
 Keywords: Port Scanner,Modern
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

