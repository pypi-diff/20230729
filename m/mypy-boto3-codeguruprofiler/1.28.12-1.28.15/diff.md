# Comparing `tmp/mypy-boto3-codeguruprofiler-1.28.12.tar.gz` & `tmp/mypy-boto3-codeguruprofiler-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguruprofiler-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguruprofiler-1.28.15.tar", last modified: Fri Jul 28 20:42:31 2023, max compression
```

## Comparing `mypy-boto3-codeguruprofiler-1.28.12.tar` & `mypy-boto3-codeguruprofiler-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.012550 mypy-boto3-codeguruprofiler-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-07-27 05:34:29.008550 mypy-boto3-codeguruprofiler-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.004550 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19828 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23179 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-07-27 05:19:10.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.008550 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:28.000000 mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.012550 mypy-boto3-codeguruprofiler-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:19:09.000000 mypy-boto3-codeguruprofiler-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.176862 mypy-boto3-codeguruprofiler-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15615 2023-07-28 20:42:31.176862 mypy-boto3-codeguruprofiler-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.164862 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19828 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-07-28 20:21:38.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22913 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:37.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.176862 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15615 2023-07-28 20:42:30.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:42:30.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:30.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:30.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:30.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:42:30.000000 mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:31.176862 mypy-boto3-codeguruprofiler-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:21:36.000000 mypy-boto3-codeguruprofiler-1.28.15/setup.py
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/LICENSE` & `mypy-boto3-codeguruprofiler-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/PKG-INFO` & `mypy-boto3-codeguruprofiler-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguruprofiler
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeGuruProfiler 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeGuruProfiler 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguruprofiler)](https://pepy.tech/project/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,16 +329,16 @@
 
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
     ChannelTypeDef,
+    ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
-    AgentOrchestrationConfigOutputTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
     FrameMetricTypeDef,
     TimestampStructureTypeDef,
     ChannelOutputTypeDef,
@@ -346,49 +346,48 @@
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
     FrameMetricOutputTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetProfileRequestRequestTypeDef,
-    GetProfileResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     ListFindingsReportsRequestRequestTypeDef,
-    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListProfileTimesRequestRequestTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MatchTypeDef,
-    PaginatorConfigTypeDef,
     PatternTypeDef,
     PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
-    PutPermissionResponseTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    RemovePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddNotificationChannelsRequestRequestTypeDef,
+    GetPolicyResponseTypeDef,
+    GetProfileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutPermissionResponseTypeDef,
+    RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
     BatchGetFrameMetricDataRequestRequestTypeDef,
     NotificationConfigurationTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
     FrameMetricDatumTypeDef,
+    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
     ProfilingGroupDescriptionTypeDef,
     AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/README.md` & `mypy-boto3-codeguruprofiler-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguruprofiler)](https://pepy.tech/project/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,16 +297,16 @@
 
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
     ChannelTypeDef,
+    ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
-    AgentOrchestrationConfigOutputTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
     FrameMetricTypeDef,
     TimestampStructureTypeDef,
     ChannelOutputTypeDef,
@@ -314,49 +314,48 @@
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
     FrameMetricOutputTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetProfileRequestRequestTypeDef,
-    GetProfileResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     ListFindingsReportsRequestRequestTypeDef,
-    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListProfileTimesRequestRequestTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MatchTypeDef,
-    PaginatorConfigTypeDef,
     PatternTypeDef,
     PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
-    PutPermissionResponseTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    RemovePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddNotificationChannelsRequestRequestTypeDef,
+    GetPolicyResponseTypeDef,
+    GetProfileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutPermissionResponseTypeDef,
+    RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
     BatchGetFrameMetricDataRequestRequestTypeDef,
     NotificationConfigurationTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
     FrameMetricDatumTypeDef,
+    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
     ProfilingGroupDescriptionTypeDef,
     AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__init__.py` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__init__.pyi` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/__main__.py` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruProfiler 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodeGuruProfiler 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/client.py` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/client.pyi` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/literals.py` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/literals.pyi` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/paginator.py` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,38 +25,35 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AggregationPeriodType, OrderByType
 from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListProfileTimesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListProfileTimesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/paginators/#listprofiletimespaginator)
     """
 
     def paginate(
         self,
         *,
         endTime: Union[datetime, str],
         period: AggregationPeriodType,
         profilingGroupName: str,
         startTime: Union[datetime, str],
         orderBy: OrderByType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProfileTimesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/paginators/#listprofiletimespaginator)
         """
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/paginator.pyi` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,35 +25,38 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AggregationPeriodType, OrderByType
 from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListProfileTimesPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListProfileTimesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/paginators/#listprofiletimespaginator)
     """
 
     def paginate(
         self,
         *,
         endTime: Union[datetime, str],
         period: AggregationPeriodType,
         profilingGroupName: str,
         startTime: Union[datetime, str],
         orderBy: OrderByType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProfileTimesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/paginators/#listprofiletimespaginator)
         """
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/type_defs.py` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ChannelTypeDef",
+    "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
-    "AgentOrchestrationConfigOutputTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
     "FrameMetricTypeDef",
     "TimestampStructureTypeDef",
     "ChannelOutputTypeDef",
@@ -51,49 +51,48 @@
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
     "FrameMetricOutputTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetPolicyResponseTypeDef",
     "GetProfileRequestRequestTypeDef",
-    "GetProfileResponseTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "ListFindingsReportsRequestRequestTypeDef",
-    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListProfileTimesRequestRequestTypeDef",
     "ProfileTimeTypeDef",
     "ListProfilingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MatchTypeDef",
-    "PaginatorConfigTypeDef",
     "PatternTypeDef",
     "PostAgentProfileRequestRequestTypeDef",
     "PutPermissionRequestRequestTypeDef",
-    "PutPermissionResponseTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
-    "RemovePermissionResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddNotificationChannelsRequestRequestTypeDef",
+    "GetPolicyResponseTypeDef",
+    "GetProfileResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutPermissionResponseTypeDef",
+    "RemovePermissionResponseTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
     "BatchGetFrameMetricDataRequestRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
     "FrameMetricDatumTypeDef",
+    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
     "ProfilingGroupDescriptionTypeDef",
     "AnomalyTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
@@ -121,14 +120,25 @@
 )
 
 
 class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
     pass
 
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredAgentConfigurationTypeDef = TypedDict(
     "_RequiredAgentConfigurationTypeDef",
     {
         "periodInSeconds": int,
         "shouldProfile": bool,
     },
 )
