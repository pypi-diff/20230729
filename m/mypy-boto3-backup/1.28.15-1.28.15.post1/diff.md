# Comparing `tmp/mypy-boto3-backup-1.28.15.tar.gz` & `tmp/mypy-boto3-backup-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backup-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
+gzip compressed data, was "mypy-boto3-backup-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
```

## Comparing `mypy-boto3-backup-1.28.15.tar` & `mypy-boto3-backup-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.440698 mypy-boto3-backup-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-07-28 20:42:19.436698 mypy-boto3-backup-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.432698 mypy-boto3-backup-1.28.15/mypy_boto3_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54908 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54816 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-28 20:20:03.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 20:20:03.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16547 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71441 2023-07-28 20:20:05.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71358 2023-07-28 20:20:04.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.436698 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.440698 mypy-boto3-backup-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.645022 mypy-boto3-backup-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22321 2023-07-29 10:02:34.645022 mypy-boto3-backup-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.645022 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55491 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55399 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-29 09:38:55.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-29 09:38:55.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-07-29 09:38:55.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16547 2023-07-29 09:38:55.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71561 2023-07-29 09:38:58.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71478 2023-07-29 09:38:56.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.645022 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22321 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.645022 mypy-boto3-backup-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-backup-1.28.15/LICENSE` & `mypy-boto3-backup-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15/PKG-INFO` & `mypy-boto3-backup-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.28.15
-Summary: Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backup-1.28.15/README.md` & `mypy-boto3-backup-1.28.15.post1/README.md`

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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/__init__.py` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/__init__.pyi` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/__main__.py` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Backup 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Backup 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup\nOther"
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

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/client.py` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     ListRecoveryPointsByBackupVaultPaginator,
     ListRecoveryPointsByLegalHoldPaginator,
     ListRecoveryPointsByResourcePaginator,
     ListRestoreJobsPaginator,
 )
 from .type_defs import (
     BackupPlanInputTypeDef,
+    BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
     CreateBackupPlanOutputTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     CreateLegalHoldOutputTypeDef,
     CreateReportPlanOutputTypeDef,
@@ -59,14 +60,15 @@
     DescribeRecoveryPointOutputTypeDef,
     DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     DescribeRestoreJobOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateOutputTypeDef,
+    FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
     GetBackupSelectionOutputTypeDef,
     GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsOutputTypeDef,
@@ -87,16 +89,19 @@
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListReportJobsOutputTypeDef,
     ListReportPlansOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ListTagsOutputTypeDef,
+    RecoveryPointSelectionOutputTypeDef,
     RecoveryPointSelectionTypeDef,
+    ReportDeliveryChannelOutputTypeDef,
     ReportDeliveryChannelTypeDef,
+    ReportSettingOutputTypeDef,
     ReportSettingTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobOutputTypeDef,
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
@@ -192,15 +197,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_plan)
         """
 
     def create_backup_selection(
         self,
         *,
         BackupPlanId: str,
-        BackupSelection: BackupSelectionTypeDef,
+        BackupSelection: Union[BackupSelectionTypeDef, BackupSelectionOutputTypeDef],
         CreatorRequestId: str = ...
     ) -> CreateBackupSelectionOutputTypeDef:
         """
         Creates a JSON document that specifies a set of resources to assign to a backup
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
@@ -222,15 +227,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_vault)
         """
 
     def create_framework(
         self,
         *,
         FrameworkName: str,
-        FrameworkControls: Sequence[FrameworkControlTypeDef],
+        FrameworkControls: Sequence[Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]],
         FrameworkDescription: str = ...,
         IdempotencyToken: str = ...,
         FrameworkTags: Mapping[str, str] = ...
     ) -> CreateFrameworkOutputTypeDef:
         """
         Creates a framework with one or more controls.
 
@@ -240,30 +245,34 @@
 
     def create_legal_hold(
         self,
         *,
         Title: str,
         Description: str,
         IdempotencyToken: str = ...,
-        RecoveryPointSelection: RecoveryPointSelectionTypeDef = ...,
+        RecoveryPointSelection: Union[
+            RecoveryPointSelectionTypeDef, RecoveryPointSelectionOutputTypeDef
+        ] = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateLegalHoldOutputTypeDef:
         """
         This action creates a legal hold on a recovery point (backup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_legal_hold)
         """
 
     def create_report_plan(
         self,
         *,
         ReportPlanName: str,
-        ReportDeliveryChannel: ReportDeliveryChannelTypeDef,
-        ReportSetting: ReportSettingTypeDef,
+        ReportDeliveryChannel: Union[
+            ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
+        ],
+        ReportSetting: Union[ReportSettingTypeDef, ReportSettingOutputTypeDef],
         ReportPlanDescription: str = ...,
         ReportPlanTags: Mapping[str, str] = ...,
         IdempotencyToken: str = ...
     ) -> CreateReportPlanOutputTypeDef:
         """
         Creates a report plan.
 
@@ -969,15 +978,17 @@
         """
 
     def update_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkDescription: str = ...,
-        FrameworkControls: Sequence[FrameworkControlTypeDef] = ...,
+        FrameworkControls: Sequence[
+            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
+        ] = ...,
         IdempotencyToken: str = ...
     ) -> UpdateFrameworkOutputTypeDef:
         """
         Updates an existing framework identified by its `FrameworkName` with the input
         document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_framework)
@@ -1019,16 +1030,18 @@
         """
 
     def update_report_plan(
         self,
         *,
         ReportPlanName: str,
         ReportPlanDescription: str = ...,
-        ReportDeliveryChannel: ReportDeliveryChannelTypeDef = ...,
-        ReportSetting: ReportSettingTypeDef = ...,
+        ReportDeliveryChannel: Union[
+            ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
+        ] = ...,
+        ReportSetting: Union[ReportSettingTypeDef, ReportSettingOutputTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> UpdateReportPlanOutputTypeDef:
         """
         Updates an existing report plan identified by its `ReportPlanName` with the
         input document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_report_plan)
```

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/client.pyi` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     ListRecoveryPointsByBackupVaultPaginator,
     ListRecoveryPointsByLegalHoldPaginator,
     ListRecoveryPointsByResourcePaginator,
     ListRestoreJobsPaginator,
 )
 from .type_defs import (
     BackupPlanInputTypeDef,
+    BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
     CreateBackupPlanOutputTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     CreateLegalHoldOutputTypeDef,
     CreateReportPlanOutputTypeDef,
@@ -59,14 +60,15 @@
     DescribeRecoveryPointOutputTypeDef,
     DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     DescribeRestoreJobOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateOutputTypeDef,
+    FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
     GetBackupSelectionOutputTypeDef,
     GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsOutputTypeDef,
@@ -87,16 +89,19 @@
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListReportJobsOutputTypeDef,
     ListReportPlansOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ListTagsOutputTypeDef,
+    RecoveryPointSelectionOutputTypeDef,
     RecoveryPointSelectionTypeDef,
+    ReportDeliveryChannelOutputTypeDef,
     ReportDeliveryChannelTypeDef,
+    ReportSettingOutputTypeDef,
     ReportSettingTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobOutputTypeDef,
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
@@ -183,15 +188,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_plan)
         """
     def create_backup_selection(
         self,
         *,
         BackupPlanId: str,
-        BackupSelection: BackupSelectionTypeDef,
+        BackupSelection: Union[BackupSelectionTypeDef, BackupSelectionOutputTypeDef],
         CreatorRequestId: str = ...
     ) -> CreateBackupSelectionOutputTypeDef:
         """
         Creates a JSON document that specifies a set of resources to assign to a backup
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
@@ -211,15 +216,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_vault)
         """
     def create_framework(
         self,
         *,
         FrameworkName: str,
-        FrameworkControls: Sequence[FrameworkControlTypeDef],
+        FrameworkControls: Sequence[Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]],
         FrameworkDescription: str = ...,
         IdempotencyToken: str = ...,
         FrameworkTags: Mapping[str, str] = ...
     ) -> CreateFrameworkOutputTypeDef:
         """
         Creates a framework with one or more controls.
 
@@ -228,29 +233,33 @@
         """
     def create_legal_hold(
         self,
         *,
         Title: str,
         Description: str,
         IdempotencyToken: str = ...,
-        RecoveryPointSelection: RecoveryPointSelectionTypeDef = ...,
+        RecoveryPointSelection: Union[
+            RecoveryPointSelectionTypeDef, RecoveryPointSelectionOutputTypeDef
+        ] = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateLegalHoldOutputTypeDef:
         """
         This action creates a legal hold on a recovery point (backup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_legal_hold)
         """
     def create_report_plan(
         self,
         *,
         ReportPlanName: str,
-        ReportDeliveryChannel: ReportDeliveryChannelTypeDef,
-        ReportSetting: ReportSettingTypeDef,
+        ReportDeliveryChannel: Union[
+            ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
+        ],
+        ReportSetting: Union[ReportSettingTypeDef, ReportSettingOutputTypeDef],
         ReportPlanDescription: str = ...,
         ReportPlanTags: Mapping[str, str] = ...,
         IdempotencyToken: str = ...
     ) -> CreateReportPlanOutputTypeDef:
         """
         Creates a report plan.
 
@@ -894,15 +903,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_backup_plan)
         """
     def update_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkDescription: str = ...,
-        FrameworkControls: Sequence[FrameworkControlTypeDef] = ...,
+        FrameworkControls: Sequence[
+            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
+        ] = ...,
         IdempotencyToken: str = ...
     ) -> UpdateFrameworkOutputTypeDef:
         """
         Updates an existing framework identified by its `FrameworkName` with the input
         document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_framework)
@@ -940,16 +951,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_region_settings)
         """
     def update_report_plan(
         self,
         *,
         ReportPlanName: str,
         ReportPlanDescription: str = ...,
-        ReportDeliveryChannel: ReportDeliveryChannelTypeDef = ...,
-        ReportSetting: ReportSettingTypeDef = ...,
+        ReportDeliveryChannel: Union[
+            ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
+        ] = ...,
+        ReportSetting: Union[ReportSettingTypeDef, ReportSettingOutputTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> UpdateReportPlanOutputTypeDef:
         """
         Updates an existing report plan identified by its `ReportPlanName` with the
         input document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_report_plan)
```

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/literals.py` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/literals.pyi` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/paginator.py` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/paginator.pyi` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/type_defs.py` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2413,15 +2413,17 @@
     },
 )
 
 _RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
     "_RequiredCreateFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
-        "FrameworkControls": Sequence[FrameworkControlTypeDef],
+        "FrameworkControls": Sequence[
+            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
+        ],
     },
 )
 _OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
     "_OptionalCreateFrameworkInputRequestTypeDef",
     {
         "FrameworkDescription": str,
         "IdempotencyToken": str,
@@ -2443,15 +2445,17 @@
         "FrameworkName": str,
     },
 )
 _OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
     "_OptionalUpdateFrameworkInputRequestTypeDef",
     {
         "FrameworkDescription": str,
-        "FrameworkControls": Sequence[FrameworkControlTypeDef],
+        "FrameworkControls": Sequence[
+            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
+        ],
         "IdempotencyToken": str,
     },
     total=False,
 )
 
 
 class UpdateFrameworkInputRequestTypeDef(
```

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup/type_defs.pyi` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2344,15 +2344,17 @@
     },
 )
 
 _RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
     "_RequiredCreateFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
-        "FrameworkControls": Sequence[FrameworkControlTypeDef],
+        "FrameworkControls": Sequence[
+            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
+        ],
     },
 )
 _OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
     "_OptionalCreateFrameworkInputRequestTypeDef",
     {
         "FrameworkDescription": str,
         "IdempotencyToken": str,
@@ -2372,15 +2374,17 @@
         "FrameworkName": str,
     },
 )
 _OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
     "_OptionalUpdateFrameworkInputRequestTypeDef",
     {
         "FrameworkDescription": str,
-        "FrameworkControls": Sequence[FrameworkControlTypeDef],
+        "FrameworkControls": Sequence[
+            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
+        ],
         "IdempotencyToken": str,
     },
     total=False,
 )
 
 class UpdateFrameworkInputRequestTypeDef(
     _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
```

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/PKG-INFO` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.28.15
-Summary: Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/SOURCES.txt` & `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15/setup.py` & `mypy-boto3-backup-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backup",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_backup"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

