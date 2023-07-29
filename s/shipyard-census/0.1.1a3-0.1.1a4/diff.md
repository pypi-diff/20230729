# Comparing `tmp/shipyard_census-0.1.1a3.tar.gz` & `tmp/shipyard_census-0.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_census-0.1.1a3.tar", max compression
+gzip compressed data, was "shipyard_census-0.1.1a4.tar", max compression
```

## Comparing `shipyard_census-0.1.1a3.tar` & `shipyard_census-0.1.1a4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      632 2023-07-28 02:48:32.865997 shipyard_census-0.1.1a3/pyproject.toml
--rw-r--r--   0        0        0       33 2023-05-12 18:48:21.825204 shipyard_census-0.1.1a3/shipyard_census/__init__.py
--rw-r--r--   0        0        0     5852 2023-07-28 02:46:43.842558 shipyard_census-0.1.1a3/shipyard_census/census.py
--rw-r--r--   0        0        0      186 2023-07-28 00:25:41.244623 shipyard_census-0.1.1a3/shipyard_census/cli/authtest.py
--rw-r--r--   0        0        0     2844 2023-07-28 02:48:25.059554 shipyard_census-0.1.1a3/shipyard_census/cli/trigger_sync_cli.py
--rw-r--r--   0        0        0       71 2023-07-03 14:05:58.556145 shipyard_census-0.1.1a3/shipyard_census/test/tests.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 shipyard_census-0.1.1a3/PKG-INFO
+-rw-r--r--   0        0        0      632 2023-07-28 02:55:46.151323 shipyard_census-0.1.1a4/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-05-12 18:48:21.825204 shipyard_census-0.1.1a4/shipyard_census/__init__.py
+-rw-r--r--   0        0        0     5852 2023-07-28 02:46:43.842558 shipyard_census-0.1.1a4/shipyard_census/census.py
+-rw-r--r--   0        0        0      186 2023-07-28 00:25:41.244623 shipyard_census-0.1.1a4/shipyard_census/cli/authtest.py
+-rw-r--r--   0        0        0     2844 2023-07-28 02:48:25.059554 shipyard_census-0.1.1a4/shipyard_census/cli/trigger_sync_cli.py
+-rw-r--r--   0        0        0       71 2023-07-03 14:05:58.556145 shipyard_census-0.1.1a4/shipyard_census/test/tests.py
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 shipyard_census-0.1.1a4/PKG-INFO
```

### Comparing `shipyard_census-0.1.1a3/pyproject.toml` & `shipyard_census-0.1.1a4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-census"
-version = "0.1.1a3"
+version = "0.1.1a4"
 description = "A local client for connecting and working with Census"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>","wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 #readme = "README.md"
 packages = [{include = "shipyard_census"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_census-0.1.1a3/shipyard_census/census.py` & `shipyard_census-0.1.1a4/shipyard_census/census.py`

 * *Files identical despite different names*

### Comparing `shipyard_census-0.1.1a3/shipyard_census/cli/trigger_sync_cli.py` & `shipyard_census-0.1.1a4/shipyard_census/cli/trigger_sync_cli.py`

 * *Files identical despite different names*

### Comparing `shipyard_census-0.1.1a3/PKG-INFO` & `shipyard_census-0.1.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-census
-Version: 0.1.1a3
+Version: 0.1.1a4
 Summary: A local client for connecting and working with Census
 License: Apache 2.0
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

