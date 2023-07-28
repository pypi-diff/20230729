# Comparing `tmp/pforacle-0.0.1.tar.gz` & `tmp/pforacle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pforacle-0.0.1.tar", last modified: Fri Jul 28 22:16:26 2023, max compression
+gzip compressed data, was "pforacle-0.0.2.tar", last modified: Fri Jul 28 22:19:12 2023, max compression
```

## Comparing `pforacle-0.0.1.tar` & `pforacle-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 22:16:26.673543 pforacle-0.0.1/
--rw-rw-rw-   0        0        0       27 2023-07-26 20:35:31.000000 pforacle-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      166 2023-07-28 22:16:26.664296 pforacle-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 22:16:26.657297 pforacle-0.0.1/oracle/
--rw-rw-rw-   0        0        0       82 2023-07-26 20:35:31.000000 pforacle-0.0.1/oracle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 22:16:26.658297 pforacle-0.0.1/oracle/tools/
--rw-rw-rw-   0        0        0       82 2023-07-26 20:35:31.000000 pforacle-0.0.1/oracle/tools/__init__.py
--rw-rw-rw-   0        0        0     1030 2023-07-28 21:51:54.000000 pforacle-0.0.1/oracle/tools/query.py
--rw-rw-rw-   0        0        0      522 2023-07-26 20:35:31.000000 pforacle-0.0.1/oracle/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 22:16:26.659296 pforacle-0.0.1/oracle/yamls/
--rw-rw-rw-   0        0        0      362 2023-07-28 20:49:37.000000 pforacle-0.0.1/oracle/yamls/query.yaml
-drwxrwxrwx   0        0        0        0 2023-07-28 22:16:26.662296 pforacle-0.0.1/pforacle.egg-info/
--rw-rw-rw-   0        0        0      166 2023-07-28 22:16:26.000000 pforacle-0.0.1/pforacle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-07-28 22:16:26.000000 pforacle-0.0.1/pforacle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 22:16:26.000000 pforacle-0.0.1/pforacle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-28 22:16:26.000000 pforacle-0.0.1/pforacle.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-07-28 22:16:26.000000 pforacle-0.0.1/pforacle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 22:16:26.673543 pforacle-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      483 2023-07-28 22:15:07.000000 pforacle-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 22:16:26.663296 pforacle-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-26 20:35:31.000000 pforacle-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1029 2023-07-28 21:51:22.000000 pforacle-0.0.1/tests/test_query.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:19:12.241295 pforacle-0.0.2/
+-rw-rw-rw-   0        0        0       27 2023-07-26 20:35:31.000000 pforacle-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      135 2023-07-28 22:19:12.232494 pforacle-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 22:19:12.206494 pforacle-0.0.2/oracle/
+-rw-rw-rw-   0        0        0       82 2023-07-26 20:35:31.000000 pforacle-0.0.2/oracle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:19:12.215493 pforacle-0.0.2/oracle/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-26 20:35:31.000000 pforacle-0.0.2/oracle/tools/__init__.py
+-rw-rw-rw-   0        0        0     1030 2023-07-28 21:51:54.000000 pforacle-0.0.2/oracle/tools/query.py
+-rw-rw-rw-   0        0        0      522 2023-07-26 20:35:31.000000 pforacle-0.0.2/oracle/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:19:12.219494 pforacle-0.0.2/oracle/yamls/
+-rw-rw-rw-   0        0        0      362 2023-07-28 20:49:37.000000 pforacle-0.0.2/oracle/yamls/query.yaml
+drwxrwxrwx   0        0        0        0 2023-07-28 22:19:12.227493 pforacle-0.0.2/pforacle.egg-info/
+-rw-rw-rw-   0        0        0      135 2023-07-28 22:19:12.000000 pforacle-0.0.2/pforacle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-07-28 22:19:12.000000 pforacle-0.0.2/pforacle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 22:19:12.000000 pforacle-0.0.2/pforacle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-28 22:19:12.000000 pforacle-0.0.2/pforacle.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-07-28 22:19:12.000000 pforacle-0.0.2/pforacle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 22:19:12.241295 pforacle-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      452 2023-07-28 22:19:04.000000 pforacle-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:19:12.231493 pforacle-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-26 20:35:31.000000 pforacle-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1029 2023-07-28 21:51:22.000000 pforacle-0.0.2/tests/test_query.py
```

### Comparing `pforacle-0.0.1/oracle/tools/query.py` & `pforacle-0.0.2/oracle/tools/query.py`

 * *Files identical despite different names*

### Comparing `pforacle-0.0.1/oracle/tools/utils.py` & `pforacle-0.0.2/oracle/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pforacle-0.0.1/tests/test_query.py` & `pforacle-0.0.2/tests/test_query.py`

 * *Files identical despite different names*

