# Comparing `tmp/tableconv-1.9924.20230601.tar.gz` & `tmp/tableconv-1.9943.20230729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableconv-1.9924.20230601.tar", last modified: Thu Jun  1 20:01:38 2023, max compression
+gzip compressed data, was "tableconv-1.9943.20230729.tar", last modified: Sat Jul 29 02:02:34 2023, max compression
```

## Comparing `tableconv-1.9924.20230601.tar` & `tableconv-1.9943.20230729.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/
--rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-09-03 04:22:14.000000 tableconv-1.9924.20230601/LICENSE
--rw-rw-r--   0 john      (1000) john      (1000)       26 2021-09-03 04:22:14.000000 tableconv-1.9924.20230601/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     9258 2023-03-26 03:16:21.000000 tableconv-1.9924.20230601/README.md
--rw-rw-r--   0 john      (1000) john      (1000)       38 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     2232 2023-01-22 04:21:13.000000 tableconv-1.9924.20230601/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/tableconv/
--rw-rw-r--   0 john      (1000) john      (1000)      400 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)       73 2023-06-01 20:00:30.000000 tableconv-1.9924.20230601/tableconv/__version__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/tableconv/adapters/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2021-09-03 04:22:14.000000 tableconv-1.9924.20230601/tableconv/adapters/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/tableconv/adapters/df/
--rw-rw-r--   0 john      (1000) john      (1000)      926 2023-01-27 19:23:04.000000 tableconv-1.9924.20230601/tableconv/adapters/df/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4264 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/ascii.py
--rw-rw-r--   0 john      (1000) john      (1000)    14948 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/aws_athena.py
--rw-rw-r--   0 john      (1000) john      (1000)     1081 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/aws_dynamodb.py
--rw-r--r--   0 john      (1000) john      (1000)     2394 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/aws_logs.py
--rw-rw-r--   0 john      (1000) john      (1000)     1696 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/base.py
--rw-rw-r--   0 john      (1000) john      (1000)      403 2022-01-02 03:01:01.000000 tableconv-1.9924.20230601/tableconv/adapters/df/example.py
--rw-rw-r--   0 john      (1000) john      (1000)     2526 2023-05-30 16:53:38.000000 tableconv-1.9924.20230601/tableconv/adapters/df/file_adapter_mixin.py
--rw-rw-r--   0 john      (1000) john      (1000)    12737 2023-05-02 00:16:20.000000 tableconv-1.9924.20230601/tableconv/adapters/df/gsheets.py
--rw-rw-r--   0 john      (1000) john      (1000)      322 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/jira.py
--rw-rw-r--   0 john      (1000) john      (1000)     6463 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/json.py
--rw-rw-r--   0 john      (1000) john      (1000)     1876 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/nested_list.py
--rw-r--r--   0 john      (1000) john      (1000)     1509 2023-03-26 03:15:45.000000 tableconv-1.9924.20230601/tableconv/adapters/df/numbers.py
--rw-rw-r--   0 john      (1000) john      (1000)     8873 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/pandas_io.py
--rw-rw-r--   0 john      (1000) john      (1000)     1642 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/python.py
--rw-rw-r--   0 john      (1000) john      (1000)     5805 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/rdbms.py
--rw-rw-r--   0 john      (1000) john      (1000)     2494 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/smart_sheet.py
--rw-r--r--   0 john      (1000) john      (1000)      866 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/sql_literal.py
--rw-rw-r--   0 john      (1000) john      (1000)     7489 2023-05-03 19:19:16.000000 tableconv-1.9924.20230601/tableconv/adapters/df/sumo_logic.py
--rw-rw-r--   0 john      (1000) john      (1000)     2999 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/text_array.py
--rw-rw-r--   0 john      (1000) john      (1000)     1644 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/yaml.py
--rw-rw-r--   0 john      (1000) john      (1000)    15584 2023-03-26 03:19:10.000000 tableconv-1.9924.20230601/tableconv/core.py
--rw-r--r--   0 john      (1000) john      (1000)     2128 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/exceptions.py
--rw-rw-r--   0 john      (1000) john      (1000)     2905 2023-06-01 19:58:47.000000 tableconv-1.9924.20230601/tableconv/in_memory_query.py
--rw-rw-r--   0 john      (1000) john      (1000)     5836 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/interactive.py
--rw-rw-r--   0 john      (1000) john      (1000)    11203 2023-05-05 19:10:26.000000 tableconv-1.9924.20230601/tableconv/main.py
--rw-rw-r--   0 john      (1000) john      (1000)      726 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/parse_time.py
--rw-rw-r--   0 john      (1000) john      (1000)     1469 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/uri.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/tableconv.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     1242 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       66 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      243 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       27 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/top_level.txt
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/tableconv_daemon/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-01-15 04:13:45.000000 tableconv-1.9924.20230601/tableconv_daemon/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9537 2023-03-26 02:56:00.000000 tableconv-1.9924.20230601/tableconv_daemon/main.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.199421 tableconv-1.9943.20230729/
+-rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-09-03 04:22:14.000000 tableconv-1.9943.20230729/LICENSE
+-rw-rw-r--   0 john      (1000) john      (1000)       26 2021-09-03 04:22:14.000000 tableconv-1.9943.20230729/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-07-29 02:02:34.199421 tableconv-1.9943.20230729/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     9258 2023-03-26 03:16:21.000000 tableconv-1.9943.20230729/README.md
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2023-07-29 02:02:34.199421 tableconv-1.9943.20230729/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     2232 2023-01-22 04:21:13.000000 tableconv-1.9943.20230729/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.195422 tableconv-1.9943.20230729/tableconv/
+-rw-rw-r--   0 john      (1000) john      (1000)      400 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)       73 2023-07-29 02:00:37.000000 tableconv-1.9943.20230729/tableconv/__version__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.195422 tableconv-1.9943.20230729/tableconv/adapters/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2021-09-03 04:22:14.000000 tableconv-1.9943.20230729/tableconv/adapters/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.199421 tableconv-1.9943.20230729/tableconv/adapters/df/
+-rw-rw-r--   0 john      (1000) john      (1000)      926 2023-01-27 19:23:04.000000 tableconv-1.9943.20230729/tableconv/adapters/df/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4264 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/ascii.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14948 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/aws_athena.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1081 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/aws_dynamodb.py
+-rw-r--r--   0 john      (1000) john      (1000)     2394 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/aws_logs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1696 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)      403 2022-01-02 03:01:01.000000 tableconv-1.9943.20230729/tableconv/adapters/df/example.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2526 2023-05-30 16:53:38.000000 tableconv-1.9943.20230729/tableconv/adapters/df/file_adapter_mixin.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13123 2023-07-29 01:59:21.000000 tableconv-1.9943.20230729/tableconv/adapters/df/gsheets.py
+-rw-rw-r--   0 john      (1000) john      (1000)      339 2023-06-26 23:24:34.000000 tableconv-1.9943.20230729/tableconv/adapters/df/jira.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6463 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/json.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1876 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/nested_list.py
+-rw-r--r--   0 john      (1000) john      (1000)     1509 2023-03-26 03:15:45.000000 tableconv-1.9943.20230729/tableconv/adapters/df/numbers.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8885 2023-06-30 22:42:07.000000 tableconv-1.9943.20230729/tableconv/adapters/df/pandas_io.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1642 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/python.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5805 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/rdbms.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2494 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/smart_sheet.py
+-rw-r--r--   0 john      (1000) john      (1000)      866 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/sql_literal.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7489 2023-06-16 22:05:58.000000 tableconv-1.9943.20230729/tableconv/adapters/df/sumo_logic.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2999 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/text_array.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1644 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/yaml.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15649 2023-06-16 22:00:59.000000 tableconv-1.9943.20230729/tableconv/core.py
+-rw-r--r--   0 john      (1000) john      (1000)     2301 2023-07-29 01:57:22.000000 tableconv-1.9943.20230729/tableconv/exceptions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3096 2023-06-30 23:18:47.000000 tableconv-1.9943.20230729/tableconv/in_memory_query.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5836 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/interactive.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11215 2023-06-30 23:07:40.000000 tableconv-1.9943.20230729/tableconv/main.py
+-rw-rw-r--   0 john      (1000) john      (1000)      726 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/parse_time.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1469 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/uri.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.195422 tableconv-1.9943.20230729/tableconv.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     1242 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       66 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      243 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       27 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.199421 tableconv-1.9943.20230729/tableconv_daemon/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-01-15 04:13:45.000000 tableconv-1.9943.20230729/tableconv_daemon/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9537 2023-03-26 02:56:00.000000 tableconv-1.9943.20230729/tableconv_daemon/main.py
```

### Comparing `tableconv-1.9924.20230601/LICENSE` & `tableconv-1.9943.20230729/LICENSE`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/PKG-INFO` & `tableconv-1.9943.20230729/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableconv
-Version: 1.9924.20230601
+Version: 1.9943.20230729
 Summary: CLI data plumbing tool
 Home-page: https://github.com/personalcomputer/tableconv
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tableconv-1.9924.20230601/README.md` & `tableconv-1.9943.20230729/README.md`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/setup.py` & `tableconv-1.9943.20230729/setup.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/__init__.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/__init__.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/ascii.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/ascii.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/aws_athena.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/aws_athena.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/aws_dynamodb.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/aws_dynamodb.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/aws_logs.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/aws_logs.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/base.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/base.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/file_adapter_mixin.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/file_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/gsheets.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/gsheets.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from tableconv.adapters.df.base import Adapter, register_adapter
 from tableconv.exceptions import (
     AppendSchemeConflictError,
     InvalidLocationReferenceError,
     InvalidParamsError,
     TableAlreadyExistsError,
+    URLInaccessibleError,
 )
 from tableconv.uri import parse_uri
 
 logger = logging.getLogger(__name__)
 
 
 def list_ljust(ls, n, fill_value=None):
