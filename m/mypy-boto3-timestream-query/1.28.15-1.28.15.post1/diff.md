# Comparing `tmp/mypy-boto3-timestream-query-1.28.15.tar.gz` & `tmp/mypy-boto3-timestream-query-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-query-1.28.15.tar", last modified: Fri Jul 28 20:43:52 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-query-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:21 2023, max compression
```

## Comparing `mypy-boto3-timestream-query-1.28.15.tar` & `mypy-boto3-timestream-query-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.589985 mypy-boto3-timestream-query-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-07-28 20:43:52.585985 mypy-boto3-timestream-query-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.577985 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-07-28 20:40:37.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-07-28 20:40:37.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-28 20:40:37.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-07-28 20:40:37.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21640 2023-07-28 20:40:37.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.585985 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:52.589985 mypy-boto3-timestream-query-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:21.801442 mypy-boto3-timestream-query-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-07-29 10:04:21.801442 mypy-boto3-timestream-query-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:21.789441 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-07-29 10:00:49.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-07-29 10:00:49.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-07-29 10:00:49.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21640 2023-07-29 10:00:49.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:21.801442 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:04:21.000000 mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:21.801442 mypy-boto3-timestream-query-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 10:00:48.000000 mypy-boto3-timestream-query-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-timestream-query-1.28.15/LICENSE` & `mypy-boto3-timestream-query-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15/PKG-INFO` & `mypy-boto3-timestream-query-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.28.15
-Summary: Type annotations for boto3.TimestreamQuery 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.TimestreamQuery 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-timestream-query-1.28.15/README.md` & `mypy-boto3-timestream-query-1.28.15.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__init__.py` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__init__.pyi` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__main__.py` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamQuery 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.TimestreamQuery 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.15.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/client.py` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     ListScheduledQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
+    TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -114,15 +115,17 @@
         *,
         Name: str,
         QueryString: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
-        TargetConfiguration: TargetConfigurationTypeDef = ...,
+        TargetConfiguration: Union[
+            TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
+        ] = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
```

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/client.pyi` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     ListScheduledQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
+    TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -106,15 +107,17 @@
         *,
         Name: str,
         QueryString: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
-        TargetConfiguration: TargetConfigurationTypeDef = ...,
+        TargetConfiguration: Union[
+            TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
+        ] = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
```

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/literals.py` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/literals.pyi` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/paginator.py` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/paginator.pyi` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/type_defs.py` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,23 +147,23 @@
         "Value": str,
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
-        "Data": List["DatumTypeDef"],
+        "Data": List[Dict[str, Any]],
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
-        "Value": Dict[str, Any],
+        "Value": "DatumTypeDef",
     },
 )
 
 DeleteScheduledQueryRequestRequestTypeDef = TypedDict(
     "DeleteScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
```

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/type_defs.pyi` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -144,23 +144,23 @@
         "Value": str,
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
-        "Data": List["DatumTypeDef"],
+        "Data": List[Dict[str, Any]],
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
-        "Value": Dict[str, Any],
+        "Value": "DatumTypeDef",
     },
 )
 
 DeleteScheduledQueryRequestRequestTypeDef = TypedDict(
     "DeleteScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
```

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/PKG-INFO` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.28.15
-Summary: Type annotations for boto3.TimestreamQuery 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.TimestreamQuery 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/SOURCES.txt` & `mypy-boto3-timestream-query-1.28.15.post1/mypy_boto3_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.15/setup.py` & `mypy-boto3-timestream-query-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-query",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.TimestreamQuery 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

