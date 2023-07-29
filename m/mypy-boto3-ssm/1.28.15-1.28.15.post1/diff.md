# Comparing `tmp/mypy-boto3-ssm-1.28.15.tar.gz` & `tmp/mypy-boto3-ssm-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-1.28.15.tar", last modified: Fri Jul 28 20:43:49 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:16 2023, max compression
```

## Comparing `mypy-boto3-ssm-1.28.15.tar` & `mypy-boto3-ssm-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.085937 mypy-boto3-ssm-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46800 2023-07-28 20:43:49.081937 mypy-boto3-ssm-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    45329 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.073937 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   131264 2023-07-28 20:39:52.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   131071 2023-07-28 20:39:51.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-07-28 20:39:56.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    28170 2023-07-28 20:39:56.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    59186 2023-07-28 20:39:52.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    59137 2023-07-28 20:39:52.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   213242 2023-07-28 20:40:02.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   213000 2023-07-28 20:39:59.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-28 20:39:52.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-28 20:39:52.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.081937 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46800 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:49.085937 mypy-boto3-ssm-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.565421 mypy-boto3-ssm-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46806 2023-07-29 10:04:16.565421 mypy-boto3-ssm-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    45329 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.561421 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133465 2023-07-29 10:00:02.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133272 2023-07-29 10:00:02.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-07-29 10:00:04.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28170 2023-07-29 10:00:03.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    59274 2023-07-29 10:00:03.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59225 2023-07-29 10:00:03.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   214204 2023-07-29 10:00:13.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213962 2023-07-29 10:00:06.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-29 10:00:03.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-29 10:00:03.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.565421 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46806 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:16.000000 mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:16.565421 mypy-boto3-ssm-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 10:00:01.000000 mypy-boto3-ssm-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-ssm-1.28.15/LICENSE` & `mypy-boto3-ssm-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15/PKG-INFO` & `mypy-boto3-ssm-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.28.15
-Summary: Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -681,14 +681,15 @@
     RegistrationMetadataItemTypeDef,
     TargetTypeDef,
     DocumentRequiresTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
     MetadataValueTypeDef,
+    PatchSourceOutputTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
@@ -765,15 +766,14 @@
     OpsResultAttributeTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
