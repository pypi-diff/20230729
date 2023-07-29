# Comparing `tmp/mypy-boto3-appstream-1.28.15.tar.gz` & `tmp/mypy-boto3-appstream-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appstream-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
+gzip compressed data, was "mypy-boto3-appstream-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:31 2023, max compression
```

## Comparing `mypy-boto3-appstream-1.28.15.tar` & `mypy-boto3-appstream-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.236695 mypy-boto3-appstream-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-28 20:42:19.228695 mypy-boto3-appstream-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21982 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.228695 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57822 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-28 20:19:38.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-28 20:19:38.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70349 2023-07-28 20:19:40.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70250 2023-07-28 20:19:39.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-28 20:19:37.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.228695 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-28 20:42:18.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-28 20:42:19.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:18.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:18.000000 mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.236695 mypy-boto3-appstream-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:19:36.000000 mypy-boto3-appstream-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.245008 mypy-boto3-appstream-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23483 2023-07-29 10:02:31.245008 mypy-boto3-appstream-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21982 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.241008 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58261 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58167 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-29 09:38:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70476 2023-07-29 09:38:32.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70377 2023-07-29 09:38:31.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.245008 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23483 2023-07-29 10:02:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-29 10:02:31.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:02:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:31.245008 mypy-boto3-appstream-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:38:28.000000 mypy-boto3-appstream-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-appstream-1.28.15/LICENSE` & `mypy-boto3-appstream-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15/PKG-INFO` & `mypy-boto3-appstream-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.28.15
-Summary: Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -441,14 +441,15 @@
     CopyImageRequestRequestTypeDef,
     VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