@@ -143,21 +153,14 @@
 
 class AgentConfigurationTypeDef(
     _RequiredAgentConfigurationTypeDef, _OptionalAgentConfigurationTypeDef
 ):
     pass
 
 
-AgentOrchestrationConfigOutputTypeDef = TypedDict(
-    "AgentOrchestrationConfigOutputTypeDef",
-    {
-        "profilingEnabled": bool,
-    },
-)
-
 AgentOrchestrationConfigTypeDef = TypedDict(
     "AgentOrchestrationConfigTypeDef",
     {
         "profilingEnabled": bool,
     },
 )
 
@@ -299,23 +302,14 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetProfileRequestRequestTypeDef = TypedDict(
     "_RequiredGetProfileRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalGetProfileRequestRequestTypeDef = TypedDict(
@@ -333,24 +327,14 @@
 
 class GetProfileRequestRequestTypeDef(
     _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
 ):
     pass
 
 
-GetProfileResponseTypeDef = TypedDict(
-    "GetProfileResponseTypeDef",
-    {
-        "contentEncoding": str,
-        "contentType": str,
-        "profile": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecommendationsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "profilingGroupName": str,
         "startTime": Union[datetime, str],
     },
@@ -393,40 +377,24 @@
 class ListFindingsReportsRequestRequestTypeDef(
     _RequiredListFindingsReportsRequestRequestTypeDef,
     _OptionalListFindingsReportsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "period": AggregationPeriodType,
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "orderBy": OrderByType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
-    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
-    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileTimesRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "period": AggregationPeriodType,
         "profilingGroupName": str,
         "startTime": Union[datetime, str],
@@ -470,42 +438,24 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MatchTypeDef = TypedDict(
     "MatchTypeDef",
     {
         "frameAddress": str,
         "targetFramesIndex": int,
         "thresholdBreachValue": float,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PatternTypeDef = TypedDict(
     "PatternTypeDef",
     {
         "countersToAggregate": List[str],
         "description": str,
         "id": str,
         "name": str,
@@ -558,23 +508,14 @@
 
 class PutPermissionRequestRequestTypeDef(
     _RequiredPutPermissionRequestRequestTypeDef, _OptionalPutPermissionRequestRequestTypeDef
 ):
     pass
 
 
-PutPermissionResponseTypeDef = TypedDict(
-    "PutPermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveNotificationChannelRequestRequestTypeDef = TypedDict(
     "RemoveNotificationChannelRequestRequestTypeDef",
     {
         "channelId": str,
         "profilingGroupName": str,
     },
 )
@@ -584,34 +525,14 @@
     {
         "actionGroup": Literal["agentPermissions"],
         "profilingGroupName": str,
         "revisionId": str,
     },
 )
 
-RemovePermissionResponseTypeDef = TypedDict(
-    "RemovePermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitFeedbackRequestRequestTypeDef",
     {
         "anomalyInstanceId": str,
         "profilingGroupName": str,
         "type": FeedbackTypeType,
     },
@@ -651,19 +572,64 @@
     "AddNotificationChannelsRequestRequestTypeDef",
     {
         "channels": Sequence[ChannelTypeDef],
         "profilingGroupName": str,
     },
 )
 
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProfileResponseTypeDef = TypedDict(
+    "GetProfileResponseTypeDef",
+    {
+        "contentEncoding": str,
+        "contentType": str,
+        "profile": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutPermissionResponseTypeDef = TypedDict(
+    "PutPermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemovePermissionResponseTypeDef = TypedDict(
+    "RemovePermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConfigureAgentResponseTypeDef = TypedDict(
     "ConfigureAgentResponseTypeDef",
     {
         "configuration": AgentConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProfilingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfilingGroupRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -762,41 +728,67 @@
 )
 
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsReportsResponseTypeDef = TypedDict(
     "ListFindingsReportsResponseTypeDef",
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FrameMetricDatumTypeDef = TypedDict(
     "FrameMetricDatumTypeDef",
     {
         "frameMetric": FrameMetricOutputTypeDef,
         "values": List[float],
     },
 )
 
+_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "period": AggregationPeriodType,
+        "profilingGroupName": str,
+        "startTime": Union[datetime, str],
+    },
+)
+_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    {
+        "orderBy": OrderByType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
+    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
+    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
+):
+    pass
+
+
 ListProfileTimesResponseTypeDef = TypedDict(
     "ListProfileTimesResponseTypeDef",
     {
         "nextToken": str,
         "profileTimes": List[ProfileTimeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "allMatchesCount": int,
@@ -807,15 +799,15 @@
         "topMatches": List[MatchTypeDef],
     },
 )
 
 ProfilingGroupDescriptionTypeDef = TypedDict(
     "ProfilingGroupDescriptionTypeDef",
     {
-        "agentOrchestrationConfig": AgentOrchestrationConfigOutputTypeDef,
+        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
         "arn": str,
         "computePlatform": ComputePlatformType,
         "createdAt": datetime,
         "name": str,
         "profilingStatus": ProfilingStatusTypeDef,
         "tags": Dict[str, str],
         "updatedAt": datetime,
@@ -832,85 +824,85 @@
     },
 )
 
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNotificationConfigurationResponseTypeDef = TypedDict(
     "GetNotificationConfigurationResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveNotificationChannelResponseTypeDef = TypedDict(
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetFrameMetricDataResponseTypeDef = TypedDict(
     "BatchGetFrameMetricDataResponseTypeDef",
     {
         "endTime": datetime,
         "endTimes": List[TimestampStructureTypeDef],
         "frameMetricData": List[FrameMetricDatumTypeDef],
         "resolution": AggregationPeriodType,
         "startTime": datetime,
         "unprocessedEndTimes": Dict[str, List[TimestampStructureTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProfilingGroupResponseTypeDef = TypedDict(
     "CreateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProfilingGroupResponseTypeDef = TypedDict(
     "DescribeProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilingGroupsResponseTypeDef = TypedDict(
     "ListProfilingGroupsResponseTypeDef",
     {
         "nextToken": str,
         "profilingGroupNames": List[str],
         "profilingGroups": List[ProfilingGroupDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProfilingGroupResponseTypeDef = TypedDict(
     "UpdateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "anomalies": List[AnomalyTypeDef],
         "profileEndTime": datetime,
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler/type_defs.pyi` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChannelTypeDef",
+    "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
-    "AgentOrchestrationConfigOutputTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
     "FrameMetricTypeDef",
     "TimestampStructureTypeDef",
     "ChannelOutputTypeDef",
@@ -50,49 +50,48 @@
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
     "FrameMetricOutputTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetPolicyResponseTypeDef",
     "GetProfileRequestRequestTypeDef",
-    "GetProfileResponseTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "ListFindingsReportsRequestRequestTypeDef",
-    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListProfileTimesRequestRequestTypeDef",
     "ProfileTimeTypeDef",
     "ListProfilingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MatchTypeDef",
-    "PaginatorConfigTypeDef",
     "PatternTypeDef",
     "PostAgentProfileRequestRequestTypeDef",
     "PutPermissionRequestRequestTypeDef",
-    "PutPermissionResponseTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
-    "RemovePermissionResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddNotificationChannelsRequestRequestTypeDef",
+    "GetPolicyResponseTypeDef",
+    "GetProfileResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutPermissionResponseTypeDef",
+    "RemovePermissionResponseTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
     "BatchGetFrameMetricDataRequestRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
     "FrameMetricDatumTypeDef",
+    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
     "ProfilingGroupDescriptionTypeDef",
     "AnomalyTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
@@ -118,14 +117,25 @@
     },
     total=False,
 )
 
 class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
     pass
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredAgentConfigurationTypeDef = TypedDict(
     "_RequiredAgentConfigurationTypeDef",
     {
         "periodInSeconds": int,
         "shouldProfile": bool,
     },
 )
@@ -138,21 +148,14 @@
 )
 
 class AgentConfigurationTypeDef(
     _RequiredAgentConfigurationTypeDef, _OptionalAgentConfigurationTypeDef
 ):
     pass
 
-AgentOrchestrationConfigOutputTypeDef = TypedDict(
-    "AgentOrchestrationConfigOutputTypeDef",
-    {
-        "profilingEnabled": bool,
-    },
-)
-
 AgentOrchestrationConfigTypeDef = TypedDict(
     "AgentOrchestrationConfigTypeDef",
     {
         "profilingEnabled": bool,
     },
 )
 
@@ -290,23 +293,14 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetProfileRequestRequestTypeDef = TypedDict(
     "_RequiredGetProfileRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalGetProfileRequestRequestTypeDef = TypedDict(
@@ -322,24 +316,14 @@
 )
 
 class GetProfileRequestRequestTypeDef(
     _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
 ):
     pass
 
-GetProfileResponseTypeDef = TypedDict(
-    "GetProfileResponseTypeDef",
-    {
-        "contentEncoding": str,
-        "contentType": str,
-        "profile": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecommendationsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "profilingGroupName": str,
         "startTime": Union[datetime, str],
     },
@@ -378,38 +362,24 @@
 
 class ListFindingsReportsRequestRequestTypeDef(
     _RequiredListFindingsReportsRequestRequestTypeDef,
     _OptionalListFindingsReportsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "period": AggregationPeriodType,
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "orderBy": OrderByType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
-    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
-    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
-):
-    pass
-
 _RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileTimesRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "period": AggregationPeriodType,
         "profilingGroupName": str,
         "startTime": Union[datetime, str],
@@ -451,42 +421,24 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MatchTypeDef = TypedDict(
     "MatchTypeDef",
     {
         "frameAddress": str,
         "targetFramesIndex": int,
         "thresholdBreachValue": float,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PatternTypeDef = TypedDict(
     "PatternTypeDef",
     {
         "countersToAggregate": List[str],
         "description": str,
         "id": str,
         "name": str,
@@ -535,23 +487,14 @@
 )
 
 class PutPermissionRequestRequestTypeDef(
     _RequiredPutPermissionRequestRequestTypeDef, _OptionalPutPermissionRequestRequestTypeDef
 ):
     pass
 
-PutPermissionResponseTypeDef = TypedDict(
-    "PutPermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveNotificationChannelRequestRequestTypeDef = TypedDict(
     "RemoveNotificationChannelRequestRequestTypeDef",
     {
         "channelId": str,
         "profilingGroupName": str,
     },
 )
@@ -561,34 +504,14 @@
     {
         "actionGroup": Literal["agentPermissions"],
         "profilingGroupName": str,
         "revisionId": str,
     },
 )
 
-RemovePermissionResponseTypeDef = TypedDict(
-    "RemovePermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitFeedbackRequestRequestTypeDef",
     {
         "anomalyInstanceId": str,
         "profilingGroupName": str,
         "type": FeedbackTypeType,
     },
@@ -626,19 +549,64 @@
     "AddNotificationChannelsRequestRequestTypeDef",
     {
         "channels": Sequence[ChannelTypeDef],
         "profilingGroupName": str,
     },
 )
 
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProfileResponseTypeDef = TypedDict(
+    "GetProfileResponseTypeDef",
+    {
+        "contentEncoding": str,
+        "contentType": str,
+        "profile": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutPermissionResponseTypeDef = TypedDict(
+    "PutPermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemovePermissionResponseTypeDef = TypedDict(
+    "RemovePermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConfigureAgentResponseTypeDef = TypedDict(
     "ConfigureAgentResponseTypeDef",
     {
         "configuration": AgentConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProfilingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfilingGroupRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -731,41 +699,65 @@
 )
 
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsReportsResponseTypeDef = TypedDict(
     "ListFindingsReportsResponseTypeDef",
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FrameMetricDatumTypeDef = TypedDict(
     "FrameMetricDatumTypeDef",
     {
         "frameMetric": FrameMetricOutputTypeDef,
         "values": List[float],
     },
 )
 
+_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "period": AggregationPeriodType,
+        "profilingGroupName": str,
+        "startTime": Union[datetime, str],
+    },
+)
+_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    {
+        "orderBy": OrderByType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
+    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
+    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
+):
+    pass
+
 ListProfileTimesResponseTypeDef = TypedDict(
     "ListProfileTimesResponseTypeDef",
     {
         "nextToken": str,
         "profileTimes": List[ProfileTimeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "allMatchesCount": int,
@@ -776,15 +768,15 @@
         "topMatches": List[MatchTypeDef],
     },
 )
 
 ProfilingGroupDescriptionTypeDef = TypedDict(
     "ProfilingGroupDescriptionTypeDef",
     {
-        "agentOrchestrationConfig": AgentOrchestrationConfigOutputTypeDef,
+        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
         "arn": str,
         "computePlatform": ComputePlatformType,
         "createdAt": datetime,
         "name": str,
         "profilingStatus": ProfilingStatusTypeDef,
         "tags": Dict[str, str],
         "updatedAt": datetime,
@@ -801,85 +793,85 @@
     },
 )
 
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNotificationConfigurationResponseTypeDef = TypedDict(
     "GetNotificationConfigurationResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveNotificationChannelResponseTypeDef = TypedDict(
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetFrameMetricDataResponseTypeDef = TypedDict(
     "BatchGetFrameMetricDataResponseTypeDef",
     {
         "endTime": datetime,
         "endTimes": List[TimestampStructureTypeDef],
         "frameMetricData": List[FrameMetricDatumTypeDef],
         "resolution": AggregationPeriodType,
         "startTime": datetime,
         "unprocessedEndTimes": Dict[str, List[TimestampStructureTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProfilingGroupResponseTypeDef = TypedDict(
     "CreateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProfilingGroupResponseTypeDef = TypedDict(
     "DescribeProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilingGroupsResponseTypeDef = TypedDict(
     "ListProfilingGroupsResponseTypeDef",
     {
         "nextToken": str,
         "profilingGroupNames": List[str],
         "profilingGroups": List[ProfilingGroupDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProfilingGroupResponseTypeDef = TypedDict(
     "UpdateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "anomalies": List[AnomalyTypeDef],
         "profileEndTime": datetime,
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguruprofiler
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeGuruProfiler 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeGuruProfiler 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguruprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguruprofiler)](https://pepy.tech/project/mypy-boto3-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruProfiler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
+[boto3.CodeGuruProfiler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguruprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,16 +329,16 @@
 
 `mypy_boto3_codeguruprofiler.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguruprofiler.type_defs import (
     ChannelTypeDef,
+    ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
-    AgentOrchestrationConfigOutputTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
     FrameMetricTypeDef,
     TimestampStructureTypeDef,
     ChannelOutputTypeDef,
@@ -346,49 +346,48 @@
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
     FrameMetricOutputTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetProfileRequestRequestTypeDef,
-    GetProfileResponseTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     ListFindingsReportsRequestRequestTypeDef,
-    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListProfileTimesRequestRequestTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MatchTypeDef,
-    PaginatorConfigTypeDef,
     PatternTypeDef,
     PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
-    PutPermissionResponseTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    RemovePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddNotificationChannelsRequestRequestTypeDef,
+    GetPolicyResponseTypeDef,
+    GetProfileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutPermissionResponseTypeDef,
+    RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
     BatchGetFrameMetricDataRequestRequestTypeDef,
     NotificationConfigurationTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
     FrameMetricDatumTypeDef,
+    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
     ProfilingGroupDescriptionTypeDef,
     AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
```

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt` & `mypy-boto3-codeguruprofiler-1.28.15/mypy_boto3_codeguruprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguruprofiler-1.28.12/setup.py` & `mypy-boto3-codeguruprofiler-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguruprofiler",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_codeguruprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruProfiler 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CodeGuruProfiler 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

