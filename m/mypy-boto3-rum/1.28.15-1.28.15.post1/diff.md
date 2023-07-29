# Comparing `tmp/mypy-boto3-rum-1.28.15.tar.gz` & `tmp/mypy-boto3-rum-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rum-1.28.15.tar", last modified: Fri Jul 28 20:43:37 2023, max compression
+gzip compressed data, was "mypy-boto3-rum-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:04 2023, max compression
```

## Comparing `mypy-boto3-rum-1.28.15.tar` & `mypy-boto3-rum-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.213775 mypy-boto3-rum-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-28 20:43:37.213775 mypy-boto3-rum-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.209775 mypy-boto3-rum-1.28.15/mypy_boto3_rum/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21247 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.213775 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-28 20:43:36.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:37.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:36.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:36.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:37.213775 mypy-boto3-rum-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:37:24.000000 mypy-boto3-rum-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.657377 mypy-boto3-rum-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-29 10:04:04.657377 mypy-boto3-rum-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.653377 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21314 2023-07-29 09:57:34.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21277 2023-07-29 09:57:34.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.657377 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:04.000000 mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:04.657377 mypy-boto3-rum-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:57:33.000000 mypy-boto3-rum-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-rum-1.28.15/LICENSE` & `mypy-boto3-rum-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15/PKG-INFO` & `mypy-boto3-rum-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rum
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-rum-1.28.15/README.md` & `mypy-boto3-rum-1.28.15.post1/README.md`

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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/__init__.py` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/__init__.pyi` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/__main__.py` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchRUM 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.CloudWatchRUM 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM\nOther"
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

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/client.py` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,38 +10,40 @@
     from mypy_boto3_rum.client import CloudWatchRUMClient
 
     session = Session()
     client: CloudWatchRUMClient = session.client("rum")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MetricDestinationType
 from .paginator import (
     BatchGetRumMetricDefinitionsPaginator,
     GetAppMonitorDataPaginator,
     ListAppMonitorsPaginator,
     ListRumMetricsDestinationsPaginator,
 )
 from .type_defs import (
+    AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     CustomEventsTypeDef,
     GetAppMonitorDataResponseTypeDef,
     GetAppMonitorResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MetricDefinitionRequestOutputTypeDef,
     MetricDefinitionRequestTypeDef,
     QueryFilterTypeDef,
     RumEventTypeDef,
     TimeRangeTypeDef,
     UserDetailsTypeDef,
 )
 
@@ -91,15 +93,17 @@
         """
 
     def batch_create_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinitions: Sequence[MetricDefinitionRequestTypeDef],
+        MetricDefinitions: Sequence[
+            Union[MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef]
+        ],
         DestinationArn: str = ...
     ) -> BatchCreateRumMetricDefinitionsResponseTypeDef:
         """
         Specifies the extended metrics and custom metrics that you want a CloudWatch RUM
         app monitor to send to a destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_create_rum_metric_definitions)
@@ -156,15 +160,17 @@
         """
 
     def create_app_monitor(
         self,
         *,
         Domain: str,
         Name: str,
-        AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
+        AppMonitorConfiguration: Union[
+            AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
+        ] = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateAppMonitorResponseTypeDef:
         """
         Creates a Amazon CloudWatch RUM app monitor, which collects telemetry data from
         your application and sends that data to RUM.
@@ -310,15 +316,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/client/#untag_resource)
         """
 
     def update_app_monitor(
         self,
         *,
         Name: str,
-        AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
+        AppMonitorConfiguration: Union[
+            AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
+        ] = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Domain: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the configuration of an existing app monitor.
 
@@ -327,15 +335,17 @@
         """
 
     def update_rum_metric_definition(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinition: MetricDefinitionRequestTypeDef,
+        MetricDefinition: Union[
+            MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef
+        ],
         MetricDefinitionId: str,
         DestinationArn: str = ...
     ) -> Dict[str, Any]:
         """
         Modifies one existing metric definition for CloudWatch RUM extended metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.update_rum_metric_definition)
```

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/client.pyi` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,38 +10,40 @@
     from mypy_boto3_rum.client import CloudWatchRUMClient
 
     session = Session()
     client: CloudWatchRUMClient = session.client("rum")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MetricDestinationType
 from .paginator import (
     BatchGetRumMetricDefinitionsPaginator,
     GetAppMonitorDataPaginator,
     ListAppMonitorsPaginator,
     ListRumMetricsDestinationsPaginator,
 )
 from .type_defs import (
+    AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     CustomEventsTypeDef,
     GetAppMonitorDataResponseTypeDef,
     GetAppMonitorResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MetricDefinitionRequestOutputTypeDef,
     MetricDefinitionRequestTypeDef,
     QueryFilterTypeDef,
     RumEventTypeDef,
     TimeRangeTypeDef,
     UserDetailsTypeDef,
 )
 
@@ -86,15 +88,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/client/#exceptions)
         """
     def batch_create_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinitions: Sequence[MetricDefinitionRequestTypeDef],
+        MetricDefinitions: Sequence[
+            Union[MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef]
+        ],
         DestinationArn: str = ...
     ) -> BatchCreateRumMetricDefinitionsResponseTypeDef:
         """
         Specifies the extended metrics and custom metrics that you want a CloudWatch RUM
         app monitor to send to a destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_create_rum_metric_definitions)
@@ -146,15 +150,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/client/#close)
         """
     def create_app_monitor(
         self,
         *,
         Domain: str,
         Name: str,
-        AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
+        AppMonitorConfiguration: Union[
+            AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
+        ] = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateAppMonitorResponseTypeDef:
         """
         Creates a Amazon CloudWatch RUM app monitor, which collects telemetry data from
         your application and sends that data to RUM.
@@ -287,15 +293,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/client/#untag_resource)
         """
     def update_app_monitor(
         self,
         *,
         Name: str,
-        AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
+        AppMonitorConfiguration: Union[
+            AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
+        ] = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Domain: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the configuration of an existing app monitor.
 
@@ -303,15 +311,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/client/#update_app_monitor)
         """
     def update_rum_metric_definition(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinition: MetricDefinitionRequestTypeDef,
+        MetricDefinition: Union[
+            MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef
+        ],
         MetricDefinitionId: str,
         DestinationArn: str = ...
     ) -> Dict[str, Any]:
         """
         Modifies one existing metric definition for CloudWatch RUM extended metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.update_rum_metric_definition)
```

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/literals.py` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/literals.pyi` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/paginator.py` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/paginator.pyi` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/type_defs.py` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,15 +544,17 @@
 )
 
 _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
         "Destination": MetricDestinationType,
-        "MetricDefinitions": Sequence[MetricDefinitionRequestTypeDef],
+        "MetricDefinitions": Sequence[
+            Union[MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef]
+        ],
     },
 )
 _OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     {
         "DestinationArn": str,
     },
```

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum/type_defs.pyi` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -519,15 +519,17 @@
 )
 
 _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
         "Destination": MetricDestinationType,
-        "MetricDefinitions": Sequence[MetricDefinitionRequestTypeDef],
+        "MetricDefinitions": Sequence[
+            Union[MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef]
+        ],
     },
 )
 _OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     {
         "DestinationArn": str,
     },
```

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/PKG-INFO` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rum
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/SOURCES.txt` & `mypy-boto3-rum-1.28.15.post1/mypy_boto3_rum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.15/setup.py` & `mypy-boto3-rum-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rum",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_rum"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

