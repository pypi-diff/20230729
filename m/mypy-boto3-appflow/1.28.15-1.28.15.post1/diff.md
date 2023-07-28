# Comparing `tmp/mypy-boto3-appflow-1.28.15.tar.gz` & `tmp/mypy-boto3-appflow-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appflow-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
+gzip compressed data, was "mypy-boto3-appflow-1.28.15.post1.tar", last modified: Fri Jul 28 23:40:22 2023, max compression
```

## Comparing `mypy-boto3-appflow-1.28.15.tar` & `mypy-boto3-appflow-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.244654 mypy-boto3-appflow-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20709 2023-07-28 20:42:16.244654 mypy-boto3-appflow-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.240654 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19559 2023-07-28 20:19:18.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-28 20:19:18.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-07-28 20:19:19.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-07-28 20:19:18.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85991 2023-07-28 20:19:21.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85859 2023-07-28 20:19:20.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.244654 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20709 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.244654 mypy-boto3-appflow-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-28 23:40:21.987957 mypy-boto3-appflow-1.28.15.post1/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20715 2023-07-28 23:40:21.987957 mypy-boto3-appflow-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19222 2023-07-28 23:39:43.000000 mypy-boto3-appflow-1.28.15.post1/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-28 23:40:21.987957 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      373 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      372 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      919 2023-07-28 23:39:43.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20024 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19992 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18437 2023-07-28 23:35:35.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18435 2023-07-28 23:35:35.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    86173 2023-07-28 23:39:46.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    86041 2023-07-28 23:35:37.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2023-07-28 23:39:43.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-28 23:40:21.987957 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20715 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      615 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       19 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-07-28 23:40:21.987957 mypy-boto3-appflow-1.28.15.post1/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2002 2023-07-28 23:39:43.000000 mypy-boto3-appflow-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-appflow-1.28.15/LICENSE` & `mypy-boto3-appflow-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15/PKG-INFO` & `mypy-boto3-appflow-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.28.15
-Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
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
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appflow-1.28.15/README.md` & `mypy-boto3-appflow-1.28.15.post1/README.md`

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
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/__main__.py` & `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Appflow 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Appflow 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
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

### Comparing `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/client.py` & `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appflow.client import AppflowClient
 
     session = Session()
     client: AppflowClient = session.client("appflow")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConnectionModeType, ConnectorTypeType
 from .type_defs import (
     CancelFlowExecutionsResponseTypeDef,
     ConnectorProfileConfigTypeDef,
@@ -27,62 +27,62 @@
     CreateFlowResponseTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     DescribeFlowResponseTypeDef,
+    DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListFlowsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetadataCatalogConfigTypeDef,
     RegisterConnectorResponseTypeDef,
+    SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
     StartFlowResponseTypeDef,
     StopFlowResponseTypeDef,
+    TaskOutputTypeDef,
     TaskTypeDef,
+    TriggerConfigOutputTypeDef,
     TriggerConfigTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppflowClient",)
 
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
     ConnectorAuthenticationException: Type[BotocoreClientError]
     ConnectorServerException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class AppflowClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/)
     """
 
     meta: ClientMeta
@@ -91,41 +91,37 @@
     def exceptions(self) -> Exceptions:
         """
         AppflowClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#can_paginate)
         """
-
     def cancel_flow_executions(
         self, *, flowName: str, executionIds: Sequence[str] = ...
     ) -> CancelFlowExecutionsResponseTypeDef:
         """
         Cancels active runs for a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.cancel_flow_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#cancel_flow_executions)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#close)
         """
-
     def create_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectorType: ConnectorTypeType,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
@@ -136,65 +132,62 @@
         """
         Creates a new connector profile associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_connector_profile)
         """
-
     def create_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigTypeDef,
-        sourceFlowConfig: SourceFlowConfigTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
-        tasks: Sequence[TaskTypeDef],
+        triggerConfig: Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef],
+        sourceFlowConfig: Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef],
+        destinationFlowConfigList: Sequence[
+            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
+        ],
+        tasks: Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> CreateFlowResponseTypeDef:
         """
         Enables your application to create a new flow using Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_flow)
         """
-
     def delete_connector_profile(
         self, *, connectorProfileName: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Enables you to delete an existing connector profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_connector_profile)
         """
