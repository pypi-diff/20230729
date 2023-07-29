# Comparing `tmp/mypy-boto3-logs-1.28.15.tar.gz` & `tmp/mypy-boto3-logs-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-logs-1.28.15.tar", last modified: Fri Jul 28 20:43:11 2023, max compression
+gzip compressed data, was "mypy-boto3-logs-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:33 2023, max compression
```

## Comparing `mypy-boto3-logs-1.28.15.tar` & `mypy-boto3-logs-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.501422 mypy-boto3-logs-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-07-28 20:43:11.501422 mypy-boto3-logs-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.489422 mypy-boto3-logs-1.28.15/mypy_boto3_logs/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38327 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38260 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-07-28 20:30:29.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37723 2023-07-28 20:30:30.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37688 2023-07-28 20:30:29.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.501422 mypy-boto3-logs-1.28.15/mypy_boto3_logs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-07-28 20:43:11.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 20:43:11.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:11.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:43:11.000000 mypy-boto3-logs-1.28.15/mypy_boto3_logs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:11.501422 mypy-boto3-logs-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-28 20:30:28.000000 mypy-boto3-logs-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.957252 mypy-boto3-logs-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18875 2023-07-29 10:03:33.949252 mypy-boto3-logs-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.949252 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38437 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38370 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-07-29 09:50:06.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37794 2023-07-29 09:50:07.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37759 2023-07-29 09:50:07.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.949252 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18875 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:03:33.000000 mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:33.957252 mypy-boto3-logs-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-29 09:50:05.000000 mypy-boto3-logs-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-logs-1.28.15/LICENSE` & `mypy-boto3-logs-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15/PKG-INFO` & `mypy-boto3-logs-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-logs
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudWatchLogs 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudWatchLogs 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-logs-1.28.15/README.md` & `mypy-boto3-logs-1.28.15.post1/README.md`

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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/__init__.py` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/__init__.pyi` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/__main__.py` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchLogs 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.CloudWatchLogs 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs\nOther"
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

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/client.py` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_logs.client import CloudWatchLogsClient
 
     session = Session()
     client: CloudWatchLogsClient = session.client("logs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DistributionType, ExportTaskStatusCodeType, OrderByType, QueryStatusType
 from .paginator import (
     DescribeDestinationsPaginator,
     DescribeExportTasksPaginator,
@@ -49,14 +49,15 @@
     GetLogEventsResponseTypeDef,
     GetLogGroupFieldsResponseTypeDef,
     GetLogRecordResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupResponseTypeDef,
+    MetricTransformationOutputTypeDef,
     MetricTransformationTypeDef,
     PutAccountPolicyResponseTypeDef,
     PutDataProtectionPolicyResponseTypeDef,
     PutDestinationResponseTypeDef,
     PutLogEventsResponseTypeDef,
     PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
@@ -612,15 +613,17 @@
 
     def put_metric_filter(
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
-        metricTransformations: Sequence[MetricTransformationTypeDef]
+        metricTransformations: Sequence[
+            Union[MetricTransformationTypeDef, MetricTransformationOutputTypeDef]
+        ]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a metric filter and associates it with the specified log
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_metric_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#put_metric_filter)
```

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/client.pyi` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_logs.client import CloudWatchLogsClient
 
     session = Session()
     client: CloudWatchLogsClient = session.client("logs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DistributionType, ExportTaskStatusCodeType, OrderByType, QueryStatusType
 from .paginator import (
     DescribeDestinationsPaginator,
     DescribeExportTasksPaginator,
@@ -49,14 +49,15 @@
     GetLogEventsResponseTypeDef,
     GetLogGroupFieldsResponseTypeDef,
     GetLogRecordResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupResponseTypeDef,
+    MetricTransformationOutputTypeDef,
     MetricTransformationTypeDef,
     PutAccountPolicyResponseTypeDef,
     PutDataProtectionPolicyResponseTypeDef,
     PutDestinationResponseTypeDef,
     PutLogEventsResponseTypeDef,
     PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
@@ -565,15 +566,17 @@
         """
     def put_metric_filter(
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
-        metricTransformations: Sequence[MetricTransformationTypeDef]
+        metricTransformations: Sequence[
+            Union[MetricTransformationTypeDef, MetricTransformationOutputTypeDef]
+        ]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a metric filter and associates it with the specified log
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_metric_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#put_metric_filter)
```

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/literals.py` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/literals.pyi` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/paginator.py` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/paginator.pyi` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/type_defs.py` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_logs.type_defs import AccountPolicyTypeDef
 
     data: AccountPolicyTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     DataProtectionStatusType,
     DistributionType,
     ExportTaskStatusCodeType,
     OrderByType,
     QueryStatusType,
@@ -1461,15 +1461,17 @@
 
 PutMetricFilterRequestRequestTypeDef = TypedDict(
     "PutMetricFilterRequestRequestTypeDef",
     {
         "logGroupName": str,
         "filterName": str,
         "filterPattern": str,
-        "metricTransformations": Sequence[MetricTransformationTypeDef],
+        "metricTransformations": Sequence[
+            Union[MetricTransformationTypeDef, MetricTransformationOutputTypeDef]
+        ],
     },
 )
 
 PutLogEventsResponseTypeDef = TypedDict(
     "PutLogEventsResponseTypeDef",
     {
         "nextSequenceToken": str,
```

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs/type_defs.pyi` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_logs.type_defs import AccountPolicyTypeDef
 
     data: AccountPolicyTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     DataProtectionStatusType,
     DistributionType,
     ExportTaskStatusCodeType,
     OrderByType,
     QueryStatusType,
@@ -1426,15 +1426,17 @@
 
 PutMetricFilterRequestRequestTypeDef = TypedDict(
     "PutMetricFilterRequestRequestTypeDef",
     {
         "logGroupName": str,
         "filterName": str,
         "filterPattern": str,
-        "metricTransformations": Sequence[MetricTransformationTypeDef],
+        "metricTransformations": Sequence[
+            Union[MetricTransformationTypeDef, MetricTransformationOutputTypeDef]
+        ],
     },
 )
 
 PutLogEventsResponseTypeDef = TypedDict(
     "PutLogEventsResponseTypeDef",
     {
         "nextSequenceToken": str,
```

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs.egg-info/PKG-INFO` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-logs
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudWatchLogs 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudWatchLogs 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-logs-1.28.15/mypy_boto3_logs.egg-info/SOURCES.txt` & `mypy-boto3-logs-1.28.15.post1/mypy_boto3_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.28.15/setup.py` & `mypy-boto3-logs-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-logs",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_logs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CloudWatchLogs 1.28.15 service generated with"
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

