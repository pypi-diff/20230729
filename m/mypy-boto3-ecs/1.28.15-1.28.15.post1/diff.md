# Comparing `tmp/mypy-boto3-ecs-1.28.15.tar.gz` & `tmp/mypy-boto3-ecs-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecs-1.28.15.tar", last modified: Fri Jul 28 20:42:43 2023, max compression
+gzip compressed data, was "mypy-boto3-ecs-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
```

## Comparing `mypy-boto3-ecs-1.28.15.tar` & `mypy-boto3-ecs-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.717040 mypy-boto3-ecs-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-07-28 20:42:43.717040 mypy-boto3-ecs-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23633 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.709040 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:24:51.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49914 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-28 20:24:53.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-07-28 20:24:53.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:24:51.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    95601 2023-07-28 20:24:56.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    95482 2023-07-28 20:24:54.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.717040 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.717040 mypy-boto3-ecs-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.501128 mypy-boto3-ecs-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-07-29 10:03:02.501128 mypy-boto3-ecs-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23633 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.485128 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51100 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51024 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-29 09:44:22.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-07-29 09:44:22.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    95722 2023-07-29 09:44:26.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95603 2023-07-29 09:44:23.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.501128 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.501128 mypy-boto3-ecs-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:44:20.000000 mypy-boto3-ecs-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-ecs-1.28.15/LICENSE` & `mypy-boto3-ecs-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15/PKG-INFO` & `mypy-boto3-ecs-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.28.15
-Summary: Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecs-1.28.15/README.md` & `mypy-boto3-ecs-1.28.15.post1/README.md`

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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__init__.py` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__init__.pyi` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__main__.py` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECS 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.ECS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\nOther"
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

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/client.py` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -52,27 +52,29 @@
     AttributeTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ClusterConfigurationTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterSettingTypeDef,
+    ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
     ContainerStateChangeTypeDef,
     CreateCapacityProviderResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateServiceResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteAccountSettingResponseTypeDef,
     DeleteAttributesResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
+    DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DeploymentControllerTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     DescribeClustersResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
@@ -94,75 +96,78 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LoadBalancerTypeDef,
     ManagedAgentStateChangeTypeDef,
     NetworkBindingTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     PlatformDeviceTypeDef,
+    ProxyConfigurationOutputTypeDef,
     ProxyConfigurationTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     PutAttributesResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     RunTaskResponseTypeDef,
     RuntimePlatformTypeDef,
     ScaleTypeDef,
+    ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     ServiceRegistryTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
     TagTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     VersionInfoTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
 )
 from .waiter import (
     ServicesInactiveWaiter,
     ServicesStableWaiter,
     TasksRunningWaiter,
     TasksStoppedWaiter,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ECSClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AttributeLimitExceededException: Type[BotocoreClientError]
     BlockedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ClientException: Type[BotocoreClientError]
     ClusterContainsContainerInstancesException: Type[BotocoreClientError]
@@ -183,15 +188,14 @@
     ServiceNotFoundException: Type[BotocoreClientError]
     TargetNotConnectedException: Type[BotocoreClientError]
     TargetNotFoundException: Type[BotocoreClientError]
     TaskSetNotFoundException: Type[BotocoreClientError]
     UnsupportedFeatureException: Type[BotocoreClientError]
     UpdateInProgressException: Type[BotocoreClientError]
 
-
 class ECSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/)
     """
 
     meta: ClientMeta
@@ -200,45 +204,41 @@
     def exceptions(self) -> Exceptions:
         """
         ECSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#close)
         """
-
     def create_capacity_provider(
         self,
         *,
         name: str,
         autoScalingGroupProvider: AutoScalingGroupProviderTypeDef,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateCapacityProviderResponseTypeDef:
         """
         Creates a new capacity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_capacity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_capacity_provider)
         """
-
     def create_cluster(
         self,
         *,
         clusterName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         settings: Sequence[ClusterSettingTypeDef] = ...,
         configuration: ClusterConfigurationTypeDef = ...,
@@ -248,58 +248,64 @@
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a new Amazon ECS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_cluster)
         """
-
     def create_service(
         self,
         *,
         serviceName: str,
         cluster: str = ...,
         taskDefinition: str = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         desiredCount: int = ...,
         clientToken: str = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         role: str = ...,
-        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
+        deploymentConfiguration: Union[
+            DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
+        ] = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
         enableExecuteCommand: bool = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: Union[
+            ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
+        ] = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_service)
         """
-
     def create_task_set(
         self,
         *,
         service: str,
         cluster: str,
         taskDefinition: str,
         externalId: str = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         scale: ScaleTypeDef = ...,
         clientToken: str = ...,
@@ -307,202 +313,184 @@
     ) -> CreateTaskSetResponseTypeDef:
         """
         Create a task set in the specified cluster and service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_task_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_task_set)
         """
-
     def delete_account_setting(
         self, *, name: SettingNameType, principalArn: str = ...
     ) -> DeleteAccountSettingResponseTypeDef:
         """
         Disables an account setting for a specified user, role, or the root user for an
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_account_setting)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_account_setting)
         """
-
     def delete_attributes(
         self, *, attributes: Sequence[AttributeTypeDef], cluster: str = ...
     ) -> DeleteAttributesResponseTypeDef:
         """
         Deletes one or more custom attributes from an Amazon ECS resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_attributes)
         """
-
     def delete_capacity_provider(
         self, *, capacityProvider: str
     ) -> DeleteCapacityProviderResponseTypeDef:
         """
         Deletes the specified capacity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_capacity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_capacity_provider)
         """
-
     def delete_cluster(self, *, cluster: str) -> DeleteClusterResponseTypeDef:
         """
         Deletes the specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_cluster)
         """
-
     def delete_service(
         self, *, service: str, cluster: str = ..., force: bool = ...
     ) -> DeleteServiceResponseTypeDef:
         """
         Deletes a specified service within a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_service)
         """
-
     def delete_task_definitions(
         self, *, taskDefinitions: Sequence[str]
     ) -> DeleteTaskDefinitionsResponseTypeDef:
         """
         Deletes one or more task definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_task_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_task_definitions)
         """
-
     def delete_task_set(
         self, *, cluster: str, service: str, taskSet: str, force: bool = ...
     ) -> DeleteTaskSetResponseTypeDef:
         """
         Deletes a specified task set within a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_task_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_task_set)
         """
-
     def deregister_container_instance(
         self, *, containerInstance: str, cluster: str = ..., force: bool = ...
     ) -> DeregisterContainerInstanceResponseTypeDef:
         """
         Deregisters an Amazon ECS container instance from the specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.deregister_container_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#deregister_container_instance)
         """
-
     def deregister_task_definition(
         self, *, taskDefinition: str
     ) -> DeregisterTaskDefinitionResponseTypeDef:
         """
         Deregisters the specified task definition by family and revision.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.deregister_task_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#deregister_task_definition)
         """
-
     def describe_capacity_providers(
         self,
         *,
         capacityProviders: Sequence[str] = ...,
         include: Sequence[Literal["TAGS"]] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeCapacityProvidersResponseTypeDef:
         """
         Describes one or more of your capacity providers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_capacity_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_capacity_providers)
         """
-
     def describe_clusters(
         self, *, clusters: Sequence[str] = ..., include: Sequence[ClusterFieldType] = ...
     ) -> DescribeClustersResponseTypeDef:
         """
         Describes one or more of your clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_clusters)
         """
-
     def describe_container_instances(
         self,
         *,
         containerInstances: Sequence[str],
         cluster: str = ...,
         include: Sequence[ContainerInstanceFieldType] = ...
     ) -> DescribeContainerInstancesResponseTypeDef:
         """
         Describes one or more container instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_container_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_container_instances)
         """
-
     def describe_services(
         self,
         *,
         services: Sequence[str],
         cluster: str = ...,
         include: Sequence[Literal["TAGS"]] = ...
     ) -> DescribeServicesResponseTypeDef:
         """
         Describes the specified services running in your cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_services)
         """
-
     def describe_task_definition(
         self, *, taskDefinition: str, include: Sequence[Literal["TAGS"]] = ...
     ) -> DescribeTaskDefinitionResponseTypeDef:
         """
         Describes a task definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_task_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_task_definition)
         """
-
     def describe_task_sets(
         self,
         *,
         cluster: str,
         service: str,
         taskSets: Sequence[str] = ...,
         include: Sequence[Literal["TAGS"]] = ...
     ) -> DescribeTaskSetsResponseTypeDef:
         """
         Describes the task sets in the specified cluster and service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_task_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_task_sets)
         """
-
     def describe_tasks(
         self, *, tasks: Sequence[str], cluster: str = ..., include: Sequence[Literal["TAGS"]] = ...
     ) -> DescribeTasksResponseTypeDef:
         """
         Describes a specified task or tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_tasks)
         """
-
     def discover_poll_endpoint(
         self, *, containerInstance: str = ..., cluster: str = ...
     ) -> DiscoverPollEndpointResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.discover_poll_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#discover_poll_endpoint)
         """
-
     def execute_command(
         self,
         *,
         command: str,
         interactive: bool,
         task: str,
         cluster: str = ...,
@@ -510,39 +498,36 @@
     ) -> ExecuteCommandResponseTypeDef:
         """
         Runs a command remotely on a container within a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.execute_command)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#execute_command)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#generate_presigned_url)
         """
-
     def get_task_protection(
         self, *, cluster: str, tasks: Sequence[str] = ...
     ) -> GetTaskProtectionResponseTypeDef:
         """
         Retrieves the protection status of tasks in an Amazon ECS service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_task_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_task_protection)
         """
-
     def list_account_settings(
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
@@ -551,15 +536,14 @@
     ) -> ListAccountSettingsResponseTypeDef:
         """
         Lists the account settings for a specified principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_account_settings)
         """
-
     def list_attributes(
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
@@ -569,25 +553,23 @@
         """
         Lists the attributes for Amazon ECS resources within a specified target type and
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_attributes)
         """
-
     def list_clusters(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListClustersResponseTypeDef:
         """
         Returns a list of existing clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_clusters)
         """
-
     def list_container_instances(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
@@ -595,15 +577,14 @@
     ) -> ListContainerInstancesResponseTypeDef:
         """
         Returns a list of container instances in a specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_container_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_container_instances)
         """
-
     def list_services(
         self,
         *,
         cluster: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         launchType: LaunchTypeType = ...,
@@ -611,49 +592,45 @@
     ) -> ListServicesResponseTypeDef:
         """
         Returns a list of services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_services)
         """
-
     def list_services_by_namespace(
         self, *, namespace: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListServicesByNamespaceResponseTypeDef:
         """
         This operation lists all of the services that are associated with a Cloud Map
         namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_services_by_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_services_by_namespace)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         List the tags for an Amazon ECS resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_tags_for_resource)
         """
-
     def list_task_definition_families(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListTaskDefinitionFamiliesResponseTypeDef:
         """
         Returns a list of task definition families that are registered to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_task_definition_families)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_task_definition_families)
         """
-
     def list_task_definitions(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
         nextToken: str = ...,
@@ -661,15 +638,14 @@
     ) -> ListTaskDefinitionsResponseTypeDef:
         """
         Returns a list of task definitions that are registered to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_task_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_task_definitions)
         """
-
     def list_tasks(
         self,
         *,
         cluster: str = ...,
         containerInstance: str = ...,
         family: str = ...,
         nextToken: str = ...,
@@ -681,182 +657,177 @@
     ) -> ListTasksResponseTypeDef:
         """
         Returns a list of tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_tasks)
         """
-
     def put_account_setting(
         self, *, name: SettingNameType, value: str, principalArn: str = ...
     ) -> PutAccountSettingResponseTypeDef:
         """
         Modifies an account setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_account_setting)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_account_setting)
         """
-
     def put_account_setting_default(
         self, *, name: SettingNameType, value: str
     ) -> PutAccountSettingDefaultResponseTypeDef:
         """
         Modifies an account setting for all users on an account for whom no individual
         account setting has been specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_account_setting_default)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_account_setting_default)
         """
-
     def put_attributes(
         self, *, attributes: Sequence[AttributeTypeDef], cluster: str = ...
     ) -> PutAttributesResponseTypeDef:
         """
         Create or update an attribute on an Amazon ECS resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_attributes)
         """
-
     def put_cluster_capacity_providers(
         self,
         *,
         cluster: str,
         capacityProviders: Sequence[str],
         defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef]
     ) -> PutClusterCapacityProvidersResponseTypeDef:
         """
         Modifies the available capacity providers and the default capacity provider
         strategy for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_cluster_capacity_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_cluster_capacity_providers)
         """
-
     def register_container_instance(
         self,
         *,
         cluster: str = ...,
         instanceIdentityDocument: str = ...,
         instanceIdentityDocumentSignature: str = ...,
-        totalResources: Sequence[ResourceTypeDef] = ...,
+        totalResources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]] = ...,
         versionInfo: VersionInfoTypeDef = ...,
         containerInstanceArn: str = ...,
         attributes: Sequence[AttributeTypeDef] = ...,
         platformDevices: Sequence[PlatformDeviceTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> RegisterContainerInstanceResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_container_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#register_container_instance)
         """
-
     def register_task_definition(
         self,
         *,
         family: str,
-        containerDefinitions: Sequence[ContainerDefinitionTypeDef],
+        containerDefinitions: Sequence[
+            Union[ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef]
+        ],
         taskRoleArn: str = ...,
         executionRoleArn: str = ...,
         networkMode: NetworkModeType = ...,
-        volumes: Sequence[VolumeTypeDef] = ...,
+        volumes: Sequence[Union[VolumeTypeDef, VolumeOutputTypeDef]] = ...,
         placementConstraints: Sequence[TaskDefinitionPlacementConstraintTypeDef] = ...,
         requiresCompatibilities: Sequence[CompatibilityType] = ...,
         cpu: str = ...,
         memory: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         pidMode: PidModeType = ...,
         ipcMode: IpcModeType = ...,
-        proxyConfiguration: ProxyConfigurationTypeDef = ...,
+        proxyConfiguration: Union[ProxyConfigurationTypeDef, ProxyConfigurationOutputTypeDef] = ...,
         inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,
         ephemeralStorage: EphemeralStorageTypeDef = ...,
         runtimePlatform: RuntimePlatformTypeDef = ...
     ) -> RegisterTaskDefinitionResponseTypeDef:
         """
         Registers a new task definition from the supplied `family` and
         `containerDefinitions`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_task_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#register_task_definition)
         """
-
     def run_task(
         self,
         *,
         taskDefinition: str,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         cluster: str = ...,
         count: int = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
         launchType: LaunchTypeType = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
-        overrides: TaskOverrideTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
+        overrides: Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef] = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> RunTaskResponseTypeDef:
         """
         Starts a new task using the specified task definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.run_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#run_task)
         """
-
     def start_task(
         self,
         *,
         containerInstances: Sequence[str],
         taskDefinition: str,
         cluster: str = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
-        overrides: TaskOverrideTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
+        overrides: Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartTaskResponseTypeDef:
         """
         Starts a new task from the specified task definition on the specified container
         instance or instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.start_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#start_task)
         """
-
     def stop_task(
         self, *, task: str, cluster: str = ..., reason: str = ...
     ) -> StopTaskResponseTypeDef:
         """
         Stops a running task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.stop_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#stop_task)
         """
-
     def submit_attachment_state_changes(
         self, *, attachments: Sequence[AttachmentStateChangeTypeDef], cluster: str = ...
     ) -> SubmitAttachmentStateChangesResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_attachment_state_changes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#submit_attachment_state_changes)
         """
-
     def submit_container_state_change(
         self,
         *,
         cluster: str = ...,
         task: str = ...,
         containerName: str = ...,
         runtimeId: str = ...,
@@ -867,15 +838,14 @@
     ) -> SubmitContainerStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_container_state_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#submit_container_state_change)
         """
-
     def submit_task_state_change(
         self,
         *,
         cluster: str = ...,
         task: str = ...,
         status: str = ...,
         reason: str = ...,
@@ -888,247 +858,229 @@
     ) -> SubmitTaskStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_task_state_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#submit_task_state_change)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Associates the specified tags to a resource with the specified `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes specified tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#untag_resource)
         """
-
     def update_capacity_provider(
         self, *, name: str, autoScalingGroupProvider: AutoScalingGroupProviderUpdateTypeDef
     ) -> UpdateCapacityProviderResponseTypeDef:
         """
         Modifies the parameters for a capacity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_capacity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_capacity_provider)
         """
-
     def update_cluster(
         self,
         *,
         cluster: str,
         settings: Sequence[ClusterSettingTypeDef] = ...,
         configuration: ClusterConfigurationTypeDef = ...,
         serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...
     ) -> UpdateClusterResponseTypeDef:
         """
         Updates the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_cluster)
         """
-
     def update_cluster_settings(
         self, *, cluster: str, settings: Sequence[ClusterSettingTypeDef]
     ) -> UpdateClusterSettingsResponseTypeDef:
         """
         Modifies the settings to use for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_cluster_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_cluster_settings)
         """
-
     def update_container_agent(
         self, *, containerInstance: str, cluster: str = ...
     ) -> UpdateContainerAgentResponseTypeDef:
         """
         Updates the Amazon ECS container agent on a specified container instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_container_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_container_agent)
         """
-
     def update_container_instances_state(
         self,
         *,
         containerInstances: Sequence[str],
         status: ContainerInstanceStatusType,
         cluster: str = ...
     ) -> UpdateContainerInstancesStateResponseTypeDef:
         """
         Modifies the status of an Amazon ECS container instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_container_instances_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_container_instances_state)
         """
-
     def update_service(
         self,
         *,
         service: str,
         cluster: str = ...,
         desiredCount: int = ...,
         taskDefinition: str = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
-        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        deploymentConfiguration: Union[
+            DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
+        ] = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: Union[
+            ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
+        ] = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_service)
         """