-    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
```

### Comparing `mypy-boto3-ssm-1.28.15/README.md` & `mypy-boto3-ssm-1.28.15.post1/README.md`

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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -649,14 +649,15 @@
     RegistrationMetadataItemTypeDef,
     TargetTypeDef,
     DocumentRequiresTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
     MetadataValueTypeDef,
+    PatchSourceOutputTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
@@ -733,15 +734,14 @@
     OpsResultAttributeTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
-    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
```

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__init__.py` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__init__.pyi` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__main__.py` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSM 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.SSM 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\nOther"
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

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/client.py` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,30 +90,34 @@
     ListOpsItemEventsPaginator,
     ListOpsItemRelatedItemsPaginator,
     ListOpsMetadataPaginator,
     ListResourceComplianceSummariesPaginator,
     ListResourceDataSyncPaginator,
 )
 from .type_defs import (
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
     AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationExecutionFilterTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
+    AssociationStatusOutputTypeDef,
     AssociationStatusTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     BaselineOverrideTypeDef,
     CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
+    ComplianceExecutionSummaryOutputTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     CreateActivationResultTypeDef,
+    CreateAssociationBatchRequestEntryOutputTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
     CreateAssociationBatchResultTypeDef,
     CreateAssociationResultTypeDef,
     CreateDocumentResultTypeDef,
     CreateMaintenanceWindowResultTypeDef,
     CreateOpsItemResponseTypeDef,
     CreateOpsMetadataResultTypeDef,
@@ -209,32 +213,38 @@
     ListOpsItemRelatedItemsResponseTypeDef,
     ListOpsMetadataResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     ListTagsForResourceResultTypeDef,
     LoggingInfoTypeDef,
     MaintenanceWindowFilterTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     MetadataValueTypeDef,
+    NotificationConfigOutputTypeDef,
     NotificationConfigTypeDef,
     OpsAggregatorTypeDef,
     OpsFilterTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemFilterTypeDef,
     OpsItemNotificationTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsResultAttributeTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
+    PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
     PatchOrchestratorFilterTypeDef,
+    PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
+    PatchSourceOutputTypeDef,
     PatchSourceTypeDef,
     PutInventoryResultTypeDef,
     PutParameterResultTypeDef,
     PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupResultTypeDef,
     RegisterTargetWithMaintenanceWindowResultTypeDef,
@@ -242,23 +252,26 @@
     RegistrationMetadataItemTypeDef,
     RelatedOpsItemTypeDef,
     ResetServiceSettingResultTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     ResourceDataSyncSourceTypeDef,
     ResultAttributeTypeDef,
     ResumeSessionResponseTypeDef,
+    RunbookOutputTypeDef,
     RunbookTypeDef,
     SendCommandResultTypeDef,
     SessionFilterTypeDef,
     StartAutomationExecutionResultTypeDef,
     StartChangeRequestExecutionResultTypeDef,
     StartSessionResponseTypeDef,
     StepExecutionFilterTypeDef,
     TagTypeDef,
+    TargetLocationOutputTypeDef,
     TargetLocationTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
     TerminateSessionResponseTypeDef,
     UnlabelParameterVersionResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
     UpdateDocumentResultTypeDef,
@@ -518,41 +531,48 @@
     def create_association(
         self,
         *,
         Name: str,
         DocumentVersion: str = ...,
         InstanceId: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         AssociationName: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> CreateAssociationResultTypeDef:
         """
         A State Manager association defines the state that you want to maintain on your
         managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_association)
         """
 
     def create_association_batch(
-        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryTypeDef]
+        self,
+        *,
+        Entries: Sequence[
+            Union[
+                CreateAssociationBatchRequestEntryTypeDef,
+                CreateAssociationBatchRequestEntryOutputTypeDef,
+            ]
+        ]
     ) -> CreateAssociationBatchResultTypeDef:
         """
         Associates the specified Amazon Web Services Systems Manager document (SSM
         document) with the specified managed nodes or targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_association_batch)
@@ -646,23 +666,23 @@
         """
 
     def create_patch_baseline(
         self,
         *,
         Name: str,
         OperatingSystem: OperatingSystemType = ...,
-        GlobalFilters: PatchFilterGroupTypeDef = ...,
-        ApprovalRules: PatchRuleGroupTypeDef = ...,
+        GlobalFilters: Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef] = ...,
+        ApprovalRules: Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef] = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceTypeDef] = ...,
+        Sources: Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]] = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePatchBaselineResultTypeDef:
         """
         Creates a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_patch_baseline)
@@ -1109,15 +1129,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_maintenance_window_executions)
         """
 
     def describe_maintenance_window_schedule(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowScheduleResultTypeDef:
         """
         Retrieves information about upcoming executions of a maintenance window.
@@ -1169,15 +1189,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_maintenance_windows)
         """
 
     def describe_maintenance_windows_for_target(
         self,
         *,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         ResourceType: MaintenanceWindowResourceTypeType,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsForTargetResultTypeDef:
         """
         Retrieves information about the maintenance window targets or tasks that a
         managed node is associated with.
@@ -1847,15 +1867,17 @@
 
     def put_compliance_items(
         self,
         *,
         ResourceId: str,
         ResourceType: str,
         ComplianceType: str,
-        ExecutionSummary: ComplianceExecutionSummaryTypeDef,
+        ExecutionSummary: Union[
+            ComplianceExecutionSummaryTypeDef, ComplianceExecutionSummaryOutputTypeDef
+        ],
         Items: Sequence[ComplianceItemEntryTypeDef],
         ItemContentHash: str = ...,
         UploadType: ComplianceUploadTypeType = ...
     ) -> Dict[str, Any]:
         """
         Registers a compliance type and other compliance details on a designated
         resource.
@@ -1927,15 +1949,15 @@
         """
 
     def register_target_with_maintenance_window(
         self,
         *,
         WindowId: str,
         ResourceType: MaintenanceWindowResourceTypeType,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> RegisterTargetWithMaintenanceWindowResultTypeDef:
         """
         Registers a target with a maintenance window.
@@ -1946,27 +1968,36 @@
 
     def register_task_with_maintenance_window(
         self,
         *,
         WindowId: str,
         TaskArn: str,
         TaskType: MaintenanceWindowTaskTypeType,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
+        TaskParameters: Mapping[
+            str,
+            Union[
+                MaintenanceWindowTaskParameterValueExpressionTypeDef,
+                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+            ],
+        ] = ...,
+        TaskInvocationParameters: Union[
+            MaintenanceWindowTaskInvocationParametersTypeDef,
+            MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+        ] = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> RegisterTaskWithMaintenanceWindowResultTypeDef:
         """
         Adds a new task to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_task_with_maintenance_window)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#register_task_with_maintenance_window)
         """
@@ -2013,30 +2044,30 @@
         """
 
     def send_command(
         self,
         *,
         DocumentName: str,
         InstanceIds: Sequence[str] = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         DocumentVersion: str = ...,
         DocumentHash: str = ...,
         DocumentHashType: DocumentHashTypeType = ...,
         TimeoutSeconds: int = ...,
         Comment: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         OutputS3Region: str = ...,
         OutputS3BucketName: str = ...,
         OutputS3KeyPrefix: str = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         ServiceRoleArn: str = ...,
-        NotificationConfig: NotificationConfigTypeDef = ...,
+        NotificationConfig: Union[NotificationConfigTypeDef, NotificationConfigOutputTypeDef] = ...,
         CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> SendCommandResultTypeDef:
         """
         Runs commands on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_command)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#send_command)
         """
@@ -2054,34 +2085,34 @@
         *,
         DocumentName: str,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ClientToken: str = ...,
         Mode: ExecutionModeType = ...,
         TargetParameterName: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> StartAutomationExecutionResultTypeDef:
         """
         Initiates execution of an Automation runbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_automation_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#start_automation_execution)
         """
 
     def start_change_request_execution(
         self,
         *,
         DocumentName: str,
-        Runbooks: Sequence[RunbookTypeDef],
+        Runbooks: Sequence[Union[RunbookTypeDef, RunbookOutputTypeDef]],
         ScheduledTime: Union[datetime, str] = ...,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ChangeRequestName: str = ...,
         ClientToken: str = ...,
         AutoApprove: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
@@ -2145,38 +2176,42 @@
         *,
         AssociationId: str,
         Parameters: Mapping[str, Sequence[str]] = ...,
         DocumentVersion: str = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         Name: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         AssociationName: str = ...,
         AssociationVersion: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> UpdateAssociationResultTypeDef:
         """
         Updates an association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_association)
         """
 
     def update_association_status(
-        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusTypeDef
+        self,
+        *,
+        Name: str,
+        InstanceId: str,
+        AssociationStatus: Union[AssociationStatusTypeDef, AssociationStatusOutputTypeDef]
     ) -> UpdateAssociationStatusResultTypeDef:
         """
         Updates the status of the Amazon Web Services Systems Manager document (SSM
         document) associated with the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_association_status)
