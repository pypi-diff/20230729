# Comparing `tmp/nthp_api-0.1.6.tar.gz` & `tmp/nthp_api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nthp_api-0.1.6.tar", max compression
+gzip compressed data, was "nthp_api-0.1.7.tar", max compression
```

## Comparing `nthp_api-0.1.6.tar` & `nthp_api-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2175 2023-07-29 17:56:32.833014 nthp_api-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/__init__.py
--rw-r--r--   0        0        0     1864 2023-07-29 18:00:50.562985 nthp_api-0.1.6/nthp_api/cli/__init__.py
--rw-r--r--   0        0        0      567 2023-07-29 01:34:10.381343 nthp_api-0.1.6/nthp_api/cli/logs.py
--rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/__init__.py
--rw-r--r--   0        0        0     7378 2023-07-29 01:38:27.147185 nthp_api-0.1.6/nthp_api/nthp_build/assets.py
--rw-r--r--   0        0        0      558 2023-07-29 01:34:10.381343 nthp_api-0.1.6/nthp_api/nthp_build/config.py
--rw-r--r--   0        0        0     1103 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/content.py
--rw-r--r--   0        0        0     3996 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/database.py
--rw-r--r--   0        0        0     1427 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/documents.py
--rw-r--r--   0        0        0    12110 2023-07-29 01:33:59.733253 nthp_api-0.1.6/nthp_api/nthp_build/dumper.py
--rw-r--r--   0        0        0      276 2023-07-29 01:34:10.381343 nthp_api-0.1.6/nthp_api/nthp_build/fields.py
--rw-r--r--   0        0        0      461 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/history.py
--rw-r--r--   0        0        0     8634 2023-07-29 01:34:10.381343 nthp_api-0.1.6/nthp_api/nthp_build/loader.py
--rw-r--r--   0        0        0     5386 2023-07-29 18:03:05.004008 nthp_api-0.1.6/nthp_api/nthp_build/models.py
--rw-r--r--   0        0        0     1617 2023-07-29 01:37:44.750900 nthp_api-0.1.6/nthp_api/nthp_build/parallel.py
--rw-r--r--   0        0        0     8105 2023-07-29 01:25:49.153157 nthp_api-0.1.6/nthp_api/nthp_build/people.py
--rw-r--r--   0        0        0     3826 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/playwrights.py
--rw-r--r--   0        0        0     6388 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/roles.py
--rw-r--r--   0        0        0    10201 2023-07-29 18:03:05.004008 nthp_api-0.1.6/nthp_api/nthp_build/schema.py
--rw-r--r--   0        0        0      416 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/search.py
--rw-r--r--   0        0        0     6446 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/shows.py
--rw-r--r--   0        0        0     1098 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/smugmug.py
--rw-r--r--   0        0        0    10027 2023-07-29 18:03:05.004008 nthp_api-0.1.6/nthp_api/nthp_build/spec.py
--rw-r--r--   0        0        0     1940 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/trivia.py
--rw-r--r--   0        0        0     2117 2023-07-23 23:03:58.959516 nthp_api-0.1.6/nthp_api/nthp_build/venues.py
--rw-r--r--   0        0        0      191 2023-07-29 18:00:50.562985 nthp_api-0.1.6/nthp_api/nthp_build/version.py
--rw-r--r--   0        0        0     1168 2023-07-23 23:03:58.963517 nthp_api-0.1.6/nthp_api/nthp_build/years.py
--rw-r--r--   0        0        0      305 2023-07-23 23:03:58.963517 nthp_api-0.1.6/nthp_api/smugmugger/__init__.py
--rw-r--r--   0        0        0      649 2023-07-23 23:03:58.963517 nthp_api-0.1.6/nthp_api/smugmugger/album.py
--rw-r--r--   0        0        0     2583 2023-07-23 23:03:58.963517 nthp_api-0.1.6/nthp_api/smugmugger/client.py
--rw-r--r--   0        0        0      367 2023-07-29 01:34:10.381343 nthp_api-0.1.6/nthp_api/smugmugger/config.py
--rw-r--r--   0        0        0      661 2023-07-23 23:03:58.963517 nthp_api-0.1.6/nthp_api/smugmugger/database.py
--rw-r--r--   0        0        0     1155 2023-07-29 01:34:10.381343 nthp_api-0.1.6/nthp_api/smugmugger/schema.py
--rw-r--r--   0        0        0     2019 2023-07-23 23:03:58.963517 nthp_api-0.1.6/nthp_api/smugmugger/smugmug.py
--rw-r--r--   0        0        0     2166 2023-07-29 18:03:22.540141 nthp_api-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 nthp_api-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2175 2023-07-29 17:56:32.833014 nthp_api-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/__init__.py
+-rw-r--r--   0        0        0     1873 2023-07-29 18:04:52.416824 nthp_api-0.1.7/nthp_api/cli/__init__.py
+-rw-r--r--   0        0        0      567 2023-07-29 01:34:10.381343 nthp_api-0.1.7/nthp_api/cli/logs.py
+-rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/__init__.py
+-rw-r--r--   0        0        0     7378 2023-07-29 01:38:27.147185 nthp_api-0.1.7/nthp_api/nthp_build/assets.py
+-rw-r--r--   0        0        0      558 2023-07-29 01:34:10.381343 nthp_api-0.1.7/nthp_api/nthp_build/config.py
+-rw-r--r--   0        0        0     1103 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/content.py
+-rw-r--r--   0        0        0     3996 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/database.py
+-rw-r--r--   0        0        0     1427 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/documents.py
+-rw-r--r--   0        0        0    12110 2023-07-29 01:33:59.733253 nthp_api-0.1.7/nthp_api/nthp_build/dumper.py
+-rw-r--r--   0        0        0      276 2023-07-29 01:34:10.381343 nthp_api-0.1.7/nthp_api/nthp_build/fields.py
+-rw-r--r--   0        0        0      461 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/history.py
+-rw-r--r--   0        0        0     8634 2023-07-29 01:34:10.381343 nthp_api-0.1.7/nthp_api/nthp_build/loader.py
+-rw-r--r--   0        0        0     5386 2023-07-29 18:03:05.004008 nthp_api-0.1.7/nthp_api/nthp_build/models.py
+-rw-r--r--   0        0        0     1617 2023-07-29 01:37:44.750900 nthp_api-0.1.7/nthp_api/nthp_build/parallel.py
+-rw-r--r--   0        0        0     8105 2023-07-29 01:25:49.153157 nthp_api-0.1.7/nthp_api/nthp_build/people.py
+-rw-r--r--   0        0        0     3826 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/playwrights.py
+-rw-r--r--   0        0        0     6388 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/roles.py
+-rw-r--r--   0        0        0    10201 2023-07-29 18:03:05.004008 nthp_api-0.1.7/nthp_api/nthp_build/schema.py
+-rw-r--r--   0        0        0      416 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/search.py
+-rw-r--r--   0        0        0     6446 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/shows.py
+-rw-r--r--   0        0        0     1098 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/smugmug.py
+-rw-r--r--   0        0        0    10027 2023-07-29 18:03:05.004008 nthp_api-0.1.7/nthp_api/nthp_build/spec.py
+-rw-r--r--   0        0        0     1940 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/trivia.py
+-rw-r--r--   0        0        0     2117 2023-07-23 23:03:58.959516 nthp_api-0.1.7/nthp_api/nthp_build/venues.py
+-rw-r--r--   0        0        0      191 2023-07-29 18:00:50.562985 nthp_api-0.1.7/nthp_api/nthp_build/version.py
+-rw-r--r--   0        0        0     1168 2023-07-23 23:03:58.963517 nthp_api-0.1.7/nthp_api/nthp_build/years.py
+-rw-r--r--   0        0        0      305 2023-07-23 23:03:58.963517 nthp_api-0.1.7/nthp_api/smugmugger/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-23 23:03:58.963517 nthp_api-0.1.7/nthp_api/smugmugger/album.py
+-rw-r--r--   0        0        0     2583 2023-07-23 23:03:58.963517 nthp_api-0.1.7/nthp_api/smugmugger/client.py
+-rw-r--r--   0        0        0      367 2023-07-29 01:34:10.381343 nthp_api-0.1.7/nthp_api/smugmugger/config.py
+-rw-r--r--   0        0        0      661 2023-07-23 23:03:58.963517 nthp_api-0.1.7/nthp_api/smugmugger/database.py
+-rw-r--r--   0        0        0     1155 2023-07-29 01:34:10.381343 nthp_api-0.1.7/nthp_api/smugmugger/schema.py
+-rw-r--r--   0        0        0     2019 2023-07-23 23:03:58.963517 nthp_api-0.1.7/nthp_api/smugmugger/smugmug.py
+-rw-r--r--   0        0        0     2166 2023-07-29 18:05:04.044912 nthp_api-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 nthp_api-0.1.7/PKG-INFO
```

### Comparing `nthp_api-0.1.6/README.md` & `nthp_api-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/cli/__init__.py` & `nthp_api-0.1.7/nthp_api/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from os import environ
 
 import click
