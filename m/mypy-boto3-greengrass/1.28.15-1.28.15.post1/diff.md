# Comparing `tmp/mypy-boto3-greengrass-1.28.15.tar.gz` & `tmp/mypy-boto3-greengrass-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-greengrass-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
+gzip compressed data, was "mypy-boto3-greengrass-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:13 2023, max compression
```

## Comparing `mypy-boto3-greengrass-1.28.15.tar` & `mypy-boto3-greengrass-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.121170 mypy-boto3-greengrass-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28275 2023-07-28 20:42:53.113170 mypy-boto3-greengrass-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26776 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.105169 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-07-28 20:27:02.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68595 2023-07-28 20:27:01.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-07-28 20:27:02.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-07-28 20:27:02.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-07-28 20:27:02.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-28 20:27:02.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    93312 2023-07-28 20:27:04.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93191 2023-07-28 20:27:03.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.109169 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28275 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.121170 mypy-boto3-greengrass-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.117168 mypy-boto3-greengrass-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28281 2023-07-29 10:03:13.117168 mypy-boto3-greengrass-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26776 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.097167 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69678 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69560 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-07-29 09:46:34.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    93410 2023-07-29 09:46:38.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93289 2023-07-29 09:46:37.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.117168 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28281 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:13.117168 mypy-boto3-greengrass-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:46:32.000000 mypy-boto3-greengrass-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-greengrass-1.28.15/LICENSE` & `mypy-boto3-greengrass-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15/PKG-INFO` & `mypy-boto3-greengrass-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrass
-Version: 1.28.15
-Summary: Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-greengrass-1.28.15/README.md` & `mypy-boto3-greengrass-1.28.15.post1/README.md`

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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__init__.py` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__init__.pyi` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__main__.py` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Greengrass 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Greengrass 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass\nOther"
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

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/client.py` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_greengrass.client import GreengrassClient
 
     session = Session()
     client: GreengrassClient = session.client("greengrass")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeploymentTypeType,
     SoftwareToUpdateType,
     UpdateAgentLogLevelType,
@@ -46,16 +46,19 @@
     ListSubscriptionDefinitionsPaginator,
     ListSubscriptionDefinitionVersionsPaginator,
 )
 from .type_defs import (
     AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     ConnectivityInfoTypeDef,
+    ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
+    ConnectorOutputTypeDef,
     ConnectorTypeDef,
+    CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CoreTypeDef,
     CreateConnectorDefinitionResponseTypeDef,
     CreateConnectorDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionResponseTypeDef,
     CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
@@ -69,21 +72,24 @@
     CreateLoggerDefinitionResponseTypeDef,
     CreateLoggerDefinitionVersionResponseTypeDef,
     CreateResourceDefinitionResponseTypeDef,
     CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobResponseTypeDef,
     CreateSubscriptionDefinitionResponseTypeDef,
     CreateSubscriptionDefinitionVersionResponseTypeDef,
+    DeviceDefinitionVersionOutputTypeDef,
     DeviceDefinitionVersionTypeDef,
     DeviceTypeDef,
     DisassociateRoleFromGroupResponseTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FunctionDefaultConfigTypeDef,
+    FunctionDefinitionVersionOutputTypeDef,
     FunctionDefinitionVersionTypeDef,
+    FunctionOutputTypeDef,
     FunctionTypeDef,
     GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
     GetCoreDefinitionResponseTypeDef,
@@ -123,20 +129,24 @@
     ListLoggerDefinitionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    LoggerDefinitionVersionOutputTypeDef,
     LoggerDefinitionVersionTypeDef,
     LoggerTypeDef,
     ResetDeploymentsResponseTypeDef,
+    ResourceDefinitionVersionOutputTypeDef,
     ResourceDefinitionVersionTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     StartBulkDeploymentResponseTypeDef,
+    SubscriptionDefinitionVersionOutputTypeDef,
     SubscriptionDefinitionVersionTypeDef,
     SubscriptionTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UpdateConnectivityInfoResponseTypeDef,
     UpdateGroupCertificateConfigurationResponseTypeDef,
 )
 
@@ -216,15 +226,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#close)
         """
 
     def create_connector_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: ConnectorDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            ConnectorDefinitionVersionTypeDef, ConnectorDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateConnectorDefinitionResponseTypeDef:
         """
         Creates a connector definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition)
@@ -232,28 +244,30 @@
         """
 
     def create_connector_definition_version(
         self,
         *,
         ConnectorDefinitionId: str,
         AmznClientToken: str = ...,
-        Connectors: Sequence[ConnectorTypeDef] = ...
+        Connectors: Sequence[Union[ConnectorTypeDef, ConnectorOutputTypeDef]] = ...
     ) -> CreateConnectorDefinitionVersionResponseTypeDef:
         """
         Creates a version of a connector definition which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_connector_definition_version)
         """
 
     def create_core_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: CoreDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            CoreDefinitionVersionTypeDef, CoreDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateCoreDefinitionResponseTypeDef:
         """
         Creates a core definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_core_definition)
@@ -290,15 +304,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_deployment)
         """
 
     def create_device_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: DeviceDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            DeviceDefinitionVersionTypeDef, DeviceDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeviceDefinitionResponseTypeDef:
         """
         Creates a device definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition)
@@ -319,15 +335,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_device_definition_version)
         """
 
     def create_function_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: FunctionDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            FunctionDefinitionVersionTypeDef, FunctionDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFunctionDefinitionResponseTypeDef:
         """
         Creates a Lambda function definition which contains a list of Lambda functions
         and their configurations to be used in a group.
 
@@ -337,15 +355,15 @@
 
     def create_function_definition_version(
         self,
         *,
         FunctionDefinitionId: str,
         AmznClientToken: str = ...,
         DefaultConfig: FunctionDefaultConfigTypeDef = ...,
-        Functions: Sequence[FunctionTypeDef] = ...
+        Functions: Sequence[Union[FunctionTypeDef, FunctionOutputTypeDef]] = ...
     ) -> CreateFunctionDefinitionVersionResponseTypeDef:
         """
         Creates a version of a Lambda function definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_function_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_function_definition_version)
         """
@@ -395,15 +413,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_group_version)
         """
 
     def create_logger_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: LoggerDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            LoggerDefinitionVersionTypeDef, LoggerDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateLoggerDefinitionResponseTypeDef:
         """
         Creates a logger definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition)
@@ -424,15 +444,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_logger_definition_version)
         """
 
     def create_resource_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: ResourceDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            ResourceDefinitionVersionTypeDef, ResourceDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResourceDefinitionResponseTypeDef:
         """
         Creates a resource definition which contains a list of resources to be used in a
         group.
 
@@ -441,15 +463,15 @@
         """
 
     def create_resource_definition_version(
         self,
         *,
         ResourceDefinitionId: str,
         AmznClientToken: str = ...,
-        Resources: Sequence[ResourceTypeDef] = ...
+        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]] = ...
     ) -> CreateResourceDefinitionVersionResponseTypeDef:
         """
         Creates a version of a resource definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_resource_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_resource_definition_version)
         """
@@ -474,15 +496,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_software_update_job)
         """
 
     def create_subscription_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: SubscriptionDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            SubscriptionDefinitionVersionTypeDef, SubscriptionDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSubscriptionDefinitionResponseTypeDef:
         """
         Creates a subscription definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_subscription_definition)
```

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/client.pyi` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_greengrass.client import GreengrassClient
 
     session = Session()
     client: GreengrassClient = session.client("greengrass")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeploymentTypeType,
     SoftwareToUpdateType,
     UpdateAgentLogLevelType,
@@ -46,16 +46,19 @@
     ListSubscriptionDefinitionsPaginator,
     ListSubscriptionDefinitionVersionsPaginator,
 )
 from .type_defs import (
     AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     ConnectivityInfoTypeDef,
+    ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
+    ConnectorOutputTypeDef,
     ConnectorTypeDef,
+    CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CoreTypeDef,
     CreateConnectorDefinitionResponseTypeDef,
     CreateConnectorDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionResponseTypeDef,
     CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
@@ -69,21 +72,24 @@
     CreateLoggerDefinitionResponseTypeDef,
     CreateLoggerDefinitionVersionResponseTypeDef,
     CreateResourceDefinitionResponseTypeDef,
     CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobResponseTypeDef,
     CreateSubscriptionDefinitionResponseTypeDef,
     CreateSubscriptionDefinitionVersionResponseTypeDef,
+    DeviceDefinitionVersionOutputTypeDef,
     DeviceDefinitionVersionTypeDef,
     DeviceTypeDef,
     DisassociateRoleFromGroupResponseTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FunctionDefaultConfigTypeDef,
+    FunctionDefinitionVersionOutputTypeDef,
     FunctionDefinitionVersionTypeDef,
+    FunctionOutputTypeDef,
     FunctionTypeDef,
     GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
     GetCoreDefinitionResponseTypeDef,
@@ -123,20 +129,24 @@
     ListLoggerDefinitionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    LoggerDefinitionVersionOutputTypeDef,
     LoggerDefinitionVersionTypeDef,
     LoggerTypeDef,
     ResetDeploymentsResponseTypeDef,
+    ResourceDefinitionVersionOutputTypeDef,
     ResourceDefinitionVersionTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     StartBulkDeploymentResponseTypeDef,
+    SubscriptionDefinitionVersionOutputTypeDef,
     SubscriptionDefinitionVersionTypeDef,
     SubscriptionTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UpdateConnectivityInfoResponseTypeDef,
     UpdateGroupCertificateConfigurationResponseTypeDef,
 )
 
@@ -207,42 +217,46 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#close)
         """
     def create_connector_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: ConnectorDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            ConnectorDefinitionVersionTypeDef, ConnectorDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateConnectorDefinitionResponseTypeDef:
         """
         Creates a connector definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_connector_definition)
         """
     def create_connector_definition_version(
         self,
         *,
         ConnectorDefinitionId: str,
         AmznClientToken: str = ...,
-        Connectors: Sequence[ConnectorTypeDef] = ...
+        Connectors: Sequence[Union[ConnectorTypeDef, ConnectorOutputTypeDef]] = ...
     ) -> CreateConnectorDefinitionVersionResponseTypeDef:
         """
         Creates a version of a connector definition which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_connector_definition_version)
         """
     def create_core_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: CoreDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            CoreDefinitionVersionTypeDef, CoreDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateCoreDefinitionResponseTypeDef:
         """
         Creates a core definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_core_definition)
@@ -276,15 +290,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_deployment)
         """
     def create_device_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: DeviceDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            DeviceDefinitionVersionTypeDef, DeviceDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeviceDefinitionResponseTypeDef:
         """
         Creates a device definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition)
@@ -303,15 +319,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_device_definition_version)
         """
     def create_function_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: FunctionDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            FunctionDefinitionVersionTypeDef, FunctionDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFunctionDefinitionResponseTypeDef:
         """
         Creates a Lambda function definition which contains a list of Lambda functions
         and their configurations to be used in a group.
 
@@ -320,15 +338,15 @@
         """
     def create_function_definition_version(
         self,
         *,
         FunctionDefinitionId: str,
         AmznClientToken: str = ...,
         DefaultConfig: FunctionDefaultConfigTypeDef = ...,
-        Functions: Sequence[FunctionTypeDef] = ...
+        Functions: Sequence[Union[FunctionTypeDef, FunctionOutputTypeDef]] = ...
     ) -> CreateFunctionDefinitionVersionResponseTypeDef:
         """
         Creates a version of a Lambda function definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_function_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_function_definition_version)
         """
@@ -374,15 +392,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_group_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_group_version)
         """
     def create_logger_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: LoggerDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            LoggerDefinitionVersionTypeDef, LoggerDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateLoggerDefinitionResponseTypeDef:
         """
         Creates a logger definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition)
@@ -401,15 +421,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_logger_definition_version)
         """
     def create_resource_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: ResourceDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            ResourceDefinitionVersionTypeDef, ResourceDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResourceDefinitionResponseTypeDef:
         """
         Creates a resource definition which contains a list of resources to be used in a
         group.
 
@@ -417,15 +439,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_resource_definition)
         """
     def create_resource_definition_version(
         self,
         *,
         ResourceDefinitionId: str,
         AmznClientToken: str = ...,
-        Resources: Sequence[ResourceTypeDef] = ...
+        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]] = ...
     ) -> CreateResourceDefinitionVersionResponseTypeDef:
         """
         Creates a version of a resource definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_resource_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_resource_definition_version)
         """
@@ -448,15 +470,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_software_update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_software_update_job)
         """
     def create_subscription_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: SubscriptionDefinitionVersionTypeDef = ...,
+        InitialVersion: Union[
+            SubscriptionDefinitionVersionTypeDef, SubscriptionDefinitionVersionOutputTypeDef
+        ] = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSubscriptionDefinitionResponseTypeDef:
         """
         Creates a subscription definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_subscription_definition)
```

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/literals.py` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/literals.pyi` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/paginator.py` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/paginator.pyi` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/type_defs.py` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_greengrass.type_defs import AssociateRoleToGroupRequestRequestTypeDef
 
     data: AssociateRoleToGroupRequestRequestTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BulkDeploymentStatusType,
     ConfigurationSyncStatusType,
     DeploymentTypeType,
     EncodingTypeType,
     FunctionIsolationModeType,
@@ -2223,15 +2223,15 @@
         "ConnectorDefinitionId": str,
     },
 )
 _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "Connectors": Sequence[ConnectorTypeDef],
+        "Connectors": Sequence[Union[ConnectorTypeDef, ConnectorOutputTypeDef]],
     },
     total=False,
 )
 
 
 class CreateConnectorDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
@@ -3267,15 +3267,15 @@
         "ResourceDefinitionId": str,
     },
 )
 _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "Resources": Sequence[ResourceTypeDef],
+        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
     },
     total=False,
 )
 
 
 class CreateResourceDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
@@ -3308,15 +3308,15 @@
     },
 )
 _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "DefaultConfig": FunctionDefaultConfigTypeDef,
-        "Functions": Sequence[FunctionTypeDef],
+        "Functions": Sequence[Union[FunctionTypeDef, FunctionOutputTypeDef]],
     },
     total=False,
 )
 
 
 class CreateFunctionDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/type_defs.pyi` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_greengrass.type_defs import AssociateRoleToGroupRequestRequestTypeDef
 
     data: AssociateRoleToGroupRequestRequestTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BulkDeploymentStatusType,
     ConfigurationSyncStatusType,
     DeploymentTypeType,
     EncodingTypeType,
     FunctionIsolationModeType,
@@ -2144,15 +2144,15 @@
         "ConnectorDefinitionId": str,
     },
 )
 _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "Connectors": Sequence[ConnectorTypeDef],
+        "Connectors": Sequence[Union[ConnectorTypeDef, ConnectorOutputTypeDef]],
     },
     total=False,
 )
 
 class CreateConnectorDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
@@ -3150,15 +3150,15 @@
         "ResourceDefinitionId": str,
     },
 )
 _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "Resources": Sequence[ResourceTypeDef],
+        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
     },
     total=False,
 )
 
 class CreateResourceDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
@@ -3189,15 +3189,15 @@
     },
 )
 _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "DefaultConfig": FunctionDefaultConfigTypeDef,
-        "Functions": Sequence[FunctionTypeDef],
+        "Functions": Sequence[Union[FunctionTypeDef, FunctionOutputTypeDef]],
     },
     total=False,
 )
 
 class CreateFunctionDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/PKG-INFO` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrass
-Version: 1.28.15
-Summary: Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/SOURCES.txt` & `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15/setup.py` & `mypy-boto3-greengrass-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-greengrass",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_greengrass"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder"
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

