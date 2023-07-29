# Comparing `tmp/mypy-boto3-cognito-sync-1.28.12.tar.gz` & `tmp/mypy-boto3-cognito-sync-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-sync-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
+gzip compressed data, was "mypy-boto3-cognito-sync-1.28.15.tar", last modified: Fri Jul 28 20:42:31 2023, max compression
```

## Comparing `mypy-boto3-cognito-sync-1.28.12.tar` & `mypy-boto3-cognito-sync-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.632548 mypy-boto3-cognito-sync-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-07-27 05:34:29.632548 mypy-boto3-cognito-sync-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.624548 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.632548 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.632548 mypy-boto3-cognito-sync-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.696869 mypy-boto3-cognito-sync-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-28 20:42:31.688869 mypy-boto3-cognito-sync-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.684869 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.688869 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-28 20:42:31.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 20:42:31.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:31.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:31.000000 mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:31.696869 mypy-boto3-cognito-sync-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:21:55.000000 mypy-boto3-cognito-sync-1.28.15/setup.py
```

### Comparing `mypy-boto3-cognito-sync-1.28.12/LICENSE` & `mypy-boto3-cognito-sync-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.12/PKG-INFO` & `mypy-boto3-cognito-sync-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-sync
-Version: 1.28.12
-Summary: Type annotations for boto3.CognitoSync 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CognitoSync 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-sync)](https://pepy.tech/project/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,43 +301,42 @@
 
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
-    BulkPublishResponseTypeDef,
-    CognitoStreamsOutputTypeDef,
+    ResponseMetadataTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeIdentityPoolUsageRequestRequestTypeDef,
     IdentityPoolUsageTypeDef,
     DescribeIdentityUsageRequestRequestTypeDef,
     IdentityUsageTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsRequestRequestTypeDef,
-    GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsRequestRequestTypeDef,
-    GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationRequestRequestTypeDef,
     PushSyncOutputTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
     PushSyncTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceRequestRequestTypeDef,
-    RegisterDeviceResponseTypeDef,
-    ResponseMetadataTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
+    BulkPublishResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBulkPublishDetailsResponseTypeDef,
+    GetCognitoEventsResponseTypeDef,
+    RegisterDeviceResponseTypeDef,
     DeleteDatasetResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
```

### Comparing `mypy-boto3-cognito-sync-1.28.12/README.md` & `mypy-boto3-cognito-sync-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-sync)](https://pepy.tech/project/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,43 +269,42 @@
 
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
-    BulkPublishResponseTypeDef,
-    CognitoStreamsOutputTypeDef,
+    ResponseMetadataTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeIdentityPoolUsageRequestRequestTypeDef,
     IdentityPoolUsageTypeDef,
     DescribeIdentityUsageRequestRequestTypeDef,
     IdentityUsageTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsRequestRequestTypeDef,
-    GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsRequestRequestTypeDef,
-    GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationRequestRequestTypeDef,
     PushSyncOutputTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
     PushSyncTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceRequestRequestTypeDef,
-    RegisterDeviceResponseTypeDef,
-    ResponseMetadataTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
+    BulkPublishResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBulkPublishDetailsResponseTypeDef,
+    GetCognitoEventsResponseTypeDef,
+    RegisterDeviceResponseTypeDef,
     DeleteDatasetResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
```

### Comparing `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/__main__.py` & `mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoSync 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CognitoSync 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync\nOther"
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

### Comparing `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/client.py` & `mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/client.pyi` & `mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/literals.py` & `mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/literals.pyi` & `mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/type_defs.py` & `mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,43 +21,42 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BulkPublishRequestRequestTypeDef",
-    "BulkPublishResponseTypeDef",
-    "CognitoStreamsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CognitoStreamsTypeDef",
     "DatasetTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeIdentityPoolUsageRequestRequestTypeDef",
     "IdentityPoolUsageTypeDef",
     "DescribeIdentityUsageRequestRequestTypeDef",
     "IdentityUsageTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetBulkPublishDetailsRequestRequestTypeDef",
-    "GetBulkPublishDetailsResponseTypeDef",
     "GetCognitoEventsRequestRequestTypeDef",
-    "GetCognitoEventsResponseTypeDef",
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     "PushSyncOutputTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListIdentityPoolUsageRequestRequestTypeDef",
     "ListRecordsRequestRequestTypeDef",
     "RecordTypeDef",
     "PushSyncTypeDef",
     "RecordPatchTypeDef",
     "RegisterDeviceRequestRequestTypeDef",
-    "RegisterDeviceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SetCognitoEventsRequestRequestTypeDef",
     "SubscribeToDatasetRequestRequestTypeDef",
     "UnsubscribeFromDatasetRequestRequestTypeDef",
+    "BulkPublishResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetBulkPublishDetailsResponseTypeDef",
+    "GetCognitoEventsResponseTypeDef",
+    "RegisterDeviceResponseTypeDef",
     "DeleteDatasetResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeIdentityPoolUsageResponseTypeDef",
     "ListIdentityPoolUsageResponseTypeDef",
     "DescribeIdentityUsageResponseTypeDef",
     "GetIdentityPoolConfigurationResponseTypeDef",
@@ -71,30 +70,23 @@
 BulkPublishRequestRequestTypeDef = TypedDict(
     "BulkPublishRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-BulkPublishResponseTypeDef = TypedDict(
-    "BulkPublishResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CognitoStreamsOutputTypeDef = TypedDict(
-    "CognitoStreamsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "StreamName": str,
-        "RoleArn": str,
-        "StreamingStatus": StreamingStatusType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 CognitoStreamsTypeDef = TypedDict(
     "CognitoStreamsTypeDef",
     {
         "StreamName": str,
         "RoleArn": str,
@@ -169,55 +161,28 @@
         "LastModifiedDate": datetime,
         "DatasetCount": int,
         "DataStorage": int,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBulkPublishDetailsRequestRequestTypeDef = TypedDict(
     "GetBulkPublishDetailsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-GetBulkPublishDetailsResponseTypeDef = TypedDict(
-    "GetBulkPublishDetailsResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "BulkPublishStartTime": datetime,
-        "BulkPublishCompleteTime": datetime,
-        "BulkPublishStatus": BulkPublishStatusType,
-        "FailureMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCognitoEventsRequestRequestTypeDef = TypedDict(
     "GetCognitoEventsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-GetCognitoEventsResponseTypeDef = TypedDict(
-    "GetCognitoEventsResponseTypeDef",
-    {
-        "Events": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -338,33 +303,14 @@
         "IdentityPoolId": str,
         "IdentityId": str,
         "Platform": PlatformType,
         "Token": str,
     },
 )
 
-RegisterDeviceResponseTypeDef = TypedDict(
-    "RegisterDeviceResponseTypeDef",
-    {
-        "DeviceId": str,
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
 SetCognitoEventsRequestRequestTypeDef = TypedDict(
     "SetCognitoEventsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "Events": Mapping[str, str],
     },
 )
@@ -385,84 +331,127 @@
         "IdentityPoolId": str,
         "IdentityId": str,
         "DatasetName": str,
         "DeviceId": str,
     },
 )
 
+BulkPublishResponseTypeDef = TypedDict(
+    "BulkPublishResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBulkPublishDetailsResponseTypeDef = TypedDict(
+    "GetBulkPublishDetailsResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "BulkPublishStartTime": datetime,
+        "BulkPublishCompleteTime": datetime,
+        "BulkPublishStatus": BulkPublishStatusType,
+        "FailureMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCognitoEventsResponseTypeDef = TypedDict(
+    "GetCognitoEventsResponseTypeDef",
+    {
+        "Events": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterDeviceResponseTypeDef = TypedDict(
+    "RegisterDeviceResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteDatasetResponseTypeDef = TypedDict(
     "DeleteDatasetResponseTypeDef",
     {
         "Dataset": DatasetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "Dataset": DatasetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetTypeDef],
         "Count": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIdentityPoolUsageResponseTypeDef = TypedDict(
     "DescribeIdentityPoolUsageResponseTypeDef",
     {
         "IdentityPoolUsage": IdentityPoolUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityPoolUsageResponseTypeDef = TypedDict(
     "ListIdentityPoolUsageResponseTypeDef",
     {
         "IdentityPoolUsages": List[IdentityPoolUsageTypeDef],
         "MaxResults": int,
         "Count": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIdentityUsageResponseTypeDef = TypedDict(
     "DescribeIdentityUsageResponseTypeDef",
     {
         "IdentityUsage": IdentityUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "GetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
         "PushSync": PushSyncOutputTypeDef,
-        "CognitoStreams": CognitoStreamsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CognitoStreams": CognitoStreamsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "SetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
         "PushSync": PushSyncOutputTypeDef,
-        "CognitoStreams": CognitoStreamsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CognitoStreams": CognitoStreamsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordsResponseTypeDef = TypedDict(
     "ListRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
@@ -470,23 +459,23 @@
         "Count": int,
         "DatasetSyncCount": int,
         "LastModifiedBy": str,
         "MergedDatasetNames": List[str],
         "DatasetExists": bool,
         "DatasetDeletedAfterRequestedSyncCount": bool,
         "SyncSessionToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRecordsResponseTypeDef = TypedDict(
     "UpdateRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
```

### Comparing `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/type_defs.pyi` & `mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -20,43 +20,42 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BulkPublishRequestRequestTypeDef",
-    "BulkPublishResponseTypeDef",
-    "CognitoStreamsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CognitoStreamsTypeDef",
     "DatasetTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeIdentityPoolUsageRequestRequestTypeDef",
     "IdentityPoolUsageTypeDef",
     "DescribeIdentityUsageRequestRequestTypeDef",
     "IdentityUsageTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetBulkPublishDetailsRequestRequestTypeDef",
-    "GetBulkPublishDetailsResponseTypeDef",
     "GetCognitoEventsRequestRequestTypeDef",
-    "GetCognitoEventsResponseTypeDef",
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     "PushSyncOutputTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListIdentityPoolUsageRequestRequestTypeDef",
     "ListRecordsRequestRequestTypeDef",
     "RecordTypeDef",
     "PushSyncTypeDef",
     "RecordPatchTypeDef",
     "RegisterDeviceRequestRequestTypeDef",
-    "RegisterDeviceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SetCognitoEventsRequestRequestTypeDef",
     "SubscribeToDatasetRequestRequestTypeDef",
     "UnsubscribeFromDatasetRequestRequestTypeDef",
+    "BulkPublishResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetBulkPublishDetailsResponseTypeDef",
+    "GetCognitoEventsResponseTypeDef",
+    "RegisterDeviceResponseTypeDef",
     "DeleteDatasetResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeIdentityPoolUsageResponseTypeDef",
     "ListIdentityPoolUsageResponseTypeDef",
     "DescribeIdentityUsageResponseTypeDef",
     "GetIdentityPoolConfigurationResponseTypeDef",
@@ -70,30 +69,23 @@
 BulkPublishRequestRequestTypeDef = TypedDict(
     "BulkPublishRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-BulkPublishResponseTypeDef = TypedDict(
-    "BulkPublishResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CognitoStreamsOutputTypeDef = TypedDict(
-    "CognitoStreamsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "StreamName": str,
-        "RoleArn": str,
-        "StreamingStatus": StreamingStatusType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 CognitoStreamsTypeDef = TypedDict(
     "CognitoStreamsTypeDef",
     {
         "StreamName": str,
         "RoleArn": str,
@@ -168,55 +160,28 @@
         "LastModifiedDate": datetime,
         "DatasetCount": int,
         "DataStorage": int,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBulkPublishDetailsRequestRequestTypeDef = TypedDict(
     "GetBulkPublishDetailsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-GetBulkPublishDetailsResponseTypeDef = TypedDict(
-    "GetBulkPublishDetailsResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "BulkPublishStartTime": datetime,
-        "BulkPublishCompleteTime": datetime,
-        "BulkPublishStatus": BulkPublishStatusType,
-        "FailureMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCognitoEventsRequestRequestTypeDef = TypedDict(
     "GetCognitoEventsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-GetCognitoEventsResponseTypeDef = TypedDict(
-    "GetCognitoEventsResponseTypeDef",
-    {
-        "Events": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -331,33 +296,14 @@
         "IdentityPoolId": str,
         "IdentityId": str,
         "Platform": PlatformType,
         "Token": str,
     },
 )
 
-RegisterDeviceResponseTypeDef = TypedDict(
-    "RegisterDeviceResponseTypeDef",
-    {
-        "DeviceId": str,
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
 SetCognitoEventsRequestRequestTypeDef = TypedDict(
     "SetCognitoEventsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "Events": Mapping[str, str],
     },
 )
@@ -378,84 +324,127 @@
         "IdentityPoolId": str,
         "IdentityId": str,
         "DatasetName": str,
         "DeviceId": str,
     },
 )
 
+BulkPublishResponseTypeDef = TypedDict(
+    "BulkPublishResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBulkPublishDetailsResponseTypeDef = TypedDict(
+    "GetBulkPublishDetailsResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "BulkPublishStartTime": datetime,
+        "BulkPublishCompleteTime": datetime,
+        "BulkPublishStatus": BulkPublishStatusType,
+        "FailureMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCognitoEventsResponseTypeDef = TypedDict(
+    "GetCognitoEventsResponseTypeDef",
+    {
+        "Events": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterDeviceResponseTypeDef = TypedDict(
+    "RegisterDeviceResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteDatasetResponseTypeDef = TypedDict(
     "DeleteDatasetResponseTypeDef",
     {
         "Dataset": DatasetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "Dataset": DatasetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetTypeDef],
         "Count": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIdentityPoolUsageResponseTypeDef = TypedDict(
     "DescribeIdentityPoolUsageResponseTypeDef",
     {
         "IdentityPoolUsage": IdentityPoolUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityPoolUsageResponseTypeDef = TypedDict(
     "ListIdentityPoolUsageResponseTypeDef",
     {
         "IdentityPoolUsages": List[IdentityPoolUsageTypeDef],
         "MaxResults": int,
         "Count": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIdentityUsageResponseTypeDef = TypedDict(
     "DescribeIdentityUsageResponseTypeDef",
     {
         "IdentityUsage": IdentityUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "GetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
         "PushSync": PushSyncOutputTypeDef,
-        "CognitoStreams": CognitoStreamsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CognitoStreams": CognitoStreamsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "SetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
         "PushSync": PushSyncOutputTypeDef,
-        "CognitoStreams": CognitoStreamsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CognitoStreams": CognitoStreamsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordsResponseTypeDef = TypedDict(
     "ListRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
@@ -463,23 +452,23 @@
         "Count": int,
         "DatasetSyncCount": int,
         "LastModifiedBy": str,
         "MergedDatasetNames": List[str],
         "DatasetExists": bool,
         "DatasetDeletedAfterRequestedSyncCount": bool,
         "SyncSessionToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRecordsResponseTypeDef = TypedDict(
     "UpdateRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
```

### Comparing `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/PKG-INFO` & `mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-sync
-Version: 1.28.12
-Summary: Type annotations for boto3.CognitoSync 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CognitoSync 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-sync)](https://pepy.tech/project/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
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
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,43 +301,42 @@
 
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
-    BulkPublishResponseTypeDef,
-    CognitoStreamsOutputTypeDef,
+    ResponseMetadataTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeIdentityPoolUsageRequestRequestTypeDef,
     IdentityPoolUsageTypeDef,
     DescribeIdentityUsageRequestRequestTypeDef,
     IdentityUsageTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsRequestRequestTypeDef,
-    GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsRequestRequestTypeDef,
-    GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationRequestRequestTypeDef,
     PushSyncOutputTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
     PushSyncTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceRequestRequestTypeDef,
-    RegisterDeviceResponseTypeDef,
-    ResponseMetadataTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
+    BulkPublishResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBulkPublishDetailsResponseTypeDef,
+    GetCognitoEventsResponseTypeDef,
+    RegisterDeviceResponseTypeDef,
     DeleteDatasetResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
```

### Comparing `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/SOURCES.txt` & `mypy-boto3-cognito-sync-1.28.15/mypy_boto3_cognito_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.12/setup.py` & `mypy-boto3-cognito-sync-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-sync",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cognito_sync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoSync 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CognitoSync 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

