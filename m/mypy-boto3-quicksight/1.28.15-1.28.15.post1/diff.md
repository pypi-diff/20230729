# Comparing `tmp/mypy-boto3-quicksight-1.28.15.tar.gz` & `tmp/mypy-boto3-quicksight-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-quicksight-1.28.15.tar", last modified: Fri Jul 28 20:43:30 2023, max compression
+gzip compressed data, was "mypy-boto3-quicksight-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:57 2023, max compression
```

## Comparing `mypy-boto3-quicksight-1.28.15.tar` & `mypy-boto3-quicksight-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.937689 mypy-boto3-quicksight-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    75930 2023-07-28 20:43:30.933689 mypy-boto3-quicksight-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    74431 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.925689 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   123489 2023-07-28 20:35:47.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   123296 2023-07-28 20:35:47.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    36327 2023-07-28 20:35:48.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    36325 2023-07-28 20:35:48.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29023 2023-07-28 20:35:47.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28996 2023-07-28 20:35:47.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   550945 2023-07-28 20:36:06.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   550229 2023-07-28 20:35:58.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.929689 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    75930 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:30.937689 mypy-boto3-quicksight-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:57.065351 mypy-boto3-quicksight-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    75936 2023-07-29 10:03:57.065351 mypy-boto3-quicksight-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    74431 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:57.061351 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127673 2023-07-29 09:55:47.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127480 2023-07-29 09:55:47.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36327 2023-07-29 09:55:49.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36325 2023-07-29 09:55:48.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29023 2023-07-29 09:55:48.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28996 2023-07-29 09:55:48.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   552869 2023-07-29 09:56:12.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   552153 2023-07-29 09:56:01.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:57.065351 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    75936 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:57.065351 mypy-boto3-quicksight-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-quicksight-1.28.15/LICENSE` & `mypy-boto3-quicksight-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15/PKG-INFO` & `mypy-boto3-quicksight-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.28.15
-Summary: Type annotations for boto3.QuickSight 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.QuickSight 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
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
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
 See how it helps to find and fix potential bugs:
 
@@ -707,16 +707,18 @@
     ConditionalFormattingSolidColorTypeDef,
     ConditionalFormattingCustomIconOptionsTypeDef,
     ConditionalFormattingIconDisplayConfigurationTypeDef,
     ConditionalFormattingIconSetTypeDef,
     TagTypeDef,
     CreateAccountSubscriptionRequestRequestTypeDef,
     SignupResponseTypeDef,
+    ResourcePermissionOutputTypeDef,
     ResourcePermissionTypeDef,
     DataSetUsageConfigurationTypeDef,
+    FieldFolderOutputTypeDef,
     FieldFolderTypeDef,
     RowLevelPermissionDataSetTypeDef,
     CreateFolderMembershipRequestRequestTypeDef,
     FolderMemberTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
     GroupMemberTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -758,15 +760,14 @@
     DataPathLabelTypeTypeDef,
     FieldLabelTypeTypeDef,
     MaximumLabelTypeTypeDef,
     MinimumLabelTypeTypeDef,
     RangeEndsLabelTypeTypeDef,
     DataPathValueTypeDef,
     DataSetSearchFilterTypeDef,
-    FieldFolderOutputTypeDef,
     OutputColumnTypeDef,
     DataSourceErrorInfoTypeDef,
     DatabricksParametersTypeDef,
     ExasolParametersTypeDef,
     JiraParametersTypeDef,
     MariaDbParametersTypeDef,
     MySqlParametersTypeDef,
@@ -821,15 +822,14 @@
     DeleteUserRequestRequestTypeDef,
     DeleteVPCConnectionRequestRequestTypeDef,
     DescribeAccountCustomizationRequestRequestTypeDef,
     DescribeAccountSettingsRequestRequestTypeDef,
     DescribeAccountSubscriptionRequestRequestTypeDef,
     DescribeAnalysisDefinitionRequestRequestTypeDef,
     DescribeAnalysisPermissionsRequestRequestTypeDef,
-    ResourcePermissionOutputTypeDef,
     DescribeAnalysisRequestRequestTypeDef,
     DescribeAssetBundleExportJobRequestRequestTypeDef,
     DescribeAssetBundleImportJobRequestRequestTypeDef,
     DescribeDashboardDefinitionRequestRequestTypeDef,
     DescribeDashboardPermissionsRequestRequestTypeDef,
     DescribeDashboardRequestRequestTypeDef,
     DescribeDashboardSnapshotJobRequestRequestTypeDef,
@@ -1173,14 +1173,28 @@
     ConditionalFormattingCustomIconConditionTypeDef,
     CreateAccountCustomizationRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateVPCConnectionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
+    DescribeAnalysisPermissionsResponseTypeDef,
+    DescribeDataSetPermissionsResponseTypeDef,
+    DescribeDataSourcePermissionsResponseTypeDef,
+    DescribeFolderPermissionsResponseTypeDef,
+    DescribeFolderResolvedPermissionsResponseTypeDef,
+    DescribeTemplatePermissionsResponseTypeDef,
+    DescribeThemePermissionsResponseTypeDef,
+    DescribeTopicPermissionsResponseTypeDef,
+    LinkSharingConfigurationTypeDef,
+    UpdateAnalysisPermissionsResponseTypeDef,
+    UpdateFolderPermissionsResponseTypeDef,
+    UpdateTemplatePermissionsResponseTypeDef,
+    UpdateThemePermissionsResponseTypeDef,
+    UpdateTopicPermissionsResponseTypeDef,
     CreateFolderRequestRequestTypeDef,
     UpdateAnalysisPermissionsRequestRequestTypeDef,
     UpdateDashboardPermissionsRequestRequestTypeDef,
     UpdateDataSetPermissionsRequestRequestTypeDef,
     UpdateDataSourcePermissionsRequestRequestTypeDef,
     UpdateFolderPermissionsRequestRequestTypeDef,
     UpdateTemplatePermissionsRequestRequestTypeDef,
@@ -1233,28 +1247,14 @@
     SearchDataSourcesResponseTypeDef,
     DateTimeDatasetParameterOutputTypeDef,
     DateTimeDatasetParameterTypeDef,
     TimeRangeFilterValueOutputTypeDef,
     TimeRangeFilterValueTypeDef,
     DecimalDatasetParameterOutputTypeDef,
     DecimalDatasetParameterTypeDef,
-    DescribeAnalysisPermissionsResponseTypeDef,
-    DescribeDataSetPermissionsResponseTypeDef,
-    DescribeDataSourcePermissionsResponseTypeDef,
-    DescribeFolderPermissionsResponseTypeDef,
-    DescribeFolderResolvedPermissionsResponseTypeDef,
-    DescribeTemplatePermissionsResponseTypeDef,
-    DescribeThemePermissionsResponseTypeDef,
-    DescribeTopicPermissionsResponseTypeDef,
-    LinkSharingConfigurationTypeDef,
-    UpdateAnalysisPermissionsResponseTypeDef,
-    UpdateFolderPermissionsResponseTypeDef,
-    UpdateTemplatePermissionsResponseTypeDef,
-    UpdateThemePermissionsResponseTypeDef,
-    UpdateTopicPermissionsResponseTypeDef,
     DescribeFolderResponseTypeDef,
     DescribeIAMPolicyAssignmentResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     TopicRefreshScheduleSummaryTypeDef,
     DescribeUserResponseTypeDef,
     ListUsersResponseTypeDef,
@@ -1390,27 +1390,27 @@
     TopicCategoryFilterOutputTypeDef,
     TopicCategoryFilterTypeDef,
     TagColumnOperationOutputTypeDef,
     TagColumnOperationTypeDef,
     DataSetConfigurationOutputTypeDef,
     DataSetConfigurationTypeDef,
     ConditionalFormattingIconTypeDef,
+    DescribeDashboardPermissionsResponseTypeDef,
+    UpdateDashboardPermissionsResponseTypeDef,
     ListDataSetsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     DestinationParameterValueConfigurationOutputTypeDef,
     DestinationParameterValueConfigurationTypeDef,
     DashboardPublishOptionsTypeDef,
     VisualPaletteOutputTypeDef,
     VisualPaletteTypeDef,
     PivotTableFieldCollapseStateOptionOutputTypeDef,
     PivotTableFieldCollapseStateOptionTypeDef,
     TimeRangeFilterOutputTypeDef,
     TimeRangeFilterTypeDef,
-    DescribeDashboardPermissionsResponseTypeDef,
-    UpdateDashboardPermissionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     DefaultFormattingTypeDef,
     CustomActionFilterOperationOutputTypeDef,
     CustomActionFilterOperationTypeDef,
     AxisLabelOptionsTypeDef,
     DataLabelOptionsOutputTypeDef,
     DataLabelOptionsTypeDef,
