# Comparing `tmp/mypy-boto3-emr-1.28.15.tar.gz` & `tmp/mypy-boto3-emr-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-1.28.15.tar", last modified: Fri Jul 28 20:42:46 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:06 2023, max compression
```

## Comparing `mypy-boto3-emr-1.28.15.tar` & `mypy-boto3-emr-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.897084 mypy-boto3-emr-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-07-28 20:42:46.897084 mypy-boto3-emr-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.885084 mypy-boto3-emr-1.28.15/mypy_boto3_emr/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43838 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43764 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-28 20:25:26.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-07-28 20:25:26.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    84915 2023-07-28 20:25:28.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    84797 2023-07-28 20:25:27.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.897084 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:46.897084 mypy-boto3-emr-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.237143 mypy-boto3-emr-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-07-29 10:03:06.233143 mypy-boto3-emr-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.225143 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44339 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44265 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85114 2023-07-29 09:44:59.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84996 2023-07-29 09:44:58.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-29 09:44:56.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.233143 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-07-29 10:03:05.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:03:06.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:05.000000 mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:06.237143 mypy-boto3-emr-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:44:55.000000 mypy-boto3-emr-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-emr-1.28.15/LICENSE` & `mypy-boto3-emr-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15/PKG-INFO` & `mypy-boto3-emr-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.28.15
-Summary: Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-1.28.15/README.md` & `mypy-boto3-emr-1.28.15.post1/README.md`

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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/__init__.py` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/__init__.pyi` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/__main__.py` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMR 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.EMR 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR\nOther"
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

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/client.py` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,20 +45,24 @@
     ListStudioSessionMappingsPaginator,
     ListStudiosPaginator,
 )
 from .type_defs import (
     AddInstanceFleetOutputTypeDef,
     AddInstanceGroupsOutputTypeDef,
     AddJobFlowStepsOutputTypeDef,
+    ApplicationOutputTypeDef,
     ApplicationTypeDef,
     AutoScalingPolicyTypeDef,
     AutoTerminationPolicyTypeDef,
+    BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
+    BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
     CancelStepsOutputTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationOutputTypeDef,
     CreateStudioOutputTypeDef,
     DescribeClusterOutputTypeDef,
     DescribeJobFlowsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
     DescribeReleaseLabelOutputTypeDef,
@@ -95,14 +99,15 @@
     NotebookS3LocationFromInputTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
     PlacementGroupConfigTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     ReleaseLabelFilterTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
+    StepConfigOutputTypeDef,
     StepConfigTypeDef,
     SupportedProductConfigTypeDef,
     TagTypeDef,
 )
 from .waiter import ClusterRunningWaiter, ClusterTerminatedWaiter, StepCompleteWaiter
 
 if sys.version_info >= (3, 9):
@@ -163,15 +168,19 @@
         Adds one or more instance groups to a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_instance_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#add_instance_groups)
         """
 
     def add_job_flow_steps(
-        self, *, JobFlowId: str, Steps: Sequence[StepConfigTypeDef], ExecutionRoleArn: str = ...
+        self,
+        *,
+        JobFlowId: str,
+        Steps: Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
+        ExecutionRoleArn: str = ...
     ) -> AddJobFlowStepsOutputTypeDef:
         """
         AddJobFlowSteps adds new steps to a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_job_flow_steps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#add_job_flow_steps)
         """
@@ -649,15 +658,19 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_auto_termination_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#put_auto_termination_policy)
         """
 
     def put_block_public_access_configuration(
-        self, *, BlockPublicAccessConfiguration: BlockPublicAccessConfigurationTypeDef
+        self,
+        *,
+        BlockPublicAccessConfiguration: Union[
+            BlockPublicAccessConfigurationTypeDef, BlockPublicAccessConfigurationOutputTypeDef
+        ]
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon EMR block public access configuration for your
         Amazon Web Services account in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_block_public_access_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#put_block_public_access_configuration)
@@ -713,20 +726,22 @@
         Name: str,
         Instances: JobFlowInstancesConfigTypeDef,
         LogUri: str = ...,
         LogEncryptionKmsKeyId: str = ...,
         AdditionalInfo: str = ...,
         AmiVersion: str = ...,
         ReleaseLabel: str = ...,
-        Steps: Sequence[StepConfigTypeDef] = ...,
-        BootstrapActions: Sequence[BootstrapActionConfigTypeDef] = ...,
+        Steps: Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]] = ...,
+        BootstrapActions: Sequence[
+            Union[BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef]
+        ] = ...,
         SupportedProducts: Sequence[str] = ...,
         NewSupportedProducts: Sequence[SupportedProductConfigTypeDef] = ...,
-        Applications: Sequence[ApplicationTypeDef] = ...,
-        Configurations: Sequence["ConfigurationTypeDef"] = ...,
+        Applications: Sequence[Union[ApplicationTypeDef, ApplicationOutputTypeDef]] = ...,
+        Configurations: Sequence[Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]] = ...,
         VisibleToAllUsers: bool = ...,
         JobFlowRole: str = ...,
         ServiceRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SecurityConfiguration: str = ...,
         AutoScalingRole: str = ...,
         ScaleDownBehavior: ScaleDownBehaviorType = ...,
```

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/client.pyi` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,20 +45,24 @@
     ListStudioSessionMappingsPaginator,
     ListStudiosPaginator,
 )
 from .type_defs import (
     AddInstanceFleetOutputTypeDef,
     AddInstanceGroupsOutputTypeDef,
     AddJobFlowStepsOutputTypeDef,
+    ApplicationOutputTypeDef,
     ApplicationTypeDef,
     AutoScalingPolicyTypeDef,
     AutoTerminationPolicyTypeDef,
+    BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
+    BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
     CancelStepsOutputTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationOutputTypeDef,
     CreateStudioOutputTypeDef,
     DescribeClusterOutputTypeDef,
     DescribeJobFlowsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
     DescribeReleaseLabelOutputTypeDef,
@@ -95,14 +99,15 @@
     NotebookS3LocationFromInputTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
     PlacementGroupConfigTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     ReleaseLabelFilterTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
+    StepConfigOutputTypeDef,
     StepConfigTypeDef,
     SupportedProductConfigTypeDef,
     TagTypeDef,
 )
 from .waiter import ClusterRunningWaiter, ClusterTerminatedWaiter, StepCompleteWaiter
 
 if sys.version_info >= (3, 9):
@@ -156,15 +161,19 @@
         """
         Adds one or more instance groups to a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_instance_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#add_instance_groups)
         """
     def add_job_flow_steps(
-        self, *, JobFlowId: str, Steps: Sequence[StepConfigTypeDef], ExecutionRoleArn: str = ...
+        self,
+        *,
+        JobFlowId: str,
+        Steps: Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
+        ExecutionRoleArn: str = ...
     ) -> AddJobFlowStepsOutputTypeDef:
         """
         AddJobFlowSteps adds new steps to a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_job_flow_steps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#add_job_flow_steps)
         """
@@ -601,15 +610,19 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_auto_termination_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#put_auto_termination_policy)
         """
     def put_block_public_access_configuration(
-        self, *, BlockPublicAccessConfiguration: BlockPublicAccessConfigurationTypeDef
+        self,
+        *,
+        BlockPublicAccessConfiguration: Union[
+            BlockPublicAccessConfigurationTypeDef, BlockPublicAccessConfigurationOutputTypeDef
+        ]
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon EMR block public access configuration for your
         Amazon Web Services account in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_block_public_access_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#put_block_public_access_configuration)
@@ -659,20 +672,22 @@
         Name: str,
         Instances: JobFlowInstancesConfigTypeDef,
         LogUri: str = ...,
         LogEncryptionKmsKeyId: str = ...,
         AdditionalInfo: str = ...,
         AmiVersion: str = ...,
         ReleaseLabel: str = ...,
-        Steps: Sequence[StepConfigTypeDef] = ...,
-        BootstrapActions: Sequence[BootstrapActionConfigTypeDef] = ...,
+        Steps: Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]] = ...,
+        BootstrapActions: Sequence[
+            Union[BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef]
+        ] = ...,
         SupportedProducts: Sequence[str] = ...,
         NewSupportedProducts: Sequence[SupportedProductConfigTypeDef] = ...,
-        Applications: Sequence[ApplicationTypeDef] = ...,
-        Configurations: Sequence["ConfigurationTypeDef"] = ...,
+        Applications: Sequence[Union[ApplicationTypeDef, ApplicationOutputTypeDef]] = ...,
+        Configurations: Sequence[Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]] = ...,
         VisibleToAllUsers: bool = ...,
         JobFlowRole: str = ...,
         ServiceRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SecurityConfiguration: str = ...,
         AutoScalingRole: str = ...,
         ScaleDownBehavior: ScaleDownBehaviorType = ...,
```

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/literals.py` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/literals.pyi` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/paginator.py` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/paginator.pyi` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/type_defs.py` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2961,15 +2961,15 @@
     },
 )
 
 _RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
     "_RequiredAddJobFlowStepsInputRequestTypeDef",
     {
         "JobFlowId": str,
-        "Steps": Sequence[StepConfigTypeDef],
+        "Steps": Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
     },
 )
 _OptionalAddJobFlowStepsInputRequestTypeDef = TypedDict(
     "_OptionalAddJobFlowStepsInputRequestTypeDef",
     {
         "ExecutionRoleArn": str,
     },
@@ -3271,20 +3271,22 @@
     "_OptionalRunJobFlowInputRequestTypeDef",
     {
         "LogUri": str,
         "LogEncryptionKmsKeyId": str,
         "AdditionalInfo": str,
         "AmiVersion": str,
         "ReleaseLabel": str,
-        "Steps": Sequence[StepConfigTypeDef],
-        "BootstrapActions": Sequence[BootstrapActionConfigTypeDef],
+        "Steps": Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
+        "BootstrapActions": Sequence[
+            Union[BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef]
+        ],
         "SupportedProducts": Sequence[str],
         "NewSupportedProducts": Sequence[SupportedProductConfigTypeDef],
-        "Applications": Sequence[ApplicationTypeDef],
-        "Configurations": Sequence["ConfigurationTypeDef"],
+        "Applications": Sequence[Union[ApplicationTypeDef, ApplicationOutputTypeDef]],
+        "Configurations": Sequence[Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]],
         "VisibleToAllUsers": bool,
         "JobFlowRole": str,
         "ServiceRole": str,
         "Tags": Sequence[TagTypeDef],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
```

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/type_defs.pyi` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2852,15 +2852,15 @@
     },
 )
 
 _RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
     "_RequiredAddJobFlowStepsInputRequestTypeDef",
     {
         "JobFlowId": str,
-        "Steps": Sequence[StepConfigTypeDef],
+        "Steps": Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
     },
 )
 _OptionalAddJobFlowStepsInputRequestTypeDef = TypedDict(
     "_OptionalAddJobFlowStepsInputRequestTypeDef",
     {
         "ExecutionRoleArn": str,
     },
@@ -3154,20 +3154,22 @@
     "_OptionalRunJobFlowInputRequestTypeDef",
     {
         "LogUri": str,
         "LogEncryptionKmsKeyId": str,
         "AdditionalInfo": str,
         "AmiVersion": str,
         "ReleaseLabel": str,
-        "Steps": Sequence[StepConfigTypeDef],
-        "BootstrapActions": Sequence[BootstrapActionConfigTypeDef],
+        "Steps": Sequence[Union[StepConfigTypeDef, StepConfigOutputTypeDef]],
+        "BootstrapActions": Sequence[
+            Union[BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef]
+        ],
         "SupportedProducts": Sequence[str],
         "NewSupportedProducts": Sequence[SupportedProductConfigTypeDef],
-        "Applications": Sequence[ApplicationTypeDef],
-        "Configurations": Sequence["ConfigurationTypeDef"],
+        "Applications": Sequence[Union[ApplicationTypeDef, ApplicationOutputTypeDef]],
+        "Configurations": Sequence[Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]],
         "VisibleToAllUsers": bool,
         "JobFlowRole": str,
         "ServiceRole": str,
         "Tags": Sequence[TagTypeDef],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
```

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/waiter.py` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr/waiter.pyi` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/PKG-INFO` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.28.15
-Summary: Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/SOURCES.txt` & `mypy-boto3-emr-1.28.15.post1/mypy_boto3_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.15/setup.py` & `mypy-boto3-emr-1.28.15.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