+    StorageConnectorOutputTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DeleteAppBlockBuilderRequestRequestTypeDef,
@@ -496,15 +497,14 @@
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     StackErrorTypeDef,
-    StorageConnectorOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-appstream-1.28.15/README.md` & `mypy-boto3-appstream-1.28.15.post1/README.md`

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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -409,14 +409,15 @@
     CopyImageRequestRequestTypeDef,
     VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
+    StorageConnectorOutputTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DeleteAppBlockBuilderRequestRequestTypeDef,
@@ -464,15 +465,14 @@
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     StackErrorTypeDef,
-    StorageConnectorOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__init__.py` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__init__.pyi` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/__main__.py` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppStream 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.AppStream 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream\nOther"
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

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/client.py` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appstream.client import AppStreamClient
 
     session = Session()
     client: AppStreamClient = session.client("appstream")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppBlockBuilderAttributeType,
     ApplicationAttributeType,
     AppVisibilityType,
@@ -95,24 +95,26 @@
     S3LocationTypeDef,
     ScriptDetailsTypeDef,
     ServiceAccountCredentialsTypeDef,
     StartAppBlockBuilderResultTypeDef,
     StartImageBuilderResultTypeDef,
     StopAppBlockBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
+    StorageConnectorOutputTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UpdateAppBlockBuilderResultTypeDef,
     UpdateApplicationResultTypeDef,
     UpdateDirectoryConfigResultTypeDef,
     UpdateEntitlementResultTypeDef,
     UpdateFleetResultTypeDef,
     UpdateStackResultTypeDef,
     UserSettingTypeDef,
     UserStackAssociationTypeDef,
+    VpcConfigOutputTypeDef,
     VpcConfigTypeDef,
 )
 from .waiter import FleetStartedWaiter, FleetStoppedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -276,15 +278,15 @@
 
     def create_app_block_builder(
         self,
         *,
         Name: str,
         Platform: Literal["WINDOWS_SERVER_2019"],
         InstanceType: str,
-        VpcConfig: VpcConfigTypeDef,
+        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef],
         Description: str = ...,
         DisplayName: str = ...,
         Tags: Mapping[str, str] = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
     ) -> CreateAppBlockBuilderResultTypeDef:
@@ -363,15 +365,15 @@
         *,
         Name: str,
         InstanceType: str,
         ImageName: str = ...,
         ImageArn: str = ...,
         FleetType: FleetTypeType = ...,
         ComputeCapacity: ComputeCapacityTypeDef = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
         MaxUserDurationInSeconds: int = ...,
         DisconnectTimeoutInSeconds: int = ...,
         Description: str = ...,
         DisplayName: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
@@ -395,15 +397,15 @@
         *,
         Name: str,
         InstanceType: str,
         ImageName: str = ...,
         ImageArn: str = ...,
         Description: str = ...,
         DisplayName: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
         IamRoleArn: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
         AppstreamAgentVersion: str = ...,
         Tags: Mapping[str, str] = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
     ) -> CreateImageBuilderResultTypeDef:
@@ -426,15 +428,17 @@
 
     def create_stack(
         self,
         *,
         Name: str,
         Description: str = ...,
         DisplayName: str = ...,
-        StorageConnectors: Sequence[StorageConnectorTypeDef] = ...,
+        StorageConnectors: Sequence[
+            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
+        ] = ...,
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         EmbedHostDomains: Sequence[str] = ...,
@@ -999,15 +1003,15 @@
         self,
         *,
         Name: str,
         Description: str = ...,
         DisplayName: str = ...,
         Platform: PlatformTypeType = ...,
         InstanceType: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
     ) -> UpdateAppBlockBuilderResultTypeDef:
         """
         Updates an app block builder.
@@ -1071,15 +1075,15 @@
         self,
         *,
         ImageName: str = ...,
         ImageArn: str = ...,
         Name: str = ...,
         InstanceType: str = ...,
         ComputeCapacity: ComputeCapacityTypeDef = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
         MaxUserDurationInSeconds: int = ...,
         DisconnectTimeoutInSeconds: int = ...,
         DeleteVpcConfig: bool = ...,
         Description: str = ...,
         DisplayName: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
@@ -1111,15 +1115,17 @@
 
     def update_stack(
         self,
         *,
         Name: str,
         DisplayName: str = ...,
         Description: str = ...,
-        StorageConnectors: Sequence[StorageConnectorTypeDef] = ...,
+        StorageConnectors: Sequence[
+            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
+        ] = ...,
         DeleteStorageConnectors: bool = ...,
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         AttributesToDelete: Sequence[StackAttributeType] = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
```

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/client.pyi` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appstream.client import AppStreamClient
 
     session = Session()
     client: AppStreamClient = session.client("appstream")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppBlockBuilderAttributeType,
     ApplicationAttributeType,
     AppVisibilityType,
@@ -95,24 +95,26 @@
     S3LocationTypeDef,
     ScriptDetailsTypeDef,
     ServiceAccountCredentialsTypeDef,
     StartAppBlockBuilderResultTypeDef,
     StartImageBuilderResultTypeDef,
     StopAppBlockBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
+    StorageConnectorOutputTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UpdateAppBlockBuilderResultTypeDef,
     UpdateApplicationResultTypeDef,
     UpdateDirectoryConfigResultTypeDef,
     UpdateEntitlementResultTypeDef,
     UpdateFleetResultTypeDef,
     UpdateStackResultTypeDef,
     UserSettingTypeDef,
     UserStackAssociationTypeDef,
+    VpcConfigOutputTypeDef,
     VpcConfigTypeDef,
 )
 from .waiter import FleetStartedWaiter, FleetStoppedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -261,15 +263,15 @@
         """
     def create_app_block_builder(
         self,
         *,
         Name: str,
         Platform: Literal["WINDOWS_SERVER_2019"],
         InstanceType: str,
-        VpcConfig: VpcConfigTypeDef,
+        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef],
         Description: str = ...,
         DisplayName: str = ...,
         Tags: Mapping[str, str] = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
     ) -> CreateAppBlockBuilderResultTypeDef:
@@ -343,15 +345,15 @@
         *,
         Name: str,
         InstanceType: str,
         ImageName: str = ...,
         ImageArn: str = ...,
         FleetType: FleetTypeType = ...,
         ComputeCapacity: ComputeCapacityTypeDef = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
         MaxUserDurationInSeconds: int = ...,
         DisconnectTimeoutInSeconds: int = ...,
         Description: str = ...,
         DisplayName: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
@@ -374,15 +376,15 @@
         *,
         Name: str,
         InstanceType: str,
         ImageName: str = ...,
         ImageArn: str = ...,
         Description: str = ...,
         DisplayName: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
         IamRoleArn: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
         AppstreamAgentVersion: str = ...,
         Tags: Mapping[str, str] = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
     ) -> CreateImageBuilderResultTypeDef:
@@ -403,15 +405,17 @@
         """
     def create_stack(
         self,
         *,
         Name: str,
         Description: str = ...,
         DisplayName: str = ...,
-        StorageConnectors: Sequence[StorageConnectorTypeDef] = ...,
+        StorageConnectors: Sequence[
+            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
+        ] = ...,
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         EmbedHostDomains: Sequence[str] = ...,
@@ -923,15 +927,15 @@
         self,
         *,
         Name: str,
         Description: str = ...,
         DisplayName: str = ...,
         Platform: PlatformTypeType = ...,
         InstanceType: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
     ) -> UpdateAppBlockBuilderResultTypeDef:
         """
         Updates an app block builder.
@@ -991,15 +995,15 @@
         self,
         *,
         ImageName: str = ...,
         ImageArn: str = ...,
         Name: str = ...,
         InstanceType: str = ...,
         ComputeCapacity: ComputeCapacityTypeDef = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
         MaxUserDurationInSeconds: int = ...,
         DisconnectTimeoutInSeconds: int = ...,
         DeleteVpcConfig: bool = ...,
         Description: str = ...,
         DisplayName: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
@@ -1029,15 +1033,17 @@
         """
     def update_stack(
         self,
         *,
         Name: str,
         DisplayName: str = ...,
         Description: str = ...,
-        StorageConnectors: Sequence[StorageConnectorTypeDef] = ...,
+        StorageConnectors: Sequence[
+            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
+        ] = ...,
         DeleteStorageConnectors: bool = ...,
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         AttributesToDelete: Sequence[StackAttributeType] = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
```

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/literals.py` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/literals.pyi` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/paginator.py` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/paginator.pyi` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/type_defs.py` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_appstream.type_defs import AccessEndpointTypeDef
 
     data: AccessEndpointTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ActionType,
     AppBlockBuilderAttributeType,
     AppBlockBuilderStateType,
     AppBlockStateType,
     ApplicationAttributeType,
@@ -81,14 +81,15 @@
     "CopyImageRequestRequestTypeDef",
     "VpcConfigTypeDef",
     "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
+    "StorageConnectorOutputTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DeleteAppBlockBuilderRequestRequestTypeDef",
@@ -136,15 +137,14 @@
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "StackErrorTypeDef",
-    "StorageConnectorOutputTypeDef",
     "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
     "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -569,14 +569,36 @@
 class CreateImageBuilderStreamingURLRequestRequestTypeDef(
     _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef,
     _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredStorageConnectorOutputTypeDef = TypedDict(
+    "_RequiredStorageConnectorOutputTypeDef",
+    {
+        "ConnectorType": StorageConnectorTypeType,
+    },
+)
+_OptionalStorageConnectorOutputTypeDef = TypedDict(
+    "_OptionalStorageConnectorOutputTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "Domains": List[str],
+    },
+    total=False,
+)
+
+
+class StorageConnectorOutputTypeDef(
+    _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
+):
+    pass
+
+
 _RequiredStorageConnectorTypeDef = TypedDict(
     "_RequiredStorageConnectorTypeDef",
     {
         "ConnectorType": StorageConnectorTypeType,
     },
 )
 _OptionalStorageConnectorTypeDef = TypedDict(
@@ -1224,36 +1246,14 @@
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredStorageConnectorOutputTypeDef = TypedDict(
-    "_RequiredStorageConnectorOutputTypeDef",
-    {
-        "ConnectorType": StorageConnectorTypeType,
-    },
-)
-_OptionalStorageConnectorOutputTypeDef = TypedDict(
-    "_OptionalStorageConnectorOutputTypeDef",
-    {
-        "ResourceIdentifier": str,
-        "Domains": List[str],
-    },
-    total=False,
-)
-
-
-class StorageConnectorOutputTypeDef(
-    _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
-):
-    pass
-
-
 StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "StartAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1901,15 +1901,17 @@
     },
 )
 _OptionalCreateStackRequestRequestTypeDef = TypedDict(
     "_OptionalCreateStackRequestRequestTypeDef",
     {
         "Description": str,
         "DisplayName": str,
-        "StorageConnectors": Sequence[StorageConnectorTypeDef],
+        "StorageConnectors": Sequence[
+            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
+        ],
         "RedirectURL": str,
         "FeedbackURL": str,
         "UserSettings": Sequence[UserSettingTypeDef],
         "ApplicationSettings": ApplicationSettingsTypeDef,
         "Tags": Mapping[str, str],
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "EmbedHostDomains": Sequence[str],
@@ -1932,15 +1934,17 @@
     },
 )
 _OptionalUpdateStackRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateStackRequestRequestTypeDef",
     {
         "DisplayName": str,
         "Description": str,
-        "StorageConnectors": Sequence[StorageConnectorTypeDef],
+        "StorageConnectors": Sequence[
+            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
+        ],
         "DeleteStorageConnectors": bool,
         "RedirectURL": str,
         "FeedbackURL": str,
         "AttributesToDelete": Sequence[StackAttributeType],
         "UserSettings": Sequence[UserSettingTypeDef],
         "ApplicationSettings": ApplicationSettingsTypeDef,
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
```

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/type_defs.pyi` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_appstream.type_defs import AccessEndpointTypeDef
 
     data: AccessEndpointTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ActionType,
     AppBlockBuilderAttributeType,
     AppBlockBuilderStateType,
     AppBlockStateType,
     ApplicationAttributeType,
@@ -80,14 +80,15 @@
     "CopyImageRequestRequestTypeDef",
     "VpcConfigTypeDef",
     "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
+    "StorageConnectorOutputTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DeleteAppBlockBuilderRequestRequestTypeDef",
@@ -135,15 +136,14 @@
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "StackErrorTypeDef",
-    "StorageConnectorOutputTypeDef",
     "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
     "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -552,14 +552,34 @@
 
 class CreateImageBuilderStreamingURLRequestRequestTypeDef(
     _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef,
     _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef,
 ):
     pass
 
+_RequiredStorageConnectorOutputTypeDef = TypedDict(
+    "_RequiredStorageConnectorOutputTypeDef",
+    {
+        "ConnectorType": StorageConnectorTypeType,
+    },
+)
+_OptionalStorageConnectorOutputTypeDef = TypedDict(
+    "_OptionalStorageConnectorOutputTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "Domains": List[str],
+    },
+    total=False,
+)
+
+class StorageConnectorOutputTypeDef(
+    _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
+):
+    pass
+
 _RequiredStorageConnectorTypeDef = TypedDict(
     "_RequiredStorageConnectorTypeDef",
     {
         "ConnectorType": StorageConnectorTypeType,
     },
 )
 _OptionalStorageConnectorTypeDef = TypedDict(
@@ -1183,34 +1203,14 @@
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredStorageConnectorOutputTypeDef = TypedDict(
-    "_RequiredStorageConnectorOutputTypeDef",
-    {
-        "ConnectorType": StorageConnectorTypeType,
-    },
-)
-_OptionalStorageConnectorOutputTypeDef = TypedDict(
-    "_OptionalStorageConnectorOutputTypeDef",
-    {
-        "ResourceIdentifier": str,
-        "Domains": List[str],
-    },
-    total=False,
-)
-
-class StorageConnectorOutputTypeDef(
-    _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
-):
-    pass
-
 StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "StartAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1828,15 +1828,17 @@
     },
 )
 _OptionalCreateStackRequestRequestTypeDef = TypedDict(
     "_OptionalCreateStackRequestRequestTypeDef",
     {
         "Description": str,
         "DisplayName": str,
-        "StorageConnectors": Sequence[StorageConnectorTypeDef],
+        "StorageConnectors": Sequence[
+            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
+        ],
         "RedirectURL": str,
         "FeedbackURL": str,
         "UserSettings": Sequence[UserSettingTypeDef],
         "ApplicationSettings": ApplicationSettingsTypeDef,
         "Tags": Mapping[str, str],
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
         "EmbedHostDomains": Sequence[str],
@@ -1857,15 +1859,17 @@
     },
 )
 _OptionalUpdateStackRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateStackRequestRequestTypeDef",
     {
         "DisplayName": str,
         "Description": str,
-        "StorageConnectors": Sequence[StorageConnectorTypeDef],
+        "StorageConnectors": Sequence[
+            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
+        ],
         "DeleteStorageConnectors": bool,
         "RedirectURL": str,
         "FeedbackURL": str,
         "AttributesToDelete": Sequence[StackAttributeType],
         "UserSettings": Sequence[UserSettingTypeDef],
         "ApplicationSettings": ApplicationSettingsTypeDef,
         "AccessEndpoints": Sequence[AccessEndpointTypeDef],
```

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/waiter.py` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream/waiter.pyi` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/PKG-INFO` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.28.15
-Summary: Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -441,14 +441,15 @@
     CopyImageRequestRequestTypeDef,
     VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
+    StorageConnectorOutputTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DeleteAppBlockBuilderRequestRequestTypeDef,
@@ -496,15 +497,14 @@
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     StackErrorTypeDef,
-    StorageConnectorOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-appstream-1.28.15/mypy_boto3_appstream.egg-info/SOURCES.txt` & `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15/setup.py` & `mypy-boto3-appstream-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appstream",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_appstream"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder"
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