-
     def update_service_primary_task_set(
         self, *, cluster: str, service: str, primaryTaskSet: str
     ) -> UpdateServicePrimaryTaskSetResponseTypeDef:
         """
         Modifies which task set in a service is the primary task set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service_primary_task_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_service_primary_task_set)
         """
-
     def update_task_protection(
         self,
         *,
         cluster: str,
         tasks: Sequence[str],
         protectionEnabled: bool,
         expiresInMinutes: int = ...
     ) -> UpdateTaskProtectionResponseTypeDef:
         """
         Updates the protection status of a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_task_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_task_protection)
         """
-
     def update_task_set(
         self, *, cluster: str, service: str, taskSet: str, scale: ScaleTypeDef
     ) -> UpdateTaskSetResponseTypeDef:
         """
         Modifies a task set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_task_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_task_set)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_account_settings"]
     ) -> ListAccountSettingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_attributes"]) -> ListAttributesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_clusters"]) -> ListClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_container_instances"]
     ) -> ListContainerInstancesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_services_by_namespace"]
     ) -> ListServicesByNamespacePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_task_definition_families"]
     ) -> ListTaskDefinitionFamiliesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_task_definitions"]
     ) -> ListTaskDefinitionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_tasks"]) -> ListTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["services_inactive"]) -> ServicesInactiveWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["services_stable"]) -> ServicesStableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["tasks_running"]) -> TasksRunningWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["tasks_stopped"]) -> TasksStoppedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/client.pyi` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,27 +52,29 @@
     AttributeTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ClusterConfigurationTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterSettingTypeDef,
+    ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
     ContainerStateChangeTypeDef,
     CreateCapacityProviderResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateServiceResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteAccountSettingResponseTypeDef,
     DeleteAttributesResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
+    DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DeploymentControllerTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     DescribeClustersResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
@@ -94,72 +96,81 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LoadBalancerTypeDef,
     ManagedAgentStateChangeTypeDef,
     NetworkBindingTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     PlatformDeviceTypeDef,
+    ProxyConfigurationOutputTypeDef,
     ProxyConfigurationTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     PutAttributesResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     RunTaskResponseTypeDef,
     RuntimePlatformTypeDef,
     ScaleTypeDef,
+    ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     ServiceRegistryTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
     TagTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     VersionInfoTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
 )
 from .waiter import (
     ServicesInactiveWaiter,
     ServicesStableWaiter,
     TasksRunningWaiter,
     TasksStoppedWaiter,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ECSClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AttributeLimitExceededException: Type[BotocoreClientError]
     BlockedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ClientException: Type[BotocoreClientError]
     ClusterContainsContainerInstancesException: Type[BotocoreClientError]
@@ -180,14 +191,15 @@
     ServiceNotFoundException: Type[BotocoreClientError]
     TargetNotConnectedException: Type[BotocoreClientError]
     TargetNotFoundException: Type[BotocoreClientError]
     TaskSetNotFoundException: Type[BotocoreClientError]
     UnsupportedFeatureException: Type[BotocoreClientError]
     UpdateInProgressException: Type[BotocoreClientError]
 
+
 class ECSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/)
     """
 
     meta: ClientMeta
