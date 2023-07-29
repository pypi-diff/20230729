# Comparing `tmp/mypy-boto3-migration-hub-refactor-spaces-1.28.15.tar.gz` & `tmp/mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.28.15.tar", last modified: Fri Jul 28 20:43:18 2023, max compression
+gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:43 2023, max compression
```

## Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15.tar` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.757522 mypy-boto3-migration-hub-refactor-spaces-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-07-28 20:43:18.757522 mypy-boto3-migration-hub-refactor-spaces-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.757522 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28978 2023-07-28 20:32:02.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28947 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.757522 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:18.757522 mypy-boto3-migration-hub-refactor-spaces-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:43.609297 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-29 10:03:43.601297 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:43.593297 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22886 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28978 2023-07-29 09:51:40.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28947 2023-07-29 09:51:40.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:43.601297 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-29 10:03:43.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:43.609297 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-29 09:51:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/LICENSE` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.28.15
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/README.md` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/README.md`

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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__init__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__main__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces\nOther"
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/client.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migration_hub_refactor_spaces.client import MigrationHubRefactorSpacesClient
 
     session = Session()
     client: MigrationHubRefactorSpacesClient = session.client("migration-hub-refactor-spaces")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     NetworkFabricTypeType,
     RouteActivationStateType,
     RouteTypeType,
@@ -51,47 +51,44 @@
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateRouteResponseTypeDef,
+    UriPathRouteInputOutputTypeDef,
     UriPathRouteInputTypeDef,
     UrlEndpointInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MigrationHubRefactorSpacesClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidResourcePolicyException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class MigrationHubRefactorSpacesClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/)
     """
 
     meta: ClientMeta
@@ -100,31 +97,28 @@
     def exceptions(self) -> Exceptions:
         """
         MigrationHubRefactorSpacesClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#close)
         """
-
     def create_application(
         self,
         *,
         EnvironmentIdentifier: str,
         Name: str,
         ProxyType: Literal["API_GATEWAY"],
         VpcId: str,
@@ -134,15 +128,14 @@
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_application)
         """
-
     def create_environment(
         self,
         *,
         Name: str,
         NetworkFabricType: NetworkFabricTypeType,
         ClientToken: str = ...,
         Description: str = ...,
@@ -150,34 +143,32 @@
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_environment)
         """
-
     def create_route(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteType: RouteTypeType,
         ServiceIdentifier: str,
         ClientToken: str = ...,
         DefaultRoute: DefaultRouteInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        UriPathRoute: UriPathRouteInputTypeDef = ...
+        UriPathRoute: Union[UriPathRouteInputTypeDef, UriPathRouteInputOutputTypeDef] = ...
     ) -> CreateRouteResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_route)
         """
-
     def create_service(
         self,
         *,
         ApplicationIdentifier: str,
         EndpointType: ServiceEndpointTypeType,
         EnvironmentIdentifier: str,
         Name: str,
@@ -190,154 +181,139 @@
     ) -> CreateServiceResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_service)
         """
-
     def delete_application(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str
     ) -> DeleteApplicationResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#delete_application)
         """
-
     def delete_environment(self, *, EnvironmentIdentifier: str) -> DeleteEnvironmentResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#delete_environment)
         """
-
     def delete_resource_policy(self, *, Identifier: str) -> Dict[str, Any]:
         """
         Deletes the resource policy set for the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#delete_resource_policy)
         """
-
     def delete_route(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, RouteIdentifier: str
     ) -> DeleteRouteResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#delete_route)
         """
-
     def delete_service(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, ServiceIdentifier: str
     ) -> DeleteServiceResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#delete_service)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#generate_presigned_url)
         """
-
     def get_application(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str
     ) -> GetApplicationResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_application)
         """
-
     def get_environment(self, *, EnvironmentIdentifier: str) -> GetEnvironmentResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_environment)
         """
-
     def get_resource_policy(self, *, Identifier: str) -> GetResourcePolicyResponseTypeDef:
         """
         Gets the resource-based permission policy that is set for the given environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_resource_policy)
         """
-
     def get_route(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, RouteIdentifier: str
     ) -> GetRouteResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_route)
         """
-
     def get_service(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, ServiceIdentifier: str
     ) -> GetServiceResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_service)
         """
-
     def list_applications(
         self, *, EnvironmentIdentifier: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces applications
         within an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_applications)
         """
-
     def list_environment_vpcs(
         self, *, EnvironmentIdentifier: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListEnvironmentVpcsResponseTypeDef:
         """
         Lists all Amazon Web Services Migration Hub Refactor Spaces service virtual
         private clouds (VPCs) that are part of the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_environment_vpcs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_environment_vpcs)
         """
-
     def list_environments(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListEnvironmentsResponseTypeDef:
         """
         Lists Amazon Web Services Migration Hub Refactor Spaces environments owned by a
         caller account or shared with the caller account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_environments)
         """
-
     def list_routes(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -345,15 +321,14 @@
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces routes within an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_routes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_routes)
         """
-
     def list_services(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -361,96 +336,86 @@
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces services within
         an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_services)
         """
-
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_tags_for_resource)
         """
-
     def put_resource_policy(self, *, Policy: str, ResourceArn: str) -> Dict[str, Any]:
         """
         Attaches a resource-based permission policy to the Amazon Web Services Migration
         Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#put_resource_policy)
         """
-
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Removes the tags of a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#untag_resource)
         """
-
     def update_route(
         self,
         *,
         ActivationState: RouteActivationStateType,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteIdentifier: str
     ) -> UpdateRouteResponseTypeDef:
         """
         Updates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.update_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#update_route)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_applications"]
     ) -> ListApplicationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_vpcs"]
     ) -> ListEnvironmentVpcsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environments"]
     ) -> ListEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_routes"]) -> ListRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/client.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migration_hub_refactor_spaces.client import MigrationHubRefactorSpacesClient
 
     session = Session()
     client: MigrationHubRefactorSpacesClient = session.client("migration-hub-refactor-spaces")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     NetworkFabricTypeType,
     RouteActivationStateType,
     RouteTypeType,
@@ -51,43 +51,48 @@
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateRouteResponseTypeDef,
+    UriPathRouteInputOutputTypeDef,
     UriPathRouteInputTypeDef,
     UrlEndpointInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("MigrationHubRefactorSpacesClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidResourcePolicyException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class MigrationHubRefactorSpacesClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/)
     """
 
     meta: ClientMeta
@@ -96,28 +101,31 @@
     def exceptions(self) -> Exceptions:
         """
         MigrationHubRefactorSpacesClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#close)
         """
+
     def create_application(
         self,
         *,
         EnvironmentIdentifier: str,
         Name: str,
         ProxyType: Literal["API_GATEWAY"],
         VpcId: str,
@@ -127,14 +135,15 @@
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_application)
         """
+
     def create_environment(
         self,
         *,
         Name: str,
         NetworkFabricType: NetworkFabricTypeType,
         ClientToken: str = ...,
         Description: str = ...,
@@ -142,32 +151,34 @@
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_environment)
         """
+
     def create_route(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteType: RouteTypeType,
         ServiceIdentifier: str,
         ClientToken: str = ...,
         DefaultRoute: DefaultRouteInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        UriPathRoute: UriPathRouteInputTypeDef = ...
+        UriPathRoute: Union[UriPathRouteInputTypeDef, UriPathRouteInputOutputTypeDef] = ...
     ) -> CreateRouteResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_route)
         """
+
     def create_service(
         self,
         *,
         ApplicationIdentifier: str,
         EndpointType: ServiceEndpointTypeType,
         EnvironmentIdentifier: str,
         Name: str,
@@ -180,139 +191,154 @@
     ) -> CreateServiceResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#create_service)
         """
+
     def delete_application(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str
     ) -> DeleteApplicationResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#delete_application)
         """
+
     def delete_environment(self, *, EnvironmentIdentifier: str) -> DeleteEnvironmentResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#delete_environment)
         """
+
     def delete_resource_policy(self, *, Identifier: str) -> Dict[str, Any]:
         """
         Deletes the resource policy set for the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#delete_resource_policy)
         """
+
     def delete_route(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, RouteIdentifier: str
     ) -> DeleteRouteResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#delete_route)
         """
+
     def delete_service(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, ServiceIdentifier: str
     ) -> DeleteServiceResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#delete_service)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#generate_presigned_url)
         """
+
     def get_application(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str
     ) -> GetApplicationResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_application)
         """
+
     def get_environment(self, *, EnvironmentIdentifier: str) -> GetEnvironmentResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_environment)
         """
+
     def get_resource_policy(self, *, Identifier: str) -> GetResourcePolicyResponseTypeDef:
         """
         Gets the resource-based permission policy that is set for the given environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_resource_policy)
         """
+
     def get_route(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, RouteIdentifier: str
     ) -> GetRouteResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_route)
         """
+
     def get_service(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, ServiceIdentifier: str
     ) -> GetServiceResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_service)
         """
+
     def list_applications(
         self, *, EnvironmentIdentifier: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces applications
         within an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_applications)
         """
+
     def list_environment_vpcs(
         self, *, EnvironmentIdentifier: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListEnvironmentVpcsResponseTypeDef:
         """
         Lists all Amazon Web Services Migration Hub Refactor Spaces service virtual
         private clouds (VPCs) that are part of the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_environment_vpcs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_environment_vpcs)
         """
+
     def list_environments(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListEnvironmentsResponseTypeDef:
         """
         Lists Amazon Web Services Migration Hub Refactor Spaces environments owned by a
         caller account or shared with the caller account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_environments)
         """
+
     def list_routes(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -320,14 +346,15 @@
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces routes within an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_routes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_routes)
         """
+
     def list_services(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -335,86 +362,96 @@
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces services within
         an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_services)
         """
+
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#list_tags_for_resource)
         """
+
     def put_resource_policy(self, *, Policy: str, ResourceArn: str) -> Dict[str, Any]:
         """
         Attaches a resource-based permission policy to the Amazon Web Services Migration
         Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#put_resource_policy)
         """
+
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Removes the tags of a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#untag_resource)
         """
+
     def update_route(
         self,
         *,
         ActivationState: RouteActivationStateType,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteIdentifier: str
     ) -> UpdateRouteResponseTypeDef:
         """
         Updates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.update_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#update_route)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_applications"]
     ) -> ListApplicationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_vpcs"]
     ) -> ListEnvironmentVpcsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environments"]
     ) -> ListEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_routes"]) -> ListRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/literals.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/literals.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/paginator.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/type_defs.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.28.15
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.15/setup.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migration-hub-refactor-spaces",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_migration_hub_refactor_spaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with"
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

