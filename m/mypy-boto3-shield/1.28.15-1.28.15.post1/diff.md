# Comparing `tmp/mypy-boto3-shield-1.28.15.tar.gz` & `tmp/mypy-boto3-shield-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-shield-1.28.15.tar", last modified: Fri Jul 28 20:43:45 2023, max compression
+gzip compressed data, was "mypy-boto3-shield-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:12 2023, max compression
```

## Comparing `mypy-boto3-shield-1.28.15.tar` & `mypy-boto3-shield-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.777892 mypy-boto3-shield-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-07-28 20:43:45.773892 mypy-boto3-shield-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.773892 mypy-boto3-shield-1.28.15/mypy_boto3_shield/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25575 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-28 20:39:31.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-28 20:39:31.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-28 20:39:31.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22613 2023-07-28 20:39:31.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.773892 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:45.777892 mypy-boto3-shield-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.497405 mypy-boto3-shield-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-07-29 10:04:12.497405 mypy-boto3-shield-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.477405 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25777 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25732 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-29 09:59:41.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-29 09:59:41.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22613 2023-07-29 09:59:41.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.497405 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:12.497405 mypy-boto3-shield-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-shield-1.28.15/LICENSE` & `mypy-boto3-shield-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15/PKG-INFO` & `mypy-boto3-shield-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-shield
-Version: 1.28.15
-Summary: Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-shield-1.28.15/README.md` & `mypy-boto3-shield-1.28.15.post1/README.md`

 * *Files 1% similar despite different names*

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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/__init__.py` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/__init__.pyi` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/__main__.py` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Shield 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Shield 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield\nOther"
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

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/client.py` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_shield.client import ShieldClient
 
     session = Session()
     client: ShieldClient = session.client("shield")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoRenewType,
     ProtectedResourceTypeType,
     ProtectionGroupAggregationType,
@@ -39,16 +39,18 @@
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     ListProtectionsResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ResponseActionOutputTypeDef,
     ResponseActionTypeDef,
     TagTypeDef,
+    TimeRangeOutputTypeDef,
     TimeRangeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -326,15 +328,15 @@
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.disassociate_health_check)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#disassociate_health_check)
         """
 
     def enable_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionTypeDef
+        self, *, ResourceArn: str, Action: Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Enable the Shield Advanced automatic application layer DDoS mitigation for the
         protected resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.enable_application_layer_automatic_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#enable_application_layer_automatic_response)
@@ -372,16 +374,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#get_subscription_state)
         """
 
     def list_attacks(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeTypeDef = ...,
-        EndTime: TimeRangeTypeDef = ...,
+        StartTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
+        EndTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListAttacksResponseTypeDef:
         """
         Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
         period.
 
@@ -449,15 +451,15 @@
         Removes tags from a resource in Shield.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#untag_resource)
         """
 
     def update_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionTypeDef
+        self, *, ResourceArn: str, Action: Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates an existing Shield Advanced automatic application layer DDoS mitigation
         configuration for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.update_application_layer_automatic_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#update_application_layer_automatic_response)
```

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/client.pyi` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_shield.client import ShieldClient
 
     session = Session()
     client: ShieldClient = session.client("shield")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoRenewType,
     ProtectedResourceTypeType,
     ProtectionGroupAggregationType,
@@ -39,16 +39,18 @@
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     ListProtectionsResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ResponseActionOutputTypeDef,
     ResponseActionTypeDef,
     TagTypeDef,
+    TimeRangeOutputTypeDef,
     TimeRangeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -297,15 +299,15 @@
         Removes health-based detection from the Shield Advanced protection for a
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.disassociate_health_check)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#disassociate_health_check)
         """
     def enable_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionTypeDef
+        self, *, ResourceArn: str, Action: Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Enable the Shield Advanced automatic application layer DDoS mitigation for the
         protected resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.enable_application_layer_automatic_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#enable_application_layer_automatic_response)
@@ -339,16 +341,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.get_subscription_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#get_subscription_state)
         """
     def list_attacks(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeTypeDef = ...,
-        EndTime: TimeRangeTypeDef = ...,
+        StartTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
+        EndTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListAttacksResponseTypeDef:
         """
         Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
         period.
 
@@ -409,15 +411,15 @@
         """
         Removes tags from a resource in Shield.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#untag_resource)
         """
     def update_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionTypeDef
+        self, *, ResourceArn: str, Action: Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates an existing Shield Advanced automatic application layer DDoS mitigation
         configuration for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.update_application_layer_automatic_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#update_application_layer_automatic_response)
```

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/literals.py` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/literals.pyi` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/paginator.py` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -17,59 +17,56 @@
     session = Session()
     client: ShieldClient = session.client("shield")
 
     list_attacks_paginator: ListAttacksPaginator = client.get_paginator("list_attacks")
     list_protections_paginator: ListProtectionsPaginator = client.get_paginator("list_protections")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     InclusionProtectionFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimeRangeOutputTypeDef,
     TimeRangeTypeDef,
 )
 
 __all__ = ("ListAttacksPaginator", "ListProtectionsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAttacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeTypeDef = ...,
-        EndTime: TimeRangeTypeDef = ...,
+        StartTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
+        EndTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
         """
 
-
 class ListProtectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/paginator.pyi` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/paginator.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,55 +17,60 @@
     session = Session()
     client: ShieldClient = session.client("shield")
 
     list_attacks_paginator: ListAttacksPaginator = client.get_paginator("list_attacks")
     list_protections_paginator: ListProtectionsPaginator = client.get_paginator("list_protections")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     InclusionProtectionFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimeRangeOutputTypeDef,
     TimeRangeTypeDef,
 )
 
 __all__ = ("ListAttacksPaginator", "ListProtectionsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAttacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeTypeDef = ...,
-        EndTime: TimeRangeTypeDef = ...,
+        StartTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
+        EndTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
         """
 
+
 class ListProtectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/type_defs.py` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield/type_defs.pyi` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/PKG-INFO` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-shield
-Version: 1.28.15
-Summary: Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/SOURCES.txt` & `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15/setup.py` & `mypy-boto3-shield-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-shield",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_shield"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