@@ -196,41 +208,45 @@
     def exceptions(self) -> Exceptions:
         """
         ECSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#close)
         """
+
     def create_capacity_provider(
         self,
         *,
         name: str,
         autoScalingGroupProvider: AutoScalingGroupProviderTypeDef,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateCapacityProviderResponseTypeDef:
         """
         Creates a new capacity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_capacity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_capacity_provider)
         """
+
     def create_cluster(
         self,
         *,
         clusterName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         settings: Sequence[ClusterSettingTypeDef] = ...,
         configuration: ClusterConfigurationTypeDef = ...,
@@ -240,56 +256,66 @@
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a new Amazon ECS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_cluster)
         """
+
     def create_service(
         self,
         *,
         serviceName: str,
         cluster: str = ...,
         taskDefinition: str = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         desiredCount: int = ...,
         clientToken: str = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         role: str = ...,
-        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
+        deploymentConfiguration: Union[
+            DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
+        ] = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
         enableExecuteCommand: bool = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: Union[
+            ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
+        ] = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_service)
         """
+
     def create_task_set(
         self,
         *,
         service: str,
         cluster: str,
         taskDefinition: str,
         externalId: str = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         scale: ScaleTypeDef = ...,
         clientToken: str = ...,
@@ -297,184 +323,202 @@
     ) -> CreateTaskSetResponseTypeDef:
         """
         Create a task set in the specified cluster and service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_task_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_task_set)
         """
+
     def delete_account_setting(
         self, *, name: SettingNameType, principalArn: str = ...
     ) -> DeleteAccountSettingResponseTypeDef:
         """
         Disables an account setting for a specified user, role, or the root user for an
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_account_setting)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_account_setting)
         """
+
     def delete_attributes(
         self, *, attributes: Sequence[AttributeTypeDef], cluster: str = ...
     ) -> DeleteAttributesResponseTypeDef:
         """
         Deletes one or more custom attributes from an Amazon ECS resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_attributes)
         """
+
     def delete_capacity_provider(
         self, *, capacityProvider: str
     ) -> DeleteCapacityProviderResponseTypeDef:
         """
         Deletes the specified capacity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_capacity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_capacity_provider)
         """
+
     def delete_cluster(self, *, cluster: str) -> DeleteClusterResponseTypeDef:
         """
         Deletes the specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_cluster)
         """
+
     def delete_service(
         self, *, service: str, cluster: str = ..., force: bool = ...
     ) -> DeleteServiceResponseTypeDef:
         """
         Deletes a specified service within a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_service)
         """
+
     def delete_task_definitions(
         self, *, taskDefinitions: Sequence[str]
     ) -> DeleteTaskDefinitionsResponseTypeDef:
         """
         Deletes one or more task definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_task_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_task_definitions)
         """
+
     def delete_task_set(
         self, *, cluster: str, service: str, taskSet: str, force: bool = ...
     ) -> DeleteTaskSetResponseTypeDef:
         """
         Deletes a specified task set within a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_task_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_task_set)
         """
+
     def deregister_container_instance(
         self, *, containerInstance: str, cluster: str = ..., force: bool = ...
     ) -> DeregisterContainerInstanceResponseTypeDef:
         """
         Deregisters an Amazon ECS container instance from the specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.deregister_container_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#deregister_container_instance)
         """
+
     def deregister_task_definition(
         self, *, taskDefinition: str
     ) -> DeregisterTaskDefinitionResponseTypeDef:
         """
         Deregisters the specified task definition by family and revision.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.deregister_task_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#deregister_task_definition)
         """
+
     def describe_capacity_providers(
         self,
         *,
         capacityProviders: Sequence[str] = ...,
         include: Sequence[Literal["TAGS"]] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeCapacityProvidersResponseTypeDef:
         """
         Describes one or more of your capacity providers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_capacity_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_capacity_providers)
         """
+
     def describe_clusters(
         self, *, clusters: Sequence[str] = ..., include: Sequence[ClusterFieldType] = ...
     ) -> DescribeClustersResponseTypeDef:
         """
         Describes one or more of your clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_clusters)
         """
+
     def describe_container_instances(
         self,
         *,
         containerInstances: Sequence[str],
         cluster: str = ...,
         include: Sequence[ContainerInstanceFieldType] = ...
     ) -> DescribeContainerInstancesResponseTypeDef:
         """
         Describes one or more container instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_container_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_container_instances)
         """
+
     def describe_services(
         self,
         *,
         services: Sequence[str],
         cluster: str = ...,
         include: Sequence[Literal["TAGS"]] = ...
     ) -> DescribeServicesResponseTypeDef:
         """
         Describes the specified services running in your cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_services)
         """
+
     def describe_task_definition(
         self, *, taskDefinition: str, include: Sequence[Literal["TAGS"]] = ...
     ) -> DescribeTaskDefinitionResponseTypeDef:
         """
         Describes a task definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_task_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_task_definition)
         """
+
     def describe_task_sets(
         self,
         *,
         cluster: str,
         service: str,
         taskSets: Sequence[str] = ...,
         include: Sequence[Literal["TAGS"]] = ...
     ) -> DescribeTaskSetsResponseTypeDef:
         """
         Describes the task sets in the specified cluster and service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_task_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_task_sets)
         """
+
     def describe_tasks(
         self, *, tasks: Sequence[str], cluster: str = ..., include: Sequence[Literal["TAGS"]] = ...
     ) -> DescribeTasksResponseTypeDef:
         """
         Describes a specified task or tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.describe_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#describe_tasks)
         """
+
     def discover_poll_endpoint(
         self, *, containerInstance: str = ..., cluster: str = ...
     ) -> DiscoverPollEndpointResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.discover_poll_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#discover_poll_endpoint)
         """
+
     def execute_command(
         self,
         *,
         command: str,
         interactive: bool,
         task: str,
         cluster: str = ...,
@@ -482,36 +526,39 @@
     ) -> ExecuteCommandResponseTypeDef:
         """
         Runs a command remotely on a container within a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.execute_command)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#execute_command)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#generate_presigned_url)
         """
+
     def get_task_protection(
         self, *, cluster: str, tasks: Sequence[str] = ...
     ) -> GetTaskProtectionResponseTypeDef:
         """
         Retrieves the protection status of tasks in an Amazon ECS service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_task_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_task_protection)
         """
+
     def list_account_settings(
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
@@ -520,14 +567,15 @@
     ) -> ListAccountSettingsResponseTypeDef:
         """
         Lists the account settings for a specified principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_account_settings)
         """
+
     def list_attributes(
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
@@ -537,23 +585,25 @@
         """
         Lists the attributes for Amazon ECS resources within a specified target type and
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_attributes)
         """
+
     def list_clusters(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListClustersResponseTypeDef:
         """
         Returns a list of existing clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_clusters)
         """
+
     def list_container_instances(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
@@ -561,14 +611,15 @@
     ) -> ListContainerInstancesResponseTypeDef:
         """
         Returns a list of container instances in a specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_container_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_container_instances)
         """
+
     def list_services(
         self,
         *,
         cluster: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         launchType: LaunchTypeType = ...,
@@ -576,45 +627,49 @@
     ) -> ListServicesResponseTypeDef:
         """
         Returns a list of services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_services)
         """
+
     def list_services_by_namespace(
         self, *, namespace: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListServicesByNamespaceResponseTypeDef:
         """
         This operation lists all of the services that are associated with a Cloud Map
         namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_services_by_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_services_by_namespace)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         List the tags for an Amazon ECS resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_tags_for_resource)
         """
+
     def list_task_definition_families(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListTaskDefinitionFamiliesResponseTypeDef:
         """
         Returns a list of task definition families that are registered to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_task_definition_families)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_task_definition_families)
         """
+
     def list_task_definitions(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
         nextToken: str = ...,
@@ -622,14 +677,15 @@
     ) -> ListTaskDefinitionsResponseTypeDef:
         """
         Returns a list of task definitions that are registered to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_task_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_task_definitions)
         """
+
     def list_tasks(
         self,
         *,
         cluster: str = ...,
         containerInstance: str = ...,
         family: str = ...,
         nextToken: str = ...,
@@ -641,171 +697,188 @@
     ) -> ListTasksResponseTypeDef:
         """
         Returns a list of tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_tasks)
         """
+
     def put_account_setting(
         self, *, name: SettingNameType, value: str, principalArn: str = ...
     ) -> PutAccountSettingResponseTypeDef:
         """
         Modifies an account setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_account_setting)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_account_setting)
         """
+
     def put_account_setting_default(
         self, *, name: SettingNameType, value: str
     ) -> PutAccountSettingDefaultResponseTypeDef:
         """
         Modifies an account setting for all users on an account for whom no individual
         account setting has been specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_account_setting_default)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_account_setting_default)
         """
+
     def put_attributes(
         self, *, attributes: Sequence[AttributeTypeDef], cluster: str = ...
     ) -> PutAttributesResponseTypeDef:
         """
         Create or update an attribute on an Amazon ECS resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_attributes)
         """
+
     def put_cluster_capacity_providers(
         self,
         *,
         cluster: str,
         capacityProviders: Sequence[str],
         defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef]
     ) -> PutClusterCapacityProvidersResponseTypeDef:
         """
         Modifies the available capacity providers and the default capacity provider
         strategy for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_cluster_capacity_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_cluster_capacity_providers)
         """
+
     def register_container_instance(
         self,
         *,
         cluster: str = ...,
         instanceIdentityDocument: str = ...,
         instanceIdentityDocumentSignature: str = ...,
-        totalResources: Sequence[ResourceTypeDef] = ...,
+        totalResources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]] = ...,
         versionInfo: VersionInfoTypeDef = ...,
         containerInstanceArn: str = ...,
         attributes: Sequence[AttributeTypeDef] = ...,
         platformDevices: Sequence[PlatformDeviceTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> RegisterContainerInstanceResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_container_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#register_container_instance)
         """
