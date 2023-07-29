# Comparing `tmp/mypy-boto3-cloudtrail-1.28.12.tar.gz` & `tmp/mypy-boto3-cloudtrail-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudtrail-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudtrail-1.28.15.tar", last modified: Fri Jul 28 20:42:28 2023, max compression
```

## Comparing `mypy-boto3-cloudtrail-1.28.12.tar` & `mypy-boto3-cloudtrail-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.004557 mypy-boto3-cloudtrail-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-07-27 05:34:27.004557 mypy-boto3-cloudtrail-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.992556 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39076 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39017 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-07-27 05:18:48.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-27 05:18:48.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42799 2023-07-27 05:18:48.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-27 05:18:48.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.004557 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.004557 mypy-boto3-cloudtrail-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.348822 mypy-boto3-cloudtrail-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:04.000000 mypy-boto3-cloudtrail-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-28 20:42:28.348822 mypy-boto3-cloudtrail-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-07-28 20:21:04.000000 mypy-boto3-cloudtrail-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.348822 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-28 20:21:04.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-28 20:21:04.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:21:04.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39076 2023-07-28 20:21:05.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39017 2023-07-28 20:21:04.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-07-28 20:21:05.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-28 20:21:05.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-28 20:21:05.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-07-28 20:21:05.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:04.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41548 2023-07-28 20:21:06.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41509 2023-07-28 20:21:06.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:04.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.348822 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-28 20:42:28.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:28.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:28.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:28.000000 mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:28.348822 mypy-boto3-cloudtrail-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:21:04.000000 mypy-boto3-cloudtrail-1.28.15/setup.py
```

### Comparing `mypy-boto3-cloudtrail-1.28.12/LICENSE` & `mypy-boto3-cloudtrail-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.12/PKG-INFO` & `mypy-boto3-cloudtrail-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudTrail 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudTrail 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,20 +351,17 @@
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
     AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
-    DestinationOutputTypeDef,
-    TagOutputTypeDef,
-    CreateTrailResponseTypeDef,
     DataResourceOutputTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
@@ -376,106 +373,104 @@
     GetChannelRequestRequestTypeDef,
     IngestionStatusTypeDef,
     GetEventDataStoreRequestRequestTypeDef,
     GetEventSelectorsRequestRequestTypeDef,
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
-    InsightSelectorOutputTypeDef,
+    InsightSelectorTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
-    GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
-    S3ImportSourceOutputTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
-    InsightSelectorTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
-    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListImportFailuresRequestRequestTypeDef,
-    ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     PublicKeyTypeDef,
     ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTrailsRequestListTrailsPaginateTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreEventDataStoreRequestRequestTypeDef,
     StartEventDataStoreIngestionRequestRequestTypeDef,
     StartLoggingRequestRequestTypeDef,
     StartQueryRequestRequestTypeDef,
-    StartQueryResponseTypeDef,
     StopEventDataStoreIngestionRequestRequestTypeDef,
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
-    UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
+    ResourceTagTypeDef,
     AdvancedEventSelectorOutputTypeDef,
     AdvancedEventSelectorTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateTrailResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetTrailStatusResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartQueryResponseTypeDef,
+    UpdateTrailResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
+    CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    ResourceTagTypeDef,
     EventSelectorOutputTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     GetTrailResponseTypeDef,
     EventTypeDef,
     GetInsightSelectorsResponseTypeDef,
+    PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
-    ImportSourceOutputTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
-    PutInsightSelectorsRequestRequestTypeDef,
+    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    ListImportsRequestListImportsPaginateTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
+    ListTrailsRequestListTrailsPaginateTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
     UpdateEventDataStoreResponseTypeDef,
     CreateEventDataStoreRequestRequestTypeDef,
     UpdateEventDataStoreRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
     PutEventSelectorsResponseTypeDef,
     PutEventSelectorsRequestRequestTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudtrail-1.28.12/README.md` & `mypy-boto3-cloudtrail-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,20 +319,17 @@
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
     AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
-    DestinationOutputTypeDef,
-    TagOutputTypeDef,
-    CreateTrailResponseTypeDef,
     DataResourceOutputTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
@@ -344,106 +341,104 @@
     GetChannelRequestRequestTypeDef,
     IngestionStatusTypeDef,
     GetEventDataStoreRequestRequestTypeDef,
     GetEventSelectorsRequestRequestTypeDef,
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
-    InsightSelectorOutputTypeDef,
+    InsightSelectorTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
-    GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
-    S3ImportSourceOutputTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
-    InsightSelectorTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
-    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListImportFailuresRequestRequestTypeDef,
-    ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     PublicKeyTypeDef,
     ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTrailsRequestListTrailsPaginateTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreEventDataStoreRequestRequestTypeDef,
     StartEventDataStoreIngestionRequestRequestTypeDef,
     StartLoggingRequestRequestTypeDef,
     StartQueryRequestRequestTypeDef,
-    StartQueryResponseTypeDef,
     StopEventDataStoreIngestionRequestRequestTypeDef,
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
-    UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
+    ResourceTagTypeDef,
     AdvancedEventSelectorOutputTypeDef,
     AdvancedEventSelectorTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateTrailResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetTrailStatusResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartQueryResponseTypeDef,
+    UpdateTrailResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
+    CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    ResourceTagTypeDef,
     EventSelectorOutputTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     GetTrailResponseTypeDef,
     EventTypeDef,
     GetInsightSelectorsResponseTypeDef,
+    PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
-    ImportSourceOutputTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
-    PutInsightSelectorsRequestRequestTypeDef,
+    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    ListImportsRequestListImportsPaginateTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
+    ListTrailsRequestListTrailsPaginateTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
     UpdateEventDataStoreResponseTypeDef,
     CreateEventDataStoreRequestRequestTypeDef,
     UpdateEventDataStoreRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
     PutEventSelectorsResponseTypeDef,
     PutEventSelectorsRequestRequestTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__init__.py` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__init__.pyi` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__main__.py` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudTrail 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudTrail 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail\nOther"
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

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/client.py` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/client.pyi` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/literals.py` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/literals.pyi` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/paginator.py` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 class ListImportFailuresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportfailurespaginator)
     """
 
     def paginate(
-        self, *, ImportId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ImportId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportFailuresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportfailurespaginator)
         """
 
 