```

### Comparing `mypy-boto3-quicksight-1.28.15/README.md` & `mypy-boto3-quicksight-1.28.15.post1/README.md`

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
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
 See how it helps to find and fix potential bugs:
 
@@ -675,16 +675,18 @@
     ConditionalFormattingSolidColorTypeDef,
     ConditionalFormattingCustomIconOptionsTypeDef,
     ConditionalFormattingIconDisplayConfigurationTypeDef,
     ConditionalFormattingIconSetTypeDef,
     TagTypeDef,
     CreateAccountSubscriptionRequestRequestTypeDef,
     SignupResponseTypeDef,
+    ResourcePermissionOutputTypeDef,
     ResourcePermissionTypeDef,
     DataSetUsageConfigurationTypeDef,
+    FieldFolderOutputTypeDef,
     FieldFolderTypeDef,
     RowLevelPermissionDataSetTypeDef,
     CreateFolderMembershipRequestRequestTypeDef,
     FolderMemberTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
     GroupMemberTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -726,15 +728,14 @@
     DataPathLabelTypeTypeDef,
     FieldLabelTypeTypeDef,
     MaximumLabelTypeTypeDef,
     MinimumLabelTypeTypeDef,
     RangeEndsLabelTypeTypeDef,
     DataPathValueTypeDef,
     DataSetSearchFilterTypeDef,
-    FieldFolderOutputTypeDef,
     OutputColumnTypeDef,
     DataSourceErrorInfoTypeDef,
     DatabricksParametersTypeDef,
     ExasolParametersTypeDef,
     JiraParametersTypeDef,
     MariaDbParametersTypeDef,
     MySqlParametersTypeDef,
@@ -789,15 +790,14 @@
     DeleteUserRequestRequestTypeDef,
     DeleteVPCConnectionRequestRequestTypeDef,
     DescribeAccountCustomizationRequestRequestTypeDef,
     DescribeAccountSettingsRequestRequestTypeDef,
     DescribeAccountSubscriptionRequestRequestTypeDef,
     DescribeAnalysisDefinitionRequestRequestTypeDef,
     DescribeAnalysisPermissionsRequestRequestTypeDef,
-    ResourcePermissionOutputTypeDef,
     DescribeAnalysisRequestRequestTypeDef,
     DescribeAssetBundleExportJobRequestRequestTypeDef,
     DescribeAssetBundleImportJobRequestRequestTypeDef,
     DescribeDashboardDefinitionRequestRequestTypeDef,
     DescribeDashboardPermissionsRequestRequestTypeDef,
     DescribeDashboardRequestRequestTypeDef,
     DescribeDashboardSnapshotJobRequestRequestTypeDef,
@@ -1141,14 +1141,28 @@
     ConditionalFormattingCustomIconConditionTypeDef,
     CreateAccountCustomizationRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateVPCConnectionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
+    DescribeAnalysisPermissionsResponseTypeDef,
+    DescribeDataSetPermissionsResponseTypeDef,
+    DescribeDataSourcePermissionsResponseTypeDef,
+    DescribeFolderPermissionsResponseTypeDef,
+    DescribeFolderResolvedPermissionsResponseTypeDef,
+    DescribeTemplatePermissionsResponseTypeDef,
+    DescribeThemePermissionsResponseTypeDef,
+    DescribeTopicPermissionsResponseTypeDef,
+    LinkSharingConfigurationTypeDef,
+    UpdateAnalysisPermissionsResponseTypeDef,
+    UpdateFolderPermissionsResponseTypeDef,
+    UpdateTemplatePermissionsResponseTypeDef,
+    UpdateThemePermissionsResponseTypeDef,
+    UpdateTopicPermissionsResponseTypeDef,
     CreateFolderRequestRequestTypeDef,
     UpdateAnalysisPermissionsRequestRequestTypeDef,
     UpdateDashboardPermissionsRequestRequestTypeDef,
     UpdateDataSetPermissionsRequestRequestTypeDef,
     UpdateDataSourcePermissionsRequestRequestTypeDef,
     UpdateFolderPermissionsRequestRequestTypeDef,
     UpdateTemplatePermissionsRequestRequestTypeDef,
@@ -1201,28 +1215,14 @@
     SearchDataSourcesResponseTypeDef,
     DateTimeDatasetParameterOutputTypeDef,
     DateTimeDatasetParameterTypeDef,
     TimeRangeFilterValueOutputTypeDef,
     TimeRangeFilterValueTypeDef,
     DecimalDatasetParameterOutputTypeDef,
     DecimalDatasetParameterTypeDef,
-    DescribeAnalysisPermissionsResponseTypeDef,
-    DescribeDataSetPermissionsResponseTypeDef,
-    DescribeDataSourcePermissionsResponseTypeDef,
-    DescribeFolderPermissionsResponseTypeDef,
-    DescribeFolderResolvedPermissionsResponseTypeDef,
-    DescribeTemplatePermissionsResponseTypeDef,
-    DescribeThemePermissionsResponseTypeDef,
-    DescribeTopicPermissionsResponseTypeDef,
-    LinkSharingConfigurationTypeDef,
-    UpdateAnalysisPermissionsResponseTypeDef,
-    UpdateFolderPermissionsResponseTypeDef,
-    UpdateTemplatePermissionsResponseTypeDef,
-    UpdateThemePermissionsResponseTypeDef,
-    UpdateTopicPermissionsResponseTypeDef,
     DescribeFolderResponseTypeDef,
     DescribeIAMPolicyAssignmentResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     TopicRefreshScheduleSummaryTypeDef,
     DescribeUserResponseTypeDef,
     ListUsersResponseTypeDef,
@@ -1358,27 +1358,27 @@
     TopicCategoryFilterOutputTypeDef,
     TopicCategoryFilterTypeDef,
     TagColumnOperationOutputTypeDef,
     TagColumnOperationTypeDef,
     DataSetConfigurationOutputTypeDef,
     DataSetConfigurationTypeDef,
     ConditionalFormattingIconTypeDef,
+    DescribeDashboardPermissionsResponseTypeDef,
+    UpdateDashboardPermissionsResponseTypeDef,
     ListDataSetsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     DestinationParameterValueConfigurationOutputTypeDef,
     DestinationParameterValueConfigurationTypeDef,
     DashboardPublishOptionsTypeDef,
     VisualPaletteOutputTypeDef,
     VisualPaletteTypeDef,
     PivotTableFieldCollapseStateOptionOutputTypeDef,
     PivotTableFieldCollapseStateOptionTypeDef,
     TimeRangeFilterOutputTypeDef,
     TimeRangeFilterTypeDef,
-    DescribeDashboardPermissionsResponseTypeDef,
-    UpdateDashboardPermissionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     DefaultFormattingTypeDef,
     CustomActionFilterOperationOutputTypeDef,
     CustomActionFilterOperationTypeDef,
     AxisLabelOptionsTypeDef,
     DataLabelOptionsOutputTypeDef,
     DataLabelOptionsTypeDef,
```

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__init__.py` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__init__.pyi` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/client.py` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_quicksight.client import QuickSightClient
 
     session = Session()
     client: QuickSightClient = session.client("quicksight")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssetBundleExportFormatType,
     AssetBundleImportFailureActionType,
     AssignmentStatusType,
@@ -58,23 +58,28 @@
     SearchDashboardsPaginator,
     SearchDataSetsPaginator,
     SearchDataSourcesPaginator,
     SearchGroupsPaginator,
 )
 from .type_defs import (
     AccountCustomizationTypeDef,
+    AnalysisDefinitionOutputTypeDef,
     AnalysisDefinitionTypeDef,
     AnalysisSearchFilterTypeDef,
     AnalysisSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
     AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+    AssetBundleImportJobOverrideParametersOutputTypeDef,
     AssetBundleImportJobOverrideParametersTypeDef,
     AssetBundleImportSourceTypeDef,
     CancelIngestionResponseTypeDef,
+    ColumnGroupOutputTypeDef,
     ColumnGroupTypeDef,
+    ColumnLevelPermissionRuleOutputTypeDef,
     ColumnLevelPermissionRuleTypeDef,
     CreateAccountCustomizationResponseTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
     CreateAnalysisResponseTypeDef,
     CreateDashboardResponseTypeDef,
     CreateDataSetResponseTypeDef,
     CreateDataSourceResponseTypeDef,
@@ -92,15 +97,17 @@
     CreateThemeResponseTypeDef,
     CreateTopicRefreshScheduleResponseTypeDef,
     CreateTopicResponseTypeDef,
     CreateVPCConnectionResponseTypeDef,
     DashboardPublishOptionsTypeDef,
     DashboardSearchFilterTypeDef,
     DashboardSourceEntityTypeDef,
+    DashboardVersionDefinitionOutputTypeDef,
     DashboardVersionDefinitionTypeDef,
+    DatasetParameterOutputTypeDef,
     DatasetParameterTypeDef,
     DataSetRefreshPropertiesTypeDef,
     DataSetSearchFilterTypeDef,
     DataSetUsageConfigurationTypeDef,
     DataSourceCredentialsTypeDef,
     DataSourceParametersTypeDef,
     DataSourceSearchFilterTypeDef,
@@ -164,14 +171,15 @@
     DescribeThemeResponseTypeDef,
     DescribeTopicPermissionsResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     DescribeTopicResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeVPCConnectionResponseTypeDef,
+    FieldFolderOutputTypeDef,
     FieldFolderTypeDef,
     FolderSearchFilterTypeDef,
     GenerateEmbedUrlForAnonymousUserResponseTypeDef,
     GenerateEmbedUrlForRegisteredUserResponseTypeDef,
     GetDashboardEmbedUrlResponseTypeDef,
     GetSessionEmbedUrlResponseTypeDef,
     GroupSearchFilterTypeDef,
@@ -199,44 +207,55 @@
     ListThemesResponseTypeDef,
     ListThemeVersionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     ListTopicsResponseTypeDef,
     ListUserGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
     ListVPCConnectionsResponseTypeDef,
+    LogicalTableOutputTypeDef,
     LogicalTableTypeDef,
+    ParametersOutputTypeDef,
     ParametersTypeDef,
+    PhysicalTableOutputTypeDef,
     PhysicalTableTypeDef,
     PutDataSetRefreshPropertiesResponseTypeDef,
+    RefreshScheduleOutputTypeDef,
     RefreshScheduleTypeDef,
     RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     RegisterUserResponseTypeDef,
+    ResourcePermissionOutputTypeDef,
     ResourcePermissionTypeDef,
     RestoreAnalysisResponseTypeDef,
     RowLevelPermissionDataSetTypeDef,
+    RowLevelPermissionTagConfigurationOutputTypeDef,
     RowLevelPermissionTagConfigurationTypeDef,
     SearchAnalysesResponseTypeDef,
     SearchDashboardsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     SearchDataSourcesResponseTypeDef,
     SearchFoldersResponseTypeDef,
     SearchGroupsResponseTypeDef,
     SessionTagTypeDef,
+    SnapshotConfigurationOutputTypeDef,
     SnapshotConfigurationTypeDef,
     SnapshotUserConfigurationTypeDef,
     SslPropertiesTypeDef,
     StartAssetBundleExportJobResponseTypeDef,
     StartAssetBundleImportJobResponseTypeDef,
     StartDashboardSnapshotJobResponseTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
     TemplateSourceEntityTypeDef,
+    TemplateVersionDefinitionOutputTypeDef,
     TemplateVersionDefinitionTypeDef,
+    ThemeConfigurationOutputTypeDef,
     ThemeConfigurationTypeDef,
+    TopicDetailsOutputTypeDef,
     TopicDetailsTypeDef,
+    TopicRefreshScheduleOutputTypeDef,
     TopicRefreshScheduleTypeDef,
     UntagResourceResponseTypeDef,
     UpdateAccountCustomizationResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     UpdateAnalysisPermissionsResponseTypeDef,
     UpdateAnalysisResponseTypeDef,
     UpdateDashboardPermissionsResponseTypeDef,
@@ -394,42 +413,48 @@
 
     def create_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Definition: AnalysisDefinitionTypeDef = ...
+        Definition: Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef] = ...
     ) -> CreateAnalysisResponseTypeDef:
         """
         Creates an analysis in Amazon QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_analysis)
         """
 
     def create_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: DashboardVersionDefinitionTypeDef = ...
+        Definition: Union[
+            DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
+        ] = ...
     ) -> CreateDashboardResponseTypeDef:
         """
         Creates a dashboard from either a template or directly with a
         `DashboardDefinition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_dashboard)
@@ -437,26 +462,35 @@
 
     def create_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],
+        PhysicalTableMap: Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,
-        ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,
-        FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        LogicalTableMap: Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]] = ...,
+        ColumnGroups: Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]] = ...,
+        FieldFolders: Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
-        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
+        RowLevelPermissionTagConfiguration: Union[
+            RowLevelPermissionTagConfigurationTypeDef,
+            RowLevelPermissionTagConfigurationOutputTypeDef,
+        ] = ...,
+        ColumnLevelPermissionRules: Sequence[
+            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...
+        DatasetParameters: Sequence[
+            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+        ] = ...
     ) -> CreateDataSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_data_set)
         """
@@ -466,15 +500,17 @@
         *,
         AwsAccountId: str,
         DataSourceId: str,
         Name: str,
         Type: DataSourceTypeType,
         DataSourceParameters: DataSourceParametersTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
         SslProperties: SslPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source.
 
@@ -486,15 +522,17 @@
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Name: str = ...,
         FolderType: Literal["SHARED"] = ...,
         ParentFolderArn: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFolderResponseTypeDef:
         """
         Creates an empty shared folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_folder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_folder)
@@ -576,34 +614,42 @@
         QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_namespace)
         """
 
     def create_refresh_schedule(
-        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleTypeDef
+        self,
+        *,
+        DataSetId: str,
+        AwsAccountId: str,
+        Schedule: Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
     ) -> CreateRefreshScheduleResponseTypeDef:
         """
         Creates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_refresh_schedule)
         """
 
     def create_template(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         Name: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
-        Definition: TemplateVersionDefinitionTypeDef = ...
+        Definition: Union[
+            TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
+        ] = ...
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template either from a `TemplateDefinition` or from an existing Amazon
         QuickSight analysis or template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_template)
@@ -622,17 +668,19 @@
     def create_theme(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         Name: str,
         BaseThemeId: str,
-        Configuration: ThemeConfigurationTypeDef,
+        Configuration: Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef],
         VersionDescription: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_theme)
@@ -649,15 +697,15 @@
         """
 
     def create_topic(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        Topic: TopicDetailsTypeDef,
+        Topic: Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateTopicResponseTypeDef:
         """
         Creates a new Q topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic)
@@ -665,15 +713,15 @@
 
     def create_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetArn: str,
-        RefreshSchedule: TopicRefreshScheduleTypeDef,
+        RefreshSchedule: Union[TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef],
         DatasetName: str = ...
     ) -> CreateTopicRefreshScheduleResponseTypeDef:
         """
         Creates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic_refresh_schedule)
