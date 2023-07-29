# Comparing `tmp/mypy-boto3-codestar-connections-1.28.12.tar.gz` & `tmp/mypy-boto3-codestar-connections-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codestar-connections-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
+gzip compressed data, was "mypy-boto3-codestar-connections-1.28.15.tar", last modified: Fri Jul 28 20:42:31 2023, max compression
```

## Comparing `mypy-boto3-codestar-connections-1.28.12.tar` & `mypy-boto3-codestar-connections-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.256549 mypy-boto3-codestar-connections-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-07-27 05:34:29.252550 mypy-boto3-codestar-connections-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.244550 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-27 05:19:15.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.252550 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 05:34:29.000000 mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.256549 mypy-boto3-codestar-connections-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-27 05:19:14.000000 mypy-boto3-codestar-connections-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.572867 mypy-boto3-codestar-connections-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-07-28 20:42:31.564867 mypy-boto3-codestar-connections-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.556867 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.564867 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-07-28 20:42:31.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-28 20:42:31.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:31.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 20:42:31.000000 mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:31.572867 mypy-boto3-codestar-connections-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-28 20:21:44.000000 mypy-boto3-codestar-connections-1.28.15/setup.py
```

### Comparing `mypy-boto3-codestar-connections-1.28.12/LICENSE` & `mypy-boto3-codestar-connections-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.12/PKG-INFO` & `mypy-boto3-codestar-connections-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-connections
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeStarconnections 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeStarconnections 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-connections)](https://pepy.tech/project/mypy-boto3-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarconnections 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[boto3.CodeStarconnections 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [mypy-boto3-codestar-connections docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,32 +301,31 @@
 `mypy_boto3_codestar_connections.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
-    TagOutputTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     DeleteConnectionInputRequestTypeDef,
     DeleteHostInputRequestTypeDef,
     GetConnectionInputRequestTypeDef,
     GetHostInputRequestTypeDef,
     VpcConfigurationOutputTypeDef,
     ListConnectionsInputRequestTypeDef,
     ListHostsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceInputRequestTypeDef,
-    GetConnectionOutputTypeDef,
-    ListConnectionsOutputTypeDef,
     CreateConnectionInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
+    GetConnectionOutputTypeDef,
+    ListConnectionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     CreateHostInputRequestTypeDef,
     UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
     ListHostsOutputTypeDef,
 )
```

### Comparing `mypy-boto3-codestar-connections-1.28.12/README.md` & `mypy-boto3-codestar-connections-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-connections)](https://pepy.tech/project/mypy-boto3-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarconnections 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[boto3.CodeStarconnections 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [mypy-boto3-codestar-connections docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,32 +269,31 @@
 `mypy_boto3_codestar_connections.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
-    TagOutputTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     DeleteConnectionInputRequestTypeDef,
     DeleteHostInputRequestTypeDef,
     GetConnectionInputRequestTypeDef,
     GetHostInputRequestTypeDef,
     VpcConfigurationOutputTypeDef,
     ListConnectionsInputRequestTypeDef,
     ListHostsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceInputRequestTypeDef,
-    GetConnectionOutputTypeDef,
-    ListConnectionsOutputTypeDef,
     CreateConnectionInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
+    GetConnectionOutputTypeDef,
+    ListConnectionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     CreateHostInputRequestTypeDef,
     UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
     ListHostsOutputTypeDef,
 )
```

### Comparing `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/__main__.py` & `mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeStarconnections 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodeStarconnections 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections\nOther"
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

### Comparing `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/client.py` & `mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/client.pyi` & `mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/literals.py` & `mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/literals.pyi` & `mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/type_defs.py` & `mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -17,36 +17,34 @@
 from .literals import ConnectionStatusType, ProviderTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ConnectionTypeDef",
     "TagTypeDef",
-    "TagOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "DeleteConnectionInputRequestTypeDef",
     "DeleteHostInputRequestTypeDef",
     "GetConnectionInputRequestTypeDef",
     "GetHostInputRequestTypeDef",
     "VpcConfigurationOutputTypeDef",
     "ListConnectionsInputRequestTypeDef",
     "ListHostsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "GetConnectionOutputTypeDef",
-    "ListConnectionsOutputTypeDef",
     "CreateConnectionInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateConnectionOutputTypeDef",
     "CreateHostOutputTypeDef",
+    "GetConnectionOutputTypeDef",
+    "ListConnectionsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "CreateHostInputRequestTypeDef",
     "UpdateHostInputRequestTypeDef",
     "GetHostOutputTypeDef",
     "HostTypeDef",
     "ListHostsOutputTypeDef",
 )
