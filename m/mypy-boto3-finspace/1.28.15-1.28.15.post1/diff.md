# Comparing `tmp/mypy-boto3-finspace-1.28.15.tar.gz` & `tmp/mypy-boto3-finspace-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-1.28.15.tar", last modified: Fri Jul 28 20:42:49 2023, max compression
+gzip compressed data, was "mypy-boto3-finspace-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:09 2023, max compression
```

## Comparing `mypy-boto3-finspace-1.28.15.tar` & `mypy-boto3-finspace-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.257116 mypy-boto3-finspace-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-07-28 20:42:49.257116 mypy-boto3-finspace-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.257116 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36402 2023-07-28 20:25:48.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36362 2023-07-28 20:25:48.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.257116 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:49.257116 mypy-boto3-finspace-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.085153 mypy-boto3-finspace-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-29 10:03:09.077153 mypy-boto3-finspace-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.073153 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25141 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25099 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36543 2023-07-29 09:45:21.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36503 2023-07-29 09:45:19.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.077153 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:09.085153 mypy-boto3-finspace-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-finspace-1.28.15/LICENSE` & `mypy-boto3-finspace-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15/PKG-INFO` & `mypy-boto3-finspace-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.28.15
-Summary: Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-finspace-1.28.15/README.md` & `mypy-boto3-finspace-1.28.15.post1/README.md`

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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__init__.py` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__init__.pyi` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__main__.py` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.finspace 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.finspace 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
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

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/client.py` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_finspace.client import finspaceClient
 
     session = Session()
     client: finspaceClient = session.client("finspace")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FederationModeType, KxAzModeType, KxClusterTypeType
 from .paginator import ListKxEnvironmentsPaginator
 from .type_defs import (
     AutoScalingConfigurationTypeDef,
@@ -28,24 +28,26 @@
     CreateEnvironmentResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
+    FederationParametersOutputTypeDef,
     FederationParametersTypeDef,
     GetEnvironmentResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxClusterResponseTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     GetKxUserResponseTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
+    KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxClustersResponseTypeDef,
     ListKxDatabasesResponseTypeDef,
@@ -55,48 +57,45 @@
     SuperuserParametersTypeDef,
     TransitGatewayConfigurationTypeDef,
     UpdateEnvironmentResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     UpdateKxUserResponseTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("finspaceClient",)
 
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
     InvalidRequestException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class finspaceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/)
     """
 
     meta: ClientMeta
@@ -105,95 +104,93 @@
     def exceptions(self) -> Exceptions:
         """
         finspaceClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#close)
         """
-
     def create_environment(
         self,
         *,
         name: str,
         description: str = ...,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersTypeDef = ...,
+        federationParameters: Union[
+            FederationParametersTypeDef, FederationParametersOutputTypeDef
+        ] = ...,
         superuserParameters: SuperuserParametersTypeDef = ...,
         dataBundles: Sequence[str] = ...
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Create a new FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_environment)
         """
-
     def create_kx_changeset(
         self,
         *,
         environmentId: str,
         databaseName: str,
         changeRequests: Sequence[ChangeRequestTypeDef],
         clientToken: str
     ) -> CreateKxChangesetResponseTypeDef:
         """
         Creates a changeset for a kdb database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_changeset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_kx_changeset)
         """
-
     def create_kx_cluster(
         self,
         *,
         environmentId: str,
         clusterName: str,
         clusterType: KxClusterTypeType,
         capacityConfiguration: CapacityConfigurationTypeDef,
         releaseLabel: str,
         azMode: KxAzModeType,
         clientToken: str = ...,
-        databases: Sequence[KxDatabaseConfigurationTypeDef] = ...,
+        databases: Sequence[
+            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
+        ] = ...,
         cacheStorageConfigurations: Sequence[KxCacheStorageConfigurationTypeDef] = ...,
         autoScalingConfiguration: AutoScalingConfigurationTypeDef = ...,
         clusterDescription: str = ...,
-        vpcConfiguration: VpcConfigurationTypeDef = ...,
+        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
         code: CodeConfigurationTypeDef = ...,
         executionRole: str = ...,
         savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,
         availabilityZoneId: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateKxClusterResponseTypeDef:
         """
         Creates a new kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_kx_cluster)
         """
-
     def create_kx_database(
         self,
         *,
         environmentId: str,
         databaseName: str,
         clientToken: str,
         description: str = ...,
@@ -201,15 +198,14 @@
     ) -> CreateKxDatabaseResponseTypeDef:
         """
         Creates a new kdb database in the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_kx_database)
         """
-
     def create_kx_environment(
         self,
         *,
         name: str,
         kmsKeyId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...,
@@ -217,15 +213,14 @@
     ) -> CreateKxEnvironmentResponseTypeDef:
         """
         Creates a managed kdb environment for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_kx_environment)
         """
-
     def create_kx_user(
         self,
         *,
         environmentId: str,
         userName: str,
         iamRole: str,
         tags: Mapping[str, str] = ...,
@@ -233,288 +228,264 @@
     ) -> CreateKxUserResponseTypeDef:
         """
         Creates a user in FinSpace kdb environment with an associated IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_kx_user)
         """
-
     def delete_environment(self, *, environmentId: str) -> Dict[str, Any]:
         """
         Delete an FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#delete_environment)
         """
-
     def delete_kx_cluster(
         self, *, environmentId: str, clusterName: str, clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#delete_kx_cluster)
         """
-
     def delete_kx_database(
         self, *, environmentId: str, databaseName: str, clientToken: str
     ) -> Dict[str, Any]:
         """
         Deletes the specified database and all of its associated data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#delete_kx_database)
         """
-
     def delete_kx_environment(self, *, environmentId: str) -> Dict[str, Any]:
         """
         Deletes the kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#delete_kx_environment)
         """
-
     def delete_kx_user(self, *, userName: str, environmentId: str) -> Dict[str, Any]:
         """
         Deletes a user in the specified kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#delete_kx_user)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#generate_presigned_url)
         """
-
     def get_environment(self, *, environmentId: str) -> GetEnvironmentResponseTypeDef:
         """
         Returns the FinSpace environment object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_environment)
         """
-
     def get_kx_changeset(
         self, *, environmentId: str, databaseName: str, changesetId: str
     ) -> GetKxChangesetResponseTypeDef:
         """
         Returns information about a kdb changeset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_changeset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_changeset)
         """
-
     def get_kx_cluster(
         self, *, environmentId: str, clusterName: str
     ) -> GetKxClusterResponseTypeDef:
         """
         Retrieves information about a kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_cluster)
         """
-
     def get_kx_connection_string(
         self, *, userArn: str, environmentId: str, clusterName: str
     ) -> GetKxConnectionStringResponseTypeDef:
         """
         Retrieves a connection string for a user to connect to a kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_connection_string)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_connection_string)
         """
-
     def get_kx_database(
         self, *, environmentId: str, databaseName: str
     ) -> GetKxDatabaseResponseTypeDef:
         """
         Returns database information for the specified environment ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_database)
         """
-
     def get_kx_environment(self, *, environmentId: str) -> GetKxEnvironmentResponseTypeDef:
         """
         Retrieves all the information for the specified kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_environment)
         """
-
     def get_kx_user(self, *, userName: str, environmentId: str) -> GetKxUserResponseTypeDef:
         """
         Retrieves information about the specified kdb user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_user)
         """
-
     def list_environments(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListEnvironmentsResponseTypeDef:
         """
         A list of all of your FinSpace environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_environments)
         """
-
     def list_kx_changesets(
         self, *, environmentId: str, databaseName: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListKxChangesetsResponseTypeDef:
         """
         Returns a list of all the changesets for a database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_changesets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_changesets)
         """
-
     def list_kx_cluster_nodes(
         self, *, environmentId: str, clusterName: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListKxClusterNodesResponseTypeDef:
         """
         Lists all the nodes in a kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_cluster_nodes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_cluster_nodes)
         """
-
     def list_kx_clusters(
         self,
         *,
         environmentId: str,
         clusterType: KxClusterTypeType = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListKxClustersResponseTypeDef:
         """
         Returns a list of clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_clusters)
         """
-
     def list_kx_databases(
         self, *, environmentId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListKxDatabasesResponseTypeDef:
         """
         Returns a list of all the databases in the kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_databases)
         """
-
     def list_kx_environments(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListKxEnvironmentsResponseTypeDef:
         """
         Returns a list of kdb environments created in an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_environments)
         """
-
     def list_kx_users(
         self, *, environmentId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListKxUsersResponseTypeDef:
         """
         Lists all the users in a kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_users)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         A list of all tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_tags_for_resource)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds metadata tags to a FinSpace resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes metadata tags from a FinSpace resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#untag_resource)
         """
-
     def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersTypeDef = ...
+        federationParameters: Union[
+            FederationParametersTypeDef, FederationParametersOutputTypeDef
+        ] = ...
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Update your FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_environment)
         """
-
     def update_kx_cluster_databases(
         self,
         *,
         environmentId: str,
         clusterName: str,
-        databases: Sequence[KxDatabaseConfigurationTypeDef],
+        databases: Sequence[
+            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
+        ],
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the databases mounted on a kdb cluster, which includes the `changesetId`
         and all the dbPaths to be cached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_kx_cluster_databases)
         """
-
     def update_kx_database(
         self, *, environmentId: str, databaseName: str, clientToken: str, description: str = ...
     ) -> UpdateKxDatabaseResponseTypeDef:
         """
         Updates information for the given kdb database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_kx_database)
         """
-
     def update_kx_environment(
         self, *, environmentId: str, name: str = ..., description: str = ..., clientToken: str = ...
     ) -> UpdateKxEnvironmentResponseTypeDef:
         """
         Updates information for the given kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_kx_environment)
         """
-
     def update_kx_environment_network(
         self,
         *,
         environmentId: str,
         transitGatewayConfiguration: TransitGatewayConfigurationTypeDef = ...,
         customDNSConfiguration: Sequence[CustomDNSServerTypeDef] = ...,
         clientToken: str = ...
@@ -522,25 +493,23 @@
         """
         Updates environment network to connect to your internal network by using a
         transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_environment_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_kx_environment_network)
         """
-
     def update_kx_user(
         self, *, environmentId: str, userName: str, iamRole: str, clientToken: str = ...
     ) -> UpdateKxUserResponseTypeDef:
         """
         Updates the user details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_kx_user)
         """
-
     def get_paginator(
         self, operation_name: Literal["list_kx_environments"]
     ) -> ListKxEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/client.pyi` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_finspace.client import finspaceClient
 
     session = Session()
     client: finspaceClient = session.client("finspace")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FederationModeType, KxAzModeType, KxClusterTypeType
 from .paginator import ListKxEnvironmentsPaginator
 from .type_defs import (
     AutoScalingConfigurationTypeDef,
@@ -28,24 +28,26 @@
     CreateEnvironmentResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
+    FederationParametersOutputTypeDef,
     FederationParametersTypeDef,
     GetEnvironmentResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxClusterResponseTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     GetKxUserResponseTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
+    KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxClustersResponseTypeDef,
     ListKxDatabasesResponseTypeDef,
@@ -55,44 +57,49 @@
     SuperuserParametersTypeDef,
     TransitGatewayConfigurationTypeDef,
     UpdateEnvironmentResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     UpdateKxUserResponseTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("finspaceClient",)
 
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
     InvalidRequestException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class finspaceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/)
     """
 
     meta: ClientMeta
@@ -101,89 +108,99 @@
     def exceptions(self) -> Exceptions:
         """
         finspaceClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#close)
         """
+
     def create_environment(
         self,
         *,
         name: str,
         description: str = ...,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersTypeDef = ...,
+        federationParameters: Union[
+            FederationParametersTypeDef, FederationParametersOutputTypeDef
+        ] = ...,
         superuserParameters: SuperuserParametersTypeDef = ...,
         dataBundles: Sequence[str] = ...
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Create a new FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_environment)
         """