@@ -2247,15 +2282,15 @@
         """
 
     def update_maintenance_window_target(
         self,
         *,
         WindowId: str,
         WindowTargetId: str,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...
     ) -> UpdateMaintenanceWindowTargetResultTypeDef:
         """
         Modifies the target of an existing maintenance window.
@@ -2265,28 +2300,37 @@
         """
 
     def update_maintenance_window_task(
         self,
         *,
         WindowId: str,
         WindowTaskId: str,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         TaskArn: str = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
+        TaskParameters: Mapping[
+            str,
+            Union[
+                MaintenanceWindowTaskParameterValueExpressionTypeDef,
+                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+            ],
+        ] = ...,
+        TaskInvocationParameters: Union[
+            MaintenanceWindowTaskInvocationParametersTypeDef,
+            MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+        ] = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> UpdateMaintenanceWindowTaskResultTypeDef:
         """
         Modifies a task assigned to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_maintenance_window_task)
         """
@@ -2343,23 +2387,23 @@
         """
 
     def update_patch_baseline(
         self,
         *,
         BaselineId: str,
         Name: str = ...,
-        GlobalFilters: PatchFilterGroupTypeDef = ...,
-        ApprovalRules: PatchRuleGroupTypeDef = ...,
+        GlobalFilters: Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef] = ...,
+        ApprovalRules: Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef] = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceTypeDef] = ...,
+        Sources: Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]] = ...,
         Replace: bool = ...
     ) -> UpdatePatchBaselineResultTypeDef:
         """
         Modifies an existing patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_patch_baseline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_patch_baseline)
```

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/client.pyi` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -90,30 +90,34 @@
     ListOpsItemEventsPaginator,
     ListOpsItemRelatedItemsPaginator,
     ListOpsMetadataPaginator,
     ListResourceComplianceSummariesPaginator,
     ListResourceDataSyncPaginator,
 )
 from .type_defs import (
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
     AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationExecutionFilterTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
+    AssociationStatusOutputTypeDef,
     AssociationStatusTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     BaselineOverrideTypeDef,
     CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
+    ComplianceExecutionSummaryOutputTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     CreateActivationResultTypeDef,
+    CreateAssociationBatchRequestEntryOutputTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
     CreateAssociationBatchResultTypeDef,
     CreateAssociationResultTypeDef,
     CreateDocumentResultTypeDef,
     CreateMaintenanceWindowResultTypeDef,
     CreateOpsItemResponseTypeDef,
     CreateOpsMetadataResultTypeDef,
@@ -209,32 +213,38 @@
     ListOpsItemRelatedItemsResponseTypeDef,
     ListOpsMetadataResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     ListTagsForResourceResultTypeDef,
     LoggingInfoTypeDef,
     MaintenanceWindowFilterTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     MetadataValueTypeDef,
+    NotificationConfigOutputTypeDef,
     NotificationConfigTypeDef,
     OpsAggregatorTypeDef,
     OpsFilterTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemFilterTypeDef,
     OpsItemNotificationTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsResultAttributeTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
+    PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
     PatchOrchestratorFilterTypeDef,
+    PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
+    PatchSourceOutputTypeDef,
     PatchSourceTypeDef,
     PutInventoryResultTypeDef,
     PutParameterResultTypeDef,
     PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupResultTypeDef,
     RegisterTargetWithMaintenanceWindowResultTypeDef,
@@ -242,23 +252,26 @@
     RegistrationMetadataItemTypeDef,
     RelatedOpsItemTypeDef,
     ResetServiceSettingResultTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     ResourceDataSyncSourceTypeDef,
     ResultAttributeTypeDef,
     ResumeSessionResponseTypeDef,
+    RunbookOutputTypeDef,
     RunbookTypeDef,
     SendCommandResultTypeDef,
     SessionFilterTypeDef,
     StartAutomationExecutionResultTypeDef,
     StartChangeRequestExecutionResultTypeDef,
     StartSessionResponseTypeDef,
     StepExecutionFilterTypeDef,
     TagTypeDef,
+    TargetLocationOutputTypeDef,
     TargetLocationTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
     TerminateSessionResponseTypeDef,
     UnlabelParameterVersionResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
     UpdateDocumentResultTypeDef,
@@ -506,40 +519,47 @@
     def create_association(
         self,
         *,
         Name: str,
         DocumentVersion: str = ...,
         InstanceId: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         AssociationName: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> CreateAssociationResultTypeDef:
         """
         A State Manager association defines the state that you want to maintain on your
         managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_association)
         """
     def create_association_batch(
-        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryTypeDef]
+        self,
+        *,
+        Entries: Sequence[
+            Union[
+                CreateAssociationBatchRequestEntryTypeDef,
+                CreateAssociationBatchRequestEntryOutputTypeDef,
+            ]
+        ]
     ) -> CreateAssociationBatchResultTypeDef:
         """
         Associates the specified Amazon Web Services Systems Manager document (SSM
         document) with the specified managed nodes or targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_association_batch)
