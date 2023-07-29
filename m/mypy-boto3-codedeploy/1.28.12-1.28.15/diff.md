# Comparing `tmp/mypy-boto3-codedeploy-1.28.12.tar.gz` & `tmp/mypy-boto3-codedeploy-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codedeploy-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
+gzip compressed data, was "mypy-boto3-codedeploy-1.28.15.tar", last modified: Fri Jul 28 20:42:28 2023, max compression
```

## Comparing `mypy-boto3-codedeploy-1.28.12.tar` & `mypy-boto3-codedeploy-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.428555 mypy-boto3-codedeploy-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-07-27 05:34:27.428555 mypy-boto3-codedeploy-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21208 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.424555 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46184 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-27 05:19:05.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-07-27 05:19:05.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58069 2023-07-27 05:19:06.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58036 2023-07-27 05:19:06.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.428555 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:27.000000 mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.428555 mypy-boto3-codedeploy-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:19:04.000000 mypy-boto3-codedeploy-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.612825 mypy-boto3-codedeploy-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:29.000000 mypy-boto3-codedeploy-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-07-28 20:42:28.604825 mypy-boto3-codedeploy-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-07-28 20:21:29.000000 mypy-boto3-codedeploy-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.596825 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-28 20:21:29.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-28 20:21:29.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:21:29.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46184 2023-07-28 20:21:31.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-28 20:21:30.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-28 20:21:31.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-07-28 20:21:31.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-28 20:21:31.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-07-28 20:21:31.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:29.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52979 2023-07-28 20:21:33.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52946 2023-07-28 20:21:32.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:29.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-28 20:21:31.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-28 20:21:31.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.604825 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-07-28 20:42:28.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 20:42:28.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:28.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:28.000000 mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:28.612825 mypy-boto3-codedeploy-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:21:29.000000 mypy-boto3-codedeploy-1.28.15/setup.py
```

### Comparing `mypy-boto3-codedeploy-1.28.12/LICENSE` & `mypy-boto3-codedeploy-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.12/PKG-INFO` & `mypy-boto3-codedeploy-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codedeploy
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeDeploy 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeDeploy 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codedeploy)](https://pepy.tech/project/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -417,176 +417,155 @@
 
 `mypy_boto3_codedeploy.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
-    AlarmOutputTypeDef,
     AlarmTypeDef,
-    AppSpecContentOutputTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
     AutoRollbackConfigurationOutputTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
-    BlueInstanceTerminationOptionOutputTypeDef,
-    DeploymentReadyOptionOutputTypeDef,
-    GreenFleetProvisioningOptionOutputTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
-    CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
-    CreateDeploymentConfigOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
     TriggerConfigTypeDef,
-    CreateDeploymentGroupOutputTypeDef,
-    CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
-    DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
-    MinimumHealthyHostsOutputTypeDef,
-    DeploymentStyleOutputTypeDef,
-    EC2TagFilterOutputTypeDef,
-    ECSServiceOutputTypeDef,
     LastDeploymentInfoTypeDef,
-    TagFilterOutputTypeDef,
     TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
-    TargetGroupInfoOutputTypeDef,
-    ELBInfoOutputTypeDef,
+    TargetGroupInfoTypeDef,
     ELBInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
-    GitHubLocationOutputTypeDef,
     GitHubLocationTypeDef,
-    TagOutputTypeDef,
     LambdaFunctionInfoTypeDef,
-    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
-    ListDeploymentConfigsOutputTypeDef,
-    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
-    ListDeploymentGroupsOutputTypeDef,
-    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
-    ListDeploymentInstancesOutputTypeDef,
-    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
-    ListDeploymentTargetsOutputTypeDef,
     TimeRangeTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
-    ListGitHubAccountTokenNamesOutputTypeDef,
-    ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TargetGroupInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
-    PutLifecycleEventHookExecutionStatusOutputTypeDef,
-    RawStringOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    S3LocationOutputTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
-    StopDeploymentOutputTypeDef,
     TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
-    TimeBasedCanaryOutputTypeDef,
     TimeBasedCanaryTypeDef,
-    TimeBasedLinearOutputTypeDef,
     TimeBasedLinearTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
+    InstanceInfoTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
     BatchGetApplicationsOutputTypeDef,
-    GetApplicationOutputTypeDef,
+    CreateApplicationOutputTypeDef,
+    CreateDeploymentConfigOutputTypeDef,
+    CreateDeploymentGroupOutputTypeDef,
+    CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
+    DeleteGitHubAccountTokenOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetApplicationOutputTypeDef,
+    ListApplicationsOutputTypeDef,
+    ListDeploymentConfigsOutputTypeDef,
+    ListDeploymentGroupsOutputTypeDef,
+    ListDeploymentInstancesOutputTypeDef,
+    ListDeploymentTargetsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListGitHubAccountTokenNamesOutputTypeDef,
+    ListOnPremisesInstancesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PutLifecycleEventHookExecutionStatusOutputTypeDef,
+    StopDeploymentOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
-    BlueGreenDeploymentConfigurationOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
+    EC2TagSetOutputTypeDef,
     EC2TagSetTypeDef,
-    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
-    OnPremisesTagSetTypeDef,
-    EC2TagSetOutputTypeDef,
     OnPremisesTagSetOutputTypeDef,
+    OnPremisesTagSetTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
-    InstanceInfoTypeDef,
-    ListTagsForResourceOutputTypeDef,
+    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
+    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
+    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
+    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
+    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
-    RevisionLocationOutputTypeDef,
     RevisionLocationTypeDef,
     TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
-    TrafficRoutingConfigOutputTypeDef,
     TrafficRoutingConfigTypeDef,
-    TargetInstancesTypeDef,
+    BatchGetOnPremisesInstancesOutputTypeDef,
+    GetOnPremisesInstanceOutputTypeDef,
     TargetInstancesOutputTypeDef,
+    TargetInstancesTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
-    BatchGetOnPremisesInstancesOutputTypeDef,
-    GetOnPremisesInstanceOutputTypeDef,
-    GetApplicationRevisionOutputTypeDef,
-    ListApplicationRevisionsOutputTypeDef,
-    RevisionInfoTypeDef,
     BatchGetApplicationRevisionsInputRequestTypeDef,
     GetApplicationRevisionInputRequestTypeDef,
+    GetApplicationRevisionOutputTypeDef,
+    ListApplicationRevisionsOutputTypeDef,
     RegisterApplicationRevisionInputRequestTypeDef,
+    RevisionInfoTypeDef,
     LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
-    DeploymentConfigInfoTypeDef,
     CreateDeploymentConfigInputRequestTypeDef,
+    DeploymentConfigInfoTypeDef,
     CreateDeploymentInputRequestTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
```

### Comparing `mypy-boto3-codedeploy-1.28.12/README.md` & `mypy-boto3-codedeploy-1.28.15/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codedeploy)](https://pepy.tech/project/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -385,176 +385,155 @@
 
 `mypy_boto3_codedeploy.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
-    AlarmOutputTypeDef,
     AlarmTypeDef,
-    AppSpecContentOutputTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
     AutoRollbackConfigurationOutputTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
-    BlueInstanceTerminationOptionOutputTypeDef,
-    DeploymentReadyOptionOutputTypeDef,
-    GreenFleetProvisioningOptionOutputTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
-    CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
-    CreateDeploymentConfigOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
     TriggerConfigTypeDef,
-    CreateDeploymentGroupOutputTypeDef,
-    CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
-    DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
-    MinimumHealthyHostsOutputTypeDef,
-    DeploymentStyleOutputTypeDef,
-    EC2TagFilterOutputTypeDef,
-    ECSServiceOutputTypeDef,
     LastDeploymentInfoTypeDef,
-    TagFilterOutputTypeDef,
     TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
-    TargetGroupInfoOutputTypeDef,
-    ELBInfoOutputTypeDef,
+    TargetGroupInfoTypeDef,
     ELBInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
-    GitHubLocationOutputTypeDef,
     GitHubLocationTypeDef,
-    TagOutputTypeDef,
     LambdaFunctionInfoTypeDef,
-    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
-    ListDeploymentConfigsOutputTypeDef,
-    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
-    ListDeploymentGroupsOutputTypeDef,
-    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
-    ListDeploymentInstancesOutputTypeDef,
-    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
-    ListDeploymentTargetsOutputTypeDef,
     TimeRangeTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
-    ListGitHubAccountTokenNamesOutputTypeDef,
-    ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TargetGroupInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
-    PutLifecycleEventHookExecutionStatusOutputTypeDef,
-    RawStringOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    S3LocationOutputTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
-    StopDeploymentOutputTypeDef,
     TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
-    TimeBasedCanaryOutputTypeDef,
     TimeBasedCanaryTypeDef,
-    TimeBasedLinearOutputTypeDef,
     TimeBasedLinearTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
+    InstanceInfoTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
     BatchGetApplicationsOutputTypeDef,
-    GetApplicationOutputTypeDef,
+    CreateApplicationOutputTypeDef,
+    CreateDeploymentConfigOutputTypeDef,
+    CreateDeploymentGroupOutputTypeDef,
+    CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
+    DeleteGitHubAccountTokenOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetApplicationOutputTypeDef,
+    ListApplicationsOutputTypeDef,
+    ListDeploymentConfigsOutputTypeDef,
+    ListDeploymentGroupsOutputTypeDef,
+    ListDeploymentInstancesOutputTypeDef,
+    ListDeploymentTargetsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListGitHubAccountTokenNamesOutputTypeDef,
+    ListOnPremisesInstancesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PutLifecycleEventHookExecutionStatusOutputTypeDef,
+    StopDeploymentOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
-    BlueGreenDeploymentConfigurationOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
+    EC2TagSetOutputTypeDef,
     EC2TagSetTypeDef,
-    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
-    OnPremisesTagSetTypeDef,
-    EC2TagSetOutputTypeDef,
     OnPremisesTagSetOutputTypeDef,
+    OnPremisesTagSetTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
-    InstanceInfoTypeDef,
-    ListTagsForResourceOutputTypeDef,
+    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
+    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
+    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
+    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
+    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
-    RevisionLocationOutputTypeDef,
     RevisionLocationTypeDef,
     TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
-    TrafficRoutingConfigOutputTypeDef,
     TrafficRoutingConfigTypeDef,
-    TargetInstancesTypeDef,
+    BatchGetOnPremisesInstancesOutputTypeDef,
+    GetOnPremisesInstanceOutputTypeDef,
     TargetInstancesOutputTypeDef,
+    TargetInstancesTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
-    BatchGetOnPremisesInstancesOutputTypeDef,
-    GetOnPremisesInstanceOutputTypeDef,
-    GetApplicationRevisionOutputTypeDef,
-    ListApplicationRevisionsOutputTypeDef,
-    RevisionInfoTypeDef,
     BatchGetApplicationRevisionsInputRequestTypeDef,
     GetApplicationRevisionInputRequestTypeDef,
+    GetApplicationRevisionOutputTypeDef,
+    ListApplicationRevisionsOutputTypeDef,
     RegisterApplicationRevisionInputRequestTypeDef,
+    RevisionInfoTypeDef,
     LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
-    DeploymentConfigInfoTypeDef,
     CreateDeploymentConfigInputRequestTypeDef,
+    DeploymentConfigInfoTypeDef,
     CreateDeploymentInputRequestTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
```

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__init__.py` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__init__.pyi` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/__main__.py` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeDeploy 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodeDeploy 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/client.py` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/client.pyi` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/literals.py` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/literals.pyi` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/paginator.py` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -72,25 +72,22 @@
     "ListDeploymentInstancesPaginator",
     "ListDeploymentTargetsPaginator",
     "ListDeploymentsPaginator",
     "ListGitHubAccountTokenNamesPaginator",
     "ListOnPremisesInstancesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListApplicationRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationrevisionspaginator)
     """
 
     def paginate(
@@ -98,153 +95,145 @@
         *,
         applicationName: str,
         sortBy: ApplicationRevisionSortByType = ...,
         sortOrder: SortOrderType = ...,
         s3Bucket: str = ...,
         s3KeyPrefix: str = ...,
         deployed: ListStateFilterActionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationRevisionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationrevisionspaginator)
         """
 
-
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationspaginator)
         """
 
-
 class ListDeploymentConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentConfigsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentconfigspaginator)
         """
 
-
 class ListDeploymentGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentgroupspaginator)
     """
 
     def paginate(
-        self, *, applicationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, applicationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentgroupspaginator)
         """
 
-
 class ListDeploymentInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         deploymentId: str,
         instanceStatusFilter: Sequence[InstanceStatusType] = ...,
         instanceTypeFilter: Sequence[InstanceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentinstancespaginator)
         """
 
-
 class ListDeploymentTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         deploymentId: str = ...,
         targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentTargetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymenttargetspaginator)
         """
 
-
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         applicationName: str = ...,
         deploymentGroupName: str = ...,
         externalId: str = ...,
         includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,
         createTimeRange: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentspaginator)
         """
 
-
 class ListGitHubAccountTokenNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listgithubaccounttokennamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGitHubAccountTokenNamesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listgithubaccounttokennamespaginator)
         """
 