@@ -95,15 +95,15 @@
     """
 
     def paginate(
         self,
         *,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportspaginator)
         """
 
 
@@ -114,45 +114,45 @@
     """
 
     def paginate(
         self,
         *,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listpublickeyspaginator)
         """
 
 
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceIdList: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceIdList: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtagspaginator)
         """
 
 
 class ListTrailsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtrailspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTrailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtrailspaginator)
         """
 
 
@@ -165,13 +165,13 @@
     def paginate(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         EventCategory: Literal["insight"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[LookupEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#lookupeventspaginator)
         """
```

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/paginator.pyi` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 class ListImportFailuresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportfailurespaginator)
     """
 
     def paginate(
-        self, *, ImportId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ImportId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportFailuresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportfailurespaginator)
         """
 
 class ListImportsPaginator(Paginator):
@@ -90,15 +90,15 @@
     """
 
     def paginate(
         self,
         *,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportspaginator)
         """
 
 class ListPublicKeysPaginator(Paginator):
@@ -108,43 +108,43 @@
     """
 
     def paginate(
         self,
         *,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listpublickeyspaginator)
         """
 
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceIdList: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceIdList: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtagspaginator)
         """
 
 class ListTrailsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtrailspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTrailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtrailspaginator)
         """
 
 class LookupEventsPaginator(Paginator):
@@ -156,13 +156,13 @@
     def paginate(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         EventCategory: Literal["insight"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[LookupEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#lookupeventspaginator)
         """
```

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/type_defs.py` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,17 @@
 
 
 __all__ = (
     "TagTypeDef",
     "AdvancedFieldSelectorOutputTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
-    "CancelQueryResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
-    "DestinationOutputTypeDef",
-    "TagOutputTypeDef",
-    "CreateTrailResponseTypeDef",
     "DataResourceOutputTypeDef",
     "DataResourceTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteEventDataStoreRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteTrailRequestRequestTypeDef",
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
@@ -63,106 +60,104 @@
     "GetChannelRequestRequestTypeDef",
     "IngestionStatusTypeDef",
     "GetEventDataStoreRequestRequestTypeDef",
     "GetEventSelectorsRequestRequestTypeDef",
     "GetImportRequestRequestTypeDef",
     "ImportStatisticsTypeDef",
     "GetInsightSelectorsRequestRequestTypeDef",
-    "InsightSelectorOutputTypeDef",
+    "InsightSelectorTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetTrailRequestRequestTypeDef",
     "GetTrailStatusRequestRequestTypeDef",
-    "GetTrailStatusResponseTypeDef",
     "ImportFailureListItemTypeDef",
-    "S3ImportSourceOutputTypeDef",
     "S3ImportSourceTypeDef",
     "ImportsListItemTypeDef",
-    "InsightSelectorTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListEventDataStoresRequestRequestTypeDef",
-    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListImportFailuresRequestRequestTypeDef",
-    "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "PublicKeyTypeDef",
     "ListQueriesRequestRequestTypeDef",
     "QueryTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "ListTrailsRequestListTrailsPaginateTypeDef",
     "ListTrailsRequestRequestTypeDef",
     "TrailInfoTypeDef",
     "LookupAttributeTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreEventDataStoreRequestRequestTypeDef",
     "StartEventDataStoreIngestionRequestRequestTypeDef",
     "StartLoggingRequestRequestTypeDef",
     "StartQueryRequestRequestTypeDef",
-    "StartQueryResponseTypeDef",
     "StopEventDataStoreIngestionRequestRequestTypeDef",
     "StopImportRequestRequestTypeDef",
     "StopLoggingRequestRequestTypeDef",
     "UpdateTrailRequestRequestTypeDef",
-    "UpdateTrailResponseTypeDef",
     "AddTagsRequestRequestTypeDef",
     "CreateTrailRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
+    "ResourceTagTypeDef",
     "AdvancedEventSelectorOutputTypeDef",
     "AdvancedEventSelectorTypeDef",
+    "CancelQueryResponseTypeDef",
+    "CreateTrailResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetTrailStatusResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "StartQueryResponseTypeDef",
+    "UpdateTrailResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
+    "CreateChannelResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
-    "CreateChannelResponseTypeDef",
-    "ResourceTagTypeDef",
     "EventSelectorOutputTypeDef",
     "EventSelectorTypeDef",
     "DescribeQueryResponseTypeDef",
     "DescribeTrailsResponseTypeDef",
     "GetTrailResponseTypeDef",
     "EventTypeDef",
     "GetInsightSelectorsResponseTypeDef",
+    "PutInsightSelectorsRequestRequestTypeDef",
     "PutInsightSelectorsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "ListImportFailuresResponseTypeDef",
-    "ImportSourceOutputTypeDef",
     "ImportSourceTypeDef",
     "ListImportsResponseTypeDef",
-    "PutInsightSelectorsRequestRequestTypeDef",
+    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    "ListImportsRequestListImportsPaginateTypeDef",
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
+    "ListTrailsRequestListTrailsPaginateTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
     "CreateEventDataStoreResponseTypeDef",
     "EventDataStoreTypeDef",
     "GetEventDataStoreResponseTypeDef",
     "RestoreEventDataStoreResponseTypeDef",
     "SourceConfigTypeDef",
     "UpdateEventDataStoreResponseTypeDef",
     "CreateEventDataStoreRequestRequestTypeDef",
     "UpdateEventDataStoreRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "GetEventSelectorsResponseTypeDef",
     "PutEventSelectorsResponseTypeDef",
     "PutEventSelectorsRequestRequestTypeDef",
     "LookupEventsResponseTypeDef",
     "GetImportResponseTypeDef",
+    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "StopImportResponseTypeDef",
-    "StartImportRequestRequestTypeDef",
     "ListEventDataStoresResponseTypeDef",
     "GetChannelResponseTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
@@ -251,20 +246,22 @@
 
 class CancelQueryRequestRequestTypeDef(
     _RequiredCancelQueryRequestRequestTypeDef, _OptionalCancelQueryRequestRequestTypeDef
 ):
     pass
 
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "QueryId": str,
-        "QueryStatus": QueryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "ChannelArn": str,
@@ -277,61 +274,14 @@
     "DestinationTypeDef",
     {
         "Type": DestinationTypeType,
         "Location": str,
     },
 )
 
-DestinationOutputTypeDef = TypedDict(
-    "DestinationOutputTypeDef",
-    {
-        "Type": DestinationTypeType,
-        "Location": str,
-    },
-)
-
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-
-CreateTrailResponseTypeDef = TypedDict(
-    "CreateTrailResponseTypeDef",
-    {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataResourceOutputTypeDef = TypedDict(
     "DataResourceOutputTypeDef",
     {
         "Type": str,
         "Values": List[str],
     },
     total=False,
@@ -499,16 +449,16 @@
 GetInsightSelectorsRequestRequestTypeDef = TypedDict(
     "GetInsightSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
     },
 )
 
-InsightSelectorOutputTypeDef = TypedDict(
-    "InsightSelectorOutputTypeDef",
+InsightSelectorTypeDef = TypedDict(
+    "InsightSelectorTypeDef",
     {
         "InsightType": InsightTypeType,
     },
     total=False,
 )
 
 _RequiredGetQueryResultsRequestRequestTypeDef = TypedDict(
@@ -547,82 +497,40 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrailRequestRequestTypeDef = TypedDict(
     "GetTrailRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 GetTrailStatusRequestRequestTypeDef = TypedDict(
     "GetTrailStatusRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-GetTrailStatusResponseTypeDef = TypedDict(
-    "GetTrailStatusResponseTypeDef",
-    {
-        "IsLogging": bool,
-        "LatestDeliveryError": str,
-        "LatestNotificationError": str,
-        "LatestDeliveryTime": datetime,
-        "LatestNotificationTime": datetime,
-        "StartLoggingTime": datetime,
-        "StopLoggingTime": datetime,
-        "LatestCloudWatchLogsDeliveryError": str,
-        "LatestCloudWatchLogsDeliveryTime": datetime,
-        "LatestDigestDeliveryTime": datetime,
-        "LatestDigestDeliveryError": str,
-        "LatestDeliveryAttemptTime": str,
-        "LatestNotificationAttemptTime": str,
-        "LatestNotificationAttemptSucceeded": str,
-        "LatestDeliveryAttemptSucceeded": str,
-        "TimeLoggingStarted": str,
-        "TimeLoggingStopped": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImportFailureListItemTypeDef = TypedDict(
     "ImportFailureListItemTypeDef",
     {
         "Location": str,
         "Status": ImportFailureStatusType,
         "ErrorType": str,
         "ErrorMessage": str,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-S3ImportSourceOutputTypeDef = TypedDict(
-    "S3ImportSourceOutputTypeDef",
-    {
-        "S3LocationUri": str,
-        "S3BucketRegion": str,
-        "S3BucketAccessRoleArn": str,
-    },
-)
-
 S3ImportSourceTypeDef = TypedDict(
     "S3ImportSourceTypeDef",
     {
         "S3LocationUri": str,
         "S3BucketRegion": str,
         "S3BucketAccessRoleArn": str,
     },
@@ -636,22 +544,14 @@
         "Destinations": List[str],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-InsightSelectorTypeDef = TypedDict(
-    "InsightSelectorTypeDef",
-    {
-        "InsightType": InsightTypeType,
-    },
-    total=False,
-)
-
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -662,36 +562,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
-    {
-        "ImportId": str,
-    },
-)
-_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
-    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
-    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListImportFailuresRequestRequestTypeDef = TypedDict(
     "_RequiredListImportFailuresRequestRequestTypeDef",
     {
         "ImportId": str,
     },
 )
 _OptionalListImportFailuresRequestRequestTypeDef = TypedDict(
@@ -707,45 +595,25 @@
 class ListImportFailuresRequestRequestTypeDef(
     _RequiredListImportFailuresRequestRequestTypeDef,
     _OptionalListImportFailuresRequestRequestTypeDef,
 ):
     pass
 
 
-ListImportsRequestListImportsPaginateTypeDef = TypedDict(
-    "ListImportsRequestListImportsPaginateTypeDef",
-    {
-        "Destination": str,
-        "ImportStatus": ImportStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "Destination": str,
         "ImportStatus": ImportStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
-ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPublicKeysRequestRequestTypeDef = TypedDict(
     "ListPublicKeysRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "NextToken": str,
     },
@@ -794,35 +662,14 @@
         "QueryId": str,
         "QueryStatus": QueryStatusType,
         "CreationTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceIdList": Sequence[str],
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceIdList": Sequence[str],
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -836,22 +683,14 @@
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
 
-ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
-    "ListTrailsRequestListTrailsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTrailsRequestRequestTypeDef = TypedDict(
     "ListTrailsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -870,59 +709,29 @@
     "LookupAttributeTypeDef",
     {
         "AttributeKey": LookupAttributeKeyType,
         "AttributeValue": str,
     },
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourcePolicy": str,
     },
 )
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterOrganizationDelegatedAdminRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
     {
         "MemberAccountId": str,
     },
 )
 
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
 RestoreEventDataStoreRequestRequestTypeDef = TypedDict(
     "RestoreEventDataStoreRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 
@@ -947,22 +756,14 @@
         "DeliveryS3Uri": str,
         "QueryAlias": str,
         "QueryParameters": Sequence[str],
     },
     total=False,
 )
 
-StartQueryResponseTypeDef = TypedDict(
-    "StartQueryResponseTypeDef",
-    {
-        "QueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopEventDataStoreIngestionRequestRequestTypeDef = TypedDict(
     "StopEventDataStoreIngestionRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 
@@ -1006,34 +807,14 @@
 
 class UpdateTrailRequestRequestTypeDef(
     _RequiredUpdateTrailRequestRequestTypeDef, _OptionalUpdateTrailRequestRequestTypeDef
 ):
     pass
 
 
-UpdateTrailResponseTypeDef = TypedDict(
-    "UpdateTrailResponseTypeDef",
-    {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddTagsRequestRequestTypeDef = TypedDict(
     "AddTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
@@ -1073,14 +854,23 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
 
+ResourceTagTypeDef = TypedDict(
+    "ResourceTagTypeDef",
+    {
+        "ResourceId": str,
+        "TagsList": List[TagTypeDef],
+    },
+    total=False,
+)
+
 _RequiredAdvancedEventSelectorOutputTypeDef = TypedDict(
     "_RequiredAdvancedEventSelectorOutputTypeDef",
     {
         "FieldSelectors": List[AdvancedFieldSelectorOutputTypeDef],
     },
 )
 _OptionalAdvancedEventSelectorOutputTypeDef = TypedDict(
@@ -1115,20 +905,119 @@
 
 class AdvancedEventSelectorTypeDef(
     _RequiredAdvancedEventSelectorTypeDef, _OptionalAdvancedEventSelectorTypeDef
 ):
     pass
 
 
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
+    {
+        "QueryId": str,
+        "QueryStatus": QueryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrailResponseTypeDef = TypedDict(
+    "CreateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTrailStatusResponseTypeDef = TypedDict(
+    "GetTrailStatusResponseTypeDef",
+    {
+        "IsLogging": bool,
+        "LatestDeliveryError": str,
+        "LatestNotificationError": str,
+        "LatestDeliveryTime": datetime,
+        "LatestNotificationTime": datetime,
+        "StartLoggingTime": datetime,
+        "StopLoggingTime": datetime,
+        "LatestCloudWatchLogsDeliveryError": str,
+        "LatestCloudWatchLogsDeliveryTime": datetime,
+        "LatestDigestDeliveryTime": datetime,
+        "LatestDigestDeliveryError": str,
+        "LatestDeliveryAttemptTime": str,
+        "LatestNotificationAttemptTime": str,
+        "LatestNotificationAttemptSucceeded": str,
+        "LatestDeliveryAttemptSucceeded": str,
+        "TimeLoggingStarted": str,
+        "TimeLoggingStopped": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryResponseTypeDef = TypedDict(
+    "StartQueryResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrailResponseTypeDef = TypedDict(
+    "UpdateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Name": str,
@@ -1147,14 +1036,26 @@
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
 
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "Name": str,
+        "Source": str,
+        "Destinations": List[DestinationTypeDef],
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "Channel": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
@@ -1175,40 +1076,19 @@
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
-        "Destinations": List[DestinationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Destinations": List[DestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "Name": str,
-        "Source": str,
-        "Destinations": List[DestinationOutputTypeDef],
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResourceTagTypeDef = TypedDict(
-    "ResourceTagTypeDef",
-    {
-        "ResourceId": str,
-        "TagsList": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 EventSelectorOutputTypeDef = TypedDict(
     "EventSelectorOutputTypeDef",
     {
         "ReadWriteType": ReadWriteTypeType,
         "IncludeManagementEvents": bool,
         "DataResources": List[DataResourceOutputTypeDef],
         "ExcludeManagementEventSources": List[str],
@@ -1233,31 +1113,31 @@
         "QueryId": str,
         "QueryString": str,
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsForDescribeQueryTypeDef,
         "ErrorMessage": str,
         "DeliveryS3Uri": str,
         "DeliveryStatus": DeliveryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrailsResponseTypeDef = TypedDict(
     "DescribeTrailsResponseTypeDef",
     {
         "trailList": List[TrailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrailResponseTypeDef = TypedDict(
     "GetTrailResponseTypeDef",
     {
         "Trail": TrailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "EventId": str,
@@ -1273,53 +1153,54 @@
     total=False,
 )
 
 GetInsightSelectorsResponseTypeDef = TypedDict(
     "GetInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "InsightSelectors": List[InsightSelectorOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InsightSelectors": List[InsightSelectorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutInsightSelectorsRequestRequestTypeDef = TypedDict(
+    "PutInsightSelectorsRequestRequestTypeDef",
+    {
+        "TrailName": str,
+        "InsightSelectors": Sequence[InsightSelectorTypeDef],
     },
 )
 
 PutInsightSelectorsResponseTypeDef = TypedDict(
     "PutInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "InsightSelectors": List[InsightSelectorOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InsightSelectors": List[InsightSelectorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsTypeDef,
         "QueryResultRows": List[List[Dict[str, str]]],
         "NextToken": str,
         "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImportFailuresResponseTypeDef = TypedDict(
     "ListImportFailuresResponseTypeDef",
     {
         "Failures": List[ImportFailureListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportSourceOutputTypeDef = TypedDict(
-    "ImportSourceOutputTypeDef",
-    {
-        "S3": S3ImportSourceOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportSourceTypeDef = TypedDict(
     "ImportSourceTypeDef",
     {
         "S3": S3ImportSourceTypeDef,
@@ -1327,61 +1208,124 @@
 )
 
 ListImportsResponseTypeDef = TypedDict(
     "ListImportsResponseTypeDef",
     {
         "Imports": List[ImportsListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutInsightSelectorsRequestRequestTypeDef = TypedDict(
-    "PutInsightSelectorsRequestRequestTypeDef",
+_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
     {
-        "TrailName": str,
-        "InsightSelectors": Sequence[InsightSelectorTypeDef],
+        "ImportId": str,
+    },
+)
+_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
+    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
+):
+    pass
+
+
+ListImportsRequestListImportsPaginateTypeDef = TypedDict(
+    "ListImportsRequestListImportsPaginateTypeDef",
+    {
+        "Destination": str,
+        "ImportStatus": ImportStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceIdList": Sequence[str],
     },
 )
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
+
+ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
+    "ListTrailsRequestListTrailsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListPublicKeysResponseTypeDef = TypedDict(
     "ListPublicKeysResponseTypeDef",
     {
         "PublicKeyList": List[PublicKeyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueriesResponseTypeDef = TypedDict(
     "ListQueriesResponseTypeDef",
     {
         "Queries": List[QueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrailsResponseTypeDef = TypedDict(
     "ListTrailsResponseTypeDef",
     {
         "Trails": List[TrailInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LookupEventsRequestLookupEventsPaginateTypeDef = TypedDict(
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "EventCategory": Literal["insight"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 LookupEventsRequestRequestTypeDef = TypedDict(
     "LookupEventsRequestRequestTypeDef",
     {
@@ -1391,30 +1335,39 @@
         "EventCategory": Literal["insight"],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "ResourceTagList": List[ResourceTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateEventDataStoreResponseTypeDef = TypedDict(
     "CreateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
         "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
-        "TagsList": List[TagOutputTypeDef],
+        "TagsList": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventDataStoreTypeDef = TypedDict(
     "EventDataStoreTypeDef",
     {
         "EventDataStoreArn": str,
@@ -1441,15 +1394,15 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreEventDataStoreResponseTypeDef = TypedDict(
     "RestoreEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
@@ -1459,15 +1412,15 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceConfigTypeDef = TypedDict(
     "SourceConfigTypeDef",
     {
         "ApplyToAllRegions": bool,
@@ -1486,15 +1439,15 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventDataStoreRequestRequestTypeDef",
     {
         "Name": str,
@@ -1547,40 +1500,31 @@
 class UpdateEventDataStoreRequestRequestTypeDef(
     _RequiredUpdateEventDataStoreRequestRequestTypeDef,
     _OptionalUpdateEventDataStoreRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "ResourceTagList": List[ResourceTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "EventSelectors": List[EventSelectorOutputTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEventSelectorsResponseTypeDef = TypedDict(
     "PutEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "EventSelectors": List[EventSelectorOutputTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
@@ -1603,91 +1547,91 @@
 
 
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImportResponseTypeDef = TypedDict(
     "GetImportResponseTypeDef",
     {
         "ImportId": str,
         "Destinations": List[str],
-        "ImportSource": ImportSourceOutputTypeDef,
+        "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartImportRequestRequestTypeDef = TypedDict(
+    "StartImportRequestRequestTypeDef",
+    {
+        "Destinations": Sequence[str],
+        "ImportSource": ImportSourceTypeDef,
+        "StartEventTime": Union[datetime, str],
+        "EndEventTime": Union[datetime, str],
+        "ImportId": str,
+    },
+    total=False,
+)
+
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "ImportId": str,
         "Destinations": List[str],
-        "ImportSource": ImportSourceOutputTypeDef,
+        "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopImportResponseTypeDef = TypedDict(
     "StopImportResponseTypeDef",
     {
         "ImportId": str,
-        "ImportSource": ImportSourceOutputTypeDef,
+        "ImportSource": ImportSourceTypeDef,
         "Destinations": List[str],
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartImportRequestRequestTypeDef = TypedDict(
-    "StartImportRequestRequestTypeDef",
-    {
-        "Destinations": Sequence[str],
-        "ImportSource": ImportSourceTypeDef,
-        "StartEventTime": Union[datetime, str],
-        "EndEventTime": Union[datetime, str],
-        "ImportId": str,
-    },
-    total=False,
-)
-
 ListEventDataStoresResponseTypeDef = TypedDict(
     "ListEventDataStoresResponseTypeDef",
     {
         "EventDataStores": List[EventDataStoreTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
-        "Destinations": List[DestinationOutputTypeDef],
+        "Destinations": List[DestinationTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/type_defs.pyi` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,17 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
     "AdvancedFieldSelectorOutputTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
-    "CancelQueryResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
-    "DestinationOutputTypeDef",
-    "TagOutputTypeDef",
-    "CreateTrailResponseTypeDef",
     "DataResourceOutputTypeDef",
     "DataResourceTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteEventDataStoreRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteTrailRequestRequestTypeDef",
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
@@ -62,106 +59,104 @@
     "GetChannelRequestRequestTypeDef",
     "IngestionStatusTypeDef",
     "GetEventDataStoreRequestRequestTypeDef",
     "GetEventSelectorsRequestRequestTypeDef",
     "GetImportRequestRequestTypeDef",
     "ImportStatisticsTypeDef",
     "GetInsightSelectorsRequestRequestTypeDef",
-    "InsightSelectorOutputTypeDef",
+    "InsightSelectorTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetTrailRequestRequestTypeDef",
     "GetTrailStatusRequestRequestTypeDef",
-    "GetTrailStatusResponseTypeDef",
     "ImportFailureListItemTypeDef",
-    "S3ImportSourceOutputTypeDef",
     "S3ImportSourceTypeDef",
     "ImportsListItemTypeDef",
-    "InsightSelectorTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListEventDataStoresRequestRequestTypeDef",
-    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListImportFailuresRequestRequestTypeDef",
-    "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "PublicKeyTypeDef",
     "ListQueriesRequestRequestTypeDef",
     "QueryTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "ListTrailsRequestListTrailsPaginateTypeDef",
     "ListTrailsRequestRequestTypeDef",
     "TrailInfoTypeDef",
     "LookupAttributeTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreEventDataStoreRequestRequestTypeDef",
     "StartEventDataStoreIngestionRequestRequestTypeDef",
     "StartLoggingRequestRequestTypeDef",
     "StartQueryRequestRequestTypeDef",
-    "StartQueryResponseTypeDef",
     "StopEventDataStoreIngestionRequestRequestTypeDef",
     "StopImportRequestRequestTypeDef",
     "StopLoggingRequestRequestTypeDef",
     "UpdateTrailRequestRequestTypeDef",
-    "UpdateTrailResponseTypeDef",
     "AddTagsRequestRequestTypeDef",
     "CreateTrailRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
+    "ResourceTagTypeDef",
     "AdvancedEventSelectorOutputTypeDef",
     "AdvancedEventSelectorTypeDef",
+    "CancelQueryResponseTypeDef",
+    "CreateTrailResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetTrailStatusResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "StartQueryResponseTypeDef",
+    "UpdateTrailResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
+    "CreateChannelResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
-    "CreateChannelResponseTypeDef",
-    "ResourceTagTypeDef",
     "EventSelectorOutputTypeDef",
     "EventSelectorTypeDef",
     "DescribeQueryResponseTypeDef",
     "DescribeTrailsResponseTypeDef",
     "GetTrailResponseTypeDef",
     "EventTypeDef",
     "GetInsightSelectorsResponseTypeDef",
+    "PutInsightSelectorsRequestRequestTypeDef",
     "PutInsightSelectorsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "ListImportFailuresResponseTypeDef",
-    "ImportSourceOutputTypeDef",
     "ImportSourceTypeDef",
     "ListImportsResponseTypeDef",
-    "PutInsightSelectorsRequestRequestTypeDef",
+    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    "ListImportsRequestListImportsPaginateTypeDef",
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
+    "ListTrailsRequestListTrailsPaginateTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
     "CreateEventDataStoreResponseTypeDef",
     "EventDataStoreTypeDef",
     "GetEventDataStoreResponseTypeDef",
     "RestoreEventDataStoreResponseTypeDef",
     "SourceConfigTypeDef",
     "UpdateEventDataStoreResponseTypeDef",
     "CreateEventDataStoreRequestRequestTypeDef",
     "UpdateEventDataStoreRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "GetEventSelectorsResponseTypeDef",
     "PutEventSelectorsResponseTypeDef",
     "PutEventSelectorsRequestRequestTypeDef",
     "LookupEventsResponseTypeDef",
     "GetImportResponseTypeDef",
+    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "StopImportResponseTypeDef",
-    "StartImportRequestRequestTypeDef",
     "ListEventDataStoresResponseTypeDef",
     "GetChannelResponseTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
@@ -242,20 +237,22 @@
 )
 
 class CancelQueryRequestRequestTypeDef(
     _RequiredCancelQueryRequestRequestTypeDef, _OptionalCancelQueryRequestRequestTypeDef
 ):
     pass
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "QueryId": str,
-        "QueryStatus": QueryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "ChannelArn": str,
@@ -268,59 +265,14 @@
     "DestinationTypeDef",
     {
         "Type": DestinationTypeType,
         "Location": str,
     },
 )
 
-DestinationOutputTypeDef = TypedDict(
-    "DestinationOutputTypeDef",
-    {
-        "Type": DestinationTypeType,
-        "Location": str,
-    },
-)
-
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-CreateTrailResponseTypeDef = TypedDict(
-    "CreateTrailResponseTypeDef",
-    {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataResourceOutputTypeDef = TypedDict(
     "DataResourceOutputTypeDef",
     {
         "Type": str,
         "Values": List[str],
     },
     total=False,
@@ -488,16 +440,16 @@
 GetInsightSelectorsRequestRequestTypeDef = TypedDict(
     "GetInsightSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
     },
 )
 
-InsightSelectorOutputTypeDef = TypedDict(
-    "InsightSelectorOutputTypeDef",
+InsightSelectorTypeDef = TypedDict(
+    "InsightSelectorTypeDef",
     {
         "InsightType": InsightTypeType,
     },
     total=False,
 )
 
 _RequiredGetQueryResultsRequestRequestTypeDef = TypedDict(
@@ -534,82 +486,40 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrailRequestRequestTypeDef = TypedDict(
     "GetTrailRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 GetTrailStatusRequestRequestTypeDef = TypedDict(
     "GetTrailStatusRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-GetTrailStatusResponseTypeDef = TypedDict(
-    "GetTrailStatusResponseTypeDef",
-    {
-        "IsLogging": bool,
-        "LatestDeliveryError": str,
-        "LatestNotificationError": str,
-        "LatestDeliveryTime": datetime,
-        "LatestNotificationTime": datetime,
-        "StartLoggingTime": datetime,
-        "StopLoggingTime": datetime,
-        "LatestCloudWatchLogsDeliveryError": str,
-        "LatestCloudWatchLogsDeliveryTime": datetime,
-        "LatestDigestDeliveryTime": datetime,
-        "LatestDigestDeliveryError": str,
-        "LatestDeliveryAttemptTime": str,
-        "LatestNotificationAttemptTime": str,
-        "LatestNotificationAttemptSucceeded": str,
-        "LatestDeliveryAttemptSucceeded": str,
-        "TimeLoggingStarted": str,
-        "TimeLoggingStopped": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImportFailureListItemTypeDef = TypedDict(
     "ImportFailureListItemTypeDef",
     {
         "Location": str,
         "Status": ImportFailureStatusType,
         "ErrorType": str,
         "ErrorMessage": str,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-S3ImportSourceOutputTypeDef = TypedDict(
-    "S3ImportSourceOutputTypeDef",
-    {
-        "S3LocationUri": str,
-        "S3BucketRegion": str,
-        "S3BucketAccessRoleArn": str,
-    },
-)
-
 S3ImportSourceTypeDef = TypedDict(
     "S3ImportSourceTypeDef",
     {
         "S3LocationUri": str,
         "S3BucketRegion": str,
         "S3BucketAccessRoleArn": str,
     },
@@ -623,22 +533,14 @@
         "Destinations": List[str],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-InsightSelectorTypeDef = TypedDict(
-    "InsightSelectorTypeDef",
-    {
-        "InsightType": InsightTypeType,
-    },
-    total=False,
-)
-
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -649,34 +551,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
-    {
-        "ImportId": str,
-    },
-)
-_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
-    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
-    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
-):
-    pass
-
 _RequiredListImportFailuresRequestRequestTypeDef = TypedDict(
     "_RequiredListImportFailuresRequestRequestTypeDef",
     {
         "ImportId": str,
     },
 )
 _OptionalListImportFailuresRequestRequestTypeDef = TypedDict(
@@ -690,45 +582,25 @@
 
 class ListImportFailuresRequestRequestTypeDef(
     _RequiredListImportFailuresRequestRequestTypeDef,
     _OptionalListImportFailuresRequestRequestTypeDef,
 ):
     pass
 
-ListImportsRequestListImportsPaginateTypeDef = TypedDict(
-    "ListImportsRequestListImportsPaginateTypeDef",
-    {
-        "Destination": str,
-        "ImportStatus": ImportStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "Destination": str,
         "ImportStatus": ImportStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
-ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPublicKeysRequestRequestTypeDef = TypedDict(
     "ListPublicKeysRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "NextToken": str,
     },
@@ -775,33 +647,14 @@
         "QueryId": str,
         "QueryStatus": QueryStatusType,
         "CreationTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceIdList": Sequence[str],
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceIdList": Sequence[str],
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -813,22 +666,14 @@
 )
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
-ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
-    "ListTrailsRequestListTrailsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTrailsRequestRequestTypeDef = TypedDict(
     "ListTrailsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -847,59 +692,29 @@
     "LookupAttributeTypeDef",
     {
         "AttributeKey": LookupAttributeKeyType,
         "AttributeValue": str,
     },
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourcePolicy": str,
     },
 )
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterOrganizationDelegatedAdminRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
     {
         "MemberAccountId": str,
     },
 )
 
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
 RestoreEventDataStoreRequestRequestTypeDef = TypedDict(
     "RestoreEventDataStoreRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 
@@ -924,22 +739,14 @@
         "DeliveryS3Uri": str,
         "QueryAlias": str,
         "QueryParameters": Sequence[str],
     },
     total=False,
 )
 
-StartQueryResponseTypeDef = TypedDict(
-    "StartQueryResponseTypeDef",
-    {
-        "QueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopEventDataStoreIngestionRequestRequestTypeDef = TypedDict(
     "StopEventDataStoreIngestionRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 
@@ -981,34 +788,14 @@
 )
 
 class UpdateTrailRequestRequestTypeDef(
     _RequiredUpdateTrailRequestRequestTypeDef, _OptionalUpdateTrailRequestRequestTypeDef
 ):
     pass
 
-UpdateTrailResponseTypeDef = TypedDict(
-    "UpdateTrailResponseTypeDef",
-    {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddTagsRequestRequestTypeDef = TypedDict(
     "AddTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
@@ -1046,14 +833,23 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
 
+ResourceTagTypeDef = TypedDict(
+    "ResourceTagTypeDef",
+    {
+        "ResourceId": str,
+        "TagsList": List[TagTypeDef],
+    },
+    total=False,
+)
+
 _RequiredAdvancedEventSelectorOutputTypeDef = TypedDict(
     "_RequiredAdvancedEventSelectorOutputTypeDef",
     {
         "FieldSelectors": List[AdvancedFieldSelectorOutputTypeDef],
     },
 )
 _OptionalAdvancedEventSelectorOutputTypeDef = TypedDict(
@@ -1084,20 +880,119 @@
 )
 
 class AdvancedEventSelectorTypeDef(
     _RequiredAdvancedEventSelectorTypeDef, _OptionalAdvancedEventSelectorTypeDef
 ):
     pass
 
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
+    {
+        "QueryId": str,
+        "QueryStatus": QueryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrailResponseTypeDef = TypedDict(
+    "CreateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTrailStatusResponseTypeDef = TypedDict(
+    "GetTrailStatusResponseTypeDef",
+    {
+        "IsLogging": bool,
+        "LatestDeliveryError": str,
+        "LatestNotificationError": str,
+        "LatestDeliveryTime": datetime,
+        "LatestNotificationTime": datetime,
+        "StartLoggingTime": datetime,
+        "StopLoggingTime": datetime,
+        "LatestCloudWatchLogsDeliveryError": str,
+        "LatestCloudWatchLogsDeliveryTime": datetime,
+        "LatestDigestDeliveryTime": datetime,
+        "LatestDigestDeliveryError": str,
+        "LatestDeliveryAttemptTime": str,
+        "LatestNotificationAttemptTime": str,
+        "LatestNotificationAttemptSucceeded": str,
+        "LatestDeliveryAttemptSucceeded": str,
+        "TimeLoggingStarted": str,
+        "TimeLoggingStopped": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryResponseTypeDef = TypedDict(
+    "StartQueryResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrailResponseTypeDef = TypedDict(
+    "UpdateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Name": str,
@@ -1114,14 +1009,26 @@
 )
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "Name": str,
+        "Source": str,
+        "Destinations": List[DestinationTypeDef],
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "Channel": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
@@ -1140,38 +1047,17 @@
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
-        "Destinations": List[DestinationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "Name": str,
-        "Source": str,
-        "Destinations": List[DestinationOutputTypeDef],
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResourceTagTypeDef = TypedDict(
-    "ResourceTagTypeDef",
-    {
-        "ResourceId": str,
-        "TagsList": List[TagOutputTypeDef],
+        "Destinations": List[DestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 EventSelectorOutputTypeDef = TypedDict(
     "EventSelectorOutputTypeDef",
     {
         "ReadWriteType": ReadWriteTypeType,
         "IncludeManagementEvents": bool,
@@ -1198,31 +1084,31 @@
         "QueryId": str,
         "QueryString": str,
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsForDescribeQueryTypeDef,
         "ErrorMessage": str,
         "DeliveryS3Uri": str,
         "DeliveryStatus": DeliveryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrailsResponseTypeDef = TypedDict(
     "DescribeTrailsResponseTypeDef",
     {
         "trailList": List[TrailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrailResponseTypeDef = TypedDict(
     "GetTrailResponseTypeDef",
     {
         "Trail": TrailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "EventId": str,
@@ -1238,53 +1124,54 @@
     total=False,
 )
 
 GetInsightSelectorsResponseTypeDef = TypedDict(
     "GetInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "InsightSelectors": List[InsightSelectorOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InsightSelectors": List[InsightSelectorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutInsightSelectorsRequestRequestTypeDef = TypedDict(
+    "PutInsightSelectorsRequestRequestTypeDef",
+    {
+        "TrailName": str,
+        "InsightSelectors": Sequence[InsightSelectorTypeDef],
     },
 )
 
 PutInsightSelectorsResponseTypeDef = TypedDict(
     "PutInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "InsightSelectors": List[InsightSelectorOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InsightSelectors": List[InsightSelectorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsTypeDef,
         "QueryResultRows": List[List[Dict[str, str]]],
         "NextToken": str,
         "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImportFailuresResponseTypeDef = TypedDict(
     "ListImportFailuresResponseTypeDef",
     {
         "Failures": List[ImportFailureListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportSourceOutputTypeDef = TypedDict(
-    "ImportSourceOutputTypeDef",
-    {
-        "S3": S3ImportSourceOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportSourceTypeDef = TypedDict(
     "ImportSourceTypeDef",
     {
         "S3": S3ImportSourceTypeDef,
@@ -1292,61 +1179,120 @@
 )
 
 ListImportsResponseTypeDef = TypedDict(
     "ListImportsResponseTypeDef",
     {
         "Imports": List[ImportsListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutInsightSelectorsRequestRequestTypeDef = TypedDict(
-    "PutInsightSelectorsRequestRequestTypeDef",
+_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
     {
-        "TrailName": str,
-        "InsightSelectors": Sequence[InsightSelectorTypeDef],
+        "ImportId": str,
+    },
+)
+_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
+    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
+):
+    pass
+
+ListImportsRequestListImportsPaginateTypeDef = TypedDict(
+    "ListImportsRequestListImportsPaginateTypeDef",
+    {
+        "Destination": str,
+        "ImportStatus": ImportStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceIdList": Sequence[str],
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
+ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
+    "ListTrailsRequestListTrailsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListPublicKeysResponseTypeDef = TypedDict(
     "ListPublicKeysResponseTypeDef",
     {
         "PublicKeyList": List[PublicKeyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueriesResponseTypeDef = TypedDict(
     "ListQueriesResponseTypeDef",
     {
         "Queries": List[QueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrailsResponseTypeDef = TypedDict(
     "ListTrailsResponseTypeDef",
     {
         "Trails": List[TrailInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LookupEventsRequestLookupEventsPaginateTypeDef = TypedDict(
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "EventCategory": Literal["insight"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 LookupEventsRequestRequestTypeDef = TypedDict(
     "LookupEventsRequestRequestTypeDef",
     {
@@ -1356,30 +1302,39 @@
         "EventCategory": Literal["insight"],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "ResourceTagList": List[ResourceTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateEventDataStoreResponseTypeDef = TypedDict(
     "CreateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
         "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
-        "TagsList": List[TagOutputTypeDef],
+        "TagsList": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventDataStoreTypeDef = TypedDict(
     "EventDataStoreTypeDef",
     {
         "EventDataStoreArn": str,
@@ -1406,15 +1361,15 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreEventDataStoreResponseTypeDef = TypedDict(
     "RestoreEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
@@ -1424,15 +1379,15 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceConfigTypeDef = TypedDict(
     "SourceConfigTypeDef",
     {
         "ApplyToAllRegions": bool,
@@ -1451,15 +1406,15 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventDataStoreRequestRequestTypeDef",
     {
         "Name": str,
@@ -1508,40 +1463,31 @@
 
 class UpdateEventDataStoreRequestRequestTypeDef(
     _RequiredUpdateEventDataStoreRequestRequestTypeDef,
     _OptionalUpdateEventDataStoreRequestRequestTypeDef,
 ):
     pass
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "ResourceTagList": List[ResourceTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "EventSelectors": List[EventSelectorOutputTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEventSelectorsResponseTypeDef = TypedDict(
     "PutEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "EventSelectors": List[EventSelectorOutputTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
@@ -1562,91 +1508,91 @@
     pass
 
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImportResponseTypeDef = TypedDict(
     "GetImportResponseTypeDef",
     {
         "ImportId": str,
         "Destinations": List[str],
-        "ImportSource": ImportSourceOutputTypeDef,
+        "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartImportRequestRequestTypeDef = TypedDict(
+    "StartImportRequestRequestTypeDef",
+    {
+        "Destinations": Sequence[str],
+        "ImportSource": ImportSourceTypeDef,
+        "StartEventTime": Union[datetime, str],
+        "EndEventTime": Union[datetime, str],
+        "ImportId": str,
+    },
+    total=False,
+)
+
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "ImportId": str,
         "Destinations": List[str],
-        "ImportSource": ImportSourceOutputTypeDef,
+        "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopImportResponseTypeDef = TypedDict(
     "StopImportResponseTypeDef",
     {
         "ImportId": str,
-        "ImportSource": ImportSourceOutputTypeDef,
+        "ImportSource": ImportSourceTypeDef,
         "Destinations": List[str],
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartImportRequestRequestTypeDef = TypedDict(
-    "StartImportRequestRequestTypeDef",
-    {
-        "Destinations": Sequence[str],
-        "ImportSource": ImportSourceTypeDef,
-        "StartEventTime": Union[datetime, str],
-        "EndEventTime": Union[datetime, str],
-        "ImportId": str,
-    },
-    total=False,
-)
-
 ListEventDataStoresResponseTypeDef = TypedDict(
     "ListEventDataStoresResponseTypeDef",
     {
         "EventDataStores": List[EventDataStoreTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
-        "Destinations": List[DestinationOutputTypeDef],
+        "Destinations": List[DestinationTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/PKG-INFO` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudTrail 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudTrail 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,20 +351,17 @@
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
     AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
-    DestinationOutputTypeDef,
-    TagOutputTypeDef,
-    CreateTrailResponseTypeDef,
     DataResourceOutputTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
@@ -376,106 +373,104 @@
     GetChannelRequestRequestTypeDef,
     IngestionStatusTypeDef,
     GetEventDataStoreRequestRequestTypeDef,
     GetEventSelectorsRequestRequestTypeDef,
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
-    InsightSelectorOutputTypeDef,
+    InsightSelectorTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
-    GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
-    S3ImportSourceOutputTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
-    InsightSelectorTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
-    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListImportFailuresRequestRequestTypeDef,
-    ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     PublicKeyTypeDef,
     ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTrailsRequestListTrailsPaginateTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreEventDataStoreRequestRequestTypeDef,
     StartEventDataStoreIngestionRequestRequestTypeDef,
     StartLoggingRequestRequestTypeDef,
     StartQueryRequestRequestTypeDef,
-    StartQueryResponseTypeDef,
     StopEventDataStoreIngestionRequestRequestTypeDef,
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
-    UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
+    ResourceTagTypeDef,
     AdvancedEventSelectorOutputTypeDef,
     AdvancedEventSelectorTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateTrailResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetTrailStatusResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartQueryResponseTypeDef,
+    UpdateTrailResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
+    CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    ResourceTagTypeDef,
     EventSelectorOutputTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     GetTrailResponseTypeDef,
     EventTypeDef,
     GetInsightSelectorsResponseTypeDef,
+    PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
-    ImportSourceOutputTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
-    PutInsightSelectorsRequestRequestTypeDef,
+    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    ListImportsRequestListImportsPaginateTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
+    ListTrailsRequestListTrailsPaginateTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
     UpdateEventDataStoreResponseTypeDef,
     CreateEventDataStoreRequestRequestTypeDef,
     UpdateEventDataStoreRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
     PutEventSelectorsResponseTypeDef,
     PutEventSelectorsRequestRequestTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/SOURCES.txt` & `mypy-boto3-cloudtrail-1.28.15/mypy_boto3_cloudtrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.12/setup.py` & `mypy-boto3-cloudtrail-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudtrail",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cloudtrail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudTrail 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CloudTrail 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