@@ -628,23 +648,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#create_ops_metadata)
         """
     def create_patch_baseline(
         self,
         *,
         Name: str,
         OperatingSystem: OperatingSystemType = ...,
-        GlobalFilters: PatchFilterGroupTypeDef = ...,
-        ApprovalRules: PatchRuleGroupTypeDef = ...,
+        GlobalFilters: Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef] = ...,
+        ApprovalRules: Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef] = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceTypeDef] = ...,
+        Sources: Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]] = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePatchBaselineResultTypeDef:
         """
         Creates a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_patch_baseline)
@@ -1054,15 +1074,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_maintenance_window_executions)
         """
     def describe_maintenance_window_schedule(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowScheduleResultTypeDef:
         """
         Retrieves information about upcoming executions of a maintenance window.
@@ -1110,15 +1130,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_maintenance_windows)
         """
     def describe_maintenance_windows_for_target(
         self,
         *,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         ResourceType: MaintenanceWindowResourceTypeType,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsForTargetResultTypeDef:
         """
         Retrieves information about the maintenance window targets or tasks that a
         managed node is associated with.
@@ -1735,15 +1755,17 @@
         """
     def put_compliance_items(
         self,
         *,
         ResourceId: str,
         ResourceType: str,
         ComplianceType: str,
-        ExecutionSummary: ComplianceExecutionSummaryTypeDef,
+        ExecutionSummary: Union[
+            ComplianceExecutionSummaryTypeDef, ComplianceExecutionSummaryOutputTypeDef
+        ],
         Items: Sequence[ComplianceItemEntryTypeDef],
         ItemContentHash: str = ...,
         UploadType: ComplianceUploadTypeType = ...
     ) -> Dict[str, Any]:
         """
         Registers a compliance type and other compliance details on a designated
         resource.
@@ -1809,15 +1831,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#register_patch_baseline_for_patch_group)
         """
     def register_target_with_maintenance_window(
         self,
         *,
         WindowId: str,
         ResourceType: MaintenanceWindowResourceTypeType,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> RegisterTargetWithMaintenanceWindowResultTypeDef:
         """
         Registers a target with a maintenance window.