+
     def create_kx_changeset(
         self,
         *,
         environmentId: str,
         databaseName: str,
         changeRequests: Sequence[ChangeRequestTypeDef],
         clientToken: str
     ) -> CreateKxChangesetResponseTypeDef:
         """
         Creates a changeset for a kdb database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_changeset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_kx_changeset)
         """
+
     def create_kx_cluster(
         self,
         *,
         environmentId: str,
         clusterName: str,
         clusterType: KxClusterTypeType,
         capacityConfiguration: CapacityConfigurationTypeDef,
         releaseLabel: str,
         azMode: KxAzModeType,
         clientToken: str = ...,
-        databases: Sequence[KxDatabaseConfigurationTypeDef] = ...,
+        databases: Sequence[
+            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
+        ] = ...,
         cacheStorageConfigurations: Sequence[KxCacheStorageConfigurationTypeDef] = ...,
         autoScalingConfiguration: AutoScalingConfigurationTypeDef = ...,
         clusterDescription: str = ...,
-        vpcConfiguration: VpcConfigurationTypeDef = ...,
+        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
         code: CodeConfigurationTypeDef = ...,
         executionRole: str = ...,
         savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,
         availabilityZoneId: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateKxClusterResponseTypeDef:
         """
         Creates a new kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_kx_cluster)
         """
+
     def create_kx_database(
         self,
         *,
         environmentId: str,
         databaseName: str,
         clientToken: str,
         description: str = ...,
@@ -191,14 +208,15 @@
     ) -> CreateKxDatabaseResponseTypeDef:
         """
         Creates a new kdb database in the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_kx_database)
         """
+
     def create_kx_environment(
         self,
         *,
         name: str,
         kmsKeyId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...,
@@ -206,14 +224,15 @@
     ) -> CreateKxEnvironmentResponseTypeDef:
         """
         Creates a managed kdb environment for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_kx_environment)
         """
+
     def create_kx_user(
         self,
         *,
         environmentId: str,
         userName: str,
         iamRole: str,
         tags: Mapping[str, str] = ...,
@@ -221,260 +240,292 @@
     ) -> CreateKxUserResponseTypeDef:
         """
         Creates a user in FinSpace kdb environment with an associated IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#create_kx_user)
         """
+
     def delete_environment(self, *, environmentId: str) -> Dict[str, Any]:
         """
         Delete an FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#delete_environment)
         """
+
     def delete_kx_cluster(
         self, *, environmentId: str, clusterName: str, clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#delete_kx_cluster)
         """
+
     def delete_kx_database(
         self, *, environmentId: str, databaseName: str, clientToken: str
     ) -> Dict[str, Any]:
         """
         Deletes the specified database and all of its associated data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#delete_kx_database)
         """
+
     def delete_kx_environment(self, *, environmentId: str) -> Dict[str, Any]:
         """
         Deletes the kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#delete_kx_environment)
         """
+
     def delete_kx_user(self, *, userName: str, environmentId: str) -> Dict[str, Any]:
         """
         Deletes a user in the specified kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.delete_kx_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#delete_kx_user)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#generate_presigned_url)
         """
+
     def get_environment(self, *, environmentId: str) -> GetEnvironmentResponseTypeDef:
         """
         Returns the FinSpace environment object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_environment)
         """
+
     def get_kx_changeset(
         self, *, environmentId: str, databaseName: str, changesetId: str
     ) -> GetKxChangesetResponseTypeDef:
         """
         Returns information about a kdb changeset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_changeset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_changeset)
         """
+
     def get_kx_cluster(
         self, *, environmentId: str, clusterName: str
     ) -> GetKxClusterResponseTypeDef:
         """
         Retrieves information about a kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_cluster)
         """
+
     def get_kx_connection_string(
         self, *, userArn: str, environmentId: str, clusterName: str
     ) -> GetKxConnectionStringResponseTypeDef:
         """
         Retrieves a connection string for a user to connect to a kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_connection_string)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_connection_string)
         """
+
     def get_kx_database(
         self, *, environmentId: str, databaseName: str
     ) -> GetKxDatabaseResponseTypeDef:
         """
         Returns database information for the specified environment ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_database)
         """
+
     def get_kx_environment(self, *, environmentId: str) -> GetKxEnvironmentResponseTypeDef:
         """
         Retrieves all the information for the specified kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_environment)
         """
+
     def get_kx_user(self, *, userName: str, environmentId: str) -> GetKxUserResponseTypeDef:
         """
         Retrieves information about the specified kdb user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_kx_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_kx_user)
         """
+
     def list_environments(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListEnvironmentsResponseTypeDef:
         """
         A list of all of your FinSpace environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_environments)
         """
+
     def list_kx_changesets(
         self, *, environmentId: str, databaseName: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListKxChangesetsResponseTypeDef:
         """
         Returns a list of all the changesets for a database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_changesets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_changesets)
         """
+
     def list_kx_cluster_nodes(
         self, *, environmentId: str, clusterName: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListKxClusterNodesResponseTypeDef:
         """
         Lists all the nodes in a kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_cluster_nodes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_cluster_nodes)
         """
+
     def list_kx_clusters(
         self,
         *,
         environmentId: str,
         clusterType: KxClusterTypeType = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListKxClustersResponseTypeDef:
         """
         Returns a list of clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_clusters)
         """
+
     def list_kx_databases(
         self, *, environmentId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListKxDatabasesResponseTypeDef:
         """
         Returns a list of all the databases in the kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_databases)
         """
+
     def list_kx_environments(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListKxEnvironmentsResponseTypeDef:
         """
         Returns a list of kdb environments created in an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_environments)
         """
+
     def list_kx_users(
         self, *, environmentId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListKxUsersResponseTypeDef:
         """
         Lists all the users in a kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_kx_users)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         A list of all tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#list_tags_for_resource)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds metadata tags to a FinSpace resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes metadata tags from a FinSpace resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#untag_resource)
         """
+
     def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersTypeDef = ...
+        federationParameters: Union[
+            FederationParametersTypeDef, FederationParametersOutputTypeDef
+        ] = ...
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Update your FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_environment)
         """