+
     def register_task_definition(
         self,
         *,
         family: str,
-        containerDefinitions: Sequence[ContainerDefinitionTypeDef],
+        containerDefinitions: Sequence[
+            Union[ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef]
+        ],
         taskRoleArn: str = ...,
         executionRoleArn: str = ...,
         networkMode: NetworkModeType = ...,
-        volumes: Sequence[VolumeTypeDef] = ...,
+        volumes: Sequence[Union[VolumeTypeDef, VolumeOutputTypeDef]] = ...,
         placementConstraints: Sequence[TaskDefinitionPlacementConstraintTypeDef] = ...,
         requiresCompatibilities: Sequence[CompatibilityType] = ...,
         cpu: str = ...,
         memory: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         pidMode: PidModeType = ...,
         ipcMode: IpcModeType = ...,
-        proxyConfiguration: ProxyConfigurationTypeDef = ...,
+        proxyConfiguration: Union[ProxyConfigurationTypeDef, ProxyConfigurationOutputTypeDef] = ...,
         inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,
         ephemeralStorage: EphemeralStorageTypeDef = ...,
         runtimePlatform: RuntimePlatformTypeDef = ...
     ) -> RegisterTaskDefinitionResponseTypeDef:
         """
         Registers a new task definition from the supplied `family` and
         `containerDefinitions`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_task_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#register_task_definition)
         """