@@ -1827,27 +1849,36 @@
         """
     def register_task_with_maintenance_window(
         self,
         *,
         WindowId: str,
         TaskArn: str,
         TaskType: MaintenanceWindowTaskTypeType,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
+        TaskParameters: Mapping[
+            str,
+            Union[
+                MaintenanceWindowTaskParameterValueExpressionTypeDef,
+                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+            ],
+        ] = ...,
+        TaskInvocationParameters: Union[
+            MaintenanceWindowTaskInvocationParametersTypeDef,
+            MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+        ] = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> RegisterTaskWithMaintenanceWindowResultTypeDef:
         """
         Adds a new task to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_task_with_maintenance_window)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#register_task_with_maintenance_window)
         """
@@ -1889,30 +1920,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#send_automation_signal)
         """
     def send_command(
         self,
         *,
         DocumentName: str,
         InstanceIds: Sequence[str] = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         DocumentVersion: str = ...,
         DocumentHash: str = ...,
         DocumentHashType: DocumentHashTypeType = ...,
         TimeoutSeconds: int = ...,
         Comment: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         OutputS3Region: str = ...,
         OutputS3BucketName: str = ...,
         OutputS3KeyPrefix: str = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         ServiceRoleArn: str = ...,
-        NotificationConfig: NotificationConfigTypeDef = ...,
+        NotificationConfig: Union[NotificationConfigTypeDef, NotificationConfigOutputTypeDef] = ...,
         CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> SendCommandResultTypeDef:
         """
         Runs commands on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_command)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#send_command)
         """
@@ -1928,33 +1959,33 @@
         *,
         DocumentName: str,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ClientToken: str = ...,
         Mode: ExecutionModeType = ...,
         TargetParameterName: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> StartAutomationExecutionResultTypeDef:
         """
         Initiates execution of an Automation runbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_automation_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#start_automation_execution)
         """
     def start_change_request_execution(
         self,
         *,
         DocumentName: str,
-        Runbooks: Sequence[RunbookTypeDef],
+        Runbooks: Sequence[Union[RunbookTypeDef, RunbookOutputTypeDef]],
         ScheduledTime: Union[datetime, str] = ...,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ChangeRequestName: str = ...,
         ClientToken: str = ...,
         AutoApprove: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
@@ -2013,37 +2044,41 @@
         *,
         AssociationId: str,
         Parameters: Mapping[str, Sequence[str]] = ...,
         DocumentVersion: str = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         Name: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         AssociationName: str = ...,
         AssociationVersion: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> UpdateAssociationResultTypeDef:
         """
         Updates an association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_association)
         """
     def update_association_status(
-        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusTypeDef
+        self,
+        *,
+        Name: str,
+        InstanceId: str,
+        AssociationStatus: Union[AssociationStatusTypeDef, AssociationStatusOutputTypeDef]
     ) -> UpdateAssociationStatusResultTypeDef:
         """
         Updates the status of the Amazon Web Services Systems Manager document (SSM
         document) associated with the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_association_status)
@@ -2109,15 +2144,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_maintenance_window)
         """
     def update_maintenance_window_target(
         self,
         *,
         WindowId: str,
         WindowTargetId: str,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...
     ) -> UpdateMaintenanceWindowTargetResultTypeDef:
         """
         Modifies the target of an existing maintenance window.
@@ -2126,28 +2161,37 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_maintenance_window_target)
         """
     def update_maintenance_window_task(
         self,
         *,
         WindowId: str,
         WindowTaskId: str,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         TaskArn: str = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
+        TaskParameters: Mapping[
+            str,
+            Union[
+                MaintenanceWindowTaskParameterValueExpressionTypeDef,
+                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+            ],
+        ] = ...,
+        TaskInvocationParameters: Union[
+            MaintenanceWindowTaskInvocationParametersTypeDef,
+            MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+        ] = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef] = ...
     ) -> UpdateMaintenanceWindowTaskResultTypeDef:
         """
         Modifies a task assigned to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_maintenance_window_task)
         """
@@ -2200,23 +2244,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_ops_metadata)
         """
     def update_patch_baseline(
         self,
         *,
         BaselineId: str,
         Name: str = ...,
-        GlobalFilters: PatchFilterGroupTypeDef = ...,
-        ApprovalRules: PatchRuleGroupTypeDef = ...,
+        GlobalFilters: Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef] = ...,
+        ApprovalRules: Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef] = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceTypeDef] = ...,
+        Sources: Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]] = ...,
         Replace: bool = ...
     ) -> UpdatePatchBaselineResultTypeDef:
         """
         Modifies an existing patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_patch_baseline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#update_patch_baseline)
