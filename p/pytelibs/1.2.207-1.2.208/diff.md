# Comparing `tmp/pytelibs-1.2.207.tar.gz` & `tmp/pytelibs-1.2.208.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytelibs-1.2.207.tar", last modified: Sun Jul 23 12:22:43 2023, max compression
+gzip compressed data, was "pytelibs-1.2.208.tar", last modified: Sat Jul 29 20:01:22 2023, max compression
```

## Comparing `pytelibs-1.2.207.tar` & `pytelibs-1.2.208.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 12:22:43.417395 pytelibs-1.2.207/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.207/LICENSE
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-23 12:22:43.417395 pytelibs-1.2.207/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.207/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 12:22:43.357395 pytelibs-1.2.207/pytelibs/
--rw-r--r--   0 root         (0) root         (0)      488 2023-07-23 12:21:39.000000 pytelibs-1.2.207/pytelibs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      307 2023-07-23 12:21:19.000000 pytelibs-1.2.207/pytelibs/_globvals.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-07-21 12:09:57.000000 pytelibs-1.2.207/pytelibs/_journal.py
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-23 12:21:52.000000 pytelibs-1.2.207/pytelibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 12:22:43.417395 pytelibs-1.2.207/pytelibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-23 12:22:42.000000 pytelibs-1.2.207/pytelibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      270 2023-07-23 12:22:43.000000 pytelibs-1.2.207/pytelibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-23 12:22:42.000000 pytelibs-1.2.207/pytelibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-23 12:22:42.000000 pytelibs-1.2.207/pytelibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-23 12:22:42.000000 pytelibs-1.2.207/pytelibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-23 12:22:43.427395 pytelibs-1.2.207/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.207/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 20:01:22.338872 pytelibs-1.2.208/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.208/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-29 20:01:22.328872 pytelibs-1.2.208/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.208/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 20:01:22.308872 pytelibs-1.2.208/pytelibs/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-07-28 20:45:05.000000 pytelibs-1.2.208/pytelibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      691 2023-07-29 20:00:05.000000 pytelibs-1.2.208/pytelibs/_globvals.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-07-21 12:09:57.000000 pytelibs-1.2.208/pytelibs/_journal.py
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-28 20:45:17.000000 pytelibs-1.2.208/pytelibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 20:01:22.328872 pytelibs-1.2.208/pytelibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-29 20:01:21.000000 pytelibs-1.2.208/pytelibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-29 20:01:22.000000 pytelibs-1.2.208/pytelibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 20:01:21.000000 pytelibs-1.2.208/pytelibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-29 20:01:21.000000 pytelibs-1.2.208/pytelibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-29 20:01:21.000000 pytelibs-1.2.208/pytelibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 20:01:22.338872 pytelibs-1.2.208/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.208/setup.py
```

### Comparing `pytelibs-1.2.207/LICENSE` & `pytelibs-1.2.208/LICENSE`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.207/PKG-INFO` & `pytelibs-1.2.208/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.207
+Version: 1.2.208
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.207/pytelibs/_journal.py` & `pytelibs-1.2.208/pytelibs/_journal.py`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.207/pytelibs.egg-info/PKG-INFO` & `pytelibs-1.2.208/pytelibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.207
+Version: 1.2.208
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.207/setup.py` & `pytelibs-1.2.208/setup.py`

 * *Files identical despite different names*