@@ -1891,30 +1939,36 @@
         self,
         *,
         AwsAccountId: str,
         AssetBundleExportJobId: str,
         ResourceArns: Sequence[str],
         ExportFormat: AssetBundleExportFormatType,
         IncludeAllDependencies: bool = ...,
-        CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef = ...
+        CloudFormationOverridePropertyConfiguration: Union[
+            AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+            AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
+        ] = ...
     ) -> StartAssetBundleExportJobResponseTypeDef:
         """
         Starts an Asset Bundle export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_asset_bundle_export_job)
         """
 
     def start_asset_bundle_import_job(
         self,
         *,
         AwsAccountId: str,
         AssetBundleImportJobId: str,
         AssetBundleImportSource: AssetBundleImportSourceTypeDef,
-        OverrideParameters: AssetBundleImportJobOverrideParametersTypeDef = ...,
+        OverrideParameters: Union[
+            AssetBundleImportJobOverrideParametersTypeDef,
+            AssetBundleImportJobOverrideParametersOutputTypeDef,
+        ] = ...,
         FailureAction: AssetBundleImportFailureActionType = ...
     ) -> StartAssetBundleImportJobResponseTypeDef:
         """
         Starts an Asset Bundle import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_asset_bundle_import_job)
@@ -1923,15 +1977,17 @@
     def start_dashboard_snapshot_job(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         SnapshotJobId: str,
         UserConfiguration: SnapshotUserConfigurationTypeDef,
-        SnapshotConfiguration: SnapshotConfigurationTypeDef
+        SnapshotConfiguration: Union[
+            SnapshotConfigurationTypeDef, SnapshotConfigurationOutputTypeDef
+        ]
     ) -> StartDashboardSnapshotJobResponseTypeDef:
         """
         Starts an asynchronous job that generates a dashboard snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_dashboard_snapshot_job)
         """
@@ -1989,34 +2045,38 @@
 
     def update_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
+        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: AnalysisDefinitionTypeDef = ...
+        Definition: Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef] = ...
     ) -> UpdateAnalysisResponseTypeDef:
         """
         Updates an analysis in Amazon QuickSight See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/quicksight-2018-04-01/UpdateAnalysis).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_analysis)
         """
 
     def update_analysis_permissions(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateAnalysisPermissionsResponseTypeDef:
         """
         Updates the read and write permissions for an analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_analysis_permissions)
         """
@@ -2024,36 +2084,46 @@
     def update_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
-        Parameters: ParametersTypeDef = ...,
+        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: DashboardVersionDefinitionTypeDef = ...
+        Definition: Union[
+            DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
+        ] = ...
     ) -> UpdateDashboardResponseTypeDef:
         """
         Updates a dashboard in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard)
         """
 
     def update_dashboard_permissions(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        GrantLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokeLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        GrantLinkPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokeLinkPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateDashboardPermissionsResponseTypeDef:
         """
         Updates read and write permissions on a dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard_permissions)
         """
@@ -2070,39 +2140,50 @@
 
     def update_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],
+        PhysicalTableMap: Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,
-        ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,
-        FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,
+        LogicalTableMap: Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]] = ...,
+        ColumnGroups: Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]] = ...,
+        FieldFolders: Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
-        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
+        RowLevelPermissionTagConfiguration: Union[
+            RowLevelPermissionTagConfigurationTypeDef,
+            RowLevelPermissionTagConfigurationOutputTypeDef,
+        ] = ...,
+        ColumnLevelPermissionRules: Sequence[
+            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
+        ] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...
+        DatasetParameters: Sequence[
+            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+        ] = ...
     ) -> UpdateDataSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set)
         """
 
     def update_data_set_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateDataSetPermissionsResponseTypeDef:
         """
         Updates the permissions on a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set_permissions)
         """
@@ -2126,16 +2207,20 @@
         """
 
     def update_data_source_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateDataSourcePermissionsResponseTypeDef:
         """
         Updates the permissions to a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_source_permissions)
         """
@@ -2151,16 +2236,20 @@
         """
 
     def update_folder_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateFolderPermissionsResponseTypeDef:
         """
         Updates permissions of a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_folder_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_folder_permissions)
         """
@@ -2214,15 +2303,19 @@
         public sharing settings of an Amazon QuickSight dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_public_sharing_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_public_sharing_settings)
         """
 
     def update_refresh_schedule(
-        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleTypeDef
+        self,
+        *,
+        DataSetId: str,
+        AwsAccountId: str,
+        Schedule: Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
     ) -> UpdateRefreshScheduleResponseTypeDef:
         """
         Updates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_refresh_schedule)
         """
@@ -2231,15 +2324,17 @@
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         VersionDescription: str = ...,
         Name: str = ...,
-        Definition: TemplateVersionDefinitionTypeDef = ...
+        Definition: Union[
+            TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
+        ] = ...
     ) -> UpdateTemplateResponseTypeDef:
         """
         Updates a template from an existing Amazon QuickSight analysis or another
         template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template)
@@ -2256,16 +2351,20 @@
         """
 
     def update_template_permissions(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateTemplatePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template_permissions)
         """
@@ -2274,15 +2373,15 @@
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         BaseThemeId: str,
         Name: str = ...,
         VersionDescription: str = ...,
-        Configuration: ThemeConfigurationTypeDef = ...
+        Configuration: Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef] = ...
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme)
         """
@@ -2298,56 +2397,68 @@
         """
 
     def update_theme_permissions(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateThemePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme_permissions)
         """
 
     def update_topic(
-        self, *, AwsAccountId: str, TopicId: str, Topic: TopicDetailsTypeDef
+        self,
+        *,
+        AwsAccountId: str,
+        TopicId: str,
+        Topic: Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef]
     ) -> UpdateTopicResponseTypeDef:
         """
         Updates a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic)
         """
 
     def update_topic_permissions(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateTopicPermissionsResponseTypeDef:
         """
         Updates the permissions of a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_permissions)
         """
 
     def update_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetId: str,
-        RefreshSchedule: TopicRefreshScheduleTypeDef
+        RefreshSchedule: Union[TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef]
     ) -> UpdateTopicRefreshScheduleResponseTypeDef:
         """
         Updates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_refresh_schedule)
         """
```

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/client.pyi` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_quicksight.client import QuickSightClient
 
     session = Session()
     client: QuickSightClient = session.client("quicksight")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssetBundleExportFormatType,
     AssetBundleImportFailureActionType,
     AssignmentStatusType,
@@ -58,23 +58,28 @@
     SearchDashboardsPaginator,
     SearchDataSetsPaginator,
     SearchDataSourcesPaginator,
     SearchGroupsPaginator,
 )
 from .type_defs import (
     AccountCustomizationTypeDef,
+    AnalysisDefinitionOutputTypeDef,
     AnalysisDefinitionTypeDef,
     AnalysisSearchFilterTypeDef,
     AnalysisSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
     AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+    AssetBundleImportJobOverrideParametersOutputTypeDef,
     AssetBundleImportJobOverrideParametersTypeDef,
     AssetBundleImportSourceTypeDef,
     CancelIngestionResponseTypeDef,
+    ColumnGroupOutputTypeDef,
     ColumnGroupTypeDef,
+    ColumnLevelPermissionRuleOutputTypeDef,
     ColumnLevelPermissionRuleTypeDef,
     CreateAccountCustomizationResponseTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
     CreateAnalysisResponseTypeDef,
     CreateDashboardResponseTypeDef,
     CreateDataSetResponseTypeDef,
     CreateDataSourceResponseTypeDef,
@@ -92,15 +97,17 @@
     CreateThemeResponseTypeDef,
     CreateTopicRefreshScheduleResponseTypeDef,
     CreateTopicResponseTypeDef,
     CreateVPCConnectionResponseTypeDef,
     DashboardPublishOptionsTypeDef,
     DashboardSearchFilterTypeDef,
     DashboardSourceEntityTypeDef,
+    DashboardVersionDefinitionOutputTypeDef,
     DashboardVersionDefinitionTypeDef,
+    DatasetParameterOutputTypeDef,
     DatasetParameterTypeDef,
     DataSetRefreshPropertiesTypeDef,
     DataSetSearchFilterTypeDef,
     DataSetUsageConfigurationTypeDef,
     DataSourceCredentialsTypeDef,
     DataSourceParametersTypeDef,
     DataSourceSearchFilterTypeDef,
@@ -164,14 +171,15 @@
     DescribeThemeResponseTypeDef,
     DescribeTopicPermissionsResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     DescribeTopicResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeVPCConnectionResponseTypeDef,
+    FieldFolderOutputTypeDef,
     FieldFolderTypeDef,
     FolderSearchFilterTypeDef,
     GenerateEmbedUrlForAnonymousUserResponseTypeDef,
     GenerateEmbedUrlForRegisteredUserResponseTypeDef,
     GetDashboardEmbedUrlResponseTypeDef,
     GetSessionEmbedUrlResponseTypeDef,
     GroupSearchFilterTypeDef,
@@ -199,44 +207,55 @@
     ListThemesResponseTypeDef,
     ListThemeVersionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     ListTopicsResponseTypeDef,
     ListUserGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
     ListVPCConnectionsResponseTypeDef,
+    LogicalTableOutputTypeDef,
     LogicalTableTypeDef,
+    ParametersOutputTypeDef,
     ParametersTypeDef,
+    PhysicalTableOutputTypeDef,
     PhysicalTableTypeDef,
     PutDataSetRefreshPropertiesResponseTypeDef,
+    RefreshScheduleOutputTypeDef,
     RefreshScheduleTypeDef,
     RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     RegisterUserResponseTypeDef,
+    ResourcePermissionOutputTypeDef,
     ResourcePermissionTypeDef,
     RestoreAnalysisResponseTypeDef,
     RowLevelPermissionDataSetTypeDef,
+    RowLevelPermissionTagConfigurationOutputTypeDef,
     RowLevelPermissionTagConfigurationTypeDef,
     SearchAnalysesResponseTypeDef,
     SearchDashboardsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     SearchDataSourcesResponseTypeDef,
     SearchFoldersResponseTypeDef,
     SearchGroupsResponseTypeDef,
     SessionTagTypeDef,
+    SnapshotConfigurationOutputTypeDef,
     SnapshotConfigurationTypeDef,
     SnapshotUserConfigurationTypeDef,
     SslPropertiesTypeDef,
     StartAssetBundleExportJobResponseTypeDef,
     StartAssetBundleImportJobResponseTypeDef,
     StartDashboardSnapshotJobResponseTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
     TemplateSourceEntityTypeDef,
+    TemplateVersionDefinitionOutputTypeDef,
     TemplateVersionDefinitionTypeDef,
+    ThemeConfigurationOutputTypeDef,
     ThemeConfigurationTypeDef,
+    TopicDetailsOutputTypeDef,
     TopicDetailsTypeDef,
+    TopicRefreshScheduleOutputTypeDef,
     TopicRefreshScheduleTypeDef,
     UntagResourceResponseTypeDef,
     UpdateAccountCustomizationResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     UpdateAnalysisPermissionsResponseTypeDef,
     UpdateAnalysisResponseTypeDef,
     UpdateDashboardPermissionsResponseTypeDef,
@@ -384,67 +403,82 @@
         """
     def create_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Definition: AnalysisDefinitionTypeDef = ...
