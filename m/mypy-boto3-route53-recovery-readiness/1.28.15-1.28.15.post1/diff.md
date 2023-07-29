# Comparing `tmp/mypy-boto3-route53-recovery-readiness-1.28.15.tar.gz` & `tmp/mypy-boto3-route53-recovery-readiness-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-recovery-readiness-1.28.15.tar", last modified: Fri Jul 28 20:43:36 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-recovery-readiness-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:02 2023, max compression
```

## Comparing `mypy-boto3-route53-recovery-readiness-1.28.15.tar` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.929771 mypy-boto3-route53-recovery-readiness-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19048 2023-07-28 20:43:36.929771 mypy-boto3-route53-recovery-readiness-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17487 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.909771 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28483 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-28 20:37:17.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-28 20:37:17.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-07-28 20:37:17.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-28 20:37:17.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30054 2023-07-28 20:37:18.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30017 2023-07-28 20:37:17.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.929771 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19048 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:36.929771 mypy-boto3-route53-recovery-readiness-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:02.785371 mypy-boto3-route53-recovery-readiness-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-07-29 10:04:02.785371 mypy-boto3-route53-recovery-readiness-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17487 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:02.769371 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28609 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30121 2023-07-29 09:57:23.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30084 2023-07-29 09:57:23.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:22.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:02.785371 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:02.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:02.785371 mypy-boto3-route53-recovery-readiness-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-29 09:57:21.000000 mypy-boto3-route53-recovery-readiness-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/LICENSE` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/PKG-INFO` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-readiness
-Version: 1.28.15
-Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/README.md` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/README.md`

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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__init__.py` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__init__.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__main__.py` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.Route53RecoveryReadiness 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness\nOther"
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/client.py` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_route53_recovery_readiness.client import Route53RecoveryReadinessClient
 
     session = Session()
     client: Route53RecoveryReadinessClient = session.client("route53-recovery-readiness")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     GetCellReadinessSummaryPaginator,
     GetReadinessCheckResourceStatusPaginator,
     GetReadinessCheckStatusPaginator,
@@ -49,14 +49,15 @@
     ListCellsResponseTypeDef,
     ListCrossAccountAuthorizationsResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListRulesResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     UpdateCellResponseTypeDef,
     UpdateReadinessCheckResponseTypeDef,
     UpdateRecoveryGroupResponseTypeDef,
     UpdateResourceSetResponseTypeDef,
 )
 
@@ -161,15 +162,15 @@
         """
 
     def create_resource_set(
         self,
         *,
         ResourceSetName: str,
         ResourceSetType: str,
-        Resources: Sequence[ResourceTypeDef],
+        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
         Tags: Mapping[str, str] = ...
     ) -> CreateResourceSetResponseTypeDef:
         """
         Creates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#create_resource_set)
@@ -437,15 +438,19 @@
         Updates a recovery group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_recovery_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#update_recovery_group)
         """
 
     def update_resource_set(
-        self, *, ResourceSetName: str, ResourceSetType: str, Resources: Sequence[ResourceTypeDef]
+        self,
+        *,
+        ResourceSetName: str,
+        ResourceSetType: str,
+        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]]
     ) -> UpdateResourceSetResponseTypeDef:
         """
         Updates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#update_resource_set)
         """
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/client.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_route53_recovery_readiness.client import Route53RecoveryReadinessClient
 
     session = Session()
     client: Route53RecoveryReadinessClient = session.client("route53-recovery-readiness")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     GetCellReadinessSummaryPaginator,
     GetReadinessCheckResourceStatusPaginator,
     GetReadinessCheckStatusPaginator,
@@ -49,14 +49,15 @@
     ListCellsResponseTypeDef,
     ListCrossAccountAuthorizationsResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListRulesResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     UpdateCellResponseTypeDef,
     UpdateReadinessCheckResponseTypeDef,
     UpdateRecoveryGroupResponseTypeDef,
     UpdateResourceSetResponseTypeDef,
 )
 
@@ -150,15 +151,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#create_recovery_group)
         """
     def create_resource_set(
         self,
         *,
         ResourceSetName: str,
         ResourceSetType: str,
-        Resources: Sequence[ResourceTypeDef],
+        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
         Tags: Mapping[str, str] = ...
     ) -> CreateResourceSetResponseTypeDef:
         """
         Creates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#create_resource_set)
@@ -398,15 +399,19 @@
         """
         Updates a recovery group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_recovery_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#update_recovery_group)
         """
     def update_resource_set(
-        self, *, ResourceSetName: str, ResourceSetType: str, Resources: Sequence[ResourceTypeDef]
+        self,
+        *,
+        ResourceSetName: str,
+        ResourceSetType: str,
+        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]]
     ) -> UpdateResourceSetResponseTypeDef:
         """
         Updates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/client/#update_resource_set)
         """
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/literals.py` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/literals.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/paginator.py` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/paginator.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/type_defs.py` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_route53_recovery_readiness.type_defs import CellOutputTypeDef
 
     data: CellOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import ReadinessType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -1101,15 +1101,15 @@
 )
 
 _RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": Sequence[ResourceTypeDef],
+        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
     },
 )
 _OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateResourceSetRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
@@ -1124,15 +1124,15 @@
 
 
 UpdateResourceSetRequestRequestTypeDef = TypedDict(
     "UpdateResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": Sequence[ResourceTypeDef],
+        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
     },
 )
 
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "NextToken": str,
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/type_defs.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_route53_recovery_readiness.type_defs import CellOutputTypeDef
 
     data: CellOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import ReadinessType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -1066,15 +1066,15 @@
 )
 
 _RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": Sequence[ResourceTypeDef],
+        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
     },
 )
 _OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateResourceSetRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
@@ -1087,15 +1087,15 @@
     pass
 
 UpdateResourceSetRequestRequestTypeDef = TypedDict(
     "UpdateResourceSetRequestRequestTypeDef",
     {
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": Sequence[ResourceTypeDef],
+        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
     },
 )
 
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "NextToken": str,
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-readiness
-Version: 1.28.15
-Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.15/setup.py` & `mypy-boto3-route53-recovery-readiness-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53-recovery-readiness",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_route53_recovery_readiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with"
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