```

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/literals.py` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/literals.pyi` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/paginator.py` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     list_ops_item_events_paginator: ListOpsItemEventsPaginator = client.get_paginator("list_ops_item_events")
     list_ops_item_related_items_paginator: ListOpsItemRelatedItemsPaginator = client.get_paginator("list_ops_item_related_items")
     list_ops_metadata_paginator: ListOpsMetadataPaginator = client.get_paginator("list_ops_metadata")
     list_resource_compliance_summaries_paginator: ListResourceComplianceSummariesPaginator = client.get_paginator("list_resource_compliance_summaries")
     list_resource_data_sync_paginator: ListResourceDataSyncPaginator = client.get_paginator("list_resource_data_sync")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     MaintenanceWindowResourceTypeType,
     OperatingSystemType,
     PatchPropertyType,
@@ -195,14 +195,15 @@
     PaginatorConfigTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     ResultAttributeTypeDef,
     SessionFilterTypeDef,
     StepExecutionFilterTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
 )
 
 __all__ = (
     "DescribeActivationsPaginator",
     "DescribeAssociationExecutionTargetsPaginator",
     "DescribeAssociationExecutionsPaginator",
@@ -572,15 +573,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
     """
 
     def paginate(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
@@ -648,15 +649,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
     """
 
     def paginate(
         self,
         *,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         ResourceType: MaintenanceWindowResourceTypeType,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
```

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/paginator.pyi` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     list_ops_item_events_paginator: ListOpsItemEventsPaginator = client.get_paginator("list_ops_item_events")
     list_ops_item_related_items_paginator: ListOpsItemRelatedItemsPaginator = client.get_paginator("list_ops_item_related_items")
     list_ops_metadata_paginator: ListOpsMetadataPaginator = client.get_paginator("list_ops_metadata")
     list_resource_compliance_summaries_paginator: ListResourceComplianceSummariesPaginator = client.get_paginator("list_resource_compliance_summaries")
     list_resource_data_sync_paginator: ListResourceDataSyncPaginator = client.get_paginator("list_resource_data_sync")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     MaintenanceWindowResourceTypeType,
     OperatingSystemType,
     PatchPropertyType,
@@ -195,14 +195,15 @@
     PaginatorConfigTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     ResultAttributeTypeDef,
     SessionFilterTypeDef,
     StepExecutionFilterTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
 )
 
 __all__ = (
     "DescribeActivationsPaginator",
     "DescribeAssociationExecutionTargetsPaginator",
     "DescribeAssociationExecutionsPaginator",
@@ -552,15 +553,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
     """
 
     def paginate(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
@@ -624,15 +625,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
     """
 
     def paginate(
         self,
         *,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         ResourceType: MaintenanceWindowResourceTypeType,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
```

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/type_defs.py` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,15 @@
     "RegistrationMetadataItemTypeDef",
     "TargetTypeDef",
     "DocumentRequiresTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
     "MetadataValueTypeDef",
+    "PatchSourceOutputTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteInventoryRequestRequestTypeDef",
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     "DeleteOpsMetadataRequestRequestTypeDef",
     "DeleteParameterRequestRequestTypeDef",
@@ -226,15 +227,14 @@
     "OpsResultAttributeTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
-    "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
@@ -1037,14 +1037,23 @@
     "MetadataValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+PatchSourceOutputTypeDef = TypedDict(
+    "PatchSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Products": List[str],
+        "Configuration": str,
+    },
+)
+
 DeleteActivationRequestRequestTypeDef = TypedDict(
     "DeleteActivationRequestRequestTypeDef",
     {
         "ActivationId": str,
     },
 )
 
@@ -2197,23 +2206,14 @@
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-PatchSourceOutputTypeDef = TypedDict(
-    "PatchSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Products": List[str],
-        "Configuration": str,
-    },
-)
-
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -3797,15 +3797,15 @@
 ):
     pass
 
 
 _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "ResourceType": MaintenanceWindowResourceTypeType,
     },
 )
 _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     {
         "MaxResults": int,
@@ -3823,15 +3823,15 @@
 
 
 _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
     },
 )
 _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
     {
         "OwnerInformation": str,
         "Name": str,
@@ -3855,15 +3855,15 @@
         "WindowId": str,
         "WindowTargetId": str,
     },
 )
 _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
         "Replace": bool,
     },
     total=False,
 )
