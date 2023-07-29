# Comparing `tmp/mypy-boto3-privatenetworks-1.28.15.tar.gz` & `tmp/mypy-boto3-privatenetworks-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-privatenetworks-1.28.15.tar", last modified: Fri Jul 28 20:43:30 2023, max compression
+gzip compressed data, was "mypy-boto3-privatenetworks-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:55 2023, max compression
```

## Comparing `mypy-boto3-privatenetworks-1.28.15.tar` & `mypy-boto3-privatenetworks-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.393681 mypy-boto3-privatenetworks-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-07-28 20:43:30.385681 mypy-boto3-privatenetworks-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15325 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.385681 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21342 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29836 2023-07-28 20:33:39.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29781 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.385681 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:30.393681 mypy-boto3-privatenetworks-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.089345 mypy-boto3-privatenetworks-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-07-29 10:03:55.089345 mypy-boto3-privatenetworks-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15325 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.089345 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21430 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29836 2023-07-29 09:53:31.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29781 2023-07-29 09:53:31.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.089345 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:03:54.000000 mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:55.089345 mypy-boto3-privatenetworks-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-29 09:53:30.000000 mypy-boto3-privatenetworks-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-privatenetworks-1.28.15/LICENSE` & `mypy-boto3-privatenetworks-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15/PKG-INFO` & `mypy-boto3-privatenetworks-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.28.15
-Summary: Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-privatenetworks-1.28.15/README.md` & `mypy-boto3-privatenetworks-1.28.15.post1/README.md`

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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__init__.py` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__init__.pyi` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__main__.py` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Private5G 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Private5G 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G\nOther"
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

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/client.py` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_privatenetworks.client import Private5GClient
 
     session = Session()
     client: Private5GClient = session.client("privatenetworks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeviceIdentifierFilterKeysType,
     NetworkResourceFilterKeysType,
     OrderFilterKeysType,
@@ -52,46 +52,43 @@
     ListNetworkResourcesResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListOrdersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     PositionTypeDef,
+    SitePlanOutputTypeDef,
     SitePlanTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Private5GClient",)
 
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
     InternalServerException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class Private5GClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/)
     """
 
     meta: ClientMeta
@@ -100,64 +97,58 @@
     def exceptions(self) -> Exceptions:
         """
         Private5GClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#exceptions)
         """
-
     def acknowledge_order_receipt(self, *, orderArn: str) -> AcknowledgeOrderReceiptResponseTypeDef:
         """
         Acknowledges that the specified network order was received.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.acknowledge_order_receipt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#acknowledge_order_receipt)
         """
-
     def activate_device_identifier(
         self, *, deviceIdentifierArn: str, clientToken: str = ...
     ) -> ActivateDeviceIdentifierResponseTypeDef:
         """
         Activates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_device_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_device_identifier)
         """
-
     def activate_network_site(
         self,
         *,
         networkSiteArn: str,
         shippingAddress: AddressTypeDef,
         clientToken: str = ...,
         commitmentConfiguration: CommitmentConfigurationTypeDef = ...
     ) -> ActivateNetworkSiteResponseTypeDef:
         """
         Activates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_network_site)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#close)
         """
-
     def configure_access_point(
         self,
         *,
         accessPointArn: str,
         cpiSecretKey: str = ...,
         cpiUserId: str = ...,
         cpiUserPassword: str = ...,
@@ -166,225 +157,206 @@
     ) -> ConfigureAccessPointResponseTypeDef:
         """
         Configures the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.configure_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#configure_access_point)
         """
-
     def create_network(
         self,
         *,
         networkName: str,
         clientToken: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateNetworkResponseTypeDef:
         """
         Creates a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#create_network)
         """
-
     def create_network_site(
         self,
         *,
         networkArn: str,
         networkSiteName: str,
         availabilityZone: str = ...,
         availabilityZoneId: str = ...,
         clientToken: str = ...,
         description: str = ...,
-        pendingPlan: SitePlanTypeDef = ...,
+        pendingPlan: Union[SitePlanTypeDef, SitePlanOutputTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateNetworkSiteResponseTypeDef:
         """
         Creates a network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#create_network_site)
         """
-
     def deactivate_device_identifier(
         self, *, deviceIdentifierArn: str, clientToken: str = ...
     ) -> DeactivateDeviceIdentifierResponseTypeDef:
         """
         Deactivates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.deactivate_device_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#deactivate_device_identifier)
         """
-
     def delete_network(
         self, *, networkArn: str, clientToken: str = ...
     ) -> DeleteNetworkResponseTypeDef:
         """
         Deletes the specified network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.delete_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#delete_network)
         """
-
     def delete_network_site(
         self, *, networkSiteArn: str, clientToken: str = ...
     ) -> DeleteNetworkSiteResponseTypeDef:
         """
         Deletes the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.delete_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#delete_network_site)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#generate_presigned_url)
         """
-
     def get_device_identifier(
         self, *, deviceIdentifierArn: str
     ) -> GetDeviceIdentifierResponseTypeDef:
         """
         Gets the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_device_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_device_identifier)
         """
-
     def get_network(self, *, networkArn: str) -> GetNetworkResponseTypeDef:
         """
         Gets the specified network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_network)
         """
-
     def get_network_resource(self, *, networkResourceArn: str) -> GetNetworkResourceResponseTypeDef:
         """
         Gets the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_network_resource)
         """
-
     def get_network_site(self, *, networkSiteArn: str) -> GetNetworkSiteResponseTypeDef:
         """
         Gets the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_network_site)
         """
-
     def get_order(self, *, orderArn: str) -> GetOrderResponseTypeDef:
         """
         Gets the specified order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_order)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_order)
         """
-
     def list_device_identifiers(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListDeviceIdentifiersResponseTypeDef:
         """
         Lists device identifiers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_device_identifiers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_device_identifiers)
         """
-
     def list_network_resources(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworkResourcesResponseTypeDef:
         """
         Lists network resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_network_resources)
         """
-
     def list_network_sites(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworkSitesResponseTypeDef:
         """
         Lists network sites.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_sites)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_network_sites)
         """
-
     def list_networks(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworksResponseTypeDef:
         """
         Lists networks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_networks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_networks)
         """
-
     def list_orders(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListOrdersResponseTypeDef:
         """
         Lists orders.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_orders)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_orders)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_tags_for_resource)
         """
-
     def ping(self) -> PingResponseTypeDef:
         """
         Checks the health of the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.ping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#ping)
         """
-
     def start_network_resource_update(
         self,
         *,
         networkResourceArn: str,
         updateType: UpdateTypeType,
         commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
         returnReason: str = ...,
@@ -393,84 +365,79 @@
         """
         Use this action to do the following tasks: * Update the duration and renewal
         status of the commitment period for a radio unit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.start_network_resource_update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#start_network_resource_update)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#untag_resource)
         """
-
     def update_network_site(
         self, *, networkSiteArn: str, clientToken: str = ..., description: str = ...
     ) -> UpdateNetworkSiteResponseTypeDef:
         """
         Updates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#update_network_site)
         """
-
     def update_network_site_plan(
-        self, *, networkSiteArn: str, pendingPlan: SitePlanTypeDef, clientToken: str = ...
+        self,
+        *,
+        networkSiteArn: str,
+        pendingPlan: Union[SitePlanTypeDef, SitePlanOutputTypeDef],
+        clientToken: str = ...
     ) -> UpdateNetworkSiteResponseTypeDef:
         """
         Updates the specified network site plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#update_network_site_plan)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_device_identifiers"]
     ) -> ListDeviceIdentifiersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_network_resources"]
     ) -> ListNetworkResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_network_sites"]
     ) -> ListNetworkSitesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_networks"]) -> ListNetworksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_orders"]) -> ListOrdersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/client.pyi` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_privatenetworks.client import Private5GClient
 
     session = Session()
     client: Private5GClient = session.client("privatenetworks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeviceIdentifierFilterKeysType,
     NetworkResourceFilterKeysType,
     OrderFilterKeysType,
@@ -52,42 +52,47 @@
     ListNetworkResourcesResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListOrdersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     PositionTypeDef,
+    SitePlanOutputTypeDef,
     SitePlanTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("Private5GClient",)
 
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
     InternalServerException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class Private5GClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/)
     """
 
     meta: ClientMeta
@@ -96,58 +101,64 @@
     def exceptions(self) -> Exceptions:
         """
         Private5GClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#exceptions)
         """
+
     def acknowledge_order_receipt(self, *, orderArn: str) -> AcknowledgeOrderReceiptResponseTypeDef:
         """
         Acknowledges that the specified network order was received.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.acknowledge_order_receipt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#acknowledge_order_receipt)
         """
+
     def activate_device_identifier(
         self, *, deviceIdentifierArn: str, clientToken: str = ...
     ) -> ActivateDeviceIdentifierResponseTypeDef:
         """
         Activates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_device_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_device_identifier)
         """
+
     def activate_network_site(
         self,
         *,
         networkSiteArn: str,
         shippingAddress: AddressTypeDef,
         clientToken: str = ...,
         commitmentConfiguration: CommitmentConfigurationTypeDef = ...
     ) -> ActivateNetworkSiteResponseTypeDef:
         """
         Activates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_network_site)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#close)
         """
+
     def configure_access_point(
         self,
         *,
         accessPointArn: str,
         cpiSecretKey: str = ...,
         cpiUserId: str = ...,
         cpiUserPassword: str = ...,
@@ -156,206 +167,225 @@
     ) -> ConfigureAccessPointResponseTypeDef:
         """
         Configures the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.configure_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#configure_access_point)
         """
+
     def create_network(
         self,
         *,
         networkName: str,
         clientToken: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateNetworkResponseTypeDef:
         """
         Creates a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#create_network)
         """
+
     def create_network_site(
         self,
         *,
         networkArn: str,
         networkSiteName: str,
         availabilityZone: str = ...,
         availabilityZoneId: str = ...,
         clientToken: str = ...,
         description: str = ...,
-        pendingPlan: SitePlanTypeDef = ...,
+        pendingPlan: Union[SitePlanTypeDef, SitePlanOutputTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateNetworkSiteResponseTypeDef:
         """
         Creates a network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#create_network_site)
         """
+
     def deactivate_device_identifier(
         self, *, deviceIdentifierArn: str, clientToken: str = ...
     ) -> DeactivateDeviceIdentifierResponseTypeDef:
         """
         Deactivates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.deactivate_device_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#deactivate_device_identifier)
         """
+
     def delete_network(
         self, *, networkArn: str, clientToken: str = ...
     ) -> DeleteNetworkResponseTypeDef:
         """
         Deletes the specified network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.delete_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#delete_network)
         """
+
     def delete_network_site(
         self, *, networkSiteArn: str, clientToken: str = ...
     ) -> DeleteNetworkSiteResponseTypeDef:
         """
         Deletes the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.delete_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#delete_network_site)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#generate_presigned_url)
         """
+
     def get_device_identifier(
         self, *, deviceIdentifierArn: str
     ) -> GetDeviceIdentifierResponseTypeDef:
         """
         Gets the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_device_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_device_identifier)
         """
+
     def get_network(self, *, networkArn: str) -> GetNetworkResponseTypeDef:
         """
         Gets the specified network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_network)
         """
+
     def get_network_resource(self, *, networkResourceArn: str) -> GetNetworkResourceResponseTypeDef:
         """
         Gets the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_network_resource)
         """
+
     def get_network_site(self, *, networkSiteArn: str) -> GetNetworkSiteResponseTypeDef:
         """
         Gets the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_network_site)
         """
+
     def get_order(self, *, orderArn: str) -> GetOrderResponseTypeDef:
         """
         Gets the specified order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_order)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_order)
         """
+
     def list_device_identifiers(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListDeviceIdentifiersResponseTypeDef:
         """
         Lists device identifiers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_device_identifiers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_device_identifiers)
         """
+
     def list_network_resources(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworkResourcesResponseTypeDef:
         """
         Lists network resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_network_resources)
         """
+
     def list_network_sites(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworkSitesResponseTypeDef:
         """
         Lists network sites.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_sites)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_network_sites)
         """
+
     def list_networks(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworksResponseTypeDef:
         """
         Lists networks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_networks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_networks)
         """
+
     def list_orders(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListOrdersResponseTypeDef:
         """
         Lists orders.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_orders)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_orders)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#list_tags_for_resource)
         """
+
     def ping(self) -> PingResponseTypeDef:
         """
         Checks the health of the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.ping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#ping)
         """
+
     def start_network_resource_update(
         self,
         *,
         networkResourceArn: str,
         updateType: UpdateTypeType,
         commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
         returnReason: str = ...,
@@ -364,75 +394,88 @@
         """
         Use this action to do the following tasks: * Update the duration and renewal
         status of the commitment period for a radio unit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.start_network_resource_update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#start_network_resource_update)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#untag_resource)
         """
+
     def update_network_site(
         self, *, networkSiteArn: str, clientToken: str = ..., description: str = ...
     ) -> UpdateNetworkSiteResponseTypeDef:
         """
         Updates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#update_network_site)
         """
+
     def update_network_site_plan(
-        self, *, networkSiteArn: str, pendingPlan: SitePlanTypeDef, clientToken: str = ...
+        self,
+        *,
+        networkSiteArn: str,
+        pendingPlan: Union[SitePlanTypeDef, SitePlanOutputTypeDef],
+        clientToken: str = ...
     ) -> UpdateNetworkSiteResponseTypeDef:
         """
         Updates the specified network site plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#update_network_site_plan)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_device_identifiers"]
     ) -> ListDeviceIdentifiersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_network_resources"]
     ) -> ListNetworkResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_network_sites"]
     ) -> ListNetworkSitesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_networks"]) -> ListNetworksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_orders"]) -> ListOrdersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/literals.py` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/literals.pyi` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/paginator.py` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/paginator.pyi` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/type_defs.py` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/type_defs.pyi` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/PKG-INFO` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.28.15
-Summary: Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/SOURCES.txt` & `mypy-boto3-privatenetworks-1.28.15.post1/mypy_boto3_privatenetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.15/setup.py` & `mypy-boto3-privatenetworks-1.28.15.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-privatenetworks",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_privatenetworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder"
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