-
     def delete_flow(self, *, flowName: str, forceDelete: bool = ...) -> Dict[str, Any]:
         """
         Enables your application to delete an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_flow)
         """
-
     def describe_connector(
         self, *, connectorType: ConnectorTypeType, connectorLabel: str = ...
     ) -> DescribeConnectorResponseTypeDef:
         """
         Describes the given custom connector registered in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector)
         """
-
     def describe_connector_entity(
         self,
         *,
         connectorEntityName: str,
         connectorType: ConnectorTypeType = ...,
         connectorProfileName: str = ...,
         apiVersion: str = ...
@@ -202,15 +195,14 @@
         """
         Provides details regarding the entity used with the connector, with a
         description of the data model for each field in that entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_entity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_entity)
         """
-
     def describe_connector_profiles(
         self,
         *,
         connectorProfileNames: Sequence[str] = ...,
         connectorType: ConnectorTypeType = ...,
         connectorLabel: str = ...,
         maxResults: int = ...,
@@ -219,61 +211,56 @@
         """
         Returns a list of `connector-profile` details matching the provided `connector-
         profile` names and `connector-types`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_profiles)
         """
-
     def describe_connectors(
         self,
         *,
         connectorTypes: Sequence[ConnectorTypeType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeConnectorsResponseTypeDef:
         """
         Describes the connectors vended by Amazon AppFlow for specified connector types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connectors)
         """
-
     def describe_flow(self, *, flowName: str) -> DescribeFlowResponseTypeDef:
         """
         Provides a description of the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow)
         """
-
     def describe_flow_execution_records(
         self, *, flowName: str, maxResults: int = ..., nextToken: str = ...
     ) -> DescribeFlowExecutionRecordsResponseTypeDef:
         """
         Fetches the execution history of the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow_execution_records)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow_execution_records)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#generate_presigned_url)
         """
-
     def list_connector_entities(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         entitiesPath: str = ...,
         apiVersion: str = ...,
@@ -282,44 +269,40 @@
     ) -> ListConnectorEntitiesResponseTypeDef:
         """
         Returns the list of available connector entities supported by Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connector_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connector_entities)
         """
-
     def list_connectors(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListConnectorsResponseTypeDef:
         """
         Returns the list of all registered custom connectors in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connectors)
         """
-
     def list_flows(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListFlowsResponseTypeDef:
         """
         Lists all of the flows associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_flows)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves the tags that are associated with a specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_tags_for_resource)
         """
-
     def register_connector(
         self,
         *,
         connectorLabel: str = ...,
         description: str = ...,
         connectorProvisioningType: Literal["LAMBDA"] = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
@@ -327,15 +310,14 @@
     ) -> RegisterConnectorResponseTypeDef:
         """
         Registers a new custom connector with your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.register_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#register_connector)
         """
-
     def reset_connector_metadata_cache(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         connectorEntityName: str = ...,
         entitiesPath: str = ...,
@@ -344,96 +326,90 @@
         """
         Resets metadata about your connector entities that Amazon AppFlow stored in its
         cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.reset_connector_metadata_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#reset_connector_metadata_cache)
         """
-
     def start_flow(self, *, flowName: str, clientToken: str = ...) -> StartFlowResponseTypeDef:
         """
         Activates an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.start_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#start_flow)
         """
-
     def stop_flow(self, *, flowName: str) -> StopFlowResponseTypeDef:
         """
         Deactivates the existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.stop_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#stop_flow)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Applies a tag to the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#tag_resource)
         """
-
     def unregister_connector(
         self, *, connectorLabel: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Unregisters the custom connector registered in your account that matches the
         connector label provided in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.unregister_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#unregister_connector)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#untag_resource)
         """
-
     def update_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
         clientToken: str = ...
     ) -> UpdateConnectorProfileResponseTypeDef:
         """
         Updates a given connector profile associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_profile)
         """
-
     def update_connector_registration(
         self,
         *,
         connectorLabel: str,
         description: str = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateConnectorRegistrationResponseTypeDef:
         """
         Updates a custom connector that you've previously registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_registration)
         """
-
     def update_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigTypeDef,
-        sourceFlowConfig: SourceFlowConfigTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
-        tasks: Sequence[TaskTypeDef],
+        triggerConfig: Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef],
+        sourceFlowConfig: Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef],
+        destinationFlowConfigList: Sequence[
+            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
+        ],
+        tasks: Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
         description: str = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
```

### Comparing `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/client.pyi` & `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appflow.client import AppflowClient
 
     session = Session()
     client: AppflowClient = session.client("appflow")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConnectionModeType, ConnectorTypeType
 from .type_defs import (
     CancelFlowExecutionsResponseTypeDef,
     ConnectorProfileConfigTypeDef,
@@ -27,58 +27,66 @@
     CreateFlowResponseTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     DescribeFlowResponseTypeDef,
+    DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListFlowsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetadataCatalogConfigTypeDef,
     RegisterConnectorResponseTypeDef,
+    SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
     StartFlowResponseTypeDef,
     StopFlowResponseTypeDef,
+    TaskOutputTypeDef,
     TaskTypeDef,
+    TriggerConfigOutputTypeDef,
     TriggerConfigTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("AppflowClient",)
 
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
     ConnectorAuthenticationException: Type[BotocoreClientError]
     ConnectorServerException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class AppflowClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/)
     """
 
     meta: ClientMeta
@@ -87,37 +95,41 @@
     def exceptions(self) -> Exceptions:
         """
         AppflowClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#can_paginate)
         """
+
     def cancel_flow_executions(
         self, *, flowName: str, executionIds: Sequence[str] = ...
     ) -> CancelFlowExecutionsResponseTypeDef:
         """
         Cancels active runs for a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.cancel_flow_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#cancel_flow_executions)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#close)
         """
+
     def create_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectorType: ConnectorTypeType,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
@@ -128,60 +140,67 @@
         """
         Creates a new connector profile associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_connector_profile)
         """
+
     def create_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigTypeDef,
-        sourceFlowConfig: SourceFlowConfigTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
-        tasks: Sequence[TaskTypeDef],
+        triggerConfig: Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef],
+        sourceFlowConfig: Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef],
+        destinationFlowConfigList: Sequence[
+            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
+        ],
+        tasks: Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> CreateFlowResponseTypeDef:
         """
         Enables your application to create a new flow using Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_flow)
         """
+
     def delete_connector_profile(
         self, *, connectorProfileName: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Enables you to delete an existing connector profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_connector_profile)
         """
+
     def delete_flow(self, *, flowName: str, forceDelete: bool = ...) -> Dict[str, Any]:
         """
         Enables your application to delete an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_flow)
         """
+
     def describe_connector(
         self, *, connectorType: ConnectorTypeType, connectorLabel: str = ...
     ) -> DescribeConnectorResponseTypeDef:
         """
         Describes the given custom connector registered in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector)
         """
+
     def describe_connector_entity(
         self,
         *,
         connectorEntityName: str,
         connectorType: ConnectorTypeType = ...,
         connectorProfileName: str = ...,
         apiVersion: str = ...
@@ -189,14 +208,15 @@
         """
         Provides details regarding the entity used with the connector, with a
         description of the data model for each field in that entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_entity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_entity)
         """
+
     def describe_connector_profiles(
         self,
         *,
         connectorProfileNames: Sequence[str] = ...,
         connectorType: ConnectorTypeType = ...,
         connectorLabel: str = ...,
         maxResults: int = ...,
@@ -205,56 +225,61 @@
         """
         Returns a list of `connector-profile` details matching the provided `connector-
         profile` names and `connector-types`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_profiles)
         """
+
     def describe_connectors(
         self,
         *,
         connectorTypes: Sequence[ConnectorTypeType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeConnectorsResponseTypeDef:
         """
         Describes the connectors vended by Amazon AppFlow for specified connector types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connectors)
         """
+
     def describe_flow(self, *, flowName: str) -> DescribeFlowResponseTypeDef:
         """
         Provides a description of the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow)
         """
+
     def describe_flow_execution_records(
         self, *, flowName: str, maxResults: int = ..., nextToken: str = ...
     ) -> DescribeFlowExecutionRecordsResponseTypeDef:
         """
         Fetches the execution history of the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow_execution_records)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow_execution_records)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#generate_presigned_url)
         """
+
     def list_connector_entities(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         entitiesPath: str = ...,
         apiVersion: str = ...,
@@ -263,40 +288,44 @@
     ) -> ListConnectorEntitiesResponseTypeDef:
         """
         Returns the list of available connector entities supported by Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connector_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connector_entities)
         """
+
     def list_connectors(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListConnectorsResponseTypeDef:
         """
         Returns the list of all registered custom connectors in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connectors)
         """
+
     def list_flows(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListFlowsResponseTypeDef:
         """
         Lists all of the flows associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_flows)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves the tags that are associated with a specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_tags_for_resource)
         """
+
     def register_connector(
         self,
         *,
         connectorLabel: str = ...,
         description: str = ...,
         connectorProvisioningType: Literal["LAMBDA"] = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
@@ -304,14 +333,15 @@
     ) -> RegisterConnectorResponseTypeDef:
         """
         Registers a new custom connector with your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.register_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#register_connector)
         """
+
     def reset_connector_metadata_cache(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         connectorEntityName: str = ...,
         entitiesPath: str = ...,
@@ -320,88 +350,98 @@
         """
         Resets metadata about your connector entities that Amazon AppFlow stored in its
         cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.reset_connector_metadata_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#reset_connector_metadata_cache)
         """
+
     def start_flow(self, *, flowName: str, clientToken: str = ...) -> StartFlowResponseTypeDef:
         """
         Activates an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.start_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#start_flow)
         """
+
     def stop_flow(self, *, flowName: str) -> StopFlowResponseTypeDef:
         """
         Deactivates the existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.stop_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#stop_flow)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Applies a tag to the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#tag_resource)
         """
+
     def unregister_connector(
         self, *, connectorLabel: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Unregisters the custom connector registered in your account that matches the
         connector label provided in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.unregister_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#unregister_connector)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#untag_resource)
         """