@@ -4299,15 +4299,15 @@
     },
     total=False,
 )
 
 _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "ResourceType": MaintenanceWindowResourceTypeType,
     },
 )
 _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -4633,28 +4633,28 @@
 
 
 DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
     TypedDict(
         "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
         {
             "WindowId": str,
-            "Targets": Sequence[TargetTypeDef],
+            "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
             "ResourceType": MaintenanceWindowResourceTypeType,
             "Filters": Sequence[PatchOrchestratorFilterTypeDef],
             "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
 DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
     {
         "WindowId": str,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "ResourceType": MaintenanceWindowResourceTypeType,
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
@@ -6051,15 +6051,15 @@
         "DocumentName": str,
     },
 )
 _OptionalSendCommandRequestRequestTypeDef = TypedDict(
     "_OptionalSendCommandRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "DocumentVersion": str,
         "DocumentHash": str,
         "DocumentHashType": DocumentHashTypeType,
         "TimeoutSeconds": int,
         "Comment": str,
         "Parameters": Mapping[str, Sequence[str]],
         "OutputS3Region": str,
@@ -6748,26 +6748,26 @@
 )
 _OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAssociationRequestRequestTypeDef",
     {
         "DocumentVersion": str,
         "InstanceId": str,
         "Parameters": Mapping[str, Sequence[str]],
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "AutomationTargetParameterName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "Tags": Sequence[TagTypeDef],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
@@ -6815,19 +6815,19 @@
     "_OptionalStartAutomationExecutionRequestRequestTypeDef",
     {
         "DocumentVersion": str,
         "Parameters": Mapping[str, Sequence[str]],
         "ClientToken": str,
         "Mode": ExecutionModeType,
         "TargetParameterName": str,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
 
@@ -6848,25 +6848,25 @@
     "_OptionalUpdateAssociationRequestRequestTypeDef",
     {
         "Parameters": Mapping[str, Sequence[str]],
         "DocumentVersion": str,
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "Name": str,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "AssociationName": str,
         "AssociationVersion": str,
         "AutomationTargetParameterName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -6977,17 +6977,23 @@
         "TaskArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
     },
 )
 _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskParameters": Mapping[
+            str,
+            Union[
+                MaintenanceWindowTaskParameterValueExpressionTypeDef,
+                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+            ],
+        ],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
@@ -7012,18 +7018,24 @@
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskParameters": Mapping[
+            str,
+            Union[
+                MaintenanceWindowTaskParameterValueExpressionTypeDef,
+                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+            ],
+        ],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
@@ -7242,23 +7254,28 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssociationBatchRequestRequestTypeDef = TypedDict(
     "CreateAssociationBatchRequestRequestTypeDef",
     {
-        "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
+        "Entries": Sequence[
+            Union[
+                CreateAssociationBatchRequestEntryTypeDef,
+                CreateAssociationBatchRequestEntryOutputTypeDef,
+            ]
+        ],
     },
 )
 
 _RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
     {
         "DocumentName": str,
-        "Runbooks": Sequence[RunbookTypeDef],
+        "Runbooks": Sequence[Union[RunbookTypeDef, RunbookOutputTypeDef]],
     },
 )
 _OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
     "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
     {
         "ScheduledTime": Union[datetime, str],
         "DocumentVersion": str,
@@ -7354,15 +7371,15 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceTypeDef],
+        "Sources": Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]],
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
@@ -7387,15 +7404,15 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceTypeDef],
+        "Sources": Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]],
         "Replace": bool,
     },
     total=False,
 )
 
 
 class UpdatePatchBaselineRequestRequestTypeDef(
```

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/type_defs.pyi` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     "RegistrationMetadataItemTypeDef",
     "TargetTypeDef",
     "DocumentRequiresTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
     "MetadataValueTypeDef",
+    "PatchSourceOutputTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteInventoryRequestRequestTypeDef",
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     "DeleteOpsMetadataRequestRequestTypeDef",
     "DeleteParameterRequestRequestTypeDef",
@@ -225,15 +226,14 @@
     "OpsResultAttributeTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
-    "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
@@ -1022,14 +1022,23 @@
     "MetadataValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+PatchSourceOutputTypeDef = TypedDict(
+    "PatchSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Products": List[str],
+        "Configuration": str,
+    },
+)
+
 DeleteActivationRequestRequestTypeDef = TypedDict(
     "DeleteActivationRequestRequestTypeDef",
     {
         "ActivationId": str,
     },
 )
 
@@ -2130,23 +2139,14 @@
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-PatchSourceOutputTypeDef = TypedDict(
-    "PatchSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Products": List[str],
-        "Configuration": str,
-    },
-)
-
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -3686,15 +3686,15 @@
     _RequiredCreateActivationRequestRequestTypeDef, _OptionalCreateActivationRequestRequestTypeDef
 ):
     pass
 
 _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "ResourceType": MaintenanceWindowResourceTypeType,
     },
 )
 _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     {
         "MaxResults": int,
@@ -3710,15 +3710,15 @@
     pass
 
 _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
     },
 )
 _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
     {
         "OwnerInformation": str,
         "Name": str,
@@ -3740,15 +3740,15 @@
         "WindowId": str,
         "WindowTargetId": str,
     },
 )
 _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
         "Replace": bool,
     },
     total=False,
 )