+        Definition: Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef] = ...
     ) -> CreateAnalysisResponseTypeDef:
         """
         Creates an analysis in Amazon QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_analysis)
         """
     def create_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: DashboardVersionDefinitionTypeDef = ...
+        Definition: Union[
+            DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
+        ] = ...
     ) -> CreateDashboardResponseTypeDef:
         """
         Creates a dashboard from either a template or directly with a
         `DashboardDefinition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_dashboard)
         """
     def create_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],
+        PhysicalTableMap: Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,
-        ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,
-        FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        LogicalTableMap: Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]] = ...,
+        ColumnGroups: Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]] = ...,
+        FieldFolders: Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
-        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
+        RowLevelPermissionTagConfiguration: Union[
+            RowLevelPermissionTagConfigurationTypeDef,
+            RowLevelPermissionTagConfigurationOutputTypeDef,
+        ] = ...,
+        ColumnLevelPermissionRules: Sequence[
+            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...
+        DatasetParameters: Sequence[
+            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+        ] = ...
     ) -> CreateDataSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_data_set)
         """
@@ -453,15 +487,17 @@
         *,
         AwsAccountId: str,
         DataSourceId: str,
         Name: str,
         Type: DataSourceTypeType,
         DataSourceParameters: DataSourceParametersTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
         SslProperties: SslPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source.
 
@@ -472,15 +508,17 @@
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Name: str = ...,
         FolderType: Literal["SHARED"] = ...,
         ParentFolderArn: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFolderResponseTypeDef:
         """
         Creates an empty shared folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_folder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_folder)
@@ -555,33 +593,41 @@
         (Enterprise edition only) Creates a new namespace for you to use with Amazon
         QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_namespace)
         """
     def create_refresh_schedule(
-        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleTypeDef
+        self,
+        *,
+        DataSetId: str,
+        AwsAccountId: str,
+        Schedule: Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
     ) -> CreateRefreshScheduleResponseTypeDef:
         """
         Creates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_refresh_schedule)
         """
     def create_template(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         Name: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
-        Definition: TemplateVersionDefinitionTypeDef = ...
+        Definition: Union[
+            TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
+        ] = ...
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template either from a `TemplateDefinition` or from an existing Amazon
         QuickSight analysis or template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_template)
@@ -598,17 +644,19 @@
     def create_theme(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         Name: str,
         BaseThemeId: str,
-        Configuration: ThemeConfigurationTypeDef,
+        Configuration: Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef],
         VersionDescription: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_theme)
@@ -623,30 +671,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_theme_alias)
         """
     def create_topic(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        Topic: TopicDetailsTypeDef,
+        Topic: Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateTopicResponseTypeDef:
         """
         Creates a new Q topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic)
         """
     def create_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetArn: str,
-        RefreshSchedule: TopicRefreshScheduleTypeDef,
+        RefreshSchedule: Union[TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef],
         DatasetName: str = ...
     ) -> CreateTopicRefreshScheduleResponseTypeDef:
         """
         Creates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic_refresh_schedule)
@@ -1756,29 +1804,35 @@
         self,
         *,
         AwsAccountId: str,
         AssetBundleExportJobId: str,
         ResourceArns: Sequence[str],
         ExportFormat: AssetBundleExportFormatType,
         IncludeAllDependencies: bool = ...,
-        CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef = ...
+        CloudFormationOverridePropertyConfiguration: Union[
+            AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+            AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
+        ] = ...
     ) -> StartAssetBundleExportJobResponseTypeDef:
         """
         Starts an Asset Bundle export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_asset_bundle_export_job)
         """
     def start_asset_bundle_import_job(
         self,
         *,
         AwsAccountId: str,
         AssetBundleImportJobId: str,
         AssetBundleImportSource: AssetBundleImportSourceTypeDef,
-        OverrideParameters: AssetBundleImportJobOverrideParametersTypeDef = ...,
+        OverrideParameters: Union[
+            AssetBundleImportJobOverrideParametersTypeDef,
+            AssetBundleImportJobOverrideParametersOutputTypeDef,
+        ] = ...,
         FailureAction: AssetBundleImportFailureActionType = ...
     ) -> StartAssetBundleImportJobResponseTypeDef:
         """
         Starts an Asset Bundle import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_asset_bundle_import_job)
@@ -1786,15 +1840,17 @@
     def start_dashboard_snapshot_job(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         SnapshotJobId: str,
         UserConfiguration: SnapshotUserConfigurationTypeDef,
-        SnapshotConfiguration: SnapshotConfigurationTypeDef
+        SnapshotConfiguration: Union[
+            SnapshotConfigurationTypeDef, SnapshotConfigurationOutputTypeDef
+        ]
     ) -> StartDashboardSnapshotJobResponseTypeDef:
         """
         Starts an asynchronous job that generates a dashboard snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_dashboard_snapshot_job)
         """
@@ -1847,68 +1903,82 @@
         """
     def update_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
+        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: AnalysisDefinitionTypeDef = ...
+        Definition: Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef] = ...
     ) -> UpdateAnalysisResponseTypeDef:
         """
         Updates an analysis in Amazon QuickSight See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/quicksight-2018-04-01/UpdateAnalysis).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_analysis)
         """
     def update_analysis_permissions(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateAnalysisPermissionsResponseTypeDef:
         """
         Updates the read and write permissions for an analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_analysis_permissions)
         """
     def update_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
-        Parameters: ParametersTypeDef = ...,
+        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: DashboardVersionDefinitionTypeDef = ...
+        Definition: Union[
+            DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
+        ] = ...
     ) -> UpdateDashboardResponseTypeDef:
         """
         Updates a dashboard in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard)
         """
     def update_dashboard_permissions(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        GrantLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokeLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        GrantLinkPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokeLinkPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateDashboardPermissionsResponseTypeDef:
         """
         Updates read and write permissions on a dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard_permissions)
         """
@@ -1923,38 +1993,49 @@
         """
     def update_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],
+        PhysicalTableMap: Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,
-        ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,
-        FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,
+        LogicalTableMap: Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]] = ...,
+        ColumnGroups: Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]] = ...,
+        FieldFolders: Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
-        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
+        RowLevelPermissionTagConfiguration: Union[
+            RowLevelPermissionTagConfigurationTypeDef,
+            RowLevelPermissionTagConfigurationOutputTypeDef,
+        ] = ...,
+        ColumnLevelPermissionRules: Sequence[
+            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
+        ] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...
+        DatasetParameters: Sequence[
+            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+        ] = ...
     ) -> UpdateDataSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set)
         """
     def update_data_set_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateDataSetPermissionsResponseTypeDef:
         """
         Updates the permissions on a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set_permissions)
         """
@@ -1976,16 +2057,20 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_source)
         """
     def update_data_source_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateDataSourcePermissionsResponseTypeDef:
         """
         Updates the permissions to a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_source_permissions)
         """
@@ -1999,16 +2084,20 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_folder)
         """
     def update_folder_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateFolderPermissionsResponseTypeDef:
         """
         Updates permissions of a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_folder_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_folder_permissions)
         """
@@ -2057,15 +2146,19 @@
         Use the `UpdatePublicSharingSettings` operation to turn on or turn off the
         public sharing settings of an Amazon QuickSight dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_public_sharing_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_public_sharing_settings)
         """
     def update_refresh_schedule(
-        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleTypeDef
+        self,
+        *,
+        DataSetId: str,
+        AwsAccountId: str,
+        Schedule: Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
     ) -> UpdateRefreshScheduleResponseTypeDef:
         """
         Updates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_refresh_schedule)
         """
@@ -2073,15 +2166,17 @@
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         VersionDescription: str = ...,
         Name: str = ...,
-        Definition: TemplateVersionDefinitionTypeDef = ...
+        Definition: Union[
+            TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
+        ] = ...
     ) -> UpdateTemplateResponseTypeDef:
         """
         Updates a template from an existing Amazon QuickSight analysis or another
         template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template)
@@ -2096,16 +2191,20 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template_alias)
         """
     def update_template_permissions(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateTemplatePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template_permissions)
         """
@@ -2113,15 +2212,15 @@
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         BaseThemeId: str,
         Name: str = ...,
         VersionDescription: str = ...,
-        Configuration: ThemeConfigurationTypeDef = ...
+        Configuration: Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef] = ...
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme)
         """
@@ -2135,53 +2234,65 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme_alias)
         """
     def update_theme_permissions(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateThemePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme_permissions)
         """
     def update_topic(
-        self, *, AwsAccountId: str, TopicId: str, Topic: TopicDetailsTypeDef
+        self,
+        *,
+        AwsAccountId: str,
+        TopicId: str,
+        Topic: Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef]
     ) -> UpdateTopicResponseTypeDef:
         """
         Updates a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic)
         """
     def update_topic_permissions(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...
+        GrantPermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...,
+        RevokePermissions: Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ] = ...
     ) -> UpdateTopicPermissionsResponseTypeDef:
         """
         Updates the permissions of a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_permissions)
         """
     def update_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetId: str,
-        RefreshSchedule: TopicRefreshScheduleTypeDef
+        RefreshSchedule: Union[TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef]
     ) -> UpdateTopicRefreshScheduleResponseTypeDef:
         """
         Updates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_refresh_schedule)
         """
```

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/literals.py` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/literals.pyi` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/paginator.py` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/paginator.pyi` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/type_defs.py` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,16 +302,18 @@
     "ConditionalFormattingSolidColorTypeDef",
     "ConditionalFormattingCustomIconOptionsTypeDef",
     "ConditionalFormattingIconDisplayConfigurationTypeDef",
     "ConditionalFormattingIconSetTypeDef",
     "TagTypeDef",
     "CreateAccountSubscriptionRequestRequestTypeDef",
     "SignupResponseTypeDef",
+    "ResourcePermissionOutputTypeDef",
     "ResourcePermissionTypeDef",
     "DataSetUsageConfigurationTypeDef",
+    "FieldFolderOutputTypeDef",
     "FieldFolderTypeDef",
     "RowLevelPermissionDataSetTypeDef",
     "CreateFolderMembershipRequestRequestTypeDef",
     "FolderMemberTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
     "GroupMemberTypeDef",
     "CreateGroupRequestRequestTypeDef",
@@ -353,15 +355,14 @@
     "DataPathLabelTypeTypeDef",
     "FieldLabelTypeTypeDef",
     "MaximumLabelTypeTypeDef",
     "MinimumLabelTypeTypeDef",
     "RangeEndsLabelTypeTypeDef",
     "DataPathValueTypeDef",
     "DataSetSearchFilterTypeDef",
-    "FieldFolderOutputTypeDef",
     "OutputColumnTypeDef",
     "DataSourceErrorInfoTypeDef",
     "DatabricksParametersTypeDef",
     "ExasolParametersTypeDef",
     "JiraParametersTypeDef",
     "MariaDbParametersTypeDef",
     "MySqlParametersTypeDef",