-
 class ListOnPremisesInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listonpremisesinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOnPremisesInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listonpremisesinstancespaginator)
         """
```

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/paginator.pyi` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,22 +72,25 @@
     "ListDeploymentInstancesPaginator",
     "ListDeploymentTargetsPaginator",
     "ListDeploymentsPaginator",
     "ListGitHubAccountTokenNamesPaginator",
     "ListOnPremisesInstancesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListApplicationRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationrevisionspaginator)
     """
 
     def paginate(
@@ -95,145 +98,153 @@
         *,
         applicationName: str,
         sortBy: ApplicationRevisionSortByType = ...,
         sortOrder: SortOrderType = ...,
         s3Bucket: str = ...,
         s3KeyPrefix: str = ...,
         deployed: ListStateFilterActionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationRevisionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationrevisionspaginator)
         """
 
+
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationspaginator)
         """
 
+
 class ListDeploymentConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentConfigsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentconfigspaginator)
         """
 
+
 class ListDeploymentGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentgroupspaginator)
     """
 
     def paginate(
-        self, *, applicationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, applicationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentgroupspaginator)
         """
 
+
 class ListDeploymentInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         deploymentId: str,
         instanceStatusFilter: Sequence[InstanceStatusType] = ...,
         instanceTypeFilter: Sequence[InstanceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentinstancespaginator)
         """
 
+
 class ListDeploymentTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         deploymentId: str = ...,
         targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentTargetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymenttargetspaginator)
         """
 
+
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         applicationName: str = ...,
         deploymentGroupName: str = ...,
         externalId: str = ...,
         includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,
         createTimeRange: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentspaginator)
         """
 
+
 class ListGitHubAccountTokenNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listgithubaccounttokennamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGitHubAccountTokenNamesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listgithubaccounttokennamespaginator)
         """
 
+
 class ListOnPremisesInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listonpremisesinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOnPremisesInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listonpremisesinstancespaginator)
         """
```

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/type_defs.py` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -52,179 +52,157 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
-    "AlarmOutputTypeDef",
     "AlarmTypeDef",
-    "AppSpecContentOutputTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
     "AutoRollbackConfigurationOutputTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetApplicationsInputRequestTypeDef",
     "BatchGetDeploymentGroupsInputRequestTypeDef",
     "BatchGetDeploymentInstancesInputRequestTypeDef",
     "BatchGetDeploymentTargetsInputRequestTypeDef",
     "BatchGetDeploymentsInputRequestTypeDef",
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
-    "BlueInstanceTerminationOptionOutputTypeDef",
-    "DeploymentReadyOptionOutputTypeDef",
-    "GreenFleetProvisioningOptionOutputTypeDef",
     "BlueInstanceTerminationOptionTypeDef",
     "DeploymentReadyOptionTypeDef",
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
-    "CreateApplicationOutputTypeDef",
     "MinimumHealthyHostsTypeDef",
-    "CreateDeploymentConfigOutputTypeDef",
     "DeploymentStyleTypeDef",
     "EC2TagFilterTypeDef",
     "ECSServiceTypeDef",
     "TagFilterTypeDef",
     "TriggerConfigTypeDef",
-    "CreateDeploymentGroupOutputTypeDef",
-    "CreateDeploymentOutputTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
-    "DeleteGitHubAccountTokenOutputTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
-    "MinimumHealthyHostsOutputTypeDef",
-    "DeploymentStyleOutputTypeDef",
-    "EC2TagFilterOutputTypeDef",
-    "ECSServiceOutputTypeDef",
     "LastDeploymentInfoTypeDef",
-    "TagFilterOutputTypeDef",
     "TriggerConfigOutputTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
-    "TargetGroupInfoOutputTypeDef",
-    "ELBInfoOutputTypeDef",
+    "TargetGroupInfoTypeDef",
     "ELBInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GenericRevisionInfoTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetDeploymentConfigInputRequestTypeDef",
     "GetDeploymentGroupInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetDeploymentInstanceInputRequestTypeDef",
     "GetDeploymentTargetInputRequestTypeDef",
     "GetOnPremisesInstanceInputRequestTypeDef",
-    "GitHubLocationOutputTypeDef",
     "GitHubLocationTypeDef",
-    "TagOutputTypeDef",
     "LambdaFunctionInfoTypeDef",
-    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationRevisionsInputRequestTypeDef",
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListApplicationsInputRequestTypeDef",
-    "ListApplicationsOutputTypeDef",
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     "ListDeploymentConfigsInputRequestTypeDef",
-    "ListDeploymentConfigsOutputTypeDef",
-    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     "ListDeploymentGroupsInputRequestTypeDef",
-    "ListDeploymentGroupsOutputTypeDef",
-    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     "ListDeploymentInstancesInputRequestTypeDef",
-    "ListDeploymentInstancesOutputTypeDef",
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     "ListDeploymentTargetsInputRequestTypeDef",
-    "ListDeploymentTargetsOutputTypeDef",
     "TimeRangeTypeDef",
-    "ListDeploymentsOutputTypeDef",
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    "ListOnPremisesInstancesOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TargetGroupInfoTypeDef",
-    "PaginatorConfigTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
-    "RawStringOutputTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
-    "StopDeploymentOutputTypeDef",
     "TrafficRouteOutputTypeDef",
     "TrafficRouteTypeDef",
-    "TimeBasedCanaryOutputTypeDef",
     "TimeBasedCanaryTypeDef",
-    "TimeBasedLinearOutputTypeDef",
     "TimeBasedLinearTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
+    "InstanceInfoTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
     "BatchGetApplicationsOutputTypeDef",
-    "GetApplicationOutputTypeDef",
+    "CreateApplicationOutputTypeDef",
+    "CreateDeploymentConfigOutputTypeDef",
+    "CreateDeploymentGroupOutputTypeDef",
+    "CreateDeploymentOutputTypeDef",
     "DeleteDeploymentGroupOutputTypeDef",
+    "DeleteGitHubAccountTokenOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetApplicationOutputTypeDef",
+    "ListApplicationsOutputTypeDef",
+    "ListDeploymentConfigsOutputTypeDef",
+    "ListDeploymentGroupsOutputTypeDef",
+    "ListDeploymentInstancesOutputTypeDef",
+    "ListDeploymentTargetsOutputTypeDef",
+    "ListDeploymentsOutputTypeDef",
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    "ListOnPremisesInstancesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    "StopDeploymentOutputTypeDef",
     "UpdateDeploymentGroupOutputTypeDef",
-    "BlueGreenDeploymentConfigurationOutputTypeDef",
     "BlueGreenDeploymentConfigurationTypeDef",
+    "EC2TagSetOutputTypeDef",
     "EC2TagSetTypeDef",
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListOnPremisesInstancesInputRequestTypeDef",
-    "OnPremisesTagSetTypeDef",
-    "EC2TagSetOutputTypeDef",
     "OnPremisesTagSetOutputTypeDef",
+    "OnPremisesTagSetTypeDef",
     "LifecycleEventTypeDef",
     "ECSTaskSetTypeDef",
     "GetDeploymentInputDeploymentSuccessfulWaitTypeDef",
-    "InstanceInfoTypeDef",
-    "ListTagsForResourceOutputTypeDef",
+    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
+    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
-    "RevisionLocationOutputTypeDef",
     "RevisionLocationTypeDef",
     "TargetGroupPairInfoOutputTypeDef",
     "TargetGroupPairInfoTypeDef",
-    "TrafficRoutingConfigOutputTypeDef",
     "TrafficRoutingConfigTypeDef",
-    "TargetInstancesTypeDef",
+    "BatchGetOnPremisesInstancesOutputTypeDef",
+    "GetOnPremisesInstanceOutputTypeDef",
     "TargetInstancesOutputTypeDef",
+    "TargetInstancesTypeDef",
     "CloudFormationTargetTypeDef",
     "InstanceSummaryTypeDef",
     "InstanceTargetTypeDef",
     "LambdaTargetTypeDef",
     "ECSTargetTypeDef",
-    "BatchGetOnPremisesInstancesOutputTypeDef",
-    "GetOnPremisesInstanceOutputTypeDef",
-    "GetApplicationRevisionOutputTypeDef",
-    "ListApplicationRevisionsOutputTypeDef",
-    "RevisionInfoTypeDef",
     "BatchGetApplicationRevisionsInputRequestTypeDef",
     "GetApplicationRevisionInputRequestTypeDef",
+    "GetApplicationRevisionOutputTypeDef",
+    "ListApplicationRevisionsOutputTypeDef",
     "RegisterApplicationRevisionInputRequestTypeDef",
+    "RevisionInfoTypeDef",
     "LoadBalancerInfoOutputTypeDef",
     "LoadBalancerInfoTypeDef",
-    "DeploymentConfigInfoTypeDef",
     "CreateDeploymentConfigInputRequestTypeDef",
+    "DeploymentConfigInfoTypeDef",
     "CreateDeploymentInputRequestTypeDef",
     "BatchGetDeploymentInstancesOutputTypeDef",
     "GetDeploymentInstanceOutputTypeDef",
     "DeploymentTargetTypeDef",
     "BatchGetApplicationRevisionsOutputTypeDef",
     "DeploymentGroupInfoTypeDef",
     "DeploymentInfoTypeDef",
