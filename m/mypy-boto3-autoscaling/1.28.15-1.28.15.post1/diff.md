# Comparing `tmp/mypy-boto3-autoscaling-1.28.15.tar.gz` & `tmp/mypy-boto3-autoscaling-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-1.28.15.tar` & `mypy-boto3-autoscaling-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.288696 mypy-boto3-autoscaling-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-07-28 20:42:19.276696 mypy-boto3-autoscaling-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.272696 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52899 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52816 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-07-28 20:19:59.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86078 2023-07-28 20:19:58.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.276696 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.288696 mypy-boto3-autoscaling-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.393021 mypy-boto3-autoscaling-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23715 2023-07-29 10:02:34.385021 mypy-boto3-autoscaling-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.381021 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53486 2023-07-29 09:38:48.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53403 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-29 09:38:49.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-29 09:38:48.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-07-29 09:38:48.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-29 09:38:48.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86078 2023-07-29 09:38:50.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:47.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.385021 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23715 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.393021 mypy-boto3-autoscaling-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:38:46.000000 mypy-boto3-autoscaling-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-autoscaling-1.28.15/LICENSE` & `mypy-boto3-autoscaling-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15/PKG-INFO` & `mypy-boto3-autoscaling-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.15
-Summary: Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-autoscaling-1.28.15/README.md` & `mypy-boto3-autoscaling-1.28.15.post1/README.md`

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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__init__.py` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__init__.pyi` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__main__.py` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScaling 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.AutoScaling 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
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

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/client.py` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,40 +51,45 @@
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     DescribeWarmPoolAnswerTypeDef,
+    DesiredConfigurationOutputTypeDef,
     DesiredConfigurationTypeDef,
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     FilterTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     InstanceReusePolicyTypeDef,
     LaunchConfigurationsTypeTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
+    MixedInstancesPolicyOutputTypeDef,
     MixedInstancesPolicyTypeDef,
     PoliciesTypeTypeDef,
     PolicyARNTypeTypeDef,
+    PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
     ProcessesTypeTypeDef,
+    RefreshPreferencesOutputTypeDef,
     RefreshPreferencesTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     ScheduledActionsTypeTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     StepAdjustmentTypeDef,
     TagsTypeTypeDef,
     TagTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
     TrafficSourceIdentifierTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -244,15 +249,17 @@
         self,
         *,
         AutoScalingGroupName: str,
         MinSize: int,
         MaxSize: int,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
+        MixedInstancesPolicy: Union[
+            MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
+        ] = ...,
         InstanceId: str = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         LoadBalancerNames: Sequence[str] = ...,
         TargetGroupARNs: Sequence[str] = ...,
         HealthCheckType: str = ...,
@@ -814,17 +821,21 @@
         MinAdjustmentStep: int = ...,
         MinAdjustmentMagnitude: int = ...,
         ScalingAdjustment: int = ...,
         Cooldown: int = ...,
         MetricAggregationType: str = ...,
         StepAdjustments: Sequence[StepAdjustmentTypeDef] = ...,
         EstimatedInstanceWarmup: int = ...,
-        TargetTrackingConfiguration: TargetTrackingConfigurationTypeDef = ...,
+        TargetTrackingConfiguration: Union[
+            TargetTrackingConfigurationTypeDef, TargetTrackingConfigurationOutputTypeDef
+        ] = ...,
         Enabled: bool = ...,
-        PredictiveScalingConfiguration: PredictiveScalingConfigurationTypeDef = ...
+        PredictiveScalingConfiguration: Union[
+            PredictiveScalingConfigurationTypeDef, PredictiveScalingConfigurationOutputTypeDef
+        ] = ...
     ) -> PolicyARNTypeTypeDef:
         """
         Creates or updates a scaling policy for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_scaling_policy)
         """
@@ -935,16 +946,18 @@
         """
 
     def start_instance_refresh(
         self,
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
-        DesiredConfiguration: DesiredConfigurationTypeDef = ...,
-        Preferences: RefreshPreferencesTypeDef = ...
+        DesiredConfiguration: Union[
+            DesiredConfigurationTypeDef, DesiredConfigurationOutputTypeDef
+        ] = ...,
+        Preferences: Union[RefreshPreferencesTypeDef, RefreshPreferencesOutputTypeDef] = ...
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
         Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#start_instance_refresh)
         """
@@ -972,15 +985,17 @@
 
     def update_auto_scaling_group(
         self,
         *,
         AutoScalingGroupName: str,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
+        MixedInstancesPolicy: Union[
+            MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
+        ] = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         HealthCheckType: str = ...,
         HealthCheckGracePeriod: int = ...,
```

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/client.pyi` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,40 +51,45 @@
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     DescribeWarmPoolAnswerTypeDef,
+    DesiredConfigurationOutputTypeDef,
     DesiredConfigurationTypeDef,
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     FilterTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     InstanceReusePolicyTypeDef,
     LaunchConfigurationsTypeTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
+    MixedInstancesPolicyOutputTypeDef,
     MixedInstancesPolicyTypeDef,
     PoliciesTypeTypeDef,
     PolicyARNTypeTypeDef,
+    PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
     ProcessesTypeTypeDef,
+    RefreshPreferencesOutputTypeDef,
     RefreshPreferencesTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     ScheduledActionsTypeTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     StepAdjustmentTypeDef,
     TagsTypeTypeDef,
     TagTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
     TrafficSourceIdentifierTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -229,15 +234,17 @@
         self,
         *,
         AutoScalingGroupName: str,
         MinSize: int,
         MaxSize: int,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
+        MixedInstancesPolicy: Union[
+            MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
+        ] = ...,
         InstanceId: str = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         LoadBalancerNames: Sequence[str] = ...,
         TargetGroupARNs: Sequence[str] = ...,
         HealthCheckType: str = ...,
@@ -754,17 +761,21 @@
         MinAdjustmentStep: int = ...,
         MinAdjustmentMagnitude: int = ...,
         ScalingAdjustment: int = ...,
         Cooldown: int = ...,
         MetricAggregationType: str = ...,
         StepAdjustments: Sequence[StepAdjustmentTypeDef] = ...,
         EstimatedInstanceWarmup: int = ...,
-        TargetTrackingConfiguration: TargetTrackingConfigurationTypeDef = ...,
+        TargetTrackingConfiguration: Union[
+            TargetTrackingConfigurationTypeDef, TargetTrackingConfigurationOutputTypeDef
+        ] = ...,
         Enabled: bool = ...,
-        PredictiveScalingConfiguration: PredictiveScalingConfigurationTypeDef = ...
+        PredictiveScalingConfiguration: Union[
+            PredictiveScalingConfigurationTypeDef, PredictiveScalingConfigurationOutputTypeDef
+        ] = ...
     ) -> PolicyARNTypeTypeDef:
         """
         Creates or updates a scaling policy for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#put_scaling_policy)
         """
@@ -866,16 +877,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#set_instance_protection)
         """
     def start_instance_refresh(
         self,
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
-        DesiredConfiguration: DesiredConfigurationTypeDef = ...,
-        Preferences: RefreshPreferencesTypeDef = ...
+        DesiredConfiguration: Union[
+            DesiredConfigurationTypeDef, DesiredConfigurationOutputTypeDef
+        ] = ...,
+        Preferences: Union[RefreshPreferencesTypeDef, RefreshPreferencesOutputTypeDef] = ...
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
         Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#start_instance_refresh)
         """
@@ -900,15 +913,17 @@
         """
     def update_auto_scaling_group(
         self,
         *,
         AutoScalingGroupName: str,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
+        MixedInstancesPolicy: Union[
+            MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
+        ] = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         HealthCheckType: str = ...,
         HealthCheckGracePeriod: int = ...,
```

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/literals.py` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/literals.pyi` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/paginator.py` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/paginator.pyi` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/type_defs.py` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/type_defs.pyi` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.15
-Summary: Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-1.28.15.post1/mypy_boto3_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.15/setup.py` & `mypy-boto3-autoscaling-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder"
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