@@ -4160,15 +4160,15 @@
     },
     total=False,
 )
 
 _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "ResourceType": MaintenanceWindowResourceTypeType,
     },
 )
 _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -4474,28 +4474,28 @@
     pass
 
 DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
     TypedDict(
         "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
         {
             "WindowId": str,
-            "Targets": Sequence[TargetTypeDef],
+            "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
             "ResourceType": MaintenanceWindowResourceTypeType,
             "Filters": Sequence[PatchOrchestratorFilterTypeDef],
             "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
 DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
     {
         "WindowId": str,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "ResourceType": MaintenanceWindowResourceTypeType,
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
@@ -5846,15 +5846,15 @@
         "DocumentName": str,
     },
 )
 _OptionalSendCommandRequestRequestTypeDef = TypedDict(
     "_OptionalSendCommandRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "DocumentVersion": str,
         "DocumentHash": str,
         "DocumentHashType": DocumentHashTypeType,
         "TimeoutSeconds": int,
         "Comment": str,
         "Parameters": Mapping[str, Sequence[str]],
         "OutputS3Region": str,
@@ -6527,26 +6527,26 @@
 )
 _OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAssociationRequestRequestTypeDef",
     {
         "DocumentVersion": str,
         "InstanceId": str,
         "Parameters": Mapping[str, Sequence[str]],
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "AutomationTargetParameterName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "Tags": Sequence[TagTypeDef],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
@@ -6590,19 +6590,19 @@
     "_OptionalStartAutomationExecutionRequestRequestTypeDef",
     {
         "DocumentVersion": str,
         "Parameters": Mapping[str, Sequence[str]],
         "ClientToken": str,
         "Mode": ExecutionModeType,
         "TargetParameterName": str,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
 class StartAutomationExecutionRequestRequestTypeDef(
@@ -6621,25 +6621,25 @@
     "_OptionalUpdateAssociationRequestRequestTypeDef",
     {
         "Parameters": Mapping[str, Sequence[str]],
         "DocumentVersion": str,
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "Name": str,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "AssociationName": str,
         "AssociationVersion": str,
         "AutomationTargetParameterName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "TargetLocations": Sequence[Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]],
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -6748,17 +6748,23 @@
         "TaskArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
     },
 )
 _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskParameters": Mapping[
+            str,
+            Union[
+                MaintenanceWindowTaskParameterValueExpressionTypeDef,
+                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+            ],
+        ],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
@@ -6781,18 +6787,24 @@
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskParameters": Mapping[
+            str,
+            Union[
+                MaintenanceWindowTaskParameterValueExpressionTypeDef,
+                MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+            ],
+        ],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
@@ -7007,23 +7019,28 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssociationBatchRequestRequestTypeDef = TypedDict(
     "CreateAssociationBatchRequestRequestTypeDef",
     {
-        "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
+        "Entries": Sequence[
+            Union[
+                CreateAssociationBatchRequestEntryTypeDef,
+                CreateAssociationBatchRequestEntryOutputTypeDef,
+            ]
+        ],
     },
 )
 
 _RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
     {
         "DocumentName": str,
-        "Runbooks": Sequence[RunbookTypeDef],
+        "Runbooks": Sequence[Union[RunbookTypeDef, RunbookOutputTypeDef]],
     },
 )
 _OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
     "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
     {
         "ScheduledTime": Union[datetime, str],
         "DocumentVersion": str,
@@ -7117,15 +7134,15 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceTypeDef],
+        "Sources": Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]],
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreatePatchBaselineRequestRequestTypeDef(
@@ -7148,15 +7165,15 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceTypeDef],
+        "Sources": Sequence[Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]],
         "Replace": bool,
     },
     total=False,
 )
 
 class UpdatePatchBaselineRequestRequestTypeDef(
     _RequiredUpdatePatchBaselineRequestRequestTypeDef,
```

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/waiter.py` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/waiter.pyi` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/PKG-INFO` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.28.15
-Summary: Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -681,14 +681,15 @@
     RegistrationMetadataItemTypeDef,
     TargetTypeDef,
     DocumentRequiresTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
     MetadataValueTypeDef,
+    PatchSourceOutputTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
@@ -765,15 +766,14 @@
     OpsResultAttributeTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
-    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
```

### Comparing `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/SOURCES.txt` & `mypy-boto3-ssm-1.28.15.post1/mypy_boto3_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.15/setup.py` & `mypy-boto3-ssm-1.28.15.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

