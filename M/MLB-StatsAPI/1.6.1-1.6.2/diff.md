# Comparing `tmp/MLB-StatsAPI-1.6.1.tar.gz` & `tmp/MLB-StatsAPI-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLB-StatsAPI-1.6.1.tar", last modified: Mon Mar  6 14:39:12 2023, max compression
+gzip compressed data, was "MLB-StatsAPI-1.6.2.tar", last modified: Sat Jul 29 18:38:54 2023, max compression
```

## Comparing `MLB-StatsAPI-1.6.1.tar` & `MLB-StatsAPI-1.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:39:12.829035 MLB-StatsAPI-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-06 14:38:59.000000 MLB-StatsAPI-1.6.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:39:12.829035 MLB-StatsAPI-1.6.1/MLB_StatsAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-06 14:39:12.000000 MLB-StatsAPI-1.6.1/MLB_StatsAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-06 14:39:12.000000 MLB-StatsAPI-1.6.1/MLB_StatsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:39:12.000000 MLB-StatsAPI-1.6.1/MLB_StatsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-06 14:39:12.000000 MLB-StatsAPI-1.6.1/MLB_StatsAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-06 14:39:12.000000 MLB-StatsAPI-1.6.1/MLB_StatsAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-06 14:39:12.829035 MLB-StatsAPI-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-06 14:38:59.000000 MLB-StatsAPI-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 14:39:12.829035 MLB-StatsAPI-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-06 14:38:59.000000 MLB-StatsAPI-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:39:12.829035 MLB-StatsAPI-1.6.1/statsapi/
--rw-r--r--   0 runner    (1001) docker     (123)    60225 2023-03-06 14:38:59.000000 MLB-StatsAPI-1.6.1/statsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41570 2023-03-06 14:38:59.000000 MLB-StatsAPI-1.6.1/statsapi/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 14:38:59.000000 MLB-StatsAPI-1.6.1/statsapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:39:12.829035 MLB-StatsAPI-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:38:59.000000 MLB-StatsAPI-1.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-06 14:38:59.000000 MLB-StatsAPI-1.6.1/tests/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:38:54.984105 MLB-StatsAPI-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 18:38:36.000000 MLB-StatsAPI-1.6.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:38:54.984105 MLB-StatsAPI-1.6.2/MLB_StatsAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-29 18:38:54.000000 MLB-StatsAPI-1.6.2/MLB_StatsAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-29 18:38:54.000000 MLB-StatsAPI-1.6.2/MLB_StatsAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:38:54.000000 MLB-StatsAPI-1.6.2/MLB_StatsAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 18:38:54.000000 MLB-StatsAPI-1.6.2/MLB_StatsAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 18:38:54.000000 MLB-StatsAPI-1.6.2/MLB_StatsAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-29 18:38:54.984105 MLB-StatsAPI-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-29 18:38:36.000000 MLB-StatsAPI-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 18:38:54.984105 MLB-StatsAPI-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-29 18:38:36.000000 MLB-StatsAPI-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:38:54.984105 MLB-StatsAPI-1.6.2/statsapi/
+-rw-r--r--   0 runner    (1001) docker     (123)    60300 2023-07-29 18:38:36.000000 MLB-StatsAPI-1.6.2/statsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41570 2023-07-29 18:38:36.000000 MLB-StatsAPI-1.6.2/statsapi/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-29 18:38:36.000000 MLB-StatsAPI-1.6.2/statsapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:38:54.984105 MLB-StatsAPI-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 18:38:36.000000 MLB-StatsAPI-1.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-29 18:38:36.000000 MLB-StatsAPI-1.6.2/tests/test_get.py
```

### Comparing `MLB-StatsAPI-1.6.1/LICENSE` & `MLB-StatsAPI-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MLB-StatsAPI-1.6.1/MLB_StatsAPI.egg-info/PKG-INFO` & `MLB-StatsAPI-1.6.2/MLB_StatsAPI.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLB-StatsAPI
-Version: 1.6.1
+Version: 1.6.2
 Summary: MLB Stats API Wrapper for Python
 Home-page: https://github.com/toddrob99/MLB-StatsAPI
 Author: Todd Roberts
 Author-email: todd@toddrob.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `MLB-StatsAPI-1.6.1/PKG-INFO` & `MLB-StatsAPI-1.6.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLB-StatsAPI
-Version: 1.6.1
+Version: 1.6.2
 Summary: MLB Stats API Wrapper for Python
 Home-page: https://github.com/toddrob99/MLB-StatsAPI
 Author: Todd Roberts
 Author-email: todd@toddrob.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `MLB-StatsAPI-1.6.1/setup.py` & `MLB-StatsAPI-1.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `MLB-StatsAPI-1.6.1/statsapi/__init__.py` & `MLB-StatsAPI-1.6.2/statsapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1473,16 +1473,17 @@
 
     divisions = {}
 
     for y in r["records"]:
         for x in (
             x
             for x in y["teamRecords"]
-            if division.lower() == "all"
-            or division.lower() == x["team"]["division"]["abbreviation"].lower()
+            if str(division).lower() == "all"
+            or str(division).lower() == x["team"]["division"]["abbreviation"].lower()
+            or str(division) == str(x["team"]["division"]["id"])
         ):
             if x["team"]["division"]["id"] not in divisions.keys():
                 divisions.update(
                     {
                         x["team"]["division"]["id"]: {
                             "div_name": x["team"]["division"]["name"],
                             "teams": [],
```

### Comparing `MLB-StatsAPI-1.6.1/statsapi/endpoints.py` & `MLB-StatsAPI-1.6.2/statsapi/endpoints.py`

 * *Files identical despite different names*

### Comparing `MLB-StatsAPI-1.6.1/tests/test_get.py` & `MLB-StatsAPI-1.6.2/tests/test_get.py`

 * *Files identical despite different names*

