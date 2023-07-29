# Comparing `tmp/mypy-boto3-cloudtrail-data-1.28.12.tar.gz` & `tmp/mypy-boto3-cloudtrail-data-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudtrail-data-1.28.12.tar", last modified: Thu Jul 27 05:34:26 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudtrail-data-1.28.15.tar", last modified: Fri Jul 28 20:42:28 2023, max compression
```

## Comparing `mypy-boto3-cloudtrail-data-1.28.12.tar` & `mypy-boto3-cloudtrail-data-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.948557 mypy-boto3-cloudtrail-data-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-27 05:34:26.948557 mypy-boto3-cloudtrail-data-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.948557 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.948557 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:26.948557 mypy-boto3-cloudtrail-data-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 05:18:49.000000 mypy-boto3-cloudtrail-data-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.216820 mypy-boto3-cloudtrail-data-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:06.000000 mypy-boto3-cloudtrail-data-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-28 20:42:28.204820 mypy-boto3-cloudtrail-data-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-07-28 20:21:06.000000 mypy-boto3-cloudtrail-data-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.200820 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-28 20:21:06.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-28 20:21:06.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-28 20:21:07.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-28 20:21:07.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-28 20:21:07.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-28 20:21:07.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-28 20:21:07.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:07.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-28 20:21:08.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-28 20:21:07.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:06.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.204820 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-28 20:42:27.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-28 20:42:28.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:27.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:27.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:27.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:42:27.000000 mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:28.216820 mypy-boto3-cloudtrail-data-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 20:21:06.000000 mypy-boto3-cloudtrail-data-1.28.15/setup.py
```

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/LICENSE` & `mypy-boto3-cloudtrail-data-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/PKG-INFO` & `mypy-boto3-cloudtrail-data-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail-data
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudTrailDataService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudTrailDataService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail-data)](https://pepy.tech/project/mypy-boto3-cloudtrail-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrailDataService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService)
+[boto3.CloudTrailDataService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService)
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
 [mypy-boto3-cloudtrail-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,16 +299,16 @@
 `mypy_boto3_cloudtrail_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail_data.type_defs import (
     AuditEventResultEntryTypeDef,
     AuditEventTypeDef,
-    ResultErrorEntryTypeDef,
     ResponseMetadataTypeDef,
+    ResultErrorEntryTypeDef,
     PutAuditEventsRequestRequestTypeDef,
     PutAuditEventsResponseTypeDef,
 )
 
 
 def get_structure() -> AuditEventResultEntryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/README.md` & `mypy-boto3-cloudtrail-data-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail-data)](https://pepy.tech/project/mypy-boto3-cloudtrail-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrailDataService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService)
+[boto3.CloudTrailDataService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService)
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
 [mypy-boto3-cloudtrail-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,16 +267,16 @@
 `mypy_boto3_cloudtrail_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail_data.type_defs import (
     AuditEventResultEntryTypeDef,
     AuditEventTypeDef,
-    ResultErrorEntryTypeDef,
     ResponseMetadataTypeDef,
+    ResultErrorEntryTypeDef,
     PutAuditEventsRequestRequestTypeDef,
     PutAuditEventsResponseTypeDef,
 )
 
 
 def get_structure() -> AuditEventResultEntryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/__main__.py` & `mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudTrailDataService 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudTrailDataService 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService\nOther"
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

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/client.py` & `mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/client.pyi` & `mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/literals.py` & `mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/literals.pyi` & `mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/type_defs.py` & `mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AuditEventResultEntryTypeDef",
     "AuditEventTypeDef",
-    "ResultErrorEntryTypeDef",
     "ResponseMetadataTypeDef",
+    "ResultErrorEntryTypeDef",
     "PutAuditEventsRequestRequestTypeDef",
     "PutAuditEventsResponseTypeDef",
 )
 
 AuditEventResultEntryTypeDef = TypedDict(
     "AuditEventResultEntryTypeDef",
     {
@@ -53,34 +53,34 @@
 )
 
 
 class AuditEventTypeDef(_RequiredAuditEventTypeDef, _OptionalAuditEventTypeDef):
     pass
 
 
-ResultErrorEntryTypeDef = TypedDict(
-    "ResultErrorEntryTypeDef",
-    {
-        "errorCode": str,
-        "errorMessage": str,
-        "id": str,
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ResultErrorEntryTypeDef = TypedDict(
+    "ResultErrorEntryTypeDef",
+    {
+        "errorCode": str,
+        "errorMessage": str,
+        "id": str,
+    },
+)
+
 _RequiredPutAuditEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutAuditEventsRequestRequestTypeDef",
     {
         "auditEvents": Sequence[AuditEventTypeDef],
         "channelArn": str,
     },
 )
@@ -100,10 +100,10 @@
 
 
 PutAuditEventsResponseTypeDef = TypedDict(
     "PutAuditEventsResponseTypeDef",
     {
         "failed": List[ResultErrorEntryTypeDef],
         "successful": List[AuditEventResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data/type_defs.pyi` & `mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AuditEventResultEntryTypeDef",
     "AuditEventTypeDef",
-    "ResultErrorEntryTypeDef",
     "ResponseMetadataTypeDef",
+    "ResultErrorEntryTypeDef",
     "PutAuditEventsRequestRequestTypeDef",
     "PutAuditEventsResponseTypeDef",
 )
 
 AuditEventResultEntryTypeDef = TypedDict(
     "AuditEventResultEntryTypeDef",
     {
@@ -50,34 +50,34 @@
     },
     total=False,
 )
 
 class AuditEventTypeDef(_RequiredAuditEventTypeDef, _OptionalAuditEventTypeDef):
     pass
 
-ResultErrorEntryTypeDef = TypedDict(
-    "ResultErrorEntryTypeDef",
-    {
-        "errorCode": str,
-        "errorMessage": str,
-        "id": str,
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ResultErrorEntryTypeDef = TypedDict(
+    "ResultErrorEntryTypeDef",
+    {
+        "errorCode": str,
+        "errorMessage": str,
+        "id": str,
+    },
+)
+
 _RequiredPutAuditEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutAuditEventsRequestRequestTypeDef",
     {
         "auditEvents": Sequence[AuditEventTypeDef],
         "channelArn": str,
     },
 )
@@ -95,10 +95,10 @@
     pass
 
 PutAuditEventsResponseTypeDef = TypedDict(
     "PutAuditEventsResponseTypeDef",
     {
         "failed": List[ResultErrorEntryTypeDef],
         "successful": List[AuditEventResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data.egg-info/PKG-INFO` & `mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail-data
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudTrailDataService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudTrailDataService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail-data)](https://pepy.tech/project/mypy-boto3-cloudtrail-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrailDataService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService)
+[boto3.CloudTrailDataService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService)
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
 [mypy-boto3-cloudtrail-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,16 +299,16 @@
 `mypy_boto3_cloudtrail_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail_data.type_defs import (
     AuditEventResultEntryTypeDef,
     AuditEventTypeDef,
-    ResultErrorEntryTypeDef,
     ResponseMetadataTypeDef,
+    ResultErrorEntryTypeDef,
     PutAuditEventsRequestRequestTypeDef,
     PutAuditEventsResponseTypeDef,
 )
 
 
 def get_structure() -> AuditEventResultEntryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/mypy_boto3_cloudtrail_data.egg-info/SOURCES.txt` & `mypy-boto3-cloudtrail-data-1.28.15/mypy_boto3_cloudtrail_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-data-1.28.12/setup.py` & `mypy-boto3-cloudtrail-data-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudtrail-data",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cloudtrail_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudTrailDataService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CloudTrailDataService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