@@ -416,15 +417,14 @@
     "DeleteUserRequestRequestTypeDef",
     "DeleteVPCConnectionRequestRequestTypeDef",
     "DescribeAccountCustomizationRequestRequestTypeDef",
     "DescribeAccountSettingsRequestRequestTypeDef",
     "DescribeAccountSubscriptionRequestRequestTypeDef",
     "DescribeAnalysisDefinitionRequestRequestTypeDef",
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
-    "ResourcePermissionOutputTypeDef",
     "DescribeAnalysisRequestRequestTypeDef",
     "DescribeAssetBundleExportJobRequestRequestTypeDef",
     "DescribeAssetBundleImportJobRequestRequestTypeDef",
     "DescribeDashboardDefinitionRequestRequestTypeDef",
     "DescribeDashboardPermissionsRequestRequestTypeDef",
     "DescribeDashboardRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobRequestRequestTypeDef",
@@ -768,14 +768,28 @@
     "ConditionalFormattingCustomIconConditionTypeDef",
     "CreateAccountCustomizationRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateVPCConnectionRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAccountSubscriptionResponseTypeDef",
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    "DescribeDataSetPermissionsResponseTypeDef",
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    "DescribeFolderPermissionsResponseTypeDef",
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    "DescribeTemplatePermissionsResponseTypeDef",
+    "DescribeThemePermissionsResponseTypeDef",
+    "DescribeTopicPermissionsResponseTypeDef",
+    "LinkSharingConfigurationTypeDef",
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    "UpdateFolderPermissionsResponseTypeDef",
+    "UpdateTemplatePermissionsResponseTypeDef",
+    "UpdateThemePermissionsResponseTypeDef",
+    "UpdateTopicPermissionsResponseTypeDef",
     "CreateFolderRequestRequestTypeDef",
     "UpdateAnalysisPermissionsRequestRequestTypeDef",
     "UpdateDashboardPermissionsRequestRequestTypeDef",
     "UpdateDataSetPermissionsRequestRequestTypeDef",
     "UpdateDataSourcePermissionsRequestRequestTypeDef",
     "UpdateFolderPermissionsRequestRequestTypeDef",
     "UpdateTemplatePermissionsRequestRequestTypeDef",
@@ -828,28 +842,14 @@
     "SearchDataSourcesResponseTypeDef",
     "DateTimeDatasetParameterOutputTypeDef",
     "DateTimeDatasetParameterTypeDef",
     "TimeRangeFilterValueOutputTypeDef",
     "TimeRangeFilterValueTypeDef",
     "DecimalDatasetParameterOutputTypeDef",
     "DecimalDatasetParameterTypeDef",
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    "DescribeDataSetPermissionsResponseTypeDef",
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    "DescribeFolderPermissionsResponseTypeDef",
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    "DescribeTemplatePermissionsResponseTypeDef",
-    "DescribeThemePermissionsResponseTypeDef",
-    "DescribeTopicPermissionsResponseTypeDef",
-    "LinkSharingConfigurationTypeDef",
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    "UpdateFolderPermissionsResponseTypeDef",
-    "UpdateTemplatePermissionsResponseTypeDef",
-    "UpdateThemePermissionsResponseTypeDef",
-    "UpdateTopicPermissionsResponseTypeDef",
     "DescribeFolderResponseTypeDef",
     "DescribeIAMPolicyAssignmentResponseTypeDef",
     "DescribeTopicRefreshResponseTypeDef",
     "DescribeTopicRefreshScheduleResponseTypeDef",
     "TopicRefreshScheduleSummaryTypeDef",
     "DescribeUserResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -985,27 +985,27 @@
     "TopicCategoryFilterOutputTypeDef",
     "TopicCategoryFilterTypeDef",
     "TagColumnOperationOutputTypeDef",
     "TagColumnOperationTypeDef",
     "DataSetConfigurationOutputTypeDef",
     "DataSetConfigurationTypeDef",
     "ConditionalFormattingIconTypeDef",
+    "DescribeDashboardPermissionsResponseTypeDef",
+    "UpdateDashboardPermissionsResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "SearchDataSetsResponseTypeDef",
     "DestinationParameterValueConfigurationOutputTypeDef",
     "DestinationParameterValueConfigurationTypeDef",
     "DashboardPublishOptionsTypeDef",
     "VisualPaletteOutputTypeDef",
     "VisualPaletteTypeDef",
     "PivotTableFieldCollapseStateOptionOutputTypeDef",
     "PivotTableFieldCollapseStateOptionTypeDef",
     "TimeRangeFilterOutputTypeDef",
     "TimeRangeFilterTypeDef",
-    "DescribeDashboardPermissionsResponseTypeDef",
-    "UpdateDashboardPermissionsResponseTypeDef",
     "ListTopicRefreshSchedulesResponseTypeDef",
     "DefaultFormattingTypeDef",
     "CustomActionFilterOperationOutputTypeDef",
     "CustomActionFilterOperationTypeDef",
     "AxisLabelOptionsTypeDef",
     "DataLabelOptionsOutputTypeDef",
     "DataLabelOptionsTypeDef",
@@ -2951,14 +2951,22 @@
         "userLoginName": str,
         "accountName": str,
         "directoryType": str,
     },
     total=False,
 )
 
+ResourcePermissionOutputTypeDef = TypedDict(
+    "ResourcePermissionOutputTypeDef",
+    {
+        "Principal": str,
+        "Actions": List[str],
+    },
+)
+
 ResourcePermissionTypeDef = TypedDict(
     "ResourcePermissionTypeDef",
     {
         "Principal": str,
         "Actions": Sequence[str],
     },
 )
@@ -2968,14 +2976,23 @@
     {
         "DisableUseAsDirectQuerySource": bool,
         "DisableUseAsImportedSource": bool,
     },
     total=False,
 )
 
+FieldFolderOutputTypeDef = TypedDict(
+    "FieldFolderOutputTypeDef",
+    {
+        "description": str,
+        "columns": List[str],
+    },
+    total=False,
+)
+
 FieldFolderTypeDef = TypedDict(
     "FieldFolderTypeDef",
     {
         "description": str,
         "columns": Sequence[str],
     },
     total=False,
@@ -3508,23 +3525,14 @@
     {
         "Operator": FilterOperatorType,
         "Name": DataSetFilterAttributeType,
         "Value": str,
     },
 )
 
-FieldFolderOutputTypeDef = TypedDict(
-    "FieldFolderOutputTypeDef",
-    {
-        "description": str,
-        "columns": List[str],
-    },
-    total=False,
-)
-
 OutputColumnTypeDef = TypedDict(
     "OutputColumnTypeDef",
     {
         "Name": str,
         "Description": str,
         "Type": ColumnDataTypeType,
     },
@@ -4156,22 +4164,14 @@
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
 
-ResourcePermissionOutputTypeDef = TypedDict(
-    "ResourcePermissionOutputTypeDef",
-    {
-        "Principal": str,
-        "Actions": List[str],
-    },
-)
-
 DescribeAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
@@ -8429,28 +8429,192 @@
         "SignupResponse": SignupResponseTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisId": str,
+        "AnalysisArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDataSetPermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSetPermissionsResponseTypeDef",
+    {
+        "DataSetArn": str,
+        "DataSetId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    {
+        "DataSourceArn": str,
+        "DataSourceId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFolderPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "FolderId": str,
+        "Arn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "FolderId": str,
+        "Arn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTemplatePermissionsResponseTypeDef = TypedDict(
+    "DescribeTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThemePermissionsResponseTypeDef = TypedDict(
+    "DescribeThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTopicPermissionsResponseTypeDef = TypedDict(
+    "DescribeTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LinkSharingConfigurationTypeDef = TypedDict(
+    "LinkSharingConfigurationTypeDef",
+    {
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+    },
+    total=False,
+)
+
+UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisArn": str,
+        "AnalysisId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFolderPermissionsResponseTypeDef = TypedDict(
+    "UpdateFolderPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "Arn": str,
+        "FolderId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTemplatePermissionsResponseTypeDef = TypedDict(
+    "UpdateTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateThemePermissionsResponseTypeDef = TypedDict(
+    "UpdateThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTopicPermissionsResponseTypeDef = TypedDict(
+    "UpdateTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFolderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFolderRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "FolderId": str,
     },
 )
 _OptionalCreateFolderRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFolderRequestRequestTypeDef",
     {
         "Name": str,
         "FolderType": Literal["SHARED"],
         "ParentFolderArn": str,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class CreateFolderRequestRequestTypeDef(
@@ -8465,16 +8629,20 @@
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
 _OptionalUpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAnalysisPermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateAnalysisPermissionsRequestRequestTypeDef(
     _RequiredUpdateAnalysisPermissionsRequestRequestTypeDef,
@@ -8489,18 +8657,26 @@
         "AwsAccountId": str,
         "DashboardId": str,
     },
 )
 _OptionalUpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDashboardPermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
-        "GrantLinkPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokeLinkPermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "GrantLinkPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokeLinkPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateDashboardPermissionsRequestRequestTypeDef(
     _RequiredUpdateDashboardPermissionsRequestRequestTypeDef,
@@ -8515,16 +8691,20 @@
         "AwsAccountId": str,
         "DataSetId": str,
     },
 )
 _OptionalUpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDataSetPermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateDataSetPermissionsRequestRequestTypeDef(
     _RequiredUpdateDataSetPermissionsRequestRequestTypeDef,
@@ -8539,16 +8719,20 @@
         "AwsAccountId": str,
         "DataSourceId": str,
     },
 )
 _OptionalUpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDataSourcePermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateDataSourcePermissionsRequestRequestTypeDef(
     _RequiredUpdateDataSourcePermissionsRequestRequestTypeDef,
@@ -8563,16 +8747,20 @@
         "AwsAccountId": str,
         "FolderId": str,
     },
 )
 _OptionalUpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFolderPermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateFolderPermissionsRequestRequestTypeDef(
     _RequiredUpdateFolderPermissionsRequestRequestTypeDef,
@@ -8587,16 +8775,20 @@
         "AwsAccountId": str,
         "TemplateId": str,
     },
 )
 _OptionalUpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTemplatePermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateTemplatePermissionsRequestRequestTypeDef(
     _RequiredUpdateTemplatePermissionsRequestRequestTypeDef,
@@ -8611,16 +8803,20 @@
         "AwsAccountId": str,
         "ThemeId": str,
     },
 )
 _OptionalUpdateThemePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateThemePermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateThemePermissionsRequestRequestTypeDef(
     _RequiredUpdateThemePermissionsRequestRequestTypeDef,
@@ -8635,16 +8831,20 @@
         "AwsAccountId": str,
         "TopicId": str,
     },
 )
 _OptionalUpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTopicPermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateTopicPermissionsRequestRequestTypeDef(
     _RequiredUpdateTopicPermissionsRequestRequestTypeDef,
@@ -9375,178 +9575,14 @@
 
 class DecimalDatasetParameterTypeDef(
     _RequiredDecimalDatasetParameterTypeDef, _OptionalDecimalDatasetParameterTypeDef
 ):
     pass
 
 
-DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisId": str,
-        "AnalysisArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDataSetPermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSetPermissionsResponseTypeDef",
-    {
-        "DataSetArn": str,
-        "DataSetId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    {
-        "DataSourceArn": str,
-        "DataSourceId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFolderPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTemplatePermissionsResponseTypeDef = TypedDict(
-    "DescribeTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeThemePermissionsResponseTypeDef = TypedDict(
-    "DescribeThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTopicPermissionsResponseTypeDef = TypedDict(
-    "DescribeTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LinkSharingConfigurationTypeDef = TypedDict(
-    "LinkSharingConfigurationTypeDef",
-    {
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-    },
-    total=False,
-)
-
-UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisArn": str,
-        "AnalysisId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFolderPermissionsResponseTypeDef = TypedDict(
-    "UpdateFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "Arn": str,
-        "FolderId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTemplatePermissionsResponseTypeDef = TypedDict(
-    "UpdateTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateThemePermissionsResponseTypeDef = TypedDict(
-    "UpdateThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTopicPermissionsResponseTypeDef = TypedDict(
-    "UpdateTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeFolderResponseTypeDef = TypedDict(
     "DescribeFolderResponseTypeDef",
     {
         "Status": int,
         "Folder": FolderTypeDef,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11525,14 +11561,40 @@
     {
         "IconSet": ConditionalFormattingIconSetTypeDef,
         "CustomCondition": ConditionalFormattingCustomIconConditionTypeDef,
     },
     total=False,
 )
 
+DescribeDashboardPermissionsResponseTypeDef = TypedDict(
+    "DescribeDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardId": str,
+        "DashboardArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDashboardPermissionsResponseTypeDef = TypedDict(
+    "UpdateDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "DataSetSummaries": List[DataSetSummaryTypeDef],
         "NextToken": str,
         "RequestId": str,
         "Status": int,
@@ -11705,40 +11767,14 @@
 )
 
 
 class TimeRangeFilterTypeDef(_RequiredTimeRangeFilterTypeDef, _OptionalTimeRangeFilterTypeDef):
     pass
 
 
-DescribeDashboardPermissionsResponseTypeDef = TypedDict(
-    "DescribeDashboardPermissionsResponseTypeDef",
-    {
-        "DashboardId": str,
-        "DashboardArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDashboardPermissionsResponseTypeDef = TypedDict(
-    "UpdateDashboardPermissionsResponseTypeDef",
-    {
-        "DashboardArn": str,
-        "DashboardId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTopicRefreshSchedulesResponseTypeDef = TypedDict(
     "ListTopicRefreshSchedulesResponseTypeDef",
     {
         "TopicId": str,
         "TopicArn": str,
         "RefreshSchedules": List[TopicRefreshScheduleSummaryTypeDef],
         "Status": int,
@@ -14797,15 +14833,15 @@
         "Configuration": ThemeConfigurationTypeDef,
     },
 )
 _OptionalCreateThemeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateThemeRequestRequestTypeDef",
     {
         "VersionDescription": str,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class CreateThemeRequestRequestTypeDef(
@@ -15142,31 +15178,35 @@
 
 _RequiredCreateDataSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSetRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DataSetId": str,
         "Name": str,
-        "PhysicalTableMap": Mapping[str, PhysicalTableTypeDef],
+        "PhysicalTableMap": Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
         "ImportMode": DataSetImportModeType,
     },
 )
 _OptionalCreateDataSetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDataSetRequestRequestTypeDef",
     {
-        "LogicalTableMap": Mapping[str, LogicalTableTypeDef],
-        "ColumnGroups": Sequence[ColumnGroupTypeDef],
-        "FieldFolders": Mapping[str, FieldFolderTypeDef],
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "LogicalTableMap": Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]],
+        "ColumnGroups": Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]],
+        "FieldFolders": Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
         "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