+
     def run_task(
         self,
         *,
         taskDefinition: str,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         cluster: str = ...,
         count: int = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
         launchType: LaunchTypeType = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
-        overrides: TaskOverrideTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
+        overrides: Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef] = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> RunTaskResponseTypeDef:
         """
         Starts a new task using the specified task definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.run_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#run_task)
         """
+
     def start_task(
         self,
         *,
         containerInstances: Sequence[str],
         taskDefinition: str,
         cluster: str = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
-        overrides: TaskOverrideTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
+        overrides: Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartTaskResponseTypeDef:
         """
         Starts a new task from the specified task definition on the specified container
         instance or instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.start_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#start_task)
         """
+
     def stop_task(
         self, *, task: str, cluster: str = ..., reason: str = ...
     ) -> StopTaskResponseTypeDef:
         """
         Stops a running task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.stop_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#stop_task)
         """
+
     def submit_attachment_state_changes(
         self, *, attachments: Sequence[AttachmentStateChangeTypeDef], cluster: str = ...
     ) -> SubmitAttachmentStateChangesResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_attachment_state_changes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#submit_attachment_state_changes)
         """
+
     def submit_container_state_change(
         self,
         *,
         cluster: str = ...,
         task: str = ...,
         containerName: str = ...,
         runtimeId: str = ...,
@@ -816,14 +889,15 @@
     ) -> SubmitContainerStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_container_state_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#submit_container_state_change)
         """
+
     def submit_task_state_change(
         self,
         *,
         cluster: str = ...,
         task: str = ...,
         status: str = ...,
         reason: str = ...,
@@ -836,223 +910,253 @@
     ) -> SubmitTaskStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_task_state_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#submit_task_state_change)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Associates the specified tags to a resource with the specified `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes specified tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#untag_resource)
         """
+
     def update_capacity_provider(
         self, *, name: str, autoScalingGroupProvider: AutoScalingGroupProviderUpdateTypeDef
     ) -> UpdateCapacityProviderResponseTypeDef:
         """
         Modifies the parameters for a capacity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_capacity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_capacity_provider)
         """
+
     def update_cluster(
         self,
         *,
         cluster: str,
         settings: Sequence[ClusterSettingTypeDef] = ...,
         configuration: ClusterConfigurationTypeDef = ...,
         serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...
     ) -> UpdateClusterResponseTypeDef:
         """
         Updates the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_cluster)
         """
+
     def update_cluster_settings(
         self, *, cluster: str, settings: Sequence[ClusterSettingTypeDef]
     ) -> UpdateClusterSettingsResponseTypeDef:
         """
         Modifies the settings to use for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_cluster_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_cluster_settings)
         """
+
     def update_container_agent(
         self, *, containerInstance: str, cluster: str = ...
     ) -> UpdateContainerAgentResponseTypeDef:
         """
         Updates the Amazon ECS container agent on a specified container instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_container_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_container_agent)
         """
+
     def update_container_instances_state(
         self,
         *,
         containerInstances: Sequence[str],
         status: ContainerInstanceStatusType,
         cluster: str = ...
     ) -> UpdateContainerInstancesStateResponseTypeDef:
         """
         Modifies the status of an Amazon ECS container instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_container_instances_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_container_instances_state)
         """
+
     def update_service(
         self,
         *,
         service: str,
         cluster: str = ...,
         desiredCount: int = ...,
         taskDefinition: str = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
-        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        deploymentConfiguration: Union[
+            DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
+        ] = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: Union[
+            ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
+        ] = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_service)
         """