+
     def update_kx_cluster_databases(
         self,
         *,
         environmentId: str,
         clusterName: str,
-        databases: Sequence[KxDatabaseConfigurationTypeDef],
+        databases: Sequence[
+            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
+        ],
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the databases mounted on a kdb cluster, which includes the `changesetId`
         and all the dbPaths to be cached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_kx_cluster_databases)
         """
+
     def update_kx_database(
         self, *, environmentId: str, databaseName: str, clientToken: str, description: str = ...
     ) -> UpdateKxDatabaseResponseTypeDef:
         """
         Updates information for the given kdb database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_kx_database)
         """
+
     def update_kx_environment(
         self, *, environmentId: str, name: str = ..., description: str = ..., clientToken: str = ...
     ) -> UpdateKxEnvironmentResponseTypeDef:
         """
         Updates information for the given kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_kx_environment)
         """
+
     def update_kx_environment_network(
         self,
         *,
         environmentId: str,
         transitGatewayConfiguration: TransitGatewayConfigurationTypeDef = ...,
         customDNSConfiguration: Sequence[CustomDNSServerTypeDef] = ...,
         clientToken: str = ...
@@ -482,23 +533,25 @@
         """
         Updates environment network to connect to your internal network by using a
         transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_environment_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_kx_environment_network)
         """
+
     def update_kx_user(
         self, *, environmentId: str, userName: str, iamRole: str, clientToken: str = ...
     ) -> UpdateKxUserResponseTypeDef:
         """
         Updates the user details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_kx_user)
         """
+
     def get_paginator(
         self, operation_name: Literal["list_kx_environments"]
     ) -> ListKxEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/literals.py` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/literals.pyi` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/paginator.py` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/paginator.pyi` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/type_defs.py` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_finspace.type_defs import AutoScalingConfigurationTypeDef
 
     data: AutoScalingConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ChangesetStatusType,
     ChangeTypeType,
     EnvironmentStatusType,
     ErrorDetailsType,
     FederationModeType,
@@ -1336,15 +1336,17 @@
         "azMode": KxAzModeType,
     },
 )
 _OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
     "_OptionalCreateKxClusterRequestRequestTypeDef",
     {
         "clientToken": str,
-        "databases": Sequence[KxDatabaseConfigurationTypeDef],
+        "databases": Sequence[
+            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
+        ],
         "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
         "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
         "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
@@ -1364,15 +1366,17 @@
 
 
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
-        "databases": Sequence[KxDatabaseConfigurationTypeDef],
+        "databases": Sequence[
+            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
+        ],
     },
 )
 _OptionalUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "clientToken": str,
     },
```

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/type_defs.pyi` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_finspace.type_defs import AutoScalingConfigurationTypeDef
 
     data: AutoScalingConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ChangesetStatusType,
     ChangeTypeType,
     EnvironmentStatusType,
     ErrorDetailsType,
     FederationModeType,
@@ -1299,15 +1299,17 @@
         "azMode": KxAzModeType,
     },
 )
 _OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
     "_OptionalCreateKxClusterRequestRequestTypeDef",
     {
         "clientToken": str,
-        "databases": Sequence[KxDatabaseConfigurationTypeDef],
+        "databases": Sequence[
+            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
+        ],
         "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
         "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
         "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
@@ -1325,15 +1327,17 @@
     pass
 
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
-        "databases": Sequence[KxDatabaseConfigurationTypeDef],
+        "databases": Sequence[
+            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
+        ],
     },
 )
 _OptionalUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "clientToken": str,
     },
```

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/PKG-INFO` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.28.15
-Summary: Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/SOURCES.txt` & `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15/setup.py` & `mypy-boto3-finspace-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder"
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

