# Comparing `tmp/app_toggles-0.1.0.tar.gz` & `tmp/app_toggles-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_toggles-0.1.0.tar", max compression
+gzip compressed data, was "app_toggles-0.1.1.tar", max compression
```

## Comparing `app_toggles-0.1.0.tar` & `app_toggles-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-07-28 20:42:22.910431 app_toggles-0.1.0/LICENSE
--rw-r--r--   0        0        0     2834 2023-07-28 21:10:47.078016 app_toggles-0.1.0/README.md
--rw-r--r--   0        0        0      160 2023-07-28 18:23:57.836410 app_toggles-0.1.0/app_toggles/__init__.py
--rw-r--r--   0        0        0      242 2023-07-28 18:23:52.819325 app_toggles-0.1.0/app_toggles/_exceptions.py
--rw-r--r--   0        0        0       84 2023-07-28 16:50:02.121909 app_toggles-0.1.0/app_toggles/_toggle_providers/__init__.py
--rw-r--r--   0        0        0      829 2023-07-28 17:46:28.016231 app_toggles-0.1.0/app_toggles/_toggle_providers/json_toggle_provider.py
--rw-r--r--   0        0        0      191 2023-07-28 16:32:11.925889 app_toggles-0.1.0/app_toggles/_toggle_providers/provider.py
--rw-r--r--   0        0        0     1205 2023-07-28 19:54:06.928779 app_toggles-0.1.0/app_toggles/_toggles.py
--rw-r--r--   0        0        0      237 2023-07-28 18:16:55.620977 app_toggles-0.1.0/app_toggles/_types.py
--rw-r--r--   0        0        0      497 2023-07-28 21:43:09.243617 app_toggles-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3210 1970-01-01 00:00:00.000000 app_toggles-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-28 20:42:22.910431 app_toggles-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2836 2023-07-28 21:59:51.944691 app_toggles-0.1.1/README.md
+-rw-r--r--   0        0        0      160 2023-07-28 18:23:57.836410 app_toggles-0.1.1/app_toggles/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-28 18:23:52.819325 app_toggles-0.1.1/app_toggles/_exceptions.py
+-rw-r--r--   0        0        0       84 2023-07-28 16:50:02.121909 app_toggles-0.1.1/app_toggles/_toggle_providers/__init__.py
+-rw-r--r--   0        0        0      829 2023-07-28 17:46:28.016231 app_toggles-0.1.1/app_toggles/_toggle_providers/json_toggle_provider.py
+-rw-r--r--   0        0        0      191 2023-07-28 16:32:11.925889 app_toggles-0.1.1/app_toggles/_toggle_providers/provider.py
+-rw-r--r--   0        0        0     1205 2023-07-28 19:54:06.928779 app_toggles-0.1.1/app_toggles/_toggles.py
+-rw-r--r--   0        0        0      237 2023-07-28 18:16:55.620977 app_toggles-0.1.1/app_toggles/_types.py
+-rw-r--r--   0        0        0      497 2023-07-28 22:04:09.587969 app_toggles-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 app_toggles-0.1.1/PKG-INFO
```

### Comparing `app_toggles-0.1.0/LICENSE` & `app_toggles-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `app_toggles-0.1.0/README.md` & `app_toggles-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # App toggles library
 
-![CI](https://github.com/eguezgustavo/app_toggles/actions/workflows/ci.yaml/badge.svg?branch=main)
+![CI](https://github.com/eguezgustavo/app_toggles/actions/workflows/cicd.yaml/badge.svg?branch=main)
 
 This library has been created taking into account the work done by [Pete Hodgson](https://thepete.net/) published in [https://martinfowler.com/](https://martinfowler.com/articles/feature-toggles.html).
 
 ## How to use it
 The example below uses a sample feature to include a cancellation link in a email so the user can cancel the sales order.
 
 1. Create the /tmp/test_app_toggles.json file with the following content:
```

### Comparing `app_toggles-0.1.0/app_toggles/_toggle_providers/json_toggle_provider.py` & `app_toggles-0.1.1/app_toggles/_toggle_providers/json_toggle_provider.py`

 * *Files identical despite different names*

### Comparing `app_toggles-0.1.0/app_toggles/_toggles.py` & `app_toggles-0.1.1/app_toggles/_toggles.py`

 * *Files identical despite different names*

### Comparing `app_toggles-0.1.0/PKG-INFO` & `app_toggles-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: app-toggles
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to manage app toggles
 Author: Gustavo Eguez
 Author-email: eguezgustavo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # App toggles library
 
-![CI](https://github.com/eguezgustavo/app_toggles/actions/workflows/ci.yaml/badge.svg?branch=main)
+![CI](https://github.com/eguezgustavo/app_toggles/actions/workflows/cicd.yaml/badge.svg?branch=main)
 
 This library has been created taking into account the work done by [Pete Hodgson](https://thepete.net/) published in [https://martinfowler.com/](https://martinfowler.com/articles/feature-toggles.html).
 
 ## How to use it
 The example below uses a sample feature to include a cancellation link in a email so the user can cancel the sales order.
 
 1. Create the /tmp/test_app_toggles.json file with the following content:
```