+
     def update_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
         clientToken: str = ...
     ) -> UpdateConnectorProfileResponseTypeDef:
         """
         Updates a given connector profile associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_profile)
         """
+
     def update_connector_registration(
         self,
         *,
         connectorLabel: str,
         description: str = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateConnectorRegistrationResponseTypeDef:
         """
         Updates a custom connector that you've previously registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_registration)
         """
+
     def update_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigTypeDef,
-        sourceFlowConfig: SourceFlowConfigTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
-        tasks: Sequence[TaskTypeDef],
+        triggerConfig: Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef],
+        sourceFlowConfig: Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef],
+        destinationFlowConfigList: Sequence[
+            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
+        ],
+        tasks: Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
         description: str = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
```

### Comparing `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/literals.py` & `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/literals.pyi` & `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/type_defs.py` & `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3117,16 +3117,18 @@
 
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
-        "tasks": Sequence[TaskTypeDef],
+        "destinationFlowConfigList": Sequence[
+            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
+        ],
+        "tasks": Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
     },
 )
 _OptionalCreateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowRequestRequestTypeDef",
     {
         "description": str,
         "kmsArn": str,
@@ -3146,16 +3148,18 @@
 
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
-        "tasks": Sequence[TaskTypeDef],
+        "destinationFlowConfigList": Sequence[
+            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
+        ],
+        "tasks": Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFlowRequestRequestTypeDef",
     {
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
```

### Comparing `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/type_defs.pyi` & `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2988,16 +2988,18 @@
 
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
-        "tasks": Sequence[TaskTypeDef],
+        "destinationFlowConfigList": Sequence[
+            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
+        ],
+        "tasks": Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
     },
 )
 _OptionalCreateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowRequestRequestTypeDef",
     {
         "description": str,
         "kmsArn": str,
@@ -3015,16 +3017,18 @@
 
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
-        "tasks": Sequence[TaskTypeDef],
+        "destinationFlowConfigList": Sequence[
+            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
+        ],
+        "tasks": Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFlowRequestRequestTypeDef",
     {
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
```

### Comparing `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/PKG-INFO` & `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.28.15
-Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
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
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/SOURCES.txt` & `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15/setup.py` & `mypy-boto3-appflow-1.28.15.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appflow",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        " 7.15.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