@@ -244,39 +222,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AlarmOutputTypeDef = TypedDict(
-    "AlarmOutputTypeDef",
-    {
-        "name": str,
-    },
-    total=False,
-)
-
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
-AppSpecContentOutputTypeDef = TypedDict(
-    "AppSpecContentOutputTypeDef",
-    {
-        "content": str,
-        "sha256": str,
-    },
-    total=False,
-)
-
 AppSpecContentTypeDef = TypedDict(
     "AppSpecContentTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -318,14 +279,25 @@
     {
         "name": str,
         "hook": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 BatchGetApplicationsInputRequestTypeDef = TypedDict(
     "BatchGetApplicationsInputRequestTypeDef",
     {
         "applicationNames": Sequence[str],
     },
 )
 
@@ -364,40 +336,14 @@
 BatchGetOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
     {
         "instanceNames": Sequence[str],
     },
 )
 
-BlueInstanceTerminationOptionOutputTypeDef = TypedDict(
-    "BlueInstanceTerminationOptionOutputTypeDef",
-    {
-        "action": InstanceActionType,
-        "terminationWaitTimeInMinutes": int,
-    },
-    total=False,
-)
-
-DeploymentReadyOptionOutputTypeDef = TypedDict(
-    "DeploymentReadyOptionOutputTypeDef",
-    {
-        "actionOnTimeout": DeploymentReadyActionType,
-        "waitTimeInMinutes": int,
-    },
-    total=False,
-)
-
-GreenFleetProvisioningOptionOutputTypeDef = TypedDict(
-    "GreenFleetProvisioningOptionOutputTypeDef",
-    {
-        "action": GreenFleetProvisioningActionType,
-    },
-    total=False,
-)
-
 BlueInstanceTerminationOptionTypeDef = TypedDict(
     "BlueInstanceTerminationOptionTypeDef",
     {
         "action": InstanceActionType,
         "terminationWaitTimeInMinutes": int,
     },
     total=False,
@@ -425,39 +371,23 @@
     {
         "deploymentId": str,
         "deploymentWaitType": DeploymentWaitTypeType,
     },
     total=False,
 )
 
-CreateApplicationOutputTypeDef = TypedDict(
-    "CreateApplicationOutputTypeDef",
-    {
-        "applicationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MinimumHealthyHostsTypeDef = TypedDict(
     "MinimumHealthyHostsTypeDef",
     {
         "type": MinimumHealthyHostsTypeType,
         "value": int,
     },
     total=False,
 )
 
-CreateDeploymentConfigOutputTypeDef = TypedDict(
-    "CreateDeploymentConfigOutputTypeDef",
-    {
-        "deploymentConfigId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentStyleTypeDef = TypedDict(
     "DeploymentStyleTypeDef",
     {
         "deploymentType": DeploymentTypeType,
         "deploymentOption": DeploymentOptionType,
     },
     total=False,
@@ -498,30 +428,14 @@
         "triggerName": str,
         "triggerTargetArn": str,
         "triggerEvents": Sequence[TriggerEventTypeType],
     },
     total=False,
 )
 
-CreateDeploymentGroupOutputTypeDef = TypedDict(
-    "CreateDeploymentGroupOutputTypeDef",
-    {
-        "deploymentGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDeploymentOutputTypeDef = TypedDict(
-    "CreateDeploymentOutputTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationInputRequestTypeDef = TypedDict(
     "DeleteApplicationInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 
@@ -544,88 +458,33 @@
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     {
         "tokenName": str,
     },
     total=False,
 )
 
-DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
-    "DeleteGitHubAccountTokenOutputTypeDef",
-    {
-        "tokenName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteResourcesByExternalIdInputRequestTypeDef = TypedDict(
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
 
-MinimumHealthyHostsOutputTypeDef = TypedDict(
-    "MinimumHealthyHostsOutputTypeDef",
-    {
-        "type": MinimumHealthyHostsTypeType,
-        "value": int,
-    },
-    total=False,
-)
-
-DeploymentStyleOutputTypeDef = TypedDict(
-    "DeploymentStyleOutputTypeDef",
-    {
-        "deploymentType": DeploymentTypeType,
-        "deploymentOption": DeploymentOptionType,
-    },
-    total=False,
-)
-
-EC2TagFilterOutputTypeDef = TypedDict(
-    "EC2TagFilterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "Type": EC2TagFilterTypeType,
-    },
-    total=False,
-)
-
-ECSServiceOutputTypeDef = TypedDict(
-    "ECSServiceOutputTypeDef",
-    {
-        "serviceName": str,
-        "clusterName": str,
-    },
-    total=False,
-)
-
 LastDeploymentInfoTypeDef = TypedDict(
     "LastDeploymentInfoTypeDef",
     {
         "deploymentId": str,
         "status": DeploymentStatusType,
         "endTime": datetime,
         "createTime": datetime,
     },
     total=False,
 )
 
-TagFilterOutputTypeDef = TypedDict(
-    "TagFilterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "Type": TagFilterTypeType,
-    },
-    total=False,
-)
-
 TriggerConfigOutputTypeDef = TypedDict(
     "TriggerConfigOutputTypeDef",
     {
         "triggerName": str,
         "triggerTargetArn": str,
         "triggerEvents": List[TriggerEventTypeType],
     },
@@ -687,45 +546,30 @@
         "scriptName": str,
         "message": str,
         "logTail": str,
     },
     total=False,
 )
 
-TargetGroupInfoOutputTypeDef = TypedDict(
-    "TargetGroupInfoOutputTypeDef",
-    {
-        "name": str,
-    },
-    total=False,
-)
-
-ELBInfoOutputTypeDef = TypedDict(
-    "ELBInfoOutputTypeDef",
+TargetGroupInfoTypeDef = TypedDict(
+    "TargetGroupInfoTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
 ELBInfoTypeDef = TypedDict(
     "ELBInfoTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GenericRevisionInfoTypeDef = TypedDict(
     "GenericRevisionInfoTypeDef",
     {
         "description": str,
         "deploymentGroups": List[str],
         "firstUsedTime": datetime,
         "lastUsedTime": datetime,
@@ -792,80 +636,45 @@
 GetOnPremisesInstanceInputRequestTypeDef = TypedDict(
     "GetOnPremisesInstanceInputRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 
-GitHubLocationOutputTypeDef = TypedDict(
-    "GitHubLocationOutputTypeDef",
-    {
-        "repository": str,
-        "commitId": str,
-    },
-    total=False,
-)
-
 GitHubLocationTypeDef = TypedDict(
     "GitHubLocationTypeDef",
     {
         "repository": str,
         "commitId": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 LambdaFunctionInfoTypeDef = TypedDict(
     "LambdaFunctionInfoTypeDef",
     {
         "functionName": str,
         "functionAlias": str,
         "currentVersion": str,
         "targetVersion": str,
         "targetVersionWeight": float,
     },
     total=False,
 )
 
-_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "sortBy": ApplicationRevisionSortByType,
-        "sortOrder": SortOrderType,
-        "s3Bucket": str,
-        "s3KeyPrefix": str,
-        "deployed": ListStateFilterActionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
-    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApplicationRevisionsInputRequestTypeDef = TypedDict(
     "_RequiredListApplicationRevisionsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListApplicationRevisionsInputRequestTypeDef = TypedDict(
@@ -877,150 +686,56 @@
         "s3KeyPrefix": str,
         "deployed": ListStateFilterActionType,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationRevisionsInputRequestTypeDef(
     _RequiredListApplicationRevisionsInputRequestTypeDef,
     _OptionalListApplicationRevisionsInputRequestTypeDef,
 ):
     pass
 
-
-ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListApplicationsOutputTypeDef = TypedDict(
-    "ListApplicationsOutputTypeDef",
-    {
-        "applications": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeploymentConfigsInputRequestTypeDef = TypedDict(
     "ListDeploymentConfigsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListDeploymentConfigsOutputTypeDef = TypedDict(
-    "ListDeploymentConfigsOutputTypeDef",
-    {
-        "deploymentConfigsList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
-    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeploymentGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentGroupsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListDeploymentGroupsInputRequestTypeDef = TypedDict(
     "_OptionalListDeploymentGroupsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListDeploymentGroupsInputRequestTypeDef(
     _RequiredListDeploymentGroupsInputRequestTypeDef,
     _OptionalListDeploymentGroupsInputRequestTypeDef,
 ):
     pass
 
-
-ListDeploymentGroupsOutputTypeDef = TypedDict(
-    "ListDeploymentGroupsOutputTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "deploymentId": str,
-    },
-)
-_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "instanceStatusFilter": Sequence[InstanceStatusType],
-        "instanceTypeFilter": Sequence[InstanceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
-    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeploymentInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentInstancesInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 _OptionalListDeploymentInstancesInputRequestTypeDef = TypedDict(
@@ -1029,178 +744,76 @@
         "nextToken": str,
         "instanceStatusFilter": Sequence[InstanceStatusType],
         "instanceTypeFilter": Sequence[InstanceTypeType],
     },
     total=False,
 )
 
-
 class ListDeploymentInstancesInputRequestTypeDef(
     _RequiredListDeploymentInstancesInputRequestTypeDef,
     _OptionalListDeploymentInstancesInputRequestTypeDef,
 ):
     pass
 
-
-ListDeploymentInstancesOutputTypeDef = TypedDict(
-    "ListDeploymentInstancesOutputTypeDef",
-    {
-        "instancesList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
-    {
-        "deploymentId": str,
-        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeploymentTargetsInputRequestTypeDef = TypedDict(
     "ListDeploymentTargetsInputRequestTypeDef",
     {
         "deploymentId": str,
         "nextToken": str,
         "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
     },
     total=False,
 )
 
-ListDeploymentTargetsOutputTypeDef = TypedDict(
-    "ListDeploymentTargetsOutputTypeDef",
-    {
-        "targetIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TimeRangeTypeDef = TypedDict(
     "TimeRangeTypeDef",
     {
         "start": Union[datetime, str],
         "end": Union[datetime, str],
     },
     total=False,
 )
 
-ListDeploymentsOutputTypeDef = TypedDict(
-    "ListDeploymentsOutputTypeDef",
-    {
-        "deployments": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGitHubAccountTokenNamesInputRequestTypeDef = TypedDict(
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    {
-        "tokenNameList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListOnPremisesInstancesOutputTypeDef = TypedDict(
-    "ListOnPremisesInstancesOutputTypeDef",
-    {
-        "instanceNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
     "_OptionalListTagsForResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-
-TargetGroupInfoTypeDef = TypedDict(
-    "TargetGroupInfoTypeDef",
-    {
-        "name": str,
-    },
-    total=False,
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PutLifecycleEventHookExecutionStatusInputRequestTypeDef = TypedDict(
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     {
         "deploymentId": str,
         "lifecycleEventHookExecutionId": str,
         "status": LifecycleEventStatusType,
     },
     total=False,
 )
 
-PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
-    {
-        "lifecycleEventHookExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RawStringOutputTypeDef = TypedDict(
-    "RawStringOutputTypeDef",
-    {
-        "content": str,
-        "sha256": str,
-    },
-    total=False,
-)
-
 RawStringTypeDef = TypedDict(
     "RawStringTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -1217,45 +830,20 @@
     {
         "iamSessionArn": str,
         "iamUserArn": str,
     },
     total=False,
 )
 
-
 class RegisterOnPremisesInstanceInputRequestTypeDef(
     _RequiredRegisterOnPremisesInstanceInputRequestTypeDef,
     _OptionalRegisterOnPremisesInstanceInputRequestTypeDef,
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-        "bundleType": BundleTypeType,
-        "version": str,
-        "eTag": str,
-    },
-    total=False,
-)
-
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "bundleType": BundleTypeType,
         "version": str,
@@ -1282,30 +870,19 @@
     "_OptionalStopDeploymentInputRequestTypeDef",
     {
         "autoRollbackEnabled": bool,
     },
     total=False,
 )
 
-
 class StopDeploymentInputRequestTypeDef(
     _RequiredStopDeploymentInputRequestTypeDef, _OptionalStopDeploymentInputRequestTypeDef
 ):
     pass
 
-
-StopDeploymentOutputTypeDef = TypedDict(
-    "StopDeploymentOutputTypeDef",
-    {
-        "status": StopStatusType,
-        "statusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TrafficRouteOutputTypeDef = TypedDict(
     "TrafficRouteOutputTypeDef",
     {
         "listenerArns": List[str],
     },
     total=False,
 )
@@ -1314,41 +891,23 @@
     "TrafficRouteTypeDef",
     {
         "listenerArns": Sequence[str],
     },
     total=False,
 )
 
-TimeBasedCanaryOutputTypeDef = TypedDict(
-    "TimeBasedCanaryOutputTypeDef",
-    {
-        "canaryPercentage": int,
-        "canaryInterval": int,
-    },
-    total=False,
-)
-
 TimeBasedCanaryTypeDef = TypedDict(
     "TimeBasedCanaryTypeDef",
     {
         "canaryPercentage": int,
         "canaryInterval": int,
     },
     total=False,
 )
 
-TimeBasedLinearOutputTypeDef = TypedDict(
-    "TimeBasedLinearOutputTypeDef",
-    {
-        "linearPercentage": int,
-        "linearInterval": int,
-    },
-    total=False,
-)
-
 TimeBasedLinearTypeDef = TypedDict(
     "TimeBasedLinearTypeDef",
     {
         "linearPercentage": int,
         "linearInterval": int,
     },
     total=False,
@@ -1390,20 +949,32 @@
     {
         "computePlatform": ComputePlatformType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateApplicationInputRequestTypeDef(
     _RequiredCreateApplicationInputRequestTypeDef, _OptionalCreateApplicationInputRequestTypeDef
 ):
     pass
 
+InstanceInfoTypeDef = TypedDict(
+    "InstanceInfoTypeDef",
+    {
+        "instanceName": str,
+        "iamSessionArn": str,
+        "iamUserArn": str,
+        "instanceArn": str,
+        "registerTime": datetime,
+        "deregisterTime": datetime,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
 
 RemoveTagsFromOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
         "instanceNames": Sequence[str],
     },
@@ -1418,15 +989,15 @@
 )
 
 AlarmConfigurationOutputTypeDef = TypedDict(
     "AlarmConfigurationOutputTypeDef",
     {
         "enabled": bool,
         "ignorePollAlarmFailure": bool,
-        "alarms": List[AlarmOutputTypeDef],
+        "alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
 AlarmConfigurationTypeDef = TypedDict(
     "AlarmConfigurationTypeDef",
     {
@@ -1437,110 +1008,236 @@
     total=False,
 )
 
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
         "applicationsInfo": List[ApplicationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetApplicationOutputTypeDef = TypedDict(
-    "GetApplicationOutputTypeDef",
+CreateApplicationOutputTypeDef = TypedDict(
+    "CreateApplicationOutputTypeDef",
     {
-        "application": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "applicationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentConfigOutputTypeDef = TypedDict(
+    "CreateDeploymentConfigOutputTypeDef",
+    {
+        "deploymentConfigId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentGroupOutputTypeDef = TypedDict(
+    "CreateDeploymentGroupOutputTypeDef",
+    {
+        "deploymentGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentOutputTypeDef = TypedDict(
+    "CreateDeploymentOutputTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDeploymentGroupOutputTypeDef = TypedDict(
     "DeleteDeploymentGroupOutputTypeDef",
     {
         "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDeploymentGroupOutputTypeDef = TypedDict(
-    "UpdateDeploymentGroupOutputTypeDef",
+DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
+    "DeleteGitHubAccountTokenOutputTypeDef",
     {
-        "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tokenName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BlueGreenDeploymentConfigurationOutputTypeDef = TypedDict(
-    "BlueGreenDeploymentConfigurationOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionOutputTypeDef,
-        "deploymentReadyOption": DeploymentReadyOptionOutputTypeDef,
-        "greenFleetProvisioningOption": GreenFleetProvisioningOptionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApplicationOutputTypeDef = TypedDict(
+    "GetApplicationOutputTypeDef",
+    {
+        "application": ApplicationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsOutputTypeDef = TypedDict(
+    "ListApplicationsOutputTypeDef",
+    {
+        "applications": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentConfigsOutputTypeDef = TypedDict(
+    "ListDeploymentConfigsOutputTypeDef",
+    {
+        "deploymentConfigsList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentGroupsOutputTypeDef = TypedDict(
+    "ListDeploymentGroupsOutputTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentInstancesOutputTypeDef = TypedDict(
+    "ListDeploymentInstancesOutputTypeDef",
+    {
+        "instancesList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentTargetsOutputTypeDef = TypedDict(
+    "ListDeploymentTargetsOutputTypeDef",
+    {
+        "targetIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
+    {
+        "deployments": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    {
+        "tokenNameList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOnPremisesInstancesOutputTypeDef = TypedDict(
+    "ListOnPremisesInstancesOutputTypeDef",
+    {
+        "instanceNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    {
+        "lifecycleEventHookExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDeploymentOutputTypeDef = TypedDict(
+    "StopDeploymentOutputTypeDef",
+    {
+        "status": StopStatusType,
+        "statusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDeploymentGroupOutputTypeDef = TypedDict(
+    "UpdateDeploymentGroupOutputTypeDef",
+    {
+        "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 BlueGreenDeploymentConfigurationTypeDef = TypedDict(
     "BlueGreenDeploymentConfigurationTypeDef",
     {
         "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionTypeDef,
         "deploymentReadyOption": DeploymentReadyOptionTypeDef,
         "greenFleetProvisioningOption": GreenFleetProvisioningOptionTypeDef,
     },
     total=False,
 )
 
-EC2TagSetTypeDef = TypedDict(
-    "EC2TagSetTypeDef",
+EC2TagSetOutputTypeDef = TypedDict(
+    "EC2TagSetOutputTypeDef",
     {
-        "ec2TagSetList": Sequence[Sequence[EC2TagFilterTypeDef]],
+        "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
-ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
+EC2TagSetTypeDef = TypedDict(
+    "EC2TagSetTypeDef",
     {
-        "registrationStatus": RegistrationStatusType,
-        "tagFilters": Sequence[TagFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ec2TagSetList": Sequence[Sequence[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
 ListOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "ListOnPremisesInstancesInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
-OnPremisesTagSetTypeDef = TypedDict(
-    "OnPremisesTagSetTypeDef",
-    {
-        "onPremisesTagSetList": Sequence[Sequence[TagFilterTypeDef]],
-    },
-    total=False,
-)
-
-EC2TagSetOutputTypeDef = TypedDict(
-    "EC2TagSetOutputTypeDef",
+OnPremisesTagSetOutputTypeDef = TypedDict(
+    "OnPremisesTagSetOutputTypeDef",
     {
-        "ec2TagSetList": List[List[EC2TagFilterOutputTypeDef]],
+        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
     },
     total=False,
 )
 
-OnPremisesTagSetOutputTypeDef = TypedDict(
-    "OnPremisesTagSetOutputTypeDef",
+OnPremisesTagSetTypeDef = TypedDict(
+    "OnPremisesTagSetTypeDef",
     {
-        "onPremisesTagSetList": List[List[TagFilterOutputTypeDef]],
+        "onPremisesTagSetList": Sequence[Sequence[TagFilterTypeDef]],
     },
     total=False,
 )
 
 LifecycleEventTypeDef = TypedDict(
     "LifecycleEventTypeDef",
     {
@@ -1558,15 +1255,15 @@
     {
         "identifer": str,
         "desiredCount": int,
         "pendingCount": int,
         "runningCount": int,
         "status": str,
         "trafficWeight": float,
-        "targetGroup": TargetGroupInfoOutputTypeDef,
+        "targetGroup": TargetGroupInfoTypeDef,
         "taskSetLabel": TargetLabelType,
     },
     total=False,
 )
 
 _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef = TypedDict(
     "_RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef",
@@ -1578,54 +1275,140 @@
     "_OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetDeploymentInputDeploymentSuccessfulWaitTypeDef(
     _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
     _OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
 ):
     pass
 
+_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    {
+        "applicationName": str,
+    },
+)
+_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    {
+        "sortBy": ApplicationRevisionSortByType,
+        "sortOrder": SortOrderType,
+        "s3Bucket": str,
+        "s3KeyPrefix": str,
+        "deployed": ListStateFilterActionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-InstanceInfoTypeDef = TypedDict(
-    "InstanceInfoTypeDef",
+class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
+    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+):
+    pass
+
+ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
     {
-        "instanceName": str,
-        "iamSessionArn": str,
-        "iamUserArn": str,
-        "instanceArn": str,
-        "registerTime": datetime,
-        "deregisterTime": datetime,
-        "tags": List[TagOutputTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    {
+        "applicationName": str,
+    },
+)
+_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
+    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "deploymentId": str,
+    },
+)
+_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "instanceStatusFilter": Sequence[InstanceStatusType],
+        "instanceTypeFilter": Sequence[InstanceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
+    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+):
+    pass
+
+ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
+    {
+        "deploymentId": str,
+        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
+    {
+        "registrationStatus": RegistrationStatusType,
+        "tagFilters": Sequence[TagFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     {
         "applicationName": str,
         "deploymentGroupName": str,
         "externalId": str,
         "includeOnlyStatuses": Sequence[DeploymentStatusType],
         "createTimeRange": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDeploymentsInputRequestTypeDef = TypedDict(
     "ListDeploymentsInputRequestTypeDef",
     {
@@ -1635,26 +1418,14 @@
         "includeOnlyStatuses": Sequence[DeploymentStatusType],
         "createTimeRange": TimeRangeTypeDef,
         "nextToken": str,
     },
     total=False,
 )
 
-RevisionLocationOutputTypeDef = TypedDict(
-    "RevisionLocationOutputTypeDef",
-    {
-        "revisionType": RevisionLocationTypeType,
-        "s3Location": S3LocationOutputTypeDef,
-        "gitHubLocation": GitHubLocationOutputTypeDef,
-        "string": RawStringOutputTypeDef,
-        "appSpecContent": AppSpecContentOutputTypeDef,
-    },
-    total=False,
-)
-
 RevisionLocationTypeDef = TypedDict(
     "RevisionLocationTypeDef",
     {
         "revisionType": RevisionLocationTypeType,
         "s3Location": S3LocationTypeDef,
         "gitHubLocation": GitHubLocationTypeDef,
         "string": RawStringTypeDef,
@@ -1662,15 +1433,15 @@
     },
     total=False,
 )
 
 TargetGroupPairInfoOutputTypeDef = TypedDict(
     "TargetGroupPairInfoOutputTypeDef",
     {
-        "targetGroups": List[TargetGroupInfoOutputTypeDef],
+        "targetGroups": List[TargetGroupInfoTypeDef],
         "prodTrafficRoute": TrafficRouteOutputTypeDef,
         "testTrafficRoute": TrafficRouteOutputTypeDef,
     },
     total=False,
 )
 
 TargetGroupPairInfoTypeDef = TypedDict(
@@ -1679,54 +1450,60 @@
         "targetGroups": Sequence[TargetGroupInfoTypeDef],
         "prodTrafficRoute": TrafficRouteTypeDef,
         "testTrafficRoute": TrafficRouteTypeDef,
     },
     total=False,
 )
 
-TrafficRoutingConfigOutputTypeDef = TypedDict(
-    "TrafficRoutingConfigOutputTypeDef",
-    {
-        "type": TrafficRoutingTypeType,
-        "timeBasedCanary": TimeBasedCanaryOutputTypeDef,
-        "timeBasedLinear": TimeBasedLinearOutputTypeDef,
-    },
-    total=False,
-)
-
 TrafficRoutingConfigTypeDef = TypedDict(
     "TrafficRoutingConfigTypeDef",
     {
         "type": TrafficRoutingTypeType,
         "timeBasedCanary": TimeBasedCanaryTypeDef,
         "timeBasedLinear": TimeBasedLinearTypeDef,
     },
     total=False,
 )
 
-TargetInstancesTypeDef = TypedDict(
-    "TargetInstancesTypeDef",
+BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
+    "BatchGetOnPremisesInstancesOutputTypeDef",
     {
-        "tagFilters": Sequence[EC2TagFilterTypeDef],
-        "autoScalingGroups": Sequence[str],
-        "ec2TagSet": EC2TagSetTypeDef,
+        "instanceInfos": List[InstanceInfoTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOnPremisesInstanceOutputTypeDef = TypedDict(
+    "GetOnPremisesInstanceOutputTypeDef",
+    {
+        "instanceInfo": InstanceInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 TargetInstancesOutputTypeDef = TypedDict(
     "TargetInstancesOutputTypeDef",
     {
-        "tagFilters": List[EC2TagFilterOutputTypeDef],
+        "tagFilters": List[EC2TagFilterTypeDef],
         "autoScalingGroups": List[str],
         "ec2TagSet": EC2TagSetOutputTypeDef,
     },
     total=False,
 )
 
+TargetInstancesTypeDef = TypedDict(
+    "TargetInstancesTypeDef",
+    {
+        "tagFilters": Sequence[EC2TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
+        "ec2TagSet": EC2TagSetTypeDef,
+    },
+    total=False,
+)
+
 CloudFormationTargetTypeDef = TypedDict(
     "CloudFormationTargetTypeDef",
     {
         "deploymentId": str,
         "targetId": str,
         "lastUpdatedAt": datetime,
         "lifecycleEvents": List[LifecycleEventTypeDef],
@@ -1788,71 +1565,46 @@
         "lifecycleEvents": List[LifecycleEventTypeDef],
         "status": TargetStatusType,
         "taskSetsInfo": List[ECSTaskSetTypeDef],
     },
     total=False,
 )
 
-BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
-    "BatchGetOnPremisesInstancesOutputTypeDef",
+BatchGetApplicationRevisionsInputRequestTypeDef = TypedDict(
+    "BatchGetApplicationRevisionsInputRequestTypeDef",
     {
-        "instanceInfos": List[InstanceInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "applicationName": str,
+        "revisions": Sequence[RevisionLocationTypeDef],
     },
 )
 
-GetOnPremisesInstanceOutputTypeDef = TypedDict(
-    "GetOnPremisesInstanceOutputTypeDef",
+GetApplicationRevisionInputRequestTypeDef = TypedDict(
+    "GetApplicationRevisionInputRequestTypeDef",
     {
-        "instanceInfo": InstanceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "applicationName": str,
+        "revision": RevisionLocationTypeDef,
     },
 )
 
 GetApplicationRevisionOutputTypeDef = TypedDict(
     "GetApplicationRevisionOutputTypeDef",
     {
         "applicationName": str,
-        "revision": RevisionLocationOutputTypeDef,
+        "revision": RevisionLocationTypeDef,
         "revisionInfo": GenericRevisionInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationRevisionsOutputTypeDef = TypedDict(
     "ListApplicationRevisionsOutputTypeDef",
     {
-        "revisions": List[RevisionLocationOutputTypeDef],
+        "revisions": List[RevisionLocationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RevisionInfoTypeDef = TypedDict(
-    "RevisionInfoTypeDef",
-    {
-        "revisionLocation": RevisionLocationOutputTypeDef,
-        "genericRevisionInfo": GenericRevisionInfoTypeDef,
-    },
-    total=False,
-)
-
-BatchGetApplicationRevisionsInputRequestTypeDef = TypedDict(
-    "BatchGetApplicationRevisionsInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "revisions": Sequence[RevisionLocationTypeDef],
-    },
-)
-
-GetApplicationRevisionInputRequestTypeDef = TypedDict(
-    "GetApplicationRevisionInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "revision": RevisionLocationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterApplicationRevisionInputRequestTypeDef = TypedDict(
     "_RequiredRegisterApplicationRevisionInputRequestTypeDef",
     {
         "applicationName": str,
@@ -1863,27 +1615,34 @@
     "_OptionalRegisterApplicationRevisionInputRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class RegisterApplicationRevisionInputRequestTypeDef(
     _RequiredRegisterApplicationRevisionInputRequestTypeDef,
     _OptionalRegisterApplicationRevisionInputRequestTypeDef,
 ):
     pass
 
+RevisionInfoTypeDef = TypedDict(
+    "RevisionInfoTypeDef",
+    {
+        "revisionLocation": RevisionLocationTypeDef,
+        "genericRevisionInfo": GenericRevisionInfoTypeDef,
+    },
+    total=False,
+)
 
 LoadBalancerInfoOutputTypeDef = TypedDict(
     "LoadBalancerInfoOutputTypeDef",
     {
-        "elbInfoList": List[ELBInfoOutputTypeDef],
-        "targetGroupInfoList": List[TargetGroupInfoOutputTypeDef],
+        "elbInfoList": List[ELBInfoTypeDef],
+        "targetGroupInfoList": List[TargetGroupInfoTypeDef],
         "targetGroupPairInfoList": List[TargetGroupPairInfoOutputTypeDef],
     },
     total=False,
 )
 
 LoadBalancerInfoTypeDef = TypedDict(
     "LoadBalancerInfoTypeDef",
@@ -1891,27 +1650,14 @@
         "elbInfoList": Sequence[ELBInfoTypeDef],
         "targetGroupInfoList": Sequence[TargetGroupInfoTypeDef],
         "targetGroupPairInfoList": Sequence[TargetGroupPairInfoTypeDef],
     },
     total=False,
 )
 
-DeploymentConfigInfoTypeDef = TypedDict(
-    "DeploymentConfigInfoTypeDef",
-    {
-        "deploymentConfigId": str,
-        "deploymentConfigName": str,
-        "minimumHealthyHosts": MinimumHealthyHostsOutputTypeDef,
-        "createTime": datetime,
-        "computePlatform": ComputePlatformType,
-        "trafficRoutingConfig": TrafficRoutingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateDeploymentConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentConfigInputRequestTypeDef",
     {
         "deploymentConfigName": str,
     },
 )
 _OptionalCreateDeploymentConfigInputRequestTypeDef = TypedDict(
@@ -1920,21 +1666,32 @@
         "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
         "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
-
 class CreateDeploymentConfigInputRequestTypeDef(
     _RequiredCreateDeploymentConfigInputRequestTypeDef,
     _OptionalCreateDeploymentConfigInputRequestTypeDef,
 ):
     pass
 
+DeploymentConfigInfoTypeDef = TypedDict(
+    "DeploymentConfigInfoTypeDef",
+    {
+        "deploymentConfigId": str,
+        "deploymentConfigName": str,
+        "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
+        "createTime": datetime,
+        "computePlatform": ComputePlatformType,
+        "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
+    },
+    total=False,
+)
 
 _RequiredCreateDeploymentInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
@@ -1951,35 +1708,33 @@
         "updateOutdatedInstancesOnly": bool,
         "fileExistsBehavior": FileExistsBehaviorType,
         "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateDeploymentInputRequestTypeDef(
     _RequiredCreateDeploymentInputRequestTypeDef, _OptionalCreateDeploymentInputRequestTypeDef
 ):
     pass
 
-
 BatchGetDeploymentInstancesOutputTypeDef = TypedDict(
     "BatchGetDeploymentInstancesOutputTypeDef",
     {
         "instancesSummary": List[InstanceSummaryTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentInstanceOutputTypeDef = TypedDict(
     "GetDeploymentInstanceOutputTypeDef",
     {
         "instanceSummary": InstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentTargetTypeDef = TypedDict(
     "DeploymentTargetTypeDef",
     {
         "deploymentTargetType": DeploymentTargetTypeType,
@@ -1993,72 +1748,72 @@
 
 BatchGetApplicationRevisionsOutputTypeDef = TypedDict(
     "BatchGetApplicationRevisionsOutputTypeDef",
     {
         "applicationName": str,
         "errorMessage": str,
         "revisions": List[RevisionInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentGroupInfoTypeDef = TypedDict(
     "DeploymentGroupInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupId": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
-        "ec2TagFilters": List[EC2TagFilterOutputTypeDef],
-        "onPremisesInstanceTagFilters": List[TagFilterOutputTypeDef],
+        "ec2TagFilters": List[EC2TagFilterTypeDef],
+        "onPremisesInstanceTagFilters": List[TagFilterTypeDef],
         "autoScalingGroups": List[AutoScalingGroupTypeDef],
         "serviceRoleArn": str,
-        "targetRevision": RevisionLocationOutputTypeDef,
+        "targetRevision": RevisionLocationTypeDef,
         "triggerConfigurations": List[TriggerConfigOutputTypeDef],
         "alarmConfiguration": AlarmConfigurationOutputTypeDef,
         "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
-        "deploymentStyle": DeploymentStyleOutputTypeDef,
+        "deploymentStyle": DeploymentStyleTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationOutputTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "lastSuccessfulDeployment": LastDeploymentInfoTypeDef,
         "lastAttemptedDeployment": LastDeploymentInfoTypeDef,
         "ec2TagSet": EC2TagSetOutputTypeDef,
         "onPremisesTagSet": OnPremisesTagSetOutputTypeDef,
         "computePlatform": ComputePlatformType,
-        "ecsServices": List[ECSServiceOutputTypeDef],
+        "ecsServices": List[ECSServiceTypeDef],
     },
     total=False,
 )
 
 DeploymentInfoTypeDef = TypedDict(
     "DeploymentInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
         "deploymentId": str,
-        "previousRevision": RevisionLocationOutputTypeDef,
-        "revision": RevisionLocationOutputTypeDef,
+        "previousRevision": RevisionLocationTypeDef,
+        "revision": RevisionLocationTypeDef,
         "status": DeploymentStatusType,
         "errorInformation": ErrorInformationTypeDef,
         "createTime": datetime,
         "startTime": datetime,
         "completeTime": datetime,
         "deploymentOverview": DeploymentOverviewTypeDef,
         "description": str,
         "creator": DeploymentCreatorType,
         "ignoreApplicationStopFailures": bool,
         "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
         "updateOutdatedInstancesOnly": bool,
         "rollbackInfo": RollbackInfoTypeDef,
-        "deploymentStyle": DeploymentStyleOutputTypeDef,
+        "deploymentStyle": DeploymentStyleTypeDef,
         "targetInstances": TargetInstancesOutputTypeDef,
         "instanceTerminationWaitTimeStarted": bool,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationOutputTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "additionalDeploymentStatusInfo": str,
         "fileExistsBehavior": FileExistsBehaviorType,
         "deploymentStatusMessages": List[str],
         "computePlatform": ComputePlatformType,
         "externalId": str,
         "relatedDeployments": RelatedDeploymentsTypeDef,
@@ -2093,22 +1848,20 @@
         "ecsServices": Sequence[ECSServiceTypeDef],
         "onPremisesTagSet": OnPremisesTagSetTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDeploymentGroupInputRequestTypeDef(
     _RequiredCreateDeploymentGroupInputRequestTypeDef,
     _OptionalCreateDeploymentGroupInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
         "currentDeploymentGroupName": str,
     },
 )
@@ -2131,71 +1884,69 @@
         "ec2TagSet": EC2TagSetTypeDef,
         "ecsServices": Sequence[ECSServiceTypeDef],
         "onPremisesTagSet": OnPremisesTagSetTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDeploymentGroupInputRequestTypeDef(
     _RequiredUpdateDeploymentGroupInputRequestTypeDef,
     _OptionalUpdateDeploymentGroupInputRequestTypeDef,
 ):
     pass
 
-
 GetDeploymentConfigOutputTypeDef = TypedDict(
     "GetDeploymentConfigOutputTypeDef",
     {
         "deploymentConfigInfo": DeploymentConfigInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentTargetsOutputTypeDef = TypedDict(
     "BatchGetDeploymentTargetsOutputTypeDef",
     {
         "deploymentTargets": List[DeploymentTargetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentTargetOutputTypeDef = TypedDict(
     "GetDeploymentTargetOutputTypeDef",
     {
         "deploymentTarget": DeploymentTargetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentGroupsOutputTypeDef = TypedDict(
     "BatchGetDeploymentGroupsOutputTypeDef",
     {
         "deploymentGroupsInfo": List[DeploymentGroupInfoTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentGroupOutputTypeDef = TypedDict(
     "GetDeploymentGroupOutputTypeDef",
     {
         "deploymentGroupInfo": DeploymentGroupInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentsOutputTypeDef = TypedDict(
     "BatchGetDeploymentsOutputTypeDef",
     {
         "deploymentsInfo": List[DeploymentInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentOutputTypeDef = TypedDict(
     "GetDeploymentOutputTypeDef",
     {
         "deploymentInfo": DeploymentInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/type_defs.pyi` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,178 +52,158 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
-    "AlarmOutputTypeDef",
     "AlarmTypeDef",
-    "AppSpecContentOutputTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
     "AutoRollbackConfigurationOutputTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetApplicationsInputRequestTypeDef",
     "BatchGetDeploymentGroupsInputRequestTypeDef",
     "BatchGetDeploymentInstancesInputRequestTypeDef",
     "BatchGetDeploymentTargetsInputRequestTypeDef",
     "BatchGetDeploymentsInputRequestTypeDef",
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
-    "BlueInstanceTerminationOptionOutputTypeDef",
-    "DeploymentReadyOptionOutputTypeDef",
-    "GreenFleetProvisioningOptionOutputTypeDef",
     "BlueInstanceTerminationOptionTypeDef",
     "DeploymentReadyOptionTypeDef",
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
-    "CreateApplicationOutputTypeDef",
     "MinimumHealthyHostsTypeDef",
-    "CreateDeploymentConfigOutputTypeDef",
     "DeploymentStyleTypeDef",
     "EC2TagFilterTypeDef",
     "ECSServiceTypeDef",
     "TagFilterTypeDef",
     "TriggerConfigTypeDef",
-    "CreateDeploymentGroupOutputTypeDef",
-    "CreateDeploymentOutputTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
-    "DeleteGitHubAccountTokenOutputTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
-    "MinimumHealthyHostsOutputTypeDef",
-    "DeploymentStyleOutputTypeDef",
-    "EC2TagFilterOutputTypeDef",
-    "ECSServiceOutputTypeDef",
     "LastDeploymentInfoTypeDef",
-    "TagFilterOutputTypeDef",
     "TriggerConfigOutputTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
-    "TargetGroupInfoOutputTypeDef",
-    "ELBInfoOutputTypeDef",
+    "TargetGroupInfoTypeDef",
     "ELBInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GenericRevisionInfoTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetDeploymentConfigInputRequestTypeDef",
     "GetDeploymentGroupInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetDeploymentInstanceInputRequestTypeDef",
     "GetDeploymentTargetInputRequestTypeDef",
     "GetOnPremisesInstanceInputRequestTypeDef",
-    "GitHubLocationOutputTypeDef",
     "GitHubLocationTypeDef",
-    "TagOutputTypeDef",
     "LambdaFunctionInfoTypeDef",
-    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationRevisionsInputRequestTypeDef",
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListApplicationsInputRequestTypeDef",
-    "ListApplicationsOutputTypeDef",
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     "ListDeploymentConfigsInputRequestTypeDef",
-    "ListDeploymentConfigsOutputTypeDef",
-    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     "ListDeploymentGroupsInputRequestTypeDef",
-    "ListDeploymentGroupsOutputTypeDef",
-    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     "ListDeploymentInstancesInputRequestTypeDef",
-    "ListDeploymentInstancesOutputTypeDef",
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     "ListDeploymentTargetsInputRequestTypeDef",
-    "ListDeploymentTargetsOutputTypeDef",
     "TimeRangeTypeDef",
-    "ListDeploymentsOutputTypeDef",
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    "ListOnPremisesInstancesOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TargetGroupInfoTypeDef",
-    "PaginatorConfigTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
-    "RawStringOutputTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
-    "StopDeploymentOutputTypeDef",
     "TrafficRouteOutputTypeDef",
     "TrafficRouteTypeDef",
-    "TimeBasedCanaryOutputTypeDef",
     "TimeBasedCanaryTypeDef",
-    "TimeBasedLinearOutputTypeDef",
     "TimeBasedLinearTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
+    "InstanceInfoTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
     "BatchGetApplicationsOutputTypeDef",
-    "GetApplicationOutputTypeDef",
+    "CreateApplicationOutputTypeDef",
+    "CreateDeploymentConfigOutputTypeDef",
+    "CreateDeploymentGroupOutputTypeDef",
+    "CreateDeploymentOutputTypeDef",
     "DeleteDeploymentGroupOutputTypeDef",
+    "DeleteGitHubAccountTokenOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetApplicationOutputTypeDef",
+    "ListApplicationsOutputTypeDef",
+    "ListDeploymentConfigsOutputTypeDef",
+    "ListDeploymentGroupsOutputTypeDef",
+    "ListDeploymentInstancesOutputTypeDef",
+    "ListDeploymentTargetsOutputTypeDef",
+    "ListDeploymentsOutputTypeDef",
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    "ListOnPremisesInstancesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    "StopDeploymentOutputTypeDef",
     "UpdateDeploymentGroupOutputTypeDef",
-    "BlueGreenDeploymentConfigurationOutputTypeDef",
     "BlueGreenDeploymentConfigurationTypeDef",
+    "EC2TagSetOutputTypeDef",
     "EC2TagSetTypeDef",
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListOnPremisesInstancesInputRequestTypeDef",
-    "OnPremisesTagSetTypeDef",
-    "EC2TagSetOutputTypeDef",
     "OnPremisesTagSetOutputTypeDef",
+    "OnPremisesTagSetTypeDef",
     "LifecycleEventTypeDef",
     "ECSTaskSetTypeDef",
     "GetDeploymentInputDeploymentSuccessfulWaitTypeDef",
-    "InstanceInfoTypeDef",
-    "ListTagsForResourceOutputTypeDef",
+    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
+    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
-    "RevisionLocationOutputTypeDef",
     "RevisionLocationTypeDef",
     "TargetGroupPairInfoOutputTypeDef",
     "TargetGroupPairInfoTypeDef",
-    "TrafficRoutingConfigOutputTypeDef",
     "TrafficRoutingConfigTypeDef",
-    "TargetInstancesTypeDef",
+    "BatchGetOnPremisesInstancesOutputTypeDef",
+    "GetOnPremisesInstanceOutputTypeDef",
     "TargetInstancesOutputTypeDef",
+    "TargetInstancesTypeDef",
     "CloudFormationTargetTypeDef",
     "InstanceSummaryTypeDef",
     "InstanceTargetTypeDef",
     "LambdaTargetTypeDef",
     "ECSTargetTypeDef",
-    "BatchGetOnPremisesInstancesOutputTypeDef",
-    "GetOnPremisesInstanceOutputTypeDef",
-    "GetApplicationRevisionOutputTypeDef",
-    "ListApplicationRevisionsOutputTypeDef",
-    "RevisionInfoTypeDef",
     "BatchGetApplicationRevisionsInputRequestTypeDef",
     "GetApplicationRevisionInputRequestTypeDef",
+    "GetApplicationRevisionOutputTypeDef",
+    "ListApplicationRevisionsOutputTypeDef",
     "RegisterApplicationRevisionInputRequestTypeDef",
+    "RevisionInfoTypeDef",
     "LoadBalancerInfoOutputTypeDef",
     "LoadBalancerInfoTypeDef",
-    "DeploymentConfigInfoTypeDef",
     "CreateDeploymentConfigInputRequestTypeDef",
+    "DeploymentConfigInfoTypeDef",
     "CreateDeploymentInputRequestTypeDef",
     "BatchGetDeploymentInstancesOutputTypeDef",
     "GetDeploymentInstanceOutputTypeDef",
     "DeploymentTargetTypeDef",
     "BatchGetApplicationRevisionsOutputTypeDef",
     "DeploymentGroupInfoTypeDef",
     "DeploymentInfoTypeDef",
@@ -243,39 +223,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AlarmOutputTypeDef = TypedDict(
-    "AlarmOutputTypeDef",
-    {
-        "name": str,
-    },
-    total=False,
-)
-
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
-AppSpecContentOutputTypeDef = TypedDict(
-    "AppSpecContentOutputTypeDef",
-    {
-        "content": str,
-        "sha256": str,
-    },
-    total=False,
-)
-
 AppSpecContentTypeDef = TypedDict(
     "AppSpecContentTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -317,14 +280,25 @@
     {
         "name": str,
         "hook": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 BatchGetApplicationsInputRequestTypeDef = TypedDict(
     "BatchGetApplicationsInputRequestTypeDef",
     {
         "applicationNames": Sequence[str],
     },
 )
 
@@ -363,40 +337,14 @@
 BatchGetOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
     {
         "instanceNames": Sequence[str],
     },
 )
 
-BlueInstanceTerminationOptionOutputTypeDef = TypedDict(
-    "BlueInstanceTerminationOptionOutputTypeDef",
-    {
-        "action": InstanceActionType,
-        "terminationWaitTimeInMinutes": int,
-    },
-    total=False,
-)
-
-DeploymentReadyOptionOutputTypeDef = TypedDict(
-    "DeploymentReadyOptionOutputTypeDef",
-    {
-        "actionOnTimeout": DeploymentReadyActionType,
-        "waitTimeInMinutes": int,
-    },
-    total=False,
-)
-
-GreenFleetProvisioningOptionOutputTypeDef = TypedDict(
-    "GreenFleetProvisioningOptionOutputTypeDef",
-    {
-        "action": GreenFleetProvisioningActionType,
-    },
-    total=False,
-)
-
 BlueInstanceTerminationOptionTypeDef = TypedDict(
     "BlueInstanceTerminationOptionTypeDef",
     {
         "action": InstanceActionType,
         "terminationWaitTimeInMinutes": int,
     },
     total=False,
@@ -424,39 +372,23 @@
     {
         "deploymentId": str,
         "deploymentWaitType": DeploymentWaitTypeType,
     },
     total=False,
 )
 
-CreateApplicationOutputTypeDef = TypedDict(
-    "CreateApplicationOutputTypeDef",
-    {
-        "applicationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MinimumHealthyHostsTypeDef = TypedDict(
     "MinimumHealthyHostsTypeDef",
     {
         "type": MinimumHealthyHostsTypeType,
         "value": int,
     },
     total=False,
 )
 
-CreateDeploymentConfigOutputTypeDef = TypedDict(
-    "CreateDeploymentConfigOutputTypeDef",
-    {
-        "deploymentConfigId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentStyleTypeDef = TypedDict(
     "DeploymentStyleTypeDef",
     {
         "deploymentType": DeploymentTypeType,
         "deploymentOption": DeploymentOptionType,
     },
     total=False,
@@ -497,30 +429,14 @@
         "triggerName": str,
         "triggerTargetArn": str,
         "triggerEvents": Sequence[TriggerEventTypeType],
     },
     total=False,
 )
 
-CreateDeploymentGroupOutputTypeDef = TypedDict(
-    "CreateDeploymentGroupOutputTypeDef",
-    {
-        "deploymentGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDeploymentOutputTypeDef = TypedDict(
-    "CreateDeploymentOutputTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationInputRequestTypeDef = TypedDict(
     "DeleteApplicationInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 
@@ -543,88 +459,33 @@
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     {
         "tokenName": str,
     },
     total=False,
 )
 
-DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
-    "DeleteGitHubAccountTokenOutputTypeDef",
-    {
-        "tokenName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteResourcesByExternalIdInputRequestTypeDef = TypedDict(
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
 
-MinimumHealthyHostsOutputTypeDef = TypedDict(
-    "MinimumHealthyHostsOutputTypeDef",
-    {
-        "type": MinimumHealthyHostsTypeType,
-        "value": int,
-    },
-    total=False,
-)
-
-DeploymentStyleOutputTypeDef = TypedDict(
-    "DeploymentStyleOutputTypeDef",
-    {
-        "deploymentType": DeploymentTypeType,
-        "deploymentOption": DeploymentOptionType,
-    },
-    total=False,
-)
-
-EC2TagFilterOutputTypeDef = TypedDict(
-    "EC2TagFilterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "Type": EC2TagFilterTypeType,
-    },
-    total=False,
-)
-
-ECSServiceOutputTypeDef = TypedDict(
-    "ECSServiceOutputTypeDef",
-    {
-        "serviceName": str,
-        "clusterName": str,
-    },
-    total=False,
-)
-
 LastDeploymentInfoTypeDef = TypedDict(
     "LastDeploymentInfoTypeDef",
     {
         "deploymentId": str,
         "status": DeploymentStatusType,
         "endTime": datetime,
         "createTime": datetime,
     },
     total=False,
 )
 
-TagFilterOutputTypeDef = TypedDict(
-    "TagFilterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "Type": TagFilterTypeType,
-    },
-    total=False,
-)
-
 TriggerConfigOutputTypeDef = TypedDict(
     "TriggerConfigOutputTypeDef",
     {
         "triggerName": str,
         "triggerTargetArn": str,
         "triggerEvents": List[TriggerEventTypeType],
     },
@@ -686,45 +547,30 @@
         "scriptName": str,
         "message": str,
         "logTail": str,
     },
     total=False,
 )
 
-TargetGroupInfoOutputTypeDef = TypedDict(
-    "TargetGroupInfoOutputTypeDef",
-    {
-        "name": str,
-    },
-    total=False,
-)
-
-ELBInfoOutputTypeDef = TypedDict(
-    "ELBInfoOutputTypeDef",
+TargetGroupInfoTypeDef = TypedDict(
+    "TargetGroupInfoTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
 ELBInfoTypeDef = TypedDict(
     "ELBInfoTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GenericRevisionInfoTypeDef = TypedDict(
     "GenericRevisionInfoTypeDef",
     {
         "description": str,
         "deploymentGroups": List[str],
         "firstUsedTime": datetime,
         "lastUsedTime": datetime,
@@ -791,78 +637,45 @@
 GetOnPremisesInstanceInputRequestTypeDef = TypedDict(
     "GetOnPremisesInstanceInputRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 
-GitHubLocationOutputTypeDef = TypedDict(
-    "GitHubLocationOutputTypeDef",
-    {
-        "repository": str,
-        "commitId": str,
-    },
-    total=False,
-)
-
 GitHubLocationTypeDef = TypedDict(
     "GitHubLocationTypeDef",
     {
         "repository": str,
         "commitId": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 LambdaFunctionInfoTypeDef = TypedDict(
     "LambdaFunctionInfoTypeDef",
     {
         "functionName": str,
         "functionAlias": str,
         "currentVersion": str,
         "targetVersion": str,
         "targetVersionWeight": float,
     },
     total=False,
 )
 
-_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "sortBy": ApplicationRevisionSortByType,
-        "sortOrder": SortOrderType,
-        "s3Bucket": str,
-        "s3KeyPrefix": str,
-        "deployed": ListStateFilterActionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
-    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListApplicationRevisionsInputRequestTypeDef = TypedDict(
     "_RequiredListApplicationRevisionsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListApplicationRevisionsInputRequestTypeDef = TypedDict(
@@ -874,141 +687,59 @@
         "s3KeyPrefix": str,
         "deployed": ListStateFilterActionType,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationRevisionsInputRequestTypeDef(
     _RequiredListApplicationRevisionsInputRequestTypeDef,
     _OptionalListApplicationRevisionsInputRequestTypeDef,
 ):
     pass
 
-ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListApplicationsOutputTypeDef = TypedDict(
-    "ListApplicationsOutputTypeDef",
-    {
-        "applications": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeploymentConfigsInputRequestTypeDef = TypedDict(
     "ListDeploymentConfigsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListDeploymentConfigsOutputTypeDef = TypedDict(
-    "ListDeploymentConfigsOutputTypeDef",
-    {
-        "deploymentConfigsList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
-    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDeploymentGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentGroupsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListDeploymentGroupsInputRequestTypeDef = TypedDict(
     "_OptionalListDeploymentGroupsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListDeploymentGroupsInputRequestTypeDef(
     _RequiredListDeploymentGroupsInputRequestTypeDef,
     _OptionalListDeploymentGroupsInputRequestTypeDef,
 ):
     pass
 
-ListDeploymentGroupsOutputTypeDef = TypedDict(
-    "ListDeploymentGroupsOutputTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "deploymentId": str,
-    },
-)
-_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "instanceStatusFilter": Sequence[InstanceStatusType],
-        "instanceTypeFilter": Sequence[InstanceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
-    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-):
-    pass
 
 _RequiredListDeploymentInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentInstancesInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
@@ -1018,174 +749,80 @@
         "nextToken": str,
         "instanceStatusFilter": Sequence[InstanceStatusType],
         "instanceTypeFilter": Sequence[InstanceTypeType],
     },
     total=False,
 )
 
+
 class ListDeploymentInstancesInputRequestTypeDef(
     _RequiredListDeploymentInstancesInputRequestTypeDef,
     _OptionalListDeploymentInstancesInputRequestTypeDef,
 ):
     pass
 
-ListDeploymentInstancesOutputTypeDef = TypedDict(
-    "ListDeploymentInstancesOutputTypeDef",
-    {
-        "instancesList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
-    {
-        "deploymentId": str,
-        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListDeploymentTargetsInputRequestTypeDef = TypedDict(
     "ListDeploymentTargetsInputRequestTypeDef",
     {
         "deploymentId": str,
         "nextToken": str,
         "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
     },
     total=False,
 )
 
-ListDeploymentTargetsOutputTypeDef = TypedDict(
-    "ListDeploymentTargetsOutputTypeDef",
-    {
-        "targetIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TimeRangeTypeDef = TypedDict(
     "TimeRangeTypeDef",
     {
         "start": Union[datetime, str],
         "end": Union[datetime, str],
     },
     total=False,
 )
 
-ListDeploymentsOutputTypeDef = TypedDict(
-    "ListDeploymentsOutputTypeDef",
-    {
-        "deployments": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGitHubAccountTokenNamesInputRequestTypeDef = TypedDict(
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    {
-        "tokenNameList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListOnPremisesInstancesOutputTypeDef = TypedDict(
-    "ListOnPremisesInstancesOutputTypeDef",
-    {
-        "instanceNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
     "_OptionalListTagsForResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-TargetGroupInfoTypeDef = TypedDict(
-    "TargetGroupInfoTypeDef",
-    {
-        "name": str,
-    },
-    total=False,
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
 
 PutLifecycleEventHookExecutionStatusInputRequestTypeDef = TypedDict(
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     {
         "deploymentId": str,
         "lifecycleEventHookExecutionId": str,
         "status": LifecycleEventStatusType,
     },
     total=False,
 )
 
-PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
-    {
-        "lifecycleEventHookExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RawStringOutputTypeDef = TypedDict(
-    "RawStringOutputTypeDef",
-    {
-        "content": str,
-        "sha256": str,
-    },
-    total=False,
-)
-
 RawStringTypeDef = TypedDict(
     "RawStringTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -1202,42 +839,21 @@
     {
         "iamSessionArn": str,
         "iamUserArn": str,
     },
     total=False,
 )
 
+
 class RegisterOnPremisesInstanceInputRequestTypeDef(
     _RequiredRegisterOnPremisesInstanceInputRequestTypeDef,
     _OptionalRegisterOnPremisesInstanceInputRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-        "bundleType": BundleTypeType,
-        "version": str,
-        "eTag": str,
-    },
-    total=False,
-)
 
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "bundleType": BundleTypeType,
@@ -1265,27 +881,20 @@
     "_OptionalStopDeploymentInputRequestTypeDef",
     {
         "autoRollbackEnabled": bool,
     },
     total=False,
 )
 
+
 class StopDeploymentInputRequestTypeDef(
     _RequiredStopDeploymentInputRequestTypeDef, _OptionalStopDeploymentInputRequestTypeDef
 ):
     pass
 
-StopDeploymentOutputTypeDef = TypedDict(
-    "StopDeploymentOutputTypeDef",
-    {
-        "status": StopStatusType,
-        "statusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TrafficRouteOutputTypeDef = TypedDict(
     "TrafficRouteOutputTypeDef",
     {
         "listenerArns": List[str],
     },
     total=False,
@@ -1295,41 +904,23 @@
     "TrafficRouteTypeDef",
     {
         "listenerArns": Sequence[str],
     },
     total=False,
 )
 
-TimeBasedCanaryOutputTypeDef = TypedDict(
-    "TimeBasedCanaryOutputTypeDef",
-    {
-        "canaryPercentage": int,
-        "canaryInterval": int,
-    },
-    total=False,
-)
-
 TimeBasedCanaryTypeDef = TypedDict(
     "TimeBasedCanaryTypeDef",
     {
         "canaryPercentage": int,
         "canaryInterval": int,
     },
     total=False,
 )
 
-TimeBasedLinearOutputTypeDef = TypedDict(
-    "TimeBasedLinearOutputTypeDef",
-    {
-        "linearPercentage": int,
-        "linearInterval": int,
-    },
-    total=False,
-)
-
 TimeBasedLinearTypeDef = TypedDict(
     "TimeBasedLinearTypeDef",
     {
         "linearPercentage": int,
         "linearInterval": int,
     },
     total=False,
@@ -1371,19 +962,35 @@
     {
         "computePlatform": ComputePlatformType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateApplicationInputRequestTypeDef(
     _RequiredCreateApplicationInputRequestTypeDef, _OptionalCreateApplicationInputRequestTypeDef
 ):
     pass
 
+
+InstanceInfoTypeDef = TypedDict(
+    "InstanceInfoTypeDef",
+    {
+        "instanceName": str,
+        "iamSessionArn": str,
+        "iamUserArn": str,
+        "instanceArn": str,
+        "registerTime": datetime,
+        "deregisterTime": datetime,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 RemoveTagsFromOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
         "instanceNames": Sequence[str],
     },
 )
@@ -1397,15 +1004,15 @@
 )
 
 AlarmConfigurationOutputTypeDef = TypedDict(
     "AlarmConfigurationOutputTypeDef",
     {
         "enabled": bool,
         "ignorePollAlarmFailure": bool,
-        "alarms": List[AlarmOutputTypeDef],
+        "alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
 AlarmConfigurationTypeDef = TypedDict(
     "AlarmConfigurationTypeDef",
     {
@@ -1416,110 +1023,236 @@
     total=False,
 )
 
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
         "applicationsInfo": List[ApplicationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetApplicationOutputTypeDef = TypedDict(
-    "GetApplicationOutputTypeDef",
+CreateApplicationOutputTypeDef = TypedDict(
+    "CreateApplicationOutputTypeDef",
     {
-        "application": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "applicationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentConfigOutputTypeDef = TypedDict(
+    "CreateDeploymentConfigOutputTypeDef",
+    {
+        "deploymentConfigId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentGroupOutputTypeDef = TypedDict(
+    "CreateDeploymentGroupOutputTypeDef",
+    {
+        "deploymentGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentOutputTypeDef = TypedDict(
+    "CreateDeploymentOutputTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDeploymentGroupOutputTypeDef = TypedDict(
     "DeleteDeploymentGroupOutputTypeDef",
     {
         "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDeploymentGroupOutputTypeDef = TypedDict(
-    "UpdateDeploymentGroupOutputTypeDef",
+DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
+    "DeleteGitHubAccountTokenOutputTypeDef",
     {
-        "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tokenName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BlueGreenDeploymentConfigurationOutputTypeDef = TypedDict(
-    "BlueGreenDeploymentConfigurationOutputTypeDef",
+GetApplicationOutputTypeDef = TypedDict(
+    "GetApplicationOutputTypeDef",
     {
-        "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionOutputTypeDef,
-        "deploymentReadyOption": DeploymentReadyOptionOutputTypeDef,
-        "greenFleetProvisioningOption": GreenFleetProvisioningOptionOutputTypeDef,
+        "application": ApplicationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsOutputTypeDef = TypedDict(
+    "ListApplicationsOutputTypeDef",
+    {
+        "applications": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentConfigsOutputTypeDef = TypedDict(
+    "ListDeploymentConfigsOutputTypeDef",
+    {
+        "deploymentConfigsList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentGroupsOutputTypeDef = TypedDict(
+    "ListDeploymentGroupsOutputTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentInstancesOutputTypeDef = TypedDict(
+    "ListDeploymentInstancesOutputTypeDef",
+    {
+        "instancesList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentTargetsOutputTypeDef = TypedDict(
+    "ListDeploymentTargetsOutputTypeDef",
+    {
+        "targetIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
+    {
+        "deployments": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    {
+        "tokenNameList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOnPremisesInstancesOutputTypeDef = TypedDict(
+    "ListOnPremisesInstancesOutputTypeDef",
+    {
+        "instanceNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    {
+        "lifecycleEventHookExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDeploymentOutputTypeDef = TypedDict(
+    "StopDeploymentOutputTypeDef",
+    {
+        "status": StopStatusType,
+        "statusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDeploymentGroupOutputTypeDef = TypedDict(
+    "UpdateDeploymentGroupOutputTypeDef",
+    {
+        "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 BlueGreenDeploymentConfigurationTypeDef = TypedDict(
     "BlueGreenDeploymentConfigurationTypeDef",
     {
         "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionTypeDef,
         "deploymentReadyOption": DeploymentReadyOptionTypeDef,
         "greenFleetProvisioningOption": GreenFleetProvisioningOptionTypeDef,
     },
     total=False,
 )
 
-EC2TagSetTypeDef = TypedDict(
-    "EC2TagSetTypeDef",
+EC2TagSetOutputTypeDef = TypedDict(
+    "EC2TagSetOutputTypeDef",
     {
-        "ec2TagSetList": Sequence[Sequence[EC2TagFilterTypeDef]],
+        "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
-ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
+EC2TagSetTypeDef = TypedDict(
+    "EC2TagSetTypeDef",
     {
-        "registrationStatus": RegistrationStatusType,
-        "tagFilters": Sequence[TagFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ec2TagSetList": Sequence[Sequence[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
 ListOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "ListOnPremisesInstancesInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
-OnPremisesTagSetTypeDef = TypedDict(
-    "OnPremisesTagSetTypeDef",
-    {
-        "onPremisesTagSetList": Sequence[Sequence[TagFilterTypeDef]],
-    },
-    total=False,
-)
-
-EC2TagSetOutputTypeDef = TypedDict(
-    "EC2TagSetOutputTypeDef",
+OnPremisesTagSetOutputTypeDef = TypedDict(
+    "OnPremisesTagSetOutputTypeDef",
     {
-        "ec2TagSetList": List[List[EC2TagFilterOutputTypeDef]],
+        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
     },
     total=False,
 )
 
-OnPremisesTagSetOutputTypeDef = TypedDict(
-    "OnPremisesTagSetOutputTypeDef",
+OnPremisesTagSetTypeDef = TypedDict(
+    "OnPremisesTagSetTypeDef",
     {
-        "onPremisesTagSetList": List[List[TagFilterOutputTypeDef]],
+        "onPremisesTagSetList": Sequence[Sequence[TagFilterTypeDef]],
     },
     total=False,
 )
 
 LifecycleEventTypeDef = TypedDict(
     "LifecycleEventTypeDef",
     {
@@ -1537,15 +1270,15 @@
     {
         "identifer": str,
         "desiredCount": int,
         "pendingCount": int,
         "runningCount": int,
         "status": str,
         "trafficWeight": float,
-        "targetGroup": TargetGroupInfoOutputTypeDef,
+        "targetGroup": TargetGroupInfoTypeDef,
         "taskSetLabel": TargetLabelType,
     },
     total=False,
 )
 
 _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef = TypedDict(
     "_RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef",
@@ -1557,52 +1290,148 @@
     "_OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetDeploymentInputDeploymentSuccessfulWaitTypeDef(
     _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
     _OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
 ):
     pass
 
-InstanceInfoTypeDef = TypedDict(
-    "InstanceInfoTypeDef",
+
+_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     {
-        "instanceName": str,
-        "iamSessionArn": str,
-        "iamUserArn": str,
-        "instanceArn": str,
-        "registerTime": datetime,
-        "deregisterTime": datetime,
-        "tags": List[TagOutputTypeDef],
+        "applicationName": str,
+    },
+)
+_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    {
+        "sortBy": ApplicationRevisionSortByType,
+        "sortOrder": SortOrderType,
+        "s3Bucket": str,
+        "s3KeyPrefix": str,
+        "deployed": ListStateFilterActionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+
+class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
+    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+):
+    pass
+
+
+ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    {
+        "applicationName": str,
+    },
+)
+_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
+    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "deploymentId": str,
+    },
+)
+_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "instanceStatusFilter": Sequence[InstanceStatusType],
+        "instanceTypeFilter": Sequence[InstanceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
+    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+):
+    pass
+
+
+ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
+    {
+        "deploymentId": str,
+        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
+    {
+        "registrationStatus": RegistrationStatusType,
+        "tagFilters": Sequence[TagFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     {
         "applicationName": str,
         "deploymentGroupName": str,
         "externalId": str,
         "includeOnlyStatuses": Sequence[DeploymentStatusType],
         "createTimeRange": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDeploymentsInputRequestTypeDef = TypedDict(
     "ListDeploymentsInputRequestTypeDef",
     {
@@ -1612,26 +1441,14 @@
         "includeOnlyStatuses": Sequence[DeploymentStatusType],
         "createTimeRange": TimeRangeTypeDef,
         "nextToken": str,
     },
     total=False,
 )
 
-RevisionLocationOutputTypeDef = TypedDict(
-    "RevisionLocationOutputTypeDef",
-    {
-        "revisionType": RevisionLocationTypeType,
-        "s3Location": S3LocationOutputTypeDef,
-        "gitHubLocation": GitHubLocationOutputTypeDef,
-        "string": RawStringOutputTypeDef,
-        "appSpecContent": AppSpecContentOutputTypeDef,
-    },
-    total=False,
-)
-
 RevisionLocationTypeDef = TypedDict(
     "RevisionLocationTypeDef",
     {
         "revisionType": RevisionLocationTypeType,
         "s3Location": S3LocationTypeDef,
         "gitHubLocation": GitHubLocationTypeDef,
         "string": RawStringTypeDef,
@@ -1639,15 +1456,15 @@
     },
     total=False,
 )
 
 TargetGroupPairInfoOutputTypeDef = TypedDict(
     "TargetGroupPairInfoOutputTypeDef",
     {
-        "targetGroups": List[TargetGroupInfoOutputTypeDef],
+        "targetGroups": List[TargetGroupInfoTypeDef],
         "prodTrafficRoute": TrafficRouteOutputTypeDef,
         "testTrafficRoute": TrafficRouteOutputTypeDef,
     },
     total=False,
 )
 
 TargetGroupPairInfoTypeDef = TypedDict(
@@ -1656,54 +1473,60 @@
         "targetGroups": Sequence[TargetGroupInfoTypeDef],
         "prodTrafficRoute": TrafficRouteTypeDef,
         "testTrafficRoute": TrafficRouteTypeDef,
     },
     total=False,
 )
 
-TrafficRoutingConfigOutputTypeDef = TypedDict(
-    "TrafficRoutingConfigOutputTypeDef",
-    {
-        "type": TrafficRoutingTypeType,
-        "timeBasedCanary": TimeBasedCanaryOutputTypeDef,
-        "timeBasedLinear": TimeBasedLinearOutputTypeDef,
-    },
-    total=False,
-)
-
 TrafficRoutingConfigTypeDef = TypedDict(
     "TrafficRoutingConfigTypeDef",
     {
         "type": TrafficRoutingTypeType,
         "timeBasedCanary": TimeBasedCanaryTypeDef,
         "timeBasedLinear": TimeBasedLinearTypeDef,
     },
     total=False,
 )
 
-TargetInstancesTypeDef = TypedDict(
-    "TargetInstancesTypeDef",
+BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
+    "BatchGetOnPremisesInstancesOutputTypeDef",
     {
-        "tagFilters": Sequence[EC2TagFilterTypeDef],
-        "autoScalingGroups": Sequence[str],
-        "ec2TagSet": EC2TagSetTypeDef,
+        "instanceInfos": List[InstanceInfoTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOnPremisesInstanceOutputTypeDef = TypedDict(
+    "GetOnPremisesInstanceOutputTypeDef",
+    {
+        "instanceInfo": InstanceInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 TargetInstancesOutputTypeDef = TypedDict(
     "TargetInstancesOutputTypeDef",
     {
-        "tagFilters": List[EC2TagFilterOutputTypeDef],
+        "tagFilters": List[EC2TagFilterTypeDef],
         "autoScalingGroups": List[str],
         "ec2TagSet": EC2TagSetOutputTypeDef,
     },
     total=False,
 )
 
+TargetInstancesTypeDef = TypedDict(
+    "TargetInstancesTypeDef",
+    {
+        "tagFilters": Sequence[EC2TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
+        "ec2TagSet": EC2TagSetTypeDef,
+    },
+    total=False,
+)
+
 CloudFormationTargetTypeDef = TypedDict(
     "CloudFormationTargetTypeDef",
     {
         "deploymentId": str,
         "targetId": str,
         "lastUpdatedAt": datetime,
         "lifecycleEvents": List[LifecycleEventTypeDef],
@@ -1765,71 +1588,46 @@
         "lifecycleEvents": List[LifecycleEventTypeDef],
         "status": TargetStatusType,
         "taskSetsInfo": List[ECSTaskSetTypeDef],
     },
     total=False,
 )
 
-BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
-    "BatchGetOnPremisesInstancesOutputTypeDef",
+BatchGetApplicationRevisionsInputRequestTypeDef = TypedDict(
+    "BatchGetApplicationRevisionsInputRequestTypeDef",
     {
-        "instanceInfos": List[InstanceInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "applicationName": str,
+        "revisions": Sequence[RevisionLocationTypeDef],
     },
 )
 
-GetOnPremisesInstanceOutputTypeDef = TypedDict(
-    "GetOnPremisesInstanceOutputTypeDef",
+GetApplicationRevisionInputRequestTypeDef = TypedDict(
+    "GetApplicationRevisionInputRequestTypeDef",
     {
-        "instanceInfo": InstanceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "applicationName": str,
+        "revision": RevisionLocationTypeDef,
     },
 )
 
 GetApplicationRevisionOutputTypeDef = TypedDict(
     "GetApplicationRevisionOutputTypeDef",
     {
         "applicationName": str,
-        "revision": RevisionLocationOutputTypeDef,
+        "revision": RevisionLocationTypeDef,
         "revisionInfo": GenericRevisionInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationRevisionsOutputTypeDef = TypedDict(
     "ListApplicationRevisionsOutputTypeDef",
     {
-        "revisions": List[RevisionLocationOutputTypeDef],
+        "revisions": List[RevisionLocationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RevisionInfoTypeDef = TypedDict(
-    "RevisionInfoTypeDef",
-    {
-        "revisionLocation": RevisionLocationOutputTypeDef,
-        "genericRevisionInfo": GenericRevisionInfoTypeDef,
-    },
-    total=False,
-)
-
-BatchGetApplicationRevisionsInputRequestTypeDef = TypedDict(
-    "BatchGetApplicationRevisionsInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "revisions": Sequence[RevisionLocationTypeDef],
-    },
-)
-
-GetApplicationRevisionInputRequestTypeDef = TypedDict(
-    "GetApplicationRevisionInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "revision": RevisionLocationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterApplicationRevisionInputRequestTypeDef = TypedDict(
     "_RequiredRegisterApplicationRevisionInputRequestTypeDef",
     {
         "applicationName": str,
@@ -1840,25 +1638,36 @@
     "_OptionalRegisterApplicationRevisionInputRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class RegisterApplicationRevisionInputRequestTypeDef(
     _RequiredRegisterApplicationRevisionInputRequestTypeDef,
     _OptionalRegisterApplicationRevisionInputRequestTypeDef,
 ):
     pass
 
+
+RevisionInfoTypeDef = TypedDict(
+    "RevisionInfoTypeDef",
+    {
+        "revisionLocation": RevisionLocationTypeDef,
+        "genericRevisionInfo": GenericRevisionInfoTypeDef,
+    },
+    total=False,
+)
+
 LoadBalancerInfoOutputTypeDef = TypedDict(
     "LoadBalancerInfoOutputTypeDef",
     {
-        "elbInfoList": List[ELBInfoOutputTypeDef],
-        "targetGroupInfoList": List[TargetGroupInfoOutputTypeDef],
+        "elbInfoList": List[ELBInfoTypeDef],
+        "targetGroupInfoList": List[TargetGroupInfoTypeDef],
         "targetGroupPairInfoList": List[TargetGroupPairInfoOutputTypeDef],
     },
     total=False,
 )
 
 LoadBalancerInfoTypeDef = TypedDict(
     "LoadBalancerInfoTypeDef",
@@ -1866,27 +1675,14 @@
         "elbInfoList": Sequence[ELBInfoTypeDef],
         "targetGroupInfoList": Sequence[TargetGroupInfoTypeDef],
         "targetGroupPairInfoList": Sequence[TargetGroupPairInfoTypeDef],
     },
     total=False,
 )
 
-DeploymentConfigInfoTypeDef = TypedDict(
-    "DeploymentConfigInfoTypeDef",
-    {
-        "deploymentConfigId": str,
-        "deploymentConfigName": str,
-        "minimumHealthyHosts": MinimumHealthyHostsOutputTypeDef,
-        "createTime": datetime,
-        "computePlatform": ComputePlatformType,
-        "trafficRoutingConfig": TrafficRoutingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateDeploymentConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentConfigInputRequestTypeDef",
     {
         "deploymentConfigName": str,
     },
 )
 _OptionalCreateDeploymentConfigInputRequestTypeDef = TypedDict(
@@ -1895,20 +1691,35 @@
         "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
         "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
+
 class CreateDeploymentConfigInputRequestTypeDef(
     _RequiredCreateDeploymentConfigInputRequestTypeDef,
     _OptionalCreateDeploymentConfigInputRequestTypeDef,
 ):
     pass
 
+
+DeploymentConfigInfoTypeDef = TypedDict(
+    "DeploymentConfigInfoTypeDef",
+    {
+        "deploymentConfigId": str,
+        "deploymentConfigName": str,
+        "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
+        "createTime": datetime,
+        "computePlatform": ComputePlatformType,
+        "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateDeploymentInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalCreateDeploymentInputRequestTypeDef = TypedDict(
@@ -1924,33 +1735,35 @@
         "updateOutdatedInstancesOnly": bool,
         "fileExistsBehavior": FileExistsBehaviorType,
         "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateDeploymentInputRequestTypeDef(
     _RequiredCreateDeploymentInputRequestTypeDef, _OptionalCreateDeploymentInputRequestTypeDef
 ):
     pass
 
+
 BatchGetDeploymentInstancesOutputTypeDef = TypedDict(
     "BatchGetDeploymentInstancesOutputTypeDef",
     {
         "instancesSummary": List[InstanceSummaryTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentInstanceOutputTypeDef = TypedDict(
     "GetDeploymentInstanceOutputTypeDef",
     {
         "instanceSummary": InstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentTargetTypeDef = TypedDict(
     "DeploymentTargetTypeDef",
     {
         "deploymentTargetType": DeploymentTargetTypeType,
@@ -1964,72 +1777,72 @@
 
 BatchGetApplicationRevisionsOutputTypeDef = TypedDict(
     "BatchGetApplicationRevisionsOutputTypeDef",
     {
         "applicationName": str,
         "errorMessage": str,
         "revisions": List[RevisionInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentGroupInfoTypeDef = TypedDict(
     "DeploymentGroupInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupId": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
-        "ec2TagFilters": List[EC2TagFilterOutputTypeDef],
-        "onPremisesInstanceTagFilters": List[TagFilterOutputTypeDef],
+        "ec2TagFilters": List[EC2TagFilterTypeDef],
+        "onPremisesInstanceTagFilters": List[TagFilterTypeDef],
         "autoScalingGroups": List[AutoScalingGroupTypeDef],
         "serviceRoleArn": str,
-        "targetRevision": RevisionLocationOutputTypeDef,
+        "targetRevision": RevisionLocationTypeDef,
         "triggerConfigurations": List[TriggerConfigOutputTypeDef],
         "alarmConfiguration": AlarmConfigurationOutputTypeDef,
         "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
-        "deploymentStyle": DeploymentStyleOutputTypeDef,
+        "deploymentStyle": DeploymentStyleTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationOutputTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "lastSuccessfulDeployment": LastDeploymentInfoTypeDef,
         "lastAttemptedDeployment": LastDeploymentInfoTypeDef,
         "ec2TagSet": EC2TagSetOutputTypeDef,
         "onPremisesTagSet": OnPremisesTagSetOutputTypeDef,
         "computePlatform": ComputePlatformType,
-        "ecsServices": List[ECSServiceOutputTypeDef],
+        "ecsServices": List[ECSServiceTypeDef],
     },
     total=False,
 )
 
 DeploymentInfoTypeDef = TypedDict(
     "DeploymentInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
         "deploymentId": str,
-        "previousRevision": RevisionLocationOutputTypeDef,
-        "revision": RevisionLocationOutputTypeDef,
+        "previousRevision": RevisionLocationTypeDef,
+        "revision": RevisionLocationTypeDef,
         "status": DeploymentStatusType,
         "errorInformation": ErrorInformationTypeDef,
         "createTime": datetime,
         "startTime": datetime,
         "completeTime": datetime,
         "deploymentOverview": DeploymentOverviewTypeDef,
         "description": str,
         "creator": DeploymentCreatorType,
         "ignoreApplicationStopFailures": bool,
         "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
         "updateOutdatedInstancesOnly": bool,
         "rollbackInfo": RollbackInfoTypeDef,
-        "deploymentStyle": DeploymentStyleOutputTypeDef,
+        "deploymentStyle": DeploymentStyleTypeDef,
         "targetInstances": TargetInstancesOutputTypeDef,
         "instanceTerminationWaitTimeStarted": bool,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationOutputTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "additionalDeploymentStatusInfo": str,
         "fileExistsBehavior": FileExistsBehaviorType,
         "deploymentStatusMessages": List[str],
         "computePlatform": ComputePlatformType,
         "externalId": str,
         "relatedDeployments": RelatedDeploymentsTypeDef,
@@ -2064,20 +1877,22 @@
         "ecsServices": Sequence[ECSServiceTypeDef],
         "onPremisesTagSet": OnPremisesTagSetTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDeploymentGroupInputRequestTypeDef(
     _RequiredCreateDeploymentGroupInputRequestTypeDef,
     _OptionalCreateDeploymentGroupInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
         "currentDeploymentGroupName": str,
     },
 )
@@ -2100,69 +1915,71 @@
         "ec2TagSet": EC2TagSetTypeDef,
         "ecsServices": Sequence[ECSServiceTypeDef],
         "onPremisesTagSet": OnPremisesTagSetTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDeploymentGroupInputRequestTypeDef(
     _RequiredUpdateDeploymentGroupInputRequestTypeDef,
     _OptionalUpdateDeploymentGroupInputRequestTypeDef,
 ):
     pass
 
+
 GetDeploymentConfigOutputTypeDef = TypedDict(
     "GetDeploymentConfigOutputTypeDef",
     {
         "deploymentConfigInfo": DeploymentConfigInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentTargetsOutputTypeDef = TypedDict(
     "BatchGetDeploymentTargetsOutputTypeDef",
     {
         "deploymentTargets": List[DeploymentTargetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentTargetOutputTypeDef = TypedDict(
     "GetDeploymentTargetOutputTypeDef",
     {
         "deploymentTarget": DeploymentTargetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentGroupsOutputTypeDef = TypedDict(
     "BatchGetDeploymentGroupsOutputTypeDef",
     {
         "deploymentGroupsInfo": List[DeploymentGroupInfoTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentGroupOutputTypeDef = TypedDict(
     "GetDeploymentGroupOutputTypeDef",
     {
         "deploymentGroupInfo": DeploymentGroupInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentsOutputTypeDef = TypedDict(
     "BatchGetDeploymentsOutputTypeDef",
     {
         "deploymentsInfo": List[DeploymentInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentOutputTypeDef = TypedDict(
     "GetDeploymentOutputTypeDef",
     {
         "deploymentInfo": DeploymentInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/waiter.py` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy/waiter.pyi` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/PKG-INFO` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codedeploy
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeDeploy 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeDeploy 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codedeploy)](https://pepy.tech/project/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -417,176 +417,155 @@
 
 `mypy_boto3_codedeploy.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
-    AlarmOutputTypeDef,
     AlarmTypeDef,
-    AppSpecContentOutputTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
     AutoRollbackConfigurationOutputTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
-    BlueInstanceTerminationOptionOutputTypeDef,
-    DeploymentReadyOptionOutputTypeDef,
-    GreenFleetProvisioningOptionOutputTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
-    CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
-    CreateDeploymentConfigOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
     TriggerConfigTypeDef,
-    CreateDeploymentGroupOutputTypeDef,
-    CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
-    DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
-    MinimumHealthyHostsOutputTypeDef,
-    DeploymentStyleOutputTypeDef,
-    EC2TagFilterOutputTypeDef,
-    ECSServiceOutputTypeDef,
     LastDeploymentInfoTypeDef,
-    TagFilterOutputTypeDef,
     TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
-    TargetGroupInfoOutputTypeDef,
-    ELBInfoOutputTypeDef,
+    TargetGroupInfoTypeDef,
     ELBInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
-    GitHubLocationOutputTypeDef,
     GitHubLocationTypeDef,
-    TagOutputTypeDef,
     LambdaFunctionInfoTypeDef,
-    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
-    ListDeploymentConfigsOutputTypeDef,
-    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
-    ListDeploymentGroupsOutputTypeDef,
-    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
-    ListDeploymentInstancesOutputTypeDef,
-    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
-    ListDeploymentTargetsOutputTypeDef,
     TimeRangeTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
-    ListGitHubAccountTokenNamesOutputTypeDef,
-    ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TargetGroupInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
-    PutLifecycleEventHookExecutionStatusOutputTypeDef,
-    RawStringOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    S3LocationOutputTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
-    StopDeploymentOutputTypeDef,
     TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
-    TimeBasedCanaryOutputTypeDef,
     TimeBasedCanaryTypeDef,
-    TimeBasedLinearOutputTypeDef,
     TimeBasedLinearTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
+    InstanceInfoTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
     BatchGetApplicationsOutputTypeDef,
-    GetApplicationOutputTypeDef,
+    CreateApplicationOutputTypeDef,
+    CreateDeploymentConfigOutputTypeDef,
+    CreateDeploymentGroupOutputTypeDef,
+    CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
+    DeleteGitHubAccountTokenOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetApplicationOutputTypeDef,
+    ListApplicationsOutputTypeDef,
+    ListDeploymentConfigsOutputTypeDef,
+    ListDeploymentGroupsOutputTypeDef,
+    ListDeploymentInstancesOutputTypeDef,
+    ListDeploymentTargetsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListGitHubAccountTokenNamesOutputTypeDef,
+    ListOnPremisesInstancesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PutLifecycleEventHookExecutionStatusOutputTypeDef,
+    StopDeploymentOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
-    BlueGreenDeploymentConfigurationOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
+    EC2TagSetOutputTypeDef,
     EC2TagSetTypeDef,
-    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
-    OnPremisesTagSetTypeDef,
-    EC2TagSetOutputTypeDef,
     OnPremisesTagSetOutputTypeDef,
+    OnPremisesTagSetTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
-    InstanceInfoTypeDef,
-    ListTagsForResourceOutputTypeDef,
+    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
+    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
+    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
+    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
+    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
-    RevisionLocationOutputTypeDef,
     RevisionLocationTypeDef,
     TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
-    TrafficRoutingConfigOutputTypeDef,
     TrafficRoutingConfigTypeDef,
-    TargetInstancesTypeDef,
+    BatchGetOnPremisesInstancesOutputTypeDef,
+    GetOnPremisesInstanceOutputTypeDef,
     TargetInstancesOutputTypeDef,
+    TargetInstancesTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
-    BatchGetOnPremisesInstancesOutputTypeDef,
-    GetOnPremisesInstanceOutputTypeDef,
-    GetApplicationRevisionOutputTypeDef,
-    ListApplicationRevisionsOutputTypeDef,
-    RevisionInfoTypeDef,
     BatchGetApplicationRevisionsInputRequestTypeDef,
     GetApplicationRevisionInputRequestTypeDef,
+    GetApplicationRevisionOutputTypeDef,
+    ListApplicationRevisionsOutputTypeDef,
     RegisterApplicationRevisionInputRequestTypeDef,
+    RevisionInfoTypeDef,
     LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
-    DeploymentConfigInfoTypeDef,
     CreateDeploymentConfigInputRequestTypeDef,
+    DeploymentConfigInfoTypeDef,
     CreateDeploymentInputRequestTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
```

### Comparing `mypy-boto3-codedeploy-1.28.12/mypy_boto3_codedeploy.egg-info/SOURCES.txt` & `mypy-boto3-codedeploy-1.28.15/mypy_boto3_codedeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.28.12/setup.py` & `mypy-boto3-codedeploy-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codedeploy",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_codedeploy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeDeploy 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CodeDeploy 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

