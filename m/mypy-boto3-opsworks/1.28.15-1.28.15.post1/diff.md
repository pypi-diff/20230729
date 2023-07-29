# Comparing `tmp/mypy-boto3-opsworks-1.28.15.tar.gz` & `tmp/mypy-boto3-opsworks-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opsworks-1.28.15.tar", last modified: Fri Jul 28 20:43:24 2023, max compression
+gzip compressed data, was "mypy-boto3-opsworks-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:48 2023, max compression
```

## Comparing `mypy-boto3-opsworks-1.28.15.tar` & `mypy-boto3-opsworks-1.28.15.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.489600 mypy-boto3-opsworks-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-07-28 20:43:24.489600 mypy-boto3-opsworks-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21429 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.489600 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51761 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51673 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    65356 2023-07-28 20:32:59.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65287 2023-07-28 20:32:58.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.489600 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:24.489600 mypy-boto3-opsworks-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:48.437318 mypy-boto3-opsworks-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22926 2023-07-29 10:03:48.433318 mypy-boto3-opsworks-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21429 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:48.429318 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52378 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52290 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    65372 2023-07-29 09:52:39.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65303 2023-07-29 09:52:38.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:48.433318 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22926 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:48.437318 mypy-boto3-opsworks-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-opsworks-1.28.15/LICENSE` & `mypy-boto3-opsworks-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/PKG-INFO` & `mypy-boto3-opsworks-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.28.15
-Summary: Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -455,14 +455,15 @@
     AutoScalingThresholdsTypeDef,
     EbsBlockDeviceTypeDef,
     ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
     DeploymentCommandTypeDef,
+    RecipesTypeDef,
     VolumeConfigurationTypeDef,
     CreateUserProfileRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
@@ -554,15 +555,14 @@
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DescribeStackProvisioningParametersResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionResultTypeDef,
     InstancesCountResponseTypeDef,
     ListTagsResultTypeDef,
-    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceResponseTypeDef,
     StackConfigurationManagerResponseTypeDef,
     CloneStackRequestRequestTypeDef,
```

### Comparing `mypy-boto3-opsworks-1.28.15/README.md` & `mypy-boto3-opsworks-1.28.15.post1/README.md`

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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,14 +423,15 @@
     AutoScalingThresholdsTypeDef,
     EbsBlockDeviceTypeDef,
     ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
     DeploymentCommandTypeDef,
+    RecipesTypeDef,
     VolumeConfigurationTypeDef,
     CreateUserProfileRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
@@ -522,15 +523,14 @@
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DescribeStackProvisioningParametersResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionResultTypeDef,
     InstancesCountResponseTypeDef,
     ListTagsResultTypeDef,
-    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceResponseTypeDef,
     StackConfigurationManagerResponseTypeDef,
     CloneStackRequestRequestTypeDef,
```

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__init__.py` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__init__.pyi` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__main__.py` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpsWorks 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.OpsWorks 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks\nOther"
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

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/client.py` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,41 +10,44 @@
     from mypy_boto3_opsworks.client import OpsWorksClient
 
     session = Session()
     client: OpsWorksClient = session.client("opsworks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppAttributesKeysType,
     AppTypeType,
     ArchitectureType,
     AutoScalingTypeType,
     LayerAttributesKeysType,
     LayerTypeType,
     RootDeviceTypeType,
 )
 from .paginator import DescribeEcsClustersPaginator
 from .type_defs import (
+    AutoScalingThresholdsOutputTypeDef,
     AutoScalingThresholdsTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationTypeDef,
     CloneStackResultTypeDef,
+    CloudWatchLogsConfigurationOutputTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DataSourceTypeDef,
+    DeploymentCommandOutputTypeDef,
     DeploymentCommandTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeCommandsResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
@@ -67,23 +70,25 @@
     EmptyResponseMetadataTypeDef,
     EnvironmentVariableTypeDef,
     GetHostnameSuggestionResultTypeDef,
     GrantAccessResultTypeDef,
     InstanceIdentityTypeDef,
     LifecycleEventConfigurationTypeDef,
     ListTagsResultTypeDef,
+    RecipesOutputTypeDef,
     RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceTypeDef,
     SslConfigurationTypeDef,
     StackConfigurationManagerTypeDef,
     VolumeConfigurationTypeDef,
+    WeeklyAutoScalingScheduleOutputTypeDef,
     WeeklyAutoScalingScheduleTypeDef,
 )
 from .waiter import (
     AppExistsWaiter,
     DeploymentSuccessfulWaiter,
     InstanceOnlineWaiter,
     InstanceRegisteredWaiter,
@@ -245,15 +250,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_app)
         """
 
     def create_deployment(
         self,
         *,
         StackId: str,
-        Command: DeploymentCommandTypeDef,
+        Command: Union[DeploymentCommandTypeDef, DeploymentCommandOutputTypeDef],
         AppId: str = ...,
         InstanceIds: Sequence[str] = ...,
         LayerIds: Sequence[str] = ...,
         Comment: str = ...,
         CustomJson: str = ...
     ) -> CreateDeploymentResultTypeDef:
         """