@@ -68,19 +66,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredVpcConfigurationTypeDef = TypedDict(
     "_RequiredVpcConfigurationTypeDef",
     {
         "VpcId": str,
@@ -92,19 +93,17 @@
     "_OptionalVpcConfigurationTypeDef",
     {
         "TlsCertificate": str,
     },
     total=False,
 )
 
-
 class VpcConfigurationTypeDef(_RequiredVpcConfigurationTypeDef, _OptionalVpcConfigurationTypeDef):
     pass
 
-
 DeleteConnectionInputRequestTypeDef = TypedDict(
     "DeleteConnectionInputRequestTypeDef",
     {
         "ConnectionArn": str,
     },
 )
 
@@ -141,21 +140,19 @@
     "_OptionalVpcConfigurationOutputTypeDef",
     {
         "TlsCertificate": str,
     },
     total=False,
 )
 
-
 class VpcConfigurationOutputTypeDef(
     _RequiredVpcConfigurationOutputTypeDef, _OptionalVpcConfigurationOutputTypeDef
 ):
     pass
 
-
 ListConnectionsInputRequestTypeDef = TypedDict(
     "ListConnectionsInputRequestTypeDef",
     {
         "ProviderTypeFilter": ProviderTypeType,
         "HostArnFilter": str,
         "MaxResults": int,
         "NextToken": str,
@@ -175,50 +172,22 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
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
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-GetConnectionOutputTypeDef = TypedDict(
-    "GetConnectionOutputTypeDef",
-    {
-        "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListConnectionsOutputTypeDef = TypedDict(
-    "ListConnectionsOutputTypeDef",
-    {
-        "Connections": List[ConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConnectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionInputRequestTypeDef",
     {
         "ConnectionName": str,
     },
 )
 _OptionalCreateConnectionInputRequestTypeDef = TypedDict(
@@ -227,52 +196,67 @@
         "ProviderType": ProviderTypeType,
         "Tags": Sequence[TagTypeDef],
         "HostArn": str,
     },
     total=False,
 )
 
-
 class CreateConnectionInputRequestTypeDef(
     _RequiredCreateConnectionInputRequestTypeDef, _OptionalCreateConnectionInputRequestTypeDef
 ):
     pass
 
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateConnectionOutputTypeDef = TypedDict(
     "CreateConnectionOutputTypeDef",
     {
         "ConnectionArn": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHostOutputTypeDef = TypedDict(
     "CreateHostOutputTypeDef",
     {
         "HostArn": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetConnectionOutputTypeDef = TypedDict(
+    "GetConnectionOutputTypeDef",
+    {
+        "Connection": ConnectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConnectionsOutputTypeDef = TypedDict(
+    "ListConnectionsOutputTypeDef",
+    {
+        "Connections": List[ConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHostInputRequestTypeDef = TypedDict(
     "_RequiredCreateHostInputRequestTypeDef",
     {
         "Name": str,
@@ -285,21 +269,19 @@
     {
         "VpcConfiguration": VpcConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateHostInputRequestTypeDef(
     _RequiredCreateHostInputRequestTypeDef, _OptionalCreateHostInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateHostInputRequestTypeDef = TypedDict(
     "_RequiredUpdateHostInputRequestTypeDef",
     {
         "HostArn": str,
     },
 )
 _OptionalUpdateHostInputRequestTypeDef = TypedDict(
@@ -307,30 +289,28 @@
     {
         "ProviderEndpoint": str,
         "VpcConfiguration": VpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateHostInputRequestTypeDef(
     _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
 ):
     pass
 
-
 GetHostOutputTypeDef = TypedDict(
     "GetHostOutputTypeDef",
     {
         "Name": str,
         "Status": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
         "VpcConfiguration": VpcConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "Name": str,
@@ -345,10 +325,10 @@
 )
 
 ListHostsOutputTypeDef = TypedDict(
     "ListHostsOutputTypeDef",
     {
         "Hosts": List[HostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections/type_defs.pyi` & `mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,35 +17,35 @@
 from .literals import ConnectionStatusType, ProviderTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ConnectionTypeDef",
     "TagTypeDef",
-    "TagOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "DeleteConnectionInputRequestTypeDef",
     "DeleteHostInputRequestTypeDef",
     "GetConnectionInputRequestTypeDef",
     "GetHostInputRequestTypeDef",
     "VpcConfigurationOutputTypeDef",
     "ListConnectionsInputRequestTypeDef",
     "ListHostsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "GetConnectionOutputTypeDef",
-    "ListConnectionsOutputTypeDef",
     "CreateConnectionInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateConnectionOutputTypeDef",
     "CreateHostOutputTypeDef",
+    "GetConnectionOutputTypeDef",
+    "ListConnectionsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "CreateHostInputRequestTypeDef",
     "UpdateHostInputRequestTypeDef",
     "GetHostOutputTypeDef",
     "HostTypeDef",
     "ListHostsOutputTypeDef",
 )
@@ -67,19 +67,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredVpcConfigurationTypeDef = TypedDict(
     "_RequiredVpcConfigurationTypeDef",
     {
         "VpcId": str,
@@ -91,17 +94,19 @@
     "_OptionalVpcConfigurationTypeDef",
     {
         "TlsCertificate": str,
     },
     total=False,
 )
 
+
 class VpcConfigurationTypeDef(_RequiredVpcConfigurationTypeDef, _OptionalVpcConfigurationTypeDef):
     pass
 
+
 DeleteConnectionInputRequestTypeDef = TypedDict(
     "DeleteConnectionInputRequestTypeDef",
     {
         "ConnectionArn": str,
     },
 )
 
@@ -138,19 +143,21 @@
     "_OptionalVpcConfigurationOutputTypeDef",
     {
         "TlsCertificate": str,
     },
     total=False,
 )
 
+
 class VpcConfigurationOutputTypeDef(
     _RequiredVpcConfigurationOutputTypeDef, _OptionalVpcConfigurationOutputTypeDef
 ):
     pass
 
+
 ListConnectionsInputRequestTypeDef = TypedDict(
     "ListConnectionsInputRequestTypeDef",
     {
         "ProviderTypeFilter": ProviderTypeType,
         "HostArnFilter": str,
         "MaxResults": int,
         "NextToken": str,
@@ -170,50 +177,22 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
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
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-GetConnectionOutputTypeDef = TypedDict(
-    "GetConnectionOutputTypeDef",
-    {
-        "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListConnectionsOutputTypeDef = TypedDict(
-    "ListConnectionsOutputTypeDef",
-    {
-        "Connections": List[ConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConnectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionInputRequestTypeDef",
     {
         "ConnectionName": str,
     },
 )
 _OptionalCreateConnectionInputRequestTypeDef = TypedDict(
@@ -222,50 +201,69 @@
         "ProviderType": ProviderTypeType,
         "Tags": Sequence[TagTypeDef],
         "HostArn": str,
     },
     total=False,
 )
 
+
 class CreateConnectionInputRequestTypeDef(
     _RequiredCreateConnectionInputRequestTypeDef, _OptionalCreateConnectionInputRequestTypeDef
 ):
     pass
 
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateConnectionOutputTypeDef = TypedDict(
     "CreateConnectionOutputTypeDef",
     {
         "ConnectionArn": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHostOutputTypeDef = TypedDict(
     "CreateHostOutputTypeDef",
     {
         "HostArn": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetConnectionOutputTypeDef = TypedDict(
+    "GetConnectionOutputTypeDef",
+    {
+        "Connection": ConnectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConnectionsOutputTypeDef = TypedDict(
+    "ListConnectionsOutputTypeDef",
+    {
+        "Connections": List[ConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHostInputRequestTypeDef = TypedDict(
     "_RequiredCreateHostInputRequestTypeDef",
     {
         "Name": str,
@@ -278,19 +276,21 @@
     {
         "VpcConfiguration": VpcConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateHostInputRequestTypeDef(
     _RequiredCreateHostInputRequestTypeDef, _OptionalCreateHostInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateHostInputRequestTypeDef = TypedDict(
     "_RequiredUpdateHostInputRequestTypeDef",
     {
         "HostArn": str,
     },
 )
 _OptionalUpdateHostInputRequestTypeDef = TypedDict(
@@ -298,28 +298,30 @@
     {
         "ProviderEndpoint": str,
         "VpcConfiguration": VpcConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateHostInputRequestTypeDef(
     _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
 ):
     pass
 
+
 GetHostOutputTypeDef = TypedDict(
     "GetHostOutputTypeDef",
     {
         "Name": str,
         "Status": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
         "VpcConfiguration": VpcConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "Name": str,
@@ -334,10 +336,10 @@
 )
 
 ListHostsOutputTypeDef = TypedDict(
     "ListHostsOutputTypeDef",
     {
         "Hosts": List[HostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/PKG-INFO` & `mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-connections
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeStarconnections 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeStarconnections 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-connections)](https://pepy.tech/project/mypy-boto3-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarconnections 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[boto3.CodeStarconnections 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [mypy-boto3-codestar-connections docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,32 +301,31 @@
 `mypy_boto3_codestar_connections.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
-    TagOutputTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     DeleteConnectionInputRequestTypeDef,
     DeleteHostInputRequestTypeDef,
     GetConnectionInputRequestTypeDef,
     GetHostInputRequestTypeDef,
     VpcConfigurationOutputTypeDef,
     ListConnectionsInputRequestTypeDef,
     ListHostsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceInputRequestTypeDef,
-    GetConnectionOutputTypeDef,
-    ListConnectionsOutputTypeDef,
     CreateConnectionInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
+    GetConnectionOutputTypeDef,
+    ListConnectionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     CreateHostInputRequestTypeDef,
     UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
     ListHostsOutputTypeDef,
 )
```

### Comparing `mypy-boto3-codestar-connections-1.28.12/mypy_boto3_codestar_connections.egg-info/SOURCES.txt` & `mypy-boto3-codestar-connections-1.28.15/mypy_boto3_codestar_connections.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.12/setup.py` & `mypy-boto3-codestar-connections-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codestar-connections",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_codestar_connections"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeStarconnections 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CodeStarconnections 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