+
     def update_service_primary_task_set(
         self, *, cluster: str, service: str, primaryTaskSet: str
     ) -> UpdateServicePrimaryTaskSetResponseTypeDef:
         """
         Modifies which task set in a service is the primary task set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service_primary_task_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_service_primary_task_set)
         """
+
     def update_task_protection(
         self,
         *,
         cluster: str,
         tasks: Sequence[str],
         protectionEnabled: bool,
         expiresInMinutes: int = ...
     ) -> UpdateTaskProtectionResponseTypeDef:
         """
         Updates the protection status of a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_task_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_task_protection)
         """
+
     def update_task_set(
         self, *, cluster: str, service: str, taskSet: str, scale: ScaleTypeDef
     ) -> UpdateTaskSetResponseTypeDef:
         """
         Modifies a task set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_task_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_task_set)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_account_settings"]
     ) -> ListAccountSettingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_attributes"]) -> ListAttributesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_clusters"]) -> ListClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_container_instances"]
     ) -> ListContainerInstancesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_services_by_namespace"]
     ) -> ListServicesByNamespacePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_task_definition_families"]
     ) -> ListTaskDefinitionFamiliesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_task_definitions"]
     ) -> ListTaskDefinitionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_tasks"]) -> ListTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["services_inactive"]) -> ServicesInactiveWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["services_stable"]) -> ServicesStableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["tasks_running"]) -> TasksRunningWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["tasks_stopped"]) -> TasksStoppedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/literals.py` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/literals.pyi` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/paginator.py` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/paginator.pyi` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/type_defs.py` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2575,15 +2575,15 @@
 
 RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
     "RegisterContainerInstanceRequestRequestTypeDef",
     {
         "cluster": str,
         "instanceIdentityDocument": str,
         "instanceIdentityDocumentSignature": str,
-        "totalResources": Sequence[ResourceTypeDef],
+        "totalResources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
         "versionInfo": VersionInfoTypeDef,
         "containerInstanceArn": str,
         "attributes": Sequence[AttributeTypeDef],
         "platformDevices": Sequence[PlatformDeviceTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
@@ -3304,24 +3304,26 @@
     total=False,
 )
 
 _RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
     {
         "family": str,
-        "containerDefinitions": Sequence[ContainerDefinitionTypeDef],
+        "containerDefinitions": Sequence[
+            Union[ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef]
+        ],
     },
 )
 _OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
     {
         "taskRoleArn": str,
         "executionRoleArn": str,
         "networkMode": NetworkModeType,
-        "volumes": Sequence[VolumeTypeDef],
+        "volumes": Sequence[Union[VolumeTypeDef, VolumeOutputTypeDef]],
         "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
         "requiresCompatibilities": Sequence[CompatibilityType],
         "cpu": str,
         "memory": str,
         "tags": Sequence[TagTypeDef],
         "pidMode": PidModeType,
         "ipcMode": IpcModeType,
```

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/type_defs.pyi` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2480,15 +2480,15 @@
 
 RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
     "RegisterContainerInstanceRequestRequestTypeDef",
     {
         "cluster": str,
         "instanceIdentityDocument": str,
         "instanceIdentityDocumentSignature": str,
-        "totalResources": Sequence[ResourceTypeDef],
+        "totalResources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
         "versionInfo": VersionInfoTypeDef,
         "containerInstanceArn": str,
         "attributes": Sequence[AttributeTypeDef],
         "platformDevices": Sequence[PlatformDeviceTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
@@ -3191,24 +3191,26 @@
     total=False,
 )
 
 _RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
     {
         "family": str,
-        "containerDefinitions": Sequence[ContainerDefinitionTypeDef],
+        "containerDefinitions": Sequence[
+            Union[ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef]
+        ],
     },
 )
 _OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
     {
         "taskRoleArn": str,
         "executionRoleArn": str,
         "networkMode": NetworkModeType,
-        "volumes": Sequence[VolumeTypeDef],
+        "volumes": Sequence[Union[VolumeTypeDef, VolumeOutputTypeDef]],
         "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
         "requiresCompatibilities": Sequence[CompatibilityType],
         "cpu": str,
         "memory": str,
         "tags": Sequence[TagTypeDef],
         "pidMode": PidModeType,
         "ipcMode": IpcModeType,
```

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/waiter.py` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/waiter.pyi` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/PKG-INFO` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.28.15
-Summary: Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/SOURCES.txt` & `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15/setup.py` & `mypy-boto3-ecs-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecs",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