@@ -296,24 +301,26 @@
         self,
         *,
         StackId: str,
         Type: LayerTypeType,
         Name: str,
         Shortname: str,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
+        CloudWatchLogsConfiguration: Union[
+            CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
+        ] = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesTypeDef = ...,
+        CustomRecipes: Union[RecipesTypeDef, RecipesOutputTypeDef] = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> CreateLayerResultTypeDef:
         """
         Creates a layer.
 
@@ -803,16 +810,16 @@
         """
 
     def set_load_based_auto_scaling(
         self,
         *,
         LayerId: str,
         Enable: bool = ...,
-        UpScaling: AutoScalingThresholdsTypeDef = ...,
-        DownScaling: AutoScalingThresholdsTypeDef = ...
+        UpScaling: Union[AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef] = ...,
+        DownScaling: Union[AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the load-based auto scaling configuration for a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_load_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_load_based_auto_scaling)
         """
@@ -830,15 +837,20 @@
         Specifies a user's permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_permission)
         """
 
     def set_time_based_auto_scaling(
-        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleTypeDef = ...
+        self,
+        *,
+        InstanceId: str,
+        AutoScalingSchedule: Union[
+            WeeklyAutoScalingScheduleTypeDef, WeeklyAutoScalingScheduleOutputTypeDef
+        ] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the time-based auto scaling configuration for a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_time_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_time_based_auto_scaling)
         """
@@ -967,24 +979,26 @@
     def update_layer(
         self,
         *,
         LayerId: str,
         Name: str = ...,
         Shortname: str = ...,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
+        CloudWatchLogsConfiguration: Union[
+            CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
+        ] = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesTypeDef = ...,
+        CustomRecipes: Union[RecipesTypeDef, RecipesOutputTypeDef] = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified layer.
```

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/client.pyi` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,41 +10,44 @@
     from mypy_boto3_opsworks.client import OpsWorksClient
 
     session = Session()
     client: OpsWorksClient = session.client("opsworks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppAttributesKeysType,
     AppTypeType,
     ArchitectureType,
     AutoScalingTypeType,
     LayerAttributesKeysType,
     LayerTypeType,
     RootDeviceTypeType,
 )
 from .paginator import DescribeEcsClustersPaginator
 from .type_defs import (
+    AutoScalingThresholdsOutputTypeDef,
     AutoScalingThresholdsTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationTypeDef,
     CloneStackResultTypeDef,
+    CloudWatchLogsConfigurationOutputTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DataSourceTypeDef,
+    DeploymentCommandOutputTypeDef,
     DeploymentCommandTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeCommandsResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
@@ -67,23 +70,25 @@
     EmptyResponseMetadataTypeDef,
     EnvironmentVariableTypeDef,
     GetHostnameSuggestionResultTypeDef,
     GrantAccessResultTypeDef,
     InstanceIdentityTypeDef,
     LifecycleEventConfigurationTypeDef,
     ListTagsResultTypeDef,
+    RecipesOutputTypeDef,
     RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceTypeDef,
     SslConfigurationTypeDef,
     StackConfigurationManagerTypeDef,
     VolumeConfigurationTypeDef,
+    WeeklyAutoScalingScheduleOutputTypeDef,
     WeeklyAutoScalingScheduleTypeDef,
 )
 from .waiter import (
     AppExistsWaiter,
     DeploymentSuccessfulWaiter,
     InstanceOnlineWaiter,
     InstanceRegisteredWaiter,
@@ -232,15 +237,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_app)
         """
     def create_deployment(
         self,
         *,
         StackId: str,
-        Command: DeploymentCommandTypeDef,
+        Command: Union[DeploymentCommandTypeDef, DeploymentCommandOutputTypeDef],
         AppId: str = ...,
         InstanceIds: Sequence[str] = ...,
         LayerIds: Sequence[str] = ...,
         Comment: str = ...,
         CustomJson: str = ...
     ) -> CreateDeploymentResultTypeDef:
         """
@@ -281,24 +286,26 @@
         self,
         *,
         StackId: str,
         Type: LayerTypeType,
         Name: str,
         Shortname: str,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
+        CloudWatchLogsConfiguration: Union[
+            CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
+        ] = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesTypeDef = ...,
+        CustomRecipes: Union[RecipesTypeDef, RecipesOutputTypeDef] = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> CreateLayerResultTypeDef:
         """
         Creates a layer.
 
@@ -741,16 +748,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#register_volume)
         """
     def set_load_based_auto_scaling(
         self,
         *,
         LayerId: str,
         Enable: bool = ...,
-        UpScaling: AutoScalingThresholdsTypeDef = ...,
-        DownScaling: AutoScalingThresholdsTypeDef = ...
+        UpScaling: Union[AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef] = ...,
+        DownScaling: Union[AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the load-based auto scaling configuration for a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_load_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_load_based_auto_scaling)
         """
@@ -766,15 +773,20 @@
         """
         Specifies a user's permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_permission)
         """
     def set_time_based_auto_scaling(
-        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleTypeDef = ...
+        self,
+        *,
+        InstanceId: str,
+        AutoScalingSchedule: Union[
+            WeeklyAutoScalingScheduleTypeDef, WeeklyAutoScalingScheduleOutputTypeDef
+        ] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the time-based auto scaling configuration for a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_time_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_time_based_auto_scaling)
         """
@@ -891,24 +903,26 @@
     def update_layer(
         self,
         *,
         LayerId: str,
         Name: str = ...,
         Shortname: str = ...,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
+        CloudWatchLogsConfiguration: Union[
+            CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
+        ] = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesTypeDef = ...,
+        CustomRecipes: Union[RecipesTypeDef, RecipesOutputTypeDef] = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified layer.
```

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/literals.py` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/literals.pyi` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/paginator.py` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/paginator.pyi` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/service_resource.py` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/service_resource.pyi` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/type_defs.py` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "AutoScalingThresholdsTypeDef",
     "EbsBlockDeviceTypeDef",
     "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
     "DeploymentCommandTypeDef",
+    "RecipesTypeDef",
     "VolumeConfigurationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
@@ -154,15 +155,14 @@
     "CreateStackResultTypeDef",
     "CreateUserProfileResultTypeDef",
     "DescribeStackProvisioningParametersResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionResultTypeDef",
     "InstancesCountResponseTypeDef",
     "ListTagsResultTypeDef",
-    "RecipesTypeDef",
     "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpResultTypeDef",
     "RegisterInstanceResultTypeDef",
     "RegisterVolumeResultTypeDef",
     "SourceResponseTypeDef",
     "StackConfigurationManagerResponseTypeDef",
     "CloneStackRequestRequestTypeDef",
@@ -463,14 +463,26 @@
 
 class DeploymentCommandTypeDef(
     _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
 ):
     pass
 
 
+RecipesTypeDef = TypedDict(
+    "RecipesTypeDef",
+    {
+        "Setup": Sequence[str],
+        "Configure": Sequence[str],
+        "Deploy": Sequence[str],
+        "Undeploy": Sequence[str],
+        "Shutdown": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredVolumeConfigurationTypeDef = TypedDict(
     "_RequiredVolumeConfigurationTypeDef",
     {
         "MountPoint": str,
         "NumberOfDisks": int,
         "Size": int,
     },
@@ -1695,26 +1707,14 @@
     {
         "Tags": Dict[str, str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RecipesTypeDef = TypedDict(
-    "RecipesTypeDef",
-    {
-        "Setup": List[str],
-        "Configure": List[str],
-        "Deploy": List[str],
-        "Undeploy": List[str],
-        "Shutdown": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RegisterEcsClusterResultTypeDef = TypedDict(
     "RegisterEcsClusterResultTypeDef",
     {
         "EcsClusterArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1958,17 +1958,17 @@
     total=False,
 )
 
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
-        "LogStreams": Sequence[CloudWatchLogsLogStreamTypeDef],
+        "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeCommandsResultTypeDef = TypedDict(
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/type_defs.pyi` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "AutoScalingThresholdsTypeDef",
     "EbsBlockDeviceTypeDef",
     "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
     "DeploymentCommandTypeDef",
+    "RecipesTypeDef",
     "VolumeConfigurationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
@@ -153,15 +154,14 @@
     "CreateStackResultTypeDef",
     "CreateUserProfileResultTypeDef",
     "DescribeStackProvisioningParametersResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionResultTypeDef",
     "InstancesCountResponseTypeDef",
     "ListTagsResultTypeDef",
-    "RecipesTypeDef",
     "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpResultTypeDef",
     "RegisterInstanceResultTypeDef",
     "RegisterVolumeResultTypeDef",
     "SourceResponseTypeDef",
     "StackConfigurationManagerResponseTypeDef",
     "CloneStackRequestRequestTypeDef",
@@ -452,14 +452,26 @@
 )
 
 class DeploymentCommandTypeDef(
     _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
 ):
     pass
 
+RecipesTypeDef = TypedDict(
+    "RecipesTypeDef",
+    {
+        "Setup": Sequence[str],
+        "Configure": Sequence[str],
+        "Deploy": Sequence[str],
+        "Undeploy": Sequence[str],
+        "Shutdown": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredVolumeConfigurationTypeDef = TypedDict(
     "_RequiredVolumeConfigurationTypeDef",
     {
         "MountPoint": str,
         "NumberOfDisks": int,
         "Size": int,
     },
@@ -1648,26 +1660,14 @@
     {
         "Tags": Dict[str, str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RecipesTypeDef = TypedDict(
-    "RecipesTypeDef",
-    {
-        "Setup": List[str],
-        "Configure": List[str],
-        "Deploy": List[str],
-        "Undeploy": List[str],
-        "Shutdown": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RegisterEcsClusterResultTypeDef = TypedDict(
     "RegisterEcsClusterResultTypeDef",
     {
         "EcsClusterArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1903,17 +1903,17 @@
     total=False,
 )
 
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
-        "LogStreams": Sequence[CloudWatchLogsLogStreamTypeDef],
+        "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeCommandsResultTypeDef = TypedDict(
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/waiter.py` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/waiter.pyi` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/PKG-INFO` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.28.15
-Summary: Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -455,14 +455,15 @@
     AutoScalingThresholdsTypeDef,
     EbsBlockDeviceTypeDef,
     ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
     DeploymentCommandTypeDef,
+    RecipesTypeDef,
     VolumeConfigurationTypeDef,
     CreateUserProfileRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
@@ -554,15 +555,14 @@
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DescribeStackProvisioningParametersResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionResultTypeDef,
     InstancesCountResponseTypeDef,
     ListTagsResultTypeDef,
-    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceResponseTypeDef,
     StackConfigurationManagerResponseTypeDef,
     CloneStackRequestRequestTypeDef,
```

### Comparing `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/SOURCES.txt` & `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15/setup.py` & `mypy-boto3-opsworks-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opsworks",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_opsworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder"
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