-        "ColumnLevelPermissionRules": Sequence[ColumnLevelPermissionRuleTypeDef],
+        "ColumnLevelPermissionRules": Sequence[
+            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
+        ],
         "Tags": Sequence[TagTypeDef],
         "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
-        "DatasetParameters": Sequence[DatasetParameterTypeDef],
+        "DatasetParameters": Sequence[
+            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class CreateDataSetRequestRequestTypeDef(
     _RequiredCreateDataSetRequestRequestTypeDef, _OptionalCreateDataSetRequestRequestTypeDef
@@ -15176,29 +15216,33 @@
 
 _RequiredUpdateDataSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSetRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DataSetId": str,
         "Name": str,
-        "PhysicalTableMap": Mapping[str, PhysicalTableTypeDef],
+        "PhysicalTableMap": Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
         "ImportMode": DataSetImportModeType,
     },
 )
 _OptionalUpdateDataSetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDataSetRequestRequestTypeDef",
     {
-        "LogicalTableMap": Mapping[str, LogicalTableTypeDef],
-        "ColumnGroups": Sequence[ColumnGroupTypeDef],
-        "FieldFolders": Mapping[str, FieldFolderTypeDef],
+        "LogicalTableMap": Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]],
+        "ColumnGroups": Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]],
+        "FieldFolders": Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]],
         "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
         "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
-        "ColumnLevelPermissionRules": Sequence[ColumnLevelPermissionRuleTypeDef],
+        "ColumnLevelPermissionRules": Sequence[
+            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
+        ],
         "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
-        "DatasetParameters": Sequence[DatasetParameterTypeDef],
+        "DatasetParameters": Sequence[
+            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateDataSetRequestRequestTypeDef(
     _RequiredUpdateDataSetRequestRequestTypeDef, _OptionalUpdateDataSetRequestRequestTypeDef
@@ -15566,15 +15610,15 @@
     },
 )
 _OptionalCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDataSourceRequestRequestTypeDef",
     {
         "DataSourceParameters": DataSourceParametersTypeDef,
         "Credentials": DataSourceCredentialsTypeDef,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "VpcConnectionProperties": VpcConnectionPropertiesTypeDef,
         "SslProperties": SslPropertiesTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
@@ -19950,15 +19994,15 @@
         "Name": str,
     },
 )
 _OptionalCreateAnalysisRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAnalysisRequestRequestTypeDef",
     {
         "Parameters": ParametersTypeDef,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "SourceEntity": AnalysisSourceEntityTypeDef,
         "ThemeArn": str,
         "Tags": Sequence[TagTypeDef],
         "Definition": AnalysisDefinitionTypeDef,
     },
     total=False,
 )
@@ -20004,15 +20048,15 @@
         "Name": str,
     },
 )
 _OptionalCreateDashboardRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDashboardRequestRequestTypeDef",
     {
         "Parameters": ParametersTypeDef,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "SourceEntity": DashboardSourceEntityTypeDef,
         "Tags": Sequence[TagTypeDef],
         "VersionDescription": str,
         "DashboardPublishOptions": DashboardPublishOptionsTypeDef,
         "ThemeArn": str,
         "Definition": DashboardVersionDefinitionTypeDef,
     },