@@ -56,15 +57,21 @@
         GoogleSheetsAdapter._get_oauth_credentials()  # Trigger OAuth flow prompt
 
     @staticmethod
     def _get_oauth_credentials():
         from oauth2client import client, tools
         from oauth2client.file import Storage
 
-        store = Storage(os.path.expanduser("~/.tableconv-gsheets-credentials"))
+        creds_path = os.path.expanduser("~/.tableconv-gsheets-credentials")
+        if not os.path.exists(creds_path):
+            raise URLInaccessibleError(
+                'gsheets integration requires configuring Google Sheets API authentication credentials. '
+                'Please run `tableconv configure gsheets --help` for help.'
+            )
+        store = Storage(creds_path)
         credentials = store.get()
         sys.argv = [""]
         if not credentials or credentials.invalid:
             SCOPES = [
                 "https://www.googleapis.com/auth/spreadsheets",
                 "https://www.googleapis.com/auth/drive",
             ]
@@ -83,16 +90,16 @@
             http = None
         else:
             # login using OAuth
             http = GoogleSheetsAdapter._get_oauth_credentials().authorize(httplib2.Http())
 
         return googleapiclient.discovery.build(service, version, http=http)
 
-    @staticmethod
-    def load(uri, query):
+    @classmethod
+    def load(cls, uri, query):
         parsed_uri = parse_uri(uri)
         spreadsheet_id = parsed_uri.authority
         sheet_name = parsed_uri.path.strip("/")
 
         if not sheet_name:
             raise InvalidLocationReferenceError("Must specify sheet_name")
 