-from nthp_build.version import get_version
 
 from nthp_api.cli import logs
+from nthp_api.nthp_build.version import get_version
 
 logs.init()
 
 
 log = logging.getLogger(__name__)
```

### Comparing `nthp_api-0.1.6/nthp_api/cli/logs.py` & `nthp_api-0.1.7/nthp_api/cli/logs.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/assets.py` & `nthp_api-0.1.7/nthp_api/nthp_build/assets.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/config.py` & `nthp_api-0.1.7/nthp_api/nthp_build/config.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/content.py` & `nthp_api-0.1.7/nthp_api/nthp_build/content.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/database.py` & `nthp_api-0.1.7/nthp_api/nthp_build/database.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/documents.py` & `nthp_api-0.1.7/nthp_api/nthp_build/documents.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/dumper.py` & `nthp_api-0.1.7/nthp_api/nthp_build/dumper.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/loader.py` & `nthp_api-0.1.7/nthp_api/nthp_build/loader.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/models.py` & `nthp_api-0.1.7/nthp_api/nthp_build/models.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/parallel.py` & `nthp_api-0.1.7/nthp_api/nthp_build/parallel.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/people.py` & `nthp_api-0.1.7/nthp_api/nthp_build/people.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/playwrights.py` & `nthp_api-0.1.7/nthp_api/nthp_build/playwrights.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/roles.py` & `nthp_api-0.1.7/nthp_api/nthp_build/roles.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/schema.py` & `nthp_api-0.1.7/nthp_api/nthp_build/schema.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/shows.py` & `nthp_api-0.1.7/nthp_api/nthp_build/shows.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/smugmug.py` & `nthp_api-0.1.7/nthp_api/nthp_build/smugmug.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/spec.py` & `nthp_api-0.1.7/nthp_api/nthp_build/spec.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/trivia.py` & `nthp_api-0.1.7/nthp_api/nthp_build/trivia.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/venues.py` & `nthp_api-0.1.7/nthp_api/nthp_build/venues.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/nthp_build/years.py` & `nthp_api-0.1.7/nthp_api/nthp_build/years.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/smugmugger/album.py` & `nthp_api-0.1.7/nthp_api/smugmugger/album.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/smugmugger/client.py` & `nthp_api-0.1.7/nthp_api/smugmugger/client.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/smugmugger/database.py` & `nthp_api-0.1.7/nthp_api/smugmugger/database.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/smugmugger/schema.py` & `nthp_api-0.1.7/nthp_api/smugmugger/schema.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/nthp_api/smugmugger/smugmug.py` & `nthp_api-0.1.7/nthp_api/smugmugger/smugmug.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.6/pyproject.toml` & `nthp_api-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nthp_api"
-version = "0.1.6"
+version = "0.1.7"
 description = "This is a CLI tool for building the Nottingham New Theatre's History Project content database."
 authors = ["Will Pimblett <will@wjdp.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/newtheatre/nthp-api"
 repository = "https://github.com/newtheatre/nthp-api"
```

### Comparing `nthp_api-0.1.6/PKG-INFO` & `nthp_api-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nthp-api
-Version: 0.1.6
+Version: 0.1.7
 Summary: This is a CLI tool for building the Nottingham New Theatre's History Project content database.
 Home-page: https://github.com/newtheatre/nthp-api
 License: MIT
 Author: Will Pimblett
 Author-email: will@wjdp.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