@@ -20061,15 +20105,15 @@
         "TemplateId": str,
     },
 )
 _OptionalCreateTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTemplateRequestRequestTypeDef",
     {
         "Name": str,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "SourceEntity": TemplateSourceEntityTypeDef,
         "Tags": Sequence[TagTypeDef],
         "VersionDescription": str,
         "Definition": TemplateVersionDefinitionTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/type_defs.pyi` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -301,16 +301,18 @@
     "ConditionalFormattingSolidColorTypeDef",
     "ConditionalFormattingCustomIconOptionsTypeDef",
     "ConditionalFormattingIconDisplayConfigurationTypeDef",
     "ConditionalFormattingIconSetTypeDef",
     "TagTypeDef",
     "CreateAccountSubscriptionRequestRequestTypeDef",
     "SignupResponseTypeDef",
+    "ResourcePermissionOutputTypeDef",
     "ResourcePermissionTypeDef",
     "DataSetUsageConfigurationTypeDef",
+    "FieldFolderOutputTypeDef",
     "FieldFolderTypeDef",
     "RowLevelPermissionDataSetTypeDef",
     "CreateFolderMembershipRequestRequestTypeDef",
     "FolderMemberTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
     "GroupMemberTypeDef",
     "CreateGroupRequestRequestTypeDef",
@@ -352,15 +354,14 @@
     "DataPathLabelTypeTypeDef",
     "FieldLabelTypeTypeDef",
     "MaximumLabelTypeTypeDef",
     "MinimumLabelTypeTypeDef",
     "RangeEndsLabelTypeTypeDef",
     "DataPathValueTypeDef",
     "DataSetSearchFilterTypeDef",
-    "FieldFolderOutputTypeDef",
     "OutputColumnTypeDef",
     "DataSourceErrorInfoTypeDef",
     "DatabricksParametersTypeDef",
     "ExasolParametersTypeDef",
     "JiraParametersTypeDef",
     "MariaDbParametersTypeDef",
     "MySqlParametersTypeDef",
@@ -415,15 +416,14 @@
     "DeleteUserRequestRequestTypeDef",
     "DeleteVPCConnectionRequestRequestTypeDef",
     "DescribeAccountCustomizationRequestRequestTypeDef",
     "DescribeAccountSettingsRequestRequestTypeDef",
     "DescribeAccountSubscriptionRequestRequestTypeDef",
     "DescribeAnalysisDefinitionRequestRequestTypeDef",
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
-    "ResourcePermissionOutputTypeDef",
     "DescribeAnalysisRequestRequestTypeDef",
     "DescribeAssetBundleExportJobRequestRequestTypeDef",
     "DescribeAssetBundleImportJobRequestRequestTypeDef",
     "DescribeDashboardDefinitionRequestRequestTypeDef",
     "DescribeDashboardPermissionsRequestRequestTypeDef",
     "DescribeDashboardRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobRequestRequestTypeDef",
@@ -767,14 +767,28 @@
     "ConditionalFormattingCustomIconConditionTypeDef",
     "CreateAccountCustomizationRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateVPCConnectionRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAccountSubscriptionResponseTypeDef",
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    "DescribeDataSetPermissionsResponseTypeDef",
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    "DescribeFolderPermissionsResponseTypeDef",
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    "DescribeTemplatePermissionsResponseTypeDef",
+    "DescribeThemePermissionsResponseTypeDef",
+    "DescribeTopicPermissionsResponseTypeDef",
+    "LinkSharingConfigurationTypeDef",
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    "UpdateFolderPermissionsResponseTypeDef",
+    "UpdateTemplatePermissionsResponseTypeDef",
+    "UpdateThemePermissionsResponseTypeDef",
+    "UpdateTopicPermissionsResponseTypeDef",
     "CreateFolderRequestRequestTypeDef",
     "UpdateAnalysisPermissionsRequestRequestTypeDef",
     "UpdateDashboardPermissionsRequestRequestTypeDef",
     "UpdateDataSetPermissionsRequestRequestTypeDef",
     "UpdateDataSourcePermissionsRequestRequestTypeDef",
     "UpdateFolderPermissionsRequestRequestTypeDef",
     "UpdateTemplatePermissionsRequestRequestTypeDef",
@@ -827,28 +841,14 @@
     "SearchDataSourcesResponseTypeDef",
     "DateTimeDatasetParameterOutputTypeDef",
     "DateTimeDatasetParameterTypeDef",
     "TimeRangeFilterValueOutputTypeDef",
     "TimeRangeFilterValueTypeDef",
     "DecimalDatasetParameterOutputTypeDef",
     "DecimalDatasetParameterTypeDef",
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    "DescribeDataSetPermissionsResponseTypeDef",
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    "DescribeFolderPermissionsResponseTypeDef",
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    "DescribeTemplatePermissionsResponseTypeDef",
-    "DescribeThemePermissionsResponseTypeDef",
-    "DescribeTopicPermissionsResponseTypeDef",
-    "LinkSharingConfigurationTypeDef",
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    "UpdateFolderPermissionsResponseTypeDef",
-    "UpdateTemplatePermissionsResponseTypeDef",
-    "UpdateThemePermissionsResponseTypeDef",
-    "UpdateTopicPermissionsResponseTypeDef",
     "DescribeFolderResponseTypeDef",
     "DescribeIAMPolicyAssignmentResponseTypeDef",
     "DescribeTopicRefreshResponseTypeDef",
     "DescribeTopicRefreshScheduleResponseTypeDef",
     "TopicRefreshScheduleSummaryTypeDef",
     "DescribeUserResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -984,27 +984,27 @@
     "TopicCategoryFilterOutputTypeDef",
     "TopicCategoryFilterTypeDef",
     "TagColumnOperationOutputTypeDef",
     "TagColumnOperationTypeDef",
     "DataSetConfigurationOutputTypeDef",
     "DataSetConfigurationTypeDef",
     "ConditionalFormattingIconTypeDef",
+    "DescribeDashboardPermissionsResponseTypeDef",
+    "UpdateDashboardPermissionsResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "SearchDataSetsResponseTypeDef",
     "DestinationParameterValueConfigurationOutputTypeDef",
     "DestinationParameterValueConfigurationTypeDef",
     "DashboardPublishOptionsTypeDef",
     "VisualPaletteOutputTypeDef",
     "VisualPaletteTypeDef",
     "PivotTableFieldCollapseStateOptionOutputTypeDef",
     "PivotTableFieldCollapseStateOptionTypeDef",
     "TimeRangeFilterOutputTypeDef",
     "TimeRangeFilterTypeDef",
-    "DescribeDashboardPermissionsResponseTypeDef",
-    "UpdateDashboardPermissionsResponseTypeDef",
     "ListTopicRefreshSchedulesResponseTypeDef",
     "DefaultFormattingTypeDef",
     "CustomActionFilterOperationOutputTypeDef",
     "CustomActionFilterOperationTypeDef",
     "AxisLabelOptionsTypeDef",
     "DataLabelOptionsOutputTypeDef",
     "DataLabelOptionsTypeDef",
@@ -2882,14 +2882,22 @@
         "userLoginName": str,
         "accountName": str,
         "directoryType": str,
     },
     total=False,
 )
 
+ResourcePermissionOutputTypeDef = TypedDict(
+    "ResourcePermissionOutputTypeDef",
+    {
+        "Principal": str,
+        "Actions": List[str],
+    },
+)
+
 ResourcePermissionTypeDef = TypedDict(
     "ResourcePermissionTypeDef",
     {
         "Principal": str,
         "Actions": Sequence[str],
     },
 )
@@ -2899,14 +2907,23 @@
     {
         "DisableUseAsDirectQuerySource": bool,
         "DisableUseAsImportedSource": bool,
     },
     total=False,
 )
 
+FieldFolderOutputTypeDef = TypedDict(
+    "FieldFolderOutputTypeDef",
+    {
+        "description": str,
+        "columns": List[str],
+    },
+    total=False,
+)
+
 FieldFolderTypeDef = TypedDict(
     "FieldFolderTypeDef",
     {
         "description": str,
         "columns": Sequence[str],
     },
     total=False,
@@ -3425,23 +3442,14 @@
     {
         "Operator": FilterOperatorType,
         "Name": DataSetFilterAttributeType,
         "Value": str,
     },
 )
 
-FieldFolderOutputTypeDef = TypedDict(
-    "FieldFolderOutputTypeDef",
-    {
-        "description": str,
-        "columns": List[str],
-    },
-    total=False,
-)
-
 OutputColumnTypeDef = TypedDict(
     "OutputColumnTypeDef",
     {
         "Name": str,
         "Description": str,
         "Type": ColumnDataTypeType,
     },
@@ -4057,22 +4065,14 @@
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
 
-ResourcePermissionOutputTypeDef = TypedDict(
-    "ResourcePermissionOutputTypeDef",
-    {
-        "Principal": str,
-        "Actions": List[str],
-    },
-)
-
 DescribeAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
@@ -8202,28 +8202,192 @@
         "SignupResponse": SignupResponseTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisId": str,
+        "AnalysisArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDataSetPermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSetPermissionsResponseTypeDef",
+    {
+        "DataSetArn": str,
+        "DataSetId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    {
+        "DataSourceArn": str,
+        "DataSourceId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFolderPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "FolderId": str,
+        "Arn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "FolderId": str,
+        "Arn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTemplatePermissionsResponseTypeDef = TypedDict(
+    "DescribeTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThemePermissionsResponseTypeDef = TypedDict(
+    "DescribeThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTopicPermissionsResponseTypeDef = TypedDict(
+    "DescribeTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LinkSharingConfigurationTypeDef = TypedDict(
+    "LinkSharingConfigurationTypeDef",
+    {
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+    },
+    total=False,
+)
+
+UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisArn": str,
+        "AnalysisId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFolderPermissionsResponseTypeDef = TypedDict(
+    "UpdateFolderPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "Arn": str,
+        "FolderId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTemplatePermissionsResponseTypeDef = TypedDict(
+    "UpdateTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateThemePermissionsResponseTypeDef = TypedDict(
+    "UpdateThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTopicPermissionsResponseTypeDef = TypedDict(
+    "UpdateTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFolderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFolderRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "FolderId": str,
     },
 )
 _OptionalCreateFolderRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFolderRequestRequestTypeDef",
     {
         "Name": str,
         "FolderType": Literal["SHARED"],
         "ParentFolderArn": str,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateFolderRequestRequestTypeDef(
     _RequiredCreateFolderRequestRequestTypeDef, _OptionalCreateFolderRequestRequestTypeDef
@@ -8236,16 +8400,20 @@
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
 _OptionalUpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAnalysisPermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateAnalysisPermissionsRequestRequestTypeDef(
     _RequiredUpdateAnalysisPermissionsRequestRequestTypeDef,
     _OptionalUpdateAnalysisPermissionsRequestRequestTypeDef,
@@ -8258,18 +8426,26 @@
         "AwsAccountId": str,
         "DashboardId": str,
     },
 )
 _OptionalUpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDashboardPermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
-        "GrantLinkPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokeLinkPermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "GrantLinkPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokeLinkPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateDashboardPermissionsRequestRequestTypeDef(
     _RequiredUpdateDashboardPermissionsRequestRequestTypeDef,
     _OptionalUpdateDashboardPermissionsRequestRequestTypeDef,
@@ -8282,16 +8458,20 @@
         "AwsAccountId": str,
         "DataSetId": str,
     },
 )
 _OptionalUpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDataSetPermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateDataSetPermissionsRequestRequestTypeDef(
     _RequiredUpdateDataSetPermissionsRequestRequestTypeDef,
     _OptionalUpdateDataSetPermissionsRequestRequestTypeDef,
@@ -8304,16 +8484,20 @@
         "AwsAccountId": str,
         "DataSourceId": str,
     },
 )
 _OptionalUpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDataSourcePermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateDataSourcePermissionsRequestRequestTypeDef(
     _RequiredUpdateDataSourcePermissionsRequestRequestTypeDef,
     _OptionalUpdateDataSourcePermissionsRequestRequestTypeDef,
@@ -8326,16 +8510,20 @@
         "AwsAccountId": str,
         "FolderId": str,
     },
 )
 _OptionalUpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFolderPermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateFolderPermissionsRequestRequestTypeDef(
     _RequiredUpdateFolderPermissionsRequestRequestTypeDef,
     _OptionalUpdateFolderPermissionsRequestRequestTypeDef,
@@ -8348,16 +8536,20 @@
         "AwsAccountId": str,
         "TemplateId": str,
     },
 )
 _OptionalUpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTemplatePermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateTemplatePermissionsRequestRequestTypeDef(
     _RequiredUpdateTemplatePermissionsRequestRequestTypeDef,
     _OptionalUpdateTemplatePermissionsRequestRequestTypeDef,
@@ -8370,16 +8562,20 @@
         "AwsAccountId": str,
         "ThemeId": str,
     },
 )
 _OptionalUpdateThemePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateThemePermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateThemePermissionsRequestRequestTypeDef(
     _RequiredUpdateThemePermissionsRequestRequestTypeDef,
     _OptionalUpdateThemePermissionsRequestRequestTypeDef,
@@ -8392,16 +8588,20 @@
         "AwsAccountId": str,
         "TopicId": str,
     },
 )
 _OptionalUpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTopicPermissionsRequestRequestTypeDef",
     {
-        "GrantPermissions": Sequence[ResourcePermissionTypeDef],
-        "RevokePermissions": Sequence[ResourcePermissionTypeDef],
+        "GrantPermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
+        "RevokePermissions": Sequence[
+            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateTopicPermissionsRequestRequestTypeDef(
     _RequiredUpdateTopicPermissionsRequestRequestTypeDef,
     _OptionalUpdateTopicPermissionsRequestRequestTypeDef,
@@ -9096,178 +9296,14 @@
 )
 
 class DecimalDatasetParameterTypeDef(
     _RequiredDecimalDatasetParameterTypeDef, _OptionalDecimalDatasetParameterTypeDef
 ):
     pass
 
-DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisId": str,
-        "AnalysisArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDataSetPermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSetPermissionsResponseTypeDef",
-    {
-        "DataSetArn": str,
-        "DataSetId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    {
-        "DataSourceArn": str,
-        "DataSourceId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFolderPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTemplatePermissionsResponseTypeDef = TypedDict(
-    "DescribeTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeThemePermissionsResponseTypeDef = TypedDict(
-    "DescribeThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTopicPermissionsResponseTypeDef = TypedDict(
-    "DescribeTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LinkSharingConfigurationTypeDef = TypedDict(
-    "LinkSharingConfigurationTypeDef",
-    {
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-    },
-    total=False,
-)
-
-UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisArn": str,
-        "AnalysisId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFolderPermissionsResponseTypeDef = TypedDict(
-    "UpdateFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "Arn": str,
-        "FolderId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTemplatePermissionsResponseTypeDef = TypedDict(
-    "UpdateTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateThemePermissionsResponseTypeDef = TypedDict(
-    "UpdateThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTopicPermissionsResponseTypeDef = TypedDict(
-    "UpdateTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeFolderResponseTypeDef = TypedDict(
     "DescribeFolderResponseTypeDef",
     {
         "Status": int,
         "Folder": FolderTypeDef,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11160,14 +11196,40 @@
     {
         "IconSet": ConditionalFormattingIconSetTypeDef,
         "CustomCondition": ConditionalFormattingCustomIconConditionTypeDef,
     },
     total=False,
 )
 
+DescribeDashboardPermissionsResponseTypeDef = TypedDict(
+    "DescribeDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardId": str,
+        "DashboardArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDashboardPermissionsResponseTypeDef = TypedDict(
+    "UpdateDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "DataSetSummaries": List[DataSetSummaryTypeDef],
         "NextToken": str,
         "RequestId": str,
         "Status": int,
@@ -11332,40 +11394,14 @@
     },
     total=False,
 )
 
 class TimeRangeFilterTypeDef(_RequiredTimeRangeFilterTypeDef, _OptionalTimeRangeFilterTypeDef):
     pass
 
-DescribeDashboardPermissionsResponseTypeDef = TypedDict(
-    "DescribeDashboardPermissionsResponseTypeDef",
-    {
-        "DashboardId": str,
-        "DashboardArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDashboardPermissionsResponseTypeDef = TypedDict(
-    "UpdateDashboardPermissionsResponseTypeDef",
-    {
-        "DashboardArn": str,
-        "DashboardId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTopicRefreshSchedulesResponseTypeDef = TypedDict(
     "ListTopicRefreshSchedulesResponseTypeDef",
     {
         "TopicId": str,
         "TopicArn": str,
         "RefreshSchedules": List[TopicRefreshScheduleSummaryTypeDef],
         "Status": int,
@@ -14296,15 +14332,15 @@
         "Configuration": ThemeConfigurationTypeDef,
     },
 )
 _OptionalCreateThemeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateThemeRequestRequestTypeDef",
     {
         "VersionDescription": str,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateThemeRequestRequestTypeDef(
     _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
@@ -14627,31 +14663,35 @@
 
 _RequiredCreateDataSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSetRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DataSetId": str,
         "Name": str,
-        "PhysicalTableMap": Mapping[str, PhysicalTableTypeDef],
+        "PhysicalTableMap": Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
         "ImportMode": DataSetImportModeType,
     },
 )
 _OptionalCreateDataSetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDataSetRequestRequestTypeDef",
     {
-        "LogicalTableMap": Mapping[str, LogicalTableTypeDef],
-        "ColumnGroups": Sequence[ColumnGroupTypeDef],
-        "FieldFolders": Mapping[str, FieldFolderTypeDef],
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "LogicalTableMap": Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]],
+        "ColumnGroups": Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]],
+        "FieldFolders": Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
         "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
-        "ColumnLevelPermissionRules": Sequence[ColumnLevelPermissionRuleTypeDef],
+        "ColumnLevelPermissionRules": Sequence[
+            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
+        ],
         "Tags": Sequence[TagTypeDef],
         "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
-        "DatasetParameters": Sequence[DatasetParameterTypeDef],
+        "DatasetParameters": Sequence[
+            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class CreateDataSetRequestRequestTypeDef(
     _RequiredCreateDataSetRequestRequestTypeDef, _OptionalCreateDataSetRequestRequestTypeDef
 ):
@@ -14659,29 +14699,33 @@
 
 _RequiredUpdateDataSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSetRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DataSetId": str,
         "Name": str,
-        "PhysicalTableMap": Mapping[str, PhysicalTableTypeDef],
+        "PhysicalTableMap": Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
         "ImportMode": DataSetImportModeType,
     },
 )
 _OptionalUpdateDataSetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDataSetRequestRequestTypeDef",
     {
-        "LogicalTableMap": Mapping[str, LogicalTableTypeDef],
-        "ColumnGroups": Sequence[ColumnGroupTypeDef],
-        "FieldFolders": Mapping[str, FieldFolderTypeDef],
+        "LogicalTableMap": Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]],
+        "ColumnGroups": Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]],
+        "FieldFolders": Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]],
         "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
         "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
-        "ColumnLevelPermissionRules": Sequence[ColumnLevelPermissionRuleTypeDef],
+        "ColumnLevelPermissionRules": Sequence[
+            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
+        ],
         "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
-        "DatasetParameters": Sequence[DatasetParameterTypeDef],
+        "DatasetParameters": Sequence[
+            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateDataSetRequestRequestTypeDef(
     _RequiredUpdateDataSetRequestRequestTypeDef, _OptionalUpdateDataSetRequestRequestTypeDef
 ):
@@ -15033,15 +15077,15 @@
     },
 )
 _OptionalCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDataSourceRequestRequestTypeDef",
     {
         "DataSourceParameters": DataSourceParametersTypeDef,
         "Credentials": DataSourceCredentialsTypeDef,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "VpcConnectionProperties": VpcConnectionPropertiesTypeDef,
         "SslProperties": SslPropertiesTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
@@ -19245,15 +19289,15 @@
         "Name": str,
     },
 )
 _OptionalCreateAnalysisRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAnalysisRequestRequestTypeDef",
     {
         "Parameters": ParametersTypeDef,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "SourceEntity": AnalysisSourceEntityTypeDef,
         "ThemeArn": str,
         "Tags": Sequence[TagTypeDef],
         "Definition": AnalysisDefinitionTypeDef,
     },
     total=False,
 )
@@ -19295,15 +19339,15 @@
         "Name": str,
     },
 )
 _OptionalCreateDashboardRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDashboardRequestRequestTypeDef",
     {
         "Parameters": ParametersTypeDef,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "SourceEntity": DashboardSourceEntityTypeDef,
         "Tags": Sequence[TagTypeDef],
         "VersionDescription": str,
         "DashboardPublishOptions": DashboardPublishOptionsTypeDef,
         "ThemeArn": str,
         "Definition": DashboardVersionDefinitionTypeDef,
     },
@@ -19348,15 +19392,15 @@
         "TemplateId": str,
     },
 )
 _OptionalCreateTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTemplateRequestRequestTypeDef",
     {
         "Name": str,
-        "Permissions": Sequence[ResourcePermissionTypeDef],
+        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
         "SourceEntity": TemplateSourceEntityTypeDef,
         "Tags": Sequence[TagTypeDef],
         "VersionDescription": str,
         "Definition": TemplateVersionDefinitionTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/PKG-INFO` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.28.15
-Summary: Type annotations for boto3.QuickSight 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.QuickSight 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
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
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
 See how it helps to find and fix potential bugs:
 
@@ -707,16 +707,18 @@
     ConditionalFormattingSolidColorTypeDef,
     ConditionalFormattingCustomIconOptionsTypeDef,
     ConditionalFormattingIconDisplayConfigurationTypeDef,
     ConditionalFormattingIconSetTypeDef,
     TagTypeDef,
     CreateAccountSubscriptionRequestRequestTypeDef,
     SignupResponseTypeDef,
+    ResourcePermissionOutputTypeDef,
     ResourcePermissionTypeDef,
     DataSetUsageConfigurationTypeDef,
+    FieldFolderOutputTypeDef,
     FieldFolderTypeDef,
     RowLevelPermissionDataSetTypeDef,
     CreateFolderMembershipRequestRequestTypeDef,
     FolderMemberTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
     GroupMemberTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -758,15 +760,14 @@
     DataPathLabelTypeTypeDef,
     FieldLabelTypeTypeDef,
     MaximumLabelTypeTypeDef,
     MinimumLabelTypeTypeDef,
     RangeEndsLabelTypeTypeDef,
     DataPathValueTypeDef,
     DataSetSearchFilterTypeDef,
-    FieldFolderOutputTypeDef,
     OutputColumnTypeDef,
     DataSourceErrorInfoTypeDef,
     DatabricksParametersTypeDef,
     ExasolParametersTypeDef,
     JiraParametersTypeDef,
     MariaDbParametersTypeDef,
     MySqlParametersTypeDef,
@@ -821,15 +822,14 @@
     DeleteUserRequestRequestTypeDef,
     DeleteVPCConnectionRequestRequestTypeDef,
     DescribeAccountCustomizationRequestRequestTypeDef,
     DescribeAccountSettingsRequestRequestTypeDef,
     DescribeAccountSubscriptionRequestRequestTypeDef,
     DescribeAnalysisDefinitionRequestRequestTypeDef,
     DescribeAnalysisPermissionsRequestRequestTypeDef,
-    ResourcePermissionOutputTypeDef,
     DescribeAnalysisRequestRequestTypeDef,
     DescribeAssetBundleExportJobRequestRequestTypeDef,
     DescribeAssetBundleImportJobRequestRequestTypeDef,
     DescribeDashboardDefinitionRequestRequestTypeDef,
     DescribeDashboardPermissionsRequestRequestTypeDef,
     DescribeDashboardRequestRequestTypeDef,
     DescribeDashboardSnapshotJobRequestRequestTypeDef,
@@ -1173,14 +1173,28 @@
     ConditionalFormattingCustomIconConditionTypeDef,
     CreateAccountCustomizationRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateVPCConnectionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
+    DescribeAnalysisPermissionsResponseTypeDef,
+    DescribeDataSetPermissionsResponseTypeDef,
+    DescribeDataSourcePermissionsResponseTypeDef,
+    DescribeFolderPermissionsResponseTypeDef,
+    DescribeFolderResolvedPermissionsResponseTypeDef,
+    DescribeTemplatePermissionsResponseTypeDef,
+    DescribeThemePermissionsResponseTypeDef,
+    DescribeTopicPermissionsResponseTypeDef,
+    LinkSharingConfigurationTypeDef,
+    UpdateAnalysisPermissionsResponseTypeDef,
+    UpdateFolderPermissionsResponseTypeDef,
+    UpdateTemplatePermissionsResponseTypeDef,
+    UpdateThemePermissionsResponseTypeDef,
+    UpdateTopicPermissionsResponseTypeDef,
     CreateFolderRequestRequestTypeDef,
     UpdateAnalysisPermissionsRequestRequestTypeDef,
     UpdateDashboardPermissionsRequestRequestTypeDef,
     UpdateDataSetPermissionsRequestRequestTypeDef,
     UpdateDataSourcePermissionsRequestRequestTypeDef,
     UpdateFolderPermissionsRequestRequestTypeDef,
     UpdateTemplatePermissionsRequestRequestTypeDef,
@@ -1233,28 +1247,14 @@
     SearchDataSourcesResponseTypeDef,
     DateTimeDatasetParameterOutputTypeDef,
     DateTimeDatasetParameterTypeDef,
     TimeRangeFilterValueOutputTypeDef,
     TimeRangeFilterValueTypeDef,
     DecimalDatasetParameterOutputTypeDef,
     DecimalDatasetParameterTypeDef,
-    DescribeAnalysisPermissionsResponseTypeDef,
-    DescribeDataSetPermissionsResponseTypeDef,
-    DescribeDataSourcePermissionsResponseTypeDef,
-    DescribeFolderPermissionsResponseTypeDef,
-    DescribeFolderResolvedPermissionsResponseTypeDef,
-    DescribeTemplatePermissionsResponseTypeDef,
-    DescribeThemePermissionsResponseTypeDef,
-    DescribeTopicPermissionsResponseTypeDef,
-    LinkSharingConfigurationTypeDef,
-    UpdateAnalysisPermissionsResponseTypeDef,
-    UpdateFolderPermissionsResponseTypeDef,
-    UpdateTemplatePermissionsResponseTypeDef,
-    UpdateThemePermissionsResponseTypeDef,
-    UpdateTopicPermissionsResponseTypeDef,
     DescribeFolderResponseTypeDef,
     DescribeIAMPolicyAssignmentResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     TopicRefreshScheduleSummaryTypeDef,
     DescribeUserResponseTypeDef,
     ListUsersResponseTypeDef,
@@ -1390,27 +1390,27 @@
     TopicCategoryFilterOutputTypeDef,
     TopicCategoryFilterTypeDef,
     TagColumnOperationOutputTypeDef,
     TagColumnOperationTypeDef,
     DataSetConfigurationOutputTypeDef,
     DataSetConfigurationTypeDef,
     ConditionalFormattingIconTypeDef,
+    DescribeDashboardPermissionsResponseTypeDef,
+    UpdateDashboardPermissionsResponseTypeDef,
     ListDataSetsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     DestinationParameterValueConfigurationOutputTypeDef,
     DestinationParameterValueConfigurationTypeDef,
     DashboardPublishOptionsTypeDef,
     VisualPaletteOutputTypeDef,
     VisualPaletteTypeDef,
     PivotTableFieldCollapseStateOptionOutputTypeDef,
     PivotTableFieldCollapseStateOptionTypeDef,
     TimeRangeFilterOutputTypeDef,
     TimeRangeFilterTypeDef,
-    DescribeDashboardPermissionsResponseTypeDef,
-    UpdateDashboardPermissionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     DefaultFormattingTypeDef,
     CustomActionFilterOperationOutputTypeDef,
     CustomActionFilterOperationTypeDef,
     AxisLabelOptionsTypeDef,
     DataLabelOptionsOutputTypeDef,
     DataLabelOptionsTypeDef,
```

### Comparing `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/SOURCES.txt` & `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15/setup.py` & `mypy-boto3-quicksight-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-quicksight",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_quicksight"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.QuickSight 1.28.15 service generated with mypy-boto3-builder"
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