@@ -108,15 +115,16 @@
             )
             .execute()
         )
 
         num_columns = max(*[len(r) for r in  raw_data["values"]])
         header = list_ljust(raw_data["values"][0], num_columns)
         values = [list_ljust(row, num_columns) for row in raw_data["values"][1:]]
-        return pd.DataFrame(values, columns=header)
+        df = pd.DataFrame(values, columns=header)
+        return cls._query_in_memory(df, query)
 
     @staticmethod
     def _create_spreadsheet(googlesheets, spreadsheet_name, first_sheet_name, columns, rows):
         sheet = {
             "properties": {
                 "autoRecalc": "ON_CHANGE",
                 "title": spreadsheet_name,
```

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/json.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/json.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/nested_list.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/nested_list.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/numbers.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/numbers.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/pandas_io.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/pandas_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                     path_or_buf = open(path, "w")
                 elif if_exists == "append":
                     with open(path) as f:
                         existing_columns = next(csv.reader(f, delimiter=params["sep"]))
                     if list(existing_columns) != list(df.columns):
                         raise ValueError(
                             f"Cannot append to {path}, existing schema does not match. "
-                            + f"(existing: {existing_columns}. new: {df.columns}))"
+                            + f"(existing: {list(existing_columns)}. new: {list(df.columns)}))"
                         )
                     params["header"] = False
                     path_or_buf = open(path, "a")
                 else:
                     assert if_exists == "fail"
                     # (continue, df.to_csv will fail)
         df.to_csv(path_or_buf, **params)
```

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/python.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/python.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/rdbms.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/rdbms.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/smart_sheet.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/smart_sheet.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/sql_literal.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/sql_literal.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/sumo_logic.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/sumo_logic.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/text_array.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/text_array.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/adapters/df/yaml.py` & `tableconv-1.9943.20230729/tableconv/adapters/df/yaml.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/core.py` & `tableconv-1.9943.20230729/tableconv/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,16 @@
         if params:
             # TODO: This is a total hack! Implementing real structured table references, including structured passing of
             # params to adapters, is still pending. Right now everything is stringly-typed internally.
             assert "?" not in url
             url += f"?{urllib.parse.urlencode(params)}"
         write_adapter_name = write_adapter.__qualname__  # type: ignore[attr-defined]
         logger.debug(f"Exporting data out via {write_adapter_name} to {url}")
-        return write_adapter.dump(self.df, url)
+        with pd.option_context('display.float_format', str):
+            return write_adapter.dump(self.df, url)
 
     def get_json_schema(self):
         """
         Warning: This is just experimental / exploratory. The current implementation is also buggy.
         """
         # Consider instead using https://github.com/pandas-dev/pandas/blob/v1.3.2/pandas/io/json/_table_schema.py
         from genson import SchemaBuilder
```

### Comparing `tableconv-1.9924.20230601/tableconv/exceptions.py` & `tableconv-1.9943.20230729/tableconv/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,20 @@
     Exposed in public API.
     Anything related to accessing the URL is considered a URL error.
     """
 
     pass
 
 
+class URLInaccessibleError(InvalidURLError):
+    """the uri is not accessible, perhaps because of permissions errors, missing authentication information, etc"""
+
+    pass
+
+
 class InvalidParamsError(InvalidURLError):
     """the parameters passed in are invalid/unsupported/unrecognized"""
 
     pass
 
 
 class IncapableDestinationError(InvalidURLError):
```

### Comparing `tableconv-1.9924.20230601/tableconv/in_memory_query.py` & `tableconv-1.9943.20230729/tableconv/in_memory_query.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,31 +30,34 @@
     if flattened:
         flattened_display = ", ".join([str(column) for column in flattened])
         logger.warning(f"Flattened some columns into strings for in-memory query: {flattened_display}")
 
 
 def pre_process(dfs, query) -> Tuple:
     """
-    Very weak hack to add support for a new type of transformation within the existing language of SQL: Gives us very
-    weak version of a `transpose()` function. Warning: this actually mutates `df`s.
+    Preprocess the SQL query, to allow us to extend the DuckDB query language. Supported extensions:
+    - transpose()
+    - from_unix()
+    - from_iso8601()
+
+    Warning: this function preprocesses both the query and the dfs, i.e. it actually mutates `dfs` too!
     """
     if "transpose(data)" in query:
-        ANTI_CONFLICT_STR = "027eade341cf"  # (random text)
+        ANTI_CONFLICT_STR = "027eade341cf"  # (random text to avoid name conflicts)
         transposed_data_table_name = f"transposed_data_{ANTI_CONFLICT_STR}"
         query = query.replace("transpose(data)", f'"{transposed_data_table_name}"')
         for table_name, df in dfs:
             if table_name == "data":
                 data_df = df
                 break
         transposed_data_df = data_df.transpose(copy=True).reset_index()
         dfs.append((transposed_data_table_name, transposed_data_df))
 
-    query = re.sub(r"\bunix\((.+?)\)", r"(TIMESTAMP '1970-01-01 00:00:00' + to_seconds(\1))", query)
-    query = re.sub(r"\biso8601\((.+?)\)", r"CAST(\1 AS TIMESTAMP)", query)
-    # re.sub(r"\biso8601\((.+?)\)", r"strptime(\1, '2023-04-01T18:36:01.200234+00:00')", query)
+    query = re.sub(r"\b(?:from_)?unix\((.+?)\)", r"(TIMESTAMP '1970-01-01 00:00:00' + to_seconds(\1))", query)
+    query = re.sub(r"\b(?:from_)?iso8601\((.+?)\)", r"CAST(\1 AS TIMESTAMP)", query)
 
     return dfs, query
 
 
 def query_in_memory(dfs: List[Tuple[str, pd.DataFrame]], query: str) -> pd.DataFrame:
     """Warning: Has a side effect of mutating the dfs"""
     import duckdb
@@ -62,11 +65,15 @@
     duck_conn = duckdb.connect(database=":memory:", read_only=False)
     dfs, query = pre_process(dfs, query)
     for table_name, df in dfs:
         flatten_arrays_for_duckdb(df)
         duck_conn.register(table_name, df)
     try:
         duck_conn.execute(query)
-    except RuntimeError as exc:
+    except (RuntimeError, duckdb.ParserException) as exc:
         raise InvalidQueryError(*exc.args) from exc
+    except duckdb.StandardException as exc:
+        if 'Parser Error' in exc.args[0]:
+            raise InvalidQueryError(*exc.args) from exc
+        raise
     result_df = duck_conn.fetchdf()
     return result_df
```

### Comparing `tableconv-1.9924.20230601/tableconv/interactive.py` & `tableconv-1.9943.20230729/tableconv/interactive.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/main.py` & `tableconv-1.9943.20230729/tableconv/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             "help & support:\n  https://github.com/personalcomputer/tableconv/issues/new"
         ),
         exit_on_error=False,
     )
     parser.add_argument("SOURCE_URL", type=str, help="Specify the data source URL.")
     parser.add_argument("-q", "-Q", "--query", dest="source_query", default=None, help="Query to run on the source. Even for non-SQL datasources (e.g. csv or json), SQL querying is still supported, try `SELECT * FROM data`.")  # noqa: E501
     parser.add_argument("-F", "--filter", dest="intermediate_filter_sql", default=None, help="Filter (i.e. transform) the input data using a SQL query operating on the dataset in memory using DuckDB SQL.")  # noqa: E501
-    parser.add_argument("-o", "--dest", "--out", dest="DEST_URL", type=str, help="Specify the data destination URL. If this destination already exists, be aware that the default behavior is to overwrite.")  # noqa: E501
+    parser.add_argument("-o", "--dest", "--out", "--output", dest="DEST_URL", type=str, help="Specify the data destination URL. If this destination already exists, be aware that the default behavior is to overwrite.")  # noqa: E501
     parser.add_argument("-i", "--interactive", action="store_true", help="Enter interactive REPL query mode.")  # noqa: E501
     parser.add_argument("--open", dest="open_dest", action="store_true", help="Open resulting file/url in the operating system desktop environment. (not supported for all destination types)")  # noqa: E501
     parser.add_argument("--schema", "--coerce-schema", dest="schema_coercion", default=None, help="Coerce source schema according to a schema definition. (WARNING: experimental feature)")  # noqa: E501
     parser.add_argument("--restrict-schema", dest="restrict_schema", action="store_true", help="Exclude all columns not included in the SCHEMA_COERCION definition. (WARNING: experimental feature)")  # noqa: E501
     parser.add_argument("-v", "--verbose", "--debug", dest="verbose", action="store_true", help="Show debug details, including API calls and error sources.")  # noqa: E501
     parser.add_argument("--version", action="version", help="Show version number and exit", version=f"%(prog)s {__version__}")  # noqa: E501
     parser.add_argument("--quiet", action="store_true", help="Only display errors.")
```

### Comparing `tableconv-1.9924.20230601/tableconv/parse_time.py` & `tableconv-1.9943.20230729/tableconv/parse_time.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv/uri.py` & `tableconv-1.9943.20230729/tableconv/uri.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv.egg-info/PKG-INFO` & `tableconv-1.9943.20230729/tableconv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableconv
-Version: 1.9924.20230601
+Version: 1.9943.20230729
 Summary: CLI data plumbing tool
 Home-page: https://github.com/personalcomputer/tableconv
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tableconv-1.9924.20230601/tableconv.egg-info/SOURCES.txt` & `tableconv-1.9943.20230729/tableconv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tableconv-1.9924.20230601/tableconv_daemon/main.py` & `tableconv-1.9943.20230729/tableconv_daemon/main.py`

 * *Files identical despite different names*

