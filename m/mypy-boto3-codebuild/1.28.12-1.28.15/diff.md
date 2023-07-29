# Comparing `tmp/mypy-boto3-codebuild-1.28.12.tar.gz` & `tmp/mypy-boto3-codebuild-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codebuild-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
+gzip compressed data, was "mypy-boto3-codebuild-1.28.15.tar", last modified: Fri Jul 28 20:42:28 2023, max compression
```

## Comparing `mypy-boto3-codebuild-1.28.12.tar` & `mypy-boto3-codebuild-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.240556 mypy-boto3-codebuild-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-07-27 05:34:27.240556 mypy-boto3-codebuild-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20291 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.236556 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41431 2023-07-27 05:18:56.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41367 2023-07-27 05:18:56.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-07-27 05:18:57.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-07-27 05:18:56.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-27 05:18:56.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-07-27 05:18:56.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-07-27 05:18:58.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65726 2023-07-27 05:18:57.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.240556 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.240556 mypy-boto3-codebuild-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.476824 mypy-boto3-codebuild-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:17.000000 mypy-boto3-codebuild-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21229 2023-07-28 20:42:28.472823 mypy-boto3-codebuild-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19734 2023-07-28 20:21:17.000000 mypy-boto3-codebuild-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.472823 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-28 20:21:17.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-28 20:21:17.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:21:17.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41431 2023-07-28 20:21:18.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41367 2023-07-28 20:21:17.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-07-28 20:21:18.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-07-28 20:21:18.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15290 2023-07-28 20:21:18.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-07-28 20:21:18.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:17.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59346 2023-07-28 20:21:21.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59283 2023-07-28 20:21:19.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:17.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.472823 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21229 2023-07-28 20:42:28.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:42:28.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:28.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:28.000000 mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:28.476824 mypy-boto3-codebuild-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:21:16.000000 mypy-boto3-codebuild-1.28.15/setup.py
```

### Comparing `mypy-boto3-codebuild-1.28.12/LICENSE` & `mypy-boto3-codebuild-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.12/PKG-INFO` & `mypy-boto3-codebuild-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codebuild
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeBuild 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeBuild 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,178 +407,162 @@
 `mypy_boto3_codebuild.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
     BatchRestrictionsOutputTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
     BuildBatchFilterTypeDef,
     PhaseContextTypeDef,
     ProjectCacheOutputTypeDef,
-    ProjectFileSystemLocationOutputTypeDef,
-    ProjectSourceVersionOutputTypeDef,
+    ProjectFileSystemLocationTypeDef,
+    ProjectSourceVersionTypeDef,
     VpcConfigOutputTypeDef,
-    BuildStatusConfigOutputTypeDef,
     BuildStatusConfigTypeDef,
     ResolvedArtifactTypeDef,
     DebugSessionTypeDef,
     ExportedEnvironmentVariableTypeDef,
     NetworkInterfaceTypeDef,
-    CloudWatchLogsConfigOutputTypeDef,
     CloudWatchLogsConfigTypeDef,
     CodeCoverageReportSummaryTypeDef,
     CodeCoverageTypeDef,
     ProjectArtifactsTypeDef,
     ProjectCacheTypeDef,
-    ProjectFileSystemLocationTypeDef,
-    ProjectSourceVersionTypeDef,
     TagTypeDef,
     VpcConfigTypeDef,
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
-    DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
-    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
-    EnvironmentVariableOutputTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
-    GetResourcePolicyOutputTypeDef,
-    GitSubmodulesConfigOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
-    ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
-    ListBuildBatchesForProjectOutputTypeDef,
-    ListBuildBatchesOutputTypeDef,
-    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     ListBuildsForProjectInputRequestTypeDef,
-    ListBuildsForProjectOutputTypeDef,
-    ListBuildsInputListBuildsPaginateTypeDef,
     ListBuildsInputRequestTypeDef,
-    ListBuildsOutputTypeDef,
-    ListProjectsInputListProjectsPaginateTypeDef,
     ListProjectsInputRequestTypeDef,
-    ListProjectsOutputTypeDef,
-    ListReportGroupsInputListReportGroupsPaginateTypeDef,
     ListReportGroupsInputRequestTypeDef,
-    ListReportGroupsOutputTypeDef,
     ReportFilterTypeDef,
-    ListReportsForReportGroupOutputTypeDef,
-    ListReportsOutputTypeDef,
-    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
-    ListSharedProjectsOutputTypeDef,
-    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
-    ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
-    S3LogsConfigOutputTypeDef,
     S3LogsConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ProjectArtifactsOutputTypeDef,
     ProjectBadgeTypeDef,
-    RegistryCredentialOutputTypeDef,
     RegistryCredentialTypeDef,
-    SourceAuthOutputTypeDef,
     SourceAuthTypeDef,
-    TagOutputTypeDef,
     PutResourcePolicyInputRequestTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    S3ReportExportConfigOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
-    UpdateProjectVisibilityOutputTypeDef,
-    WebhookFilterOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
+    DeleteSourceCredentialsOutputTypeDef,
+    GetResourcePolicyOutputTypeDef,
+    ImportSourceCredentialsOutputTypeDef,
+    ListBuildBatchesForProjectOutputTypeDef,
+    ListBuildBatchesOutputTypeDef,
+    ListBuildsForProjectOutputTypeDef,
+    ListBuildsOutputTypeDef,
+    ListProjectsOutputTypeDef,
+    ListReportGroupsOutputTypeDef,
+    ListReportsForReportGroupOutputTypeDef,
+    ListReportsOutputTypeDef,
+    ListSharedProjectsOutputTypeDef,
+    ListSharedReportGroupsOutputTypeDef,
+    PutResourcePolicyOutputTypeDef,
+    UpdateProjectVisibilityOutputTypeDef,
     ProjectBuildBatchConfigOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
-    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
-    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
+    WebhookTypeDef,
+    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
+    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
+    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    ListBuildsInputListBuildsPaginateTypeDef,
+    ListProjectsInputListProjectsPaginateTypeDef,
+    ListReportGroupsInputListReportGroupsPaginateTypeDef,
+    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
+    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
     ListReportsInputListReportsPaginateTypeDef,
     ListReportsInputRequestTypeDef,
     ListSourceCredentialsOutputTypeDef,
-    LogsConfigOutputTypeDef,
-    LogsLocationTypeDef,
     LogsConfigTypeDef,
+    LogsLocationTypeDef,
     ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
-    ProjectSourceOutputTypeDef,
     ProjectSourceTypeDef,
-    ReportExportConfigOutputTypeDef,
     ReportExportConfigTypeDef,
-    WebhookTypeDef,
     BuildGroupTypeDef,
+    CreateWebhookOutputTypeDef,
+    UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
+    ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
+    CreateReportGroupInputRequestTypeDef,
     ReportGroupTypeDef,
     ReportTypeDef,
-    CreateReportGroupInputRequestTypeDef,
     UpdateReportGroupInputRequestTypeDef,
-    CreateWebhookOutputTypeDef,
-    ProjectTypeDef,
-    UpdateWebhookOutputTypeDef,
     BuildBatchTypeDef,
     ListCuratedEnvironmentImagesOutputTypeDef,
     BatchGetBuildsOutputTypeDef,
     RetryBuildOutputTypeDef,
     StartBuildOutputTypeDef,
     StopBuildOutputTypeDef,
+    BatchGetProjectsOutputTypeDef,
+    CreateProjectOutputTypeDef,
+    UpdateProjectOutputTypeDef,
     BatchGetReportGroupsOutputTypeDef,
     CreateReportGroupOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     BatchGetReportsOutputTypeDef,
-    BatchGetProjectsOutputTypeDef,
-    CreateProjectOutputTypeDef,
-    UpdateProjectOutputTypeDef,
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
```

### Comparing `mypy-boto3-codebuild-1.28.12/README.md` & `mypy-boto3-codebuild-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,178 +375,162 @@
 `mypy_boto3_codebuild.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
     BatchRestrictionsOutputTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
     BuildBatchFilterTypeDef,
     PhaseContextTypeDef,
     ProjectCacheOutputTypeDef,
-    ProjectFileSystemLocationOutputTypeDef,
-    ProjectSourceVersionOutputTypeDef,
+    ProjectFileSystemLocationTypeDef,
+    ProjectSourceVersionTypeDef,
     VpcConfigOutputTypeDef,
-    BuildStatusConfigOutputTypeDef,
     BuildStatusConfigTypeDef,
     ResolvedArtifactTypeDef,
     DebugSessionTypeDef,
     ExportedEnvironmentVariableTypeDef,
     NetworkInterfaceTypeDef,
-    CloudWatchLogsConfigOutputTypeDef,
     CloudWatchLogsConfigTypeDef,
     CodeCoverageReportSummaryTypeDef,
     CodeCoverageTypeDef,
     ProjectArtifactsTypeDef,
     ProjectCacheTypeDef,
-    ProjectFileSystemLocationTypeDef,
-    ProjectSourceVersionTypeDef,
     TagTypeDef,
     VpcConfigTypeDef,
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
-    DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
-    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
-    EnvironmentVariableOutputTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
-    GetResourcePolicyOutputTypeDef,
-    GitSubmodulesConfigOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
-    ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
-    ListBuildBatchesForProjectOutputTypeDef,
-    ListBuildBatchesOutputTypeDef,
-    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     ListBuildsForProjectInputRequestTypeDef,
-    ListBuildsForProjectOutputTypeDef,
-    ListBuildsInputListBuildsPaginateTypeDef,
     ListBuildsInputRequestTypeDef,
-    ListBuildsOutputTypeDef,
-    ListProjectsInputListProjectsPaginateTypeDef,
     ListProjectsInputRequestTypeDef,
-    ListProjectsOutputTypeDef,
-    ListReportGroupsInputListReportGroupsPaginateTypeDef,
     ListReportGroupsInputRequestTypeDef,
-    ListReportGroupsOutputTypeDef,
     ReportFilterTypeDef,
-    ListReportsForReportGroupOutputTypeDef,
-    ListReportsOutputTypeDef,
-    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
-    ListSharedProjectsOutputTypeDef,
-    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
-    ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
-    S3LogsConfigOutputTypeDef,
     S3LogsConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ProjectArtifactsOutputTypeDef,
     ProjectBadgeTypeDef,
-    RegistryCredentialOutputTypeDef,
     RegistryCredentialTypeDef,
-    SourceAuthOutputTypeDef,
     SourceAuthTypeDef,
-    TagOutputTypeDef,
     PutResourcePolicyInputRequestTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    S3ReportExportConfigOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
-    UpdateProjectVisibilityOutputTypeDef,
-    WebhookFilterOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
+    DeleteSourceCredentialsOutputTypeDef,
+    GetResourcePolicyOutputTypeDef,
+    ImportSourceCredentialsOutputTypeDef,
+    ListBuildBatchesForProjectOutputTypeDef,
+    ListBuildBatchesOutputTypeDef,
+    ListBuildsForProjectOutputTypeDef,
+    ListBuildsOutputTypeDef,
+    ListProjectsOutputTypeDef,
+    ListReportGroupsOutputTypeDef,
+    ListReportsForReportGroupOutputTypeDef,
+    ListReportsOutputTypeDef,
+    ListSharedProjectsOutputTypeDef,
+    ListSharedReportGroupsOutputTypeDef,
+    PutResourcePolicyOutputTypeDef,
+    UpdateProjectVisibilityOutputTypeDef,
     ProjectBuildBatchConfigOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
-    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
-    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
+    WebhookTypeDef,
+    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
+    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
+    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    ListBuildsInputListBuildsPaginateTypeDef,
+    ListProjectsInputListProjectsPaginateTypeDef,
+    ListReportGroupsInputListReportGroupsPaginateTypeDef,
+    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
+    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
     ListReportsInputListReportsPaginateTypeDef,
     ListReportsInputRequestTypeDef,
     ListSourceCredentialsOutputTypeDef,
-    LogsConfigOutputTypeDef,
-    LogsLocationTypeDef,
     LogsConfigTypeDef,
+    LogsLocationTypeDef,
     ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
-    ProjectSourceOutputTypeDef,
     ProjectSourceTypeDef,
-    ReportExportConfigOutputTypeDef,
     ReportExportConfigTypeDef,
-    WebhookTypeDef,
     BuildGroupTypeDef,
+    CreateWebhookOutputTypeDef,
+    UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
+    ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
+    CreateReportGroupInputRequestTypeDef,
     ReportGroupTypeDef,
     ReportTypeDef,
-    CreateReportGroupInputRequestTypeDef,
     UpdateReportGroupInputRequestTypeDef,
-    CreateWebhookOutputTypeDef,
-    ProjectTypeDef,
-    UpdateWebhookOutputTypeDef,
     BuildBatchTypeDef,
     ListCuratedEnvironmentImagesOutputTypeDef,
     BatchGetBuildsOutputTypeDef,
     RetryBuildOutputTypeDef,
     StartBuildOutputTypeDef,
     StopBuildOutputTypeDef,
+    BatchGetProjectsOutputTypeDef,
+    CreateProjectOutputTypeDef,
+    UpdateProjectOutputTypeDef,
     BatchGetReportGroupsOutputTypeDef,
     CreateReportGroupOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     BatchGetReportsOutputTypeDef,
-    BatchGetProjectsOutputTypeDef,
-    CreateProjectOutputTypeDef,
-    UpdateProjectOutputTypeDef,
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
```

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__init__.py` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__init__.pyi` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__main__.py` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeBuild 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodeBuild 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild\nOther"
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

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/client.py` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/client.pyi` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/literals.py` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/literals.pyi` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/paginator.py` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         self,
         *,
         reportArn: str,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportCodeCoverageSortByTypeType = ...,
         minLineCoveragePercentage: float = ...,
         maxLineCoveragePercentage: float = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeCodeCoveragesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeCodeCoverages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#describecodecoveragespaginator)
         """
 
 
@@ -126,15 +126,15 @@
     """
 
     def paginate(
         self,
         *,
         reportArn: str,
         filter: TestCaseFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTestCasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeTestCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#describetestcasespaginator)
         """
 
 
@@ -145,15 +145,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBuildBatchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildbatchespaginator)
         """
 
 
@@ -165,33 +165,30 @@
 
     def paginate(
         self,
         *,
         projectName: str = ...,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBuildBatchesForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatchesForProject.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildbatchesforprojectpaginator)
         """
 
 
 class ListBuildsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, sortOrder: SortOrderTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBuildsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildspaginator)
         """
 
 
@@ -202,15 +199,15 @@
     """
 
     def paginate(
         self,
         *,
         projectName: str,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBuildsForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildsForProject.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildsforprojectpaginator)
         """
 
 
@@ -221,15 +218,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: ProjectSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listprojectspaginator)
         """
 
 
@@ -240,15 +237,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportGroupSortByTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportgroupspaginator)
         """
 
 
@@ -259,15 +256,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportspaginator)
         """
 
 
@@ -279,15 +276,15 @@
 
     def paginate(
         self,
         *,
         reportGroupArn: str,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReportsForReportGroupOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportsForReportGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportsforreportgrouppaginator)
         """
 
 
@@ -298,15 +295,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SharedResourceSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSharedProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listsharedprojectspaginator)
         """
 
 
@@ -317,13 +314,13 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: SharedResourceSortByTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSharedReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedReportGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listsharedreportgroupspaginator)
         """
```

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/paginator.pyi` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         self,
         *,
         reportArn: str,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportCodeCoverageSortByTypeType = ...,
         minLineCoveragePercentage: float = ...,
         maxLineCoveragePercentage: float = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeCodeCoveragesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeCodeCoverages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#describecodecoveragespaginator)
         """
 
 class DescribeTestCasesPaginator(Paginator):
@@ -122,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         reportArn: str,
         filter: TestCaseFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTestCasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeTestCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#describetestcasespaginator)
         """
 
 class ListBuildBatchesPaginator(Paginator):
@@ -140,15 +140,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBuildBatchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildbatchespaginator)
         """
 
 class ListBuildBatchesForProjectPaginator(Paginator):
@@ -159,32 +159,29 @@
 
     def paginate(
         self,
         *,
         projectName: str = ...,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBuildBatchesForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatchesForProject.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildbatchesforprojectpaginator)
         """
 
 class ListBuildsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, sortOrder: SortOrderTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBuildsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildspaginator)
         """
 
 class ListBuildsForProjectPaginator(Paginator):
@@ -194,15 +191,15 @@
     """
 
     def paginate(
         self,
         *,
         projectName: str,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBuildsForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildsForProject.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildsforprojectpaginator)
         """
 
 class ListProjectsPaginator(Paginator):
@@ -212,15 +209,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: ProjectSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listprojectspaginator)
         """
 
 class ListReportGroupsPaginator(Paginator):
@@ -230,15 +227,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportGroupSortByTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportgroupspaginator)
         """
 
 class ListReportsPaginator(Paginator):
@@ -248,15 +245,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportspaginator)
         """
 
 class ListReportsForReportGroupPaginator(Paginator):
@@ -267,15 +264,15 @@
 
     def paginate(
         self,
         *,
         reportGroupArn: str,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReportsForReportGroupOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportsForReportGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportsforreportgrouppaginator)
         """
 
 class ListSharedProjectsPaginator(Paginator):
@@ -285,15 +282,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SharedResourceSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSharedProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listsharedprojectspaginator)
         """
 
 class ListSharedReportGroupsPaginator(Paginator):
@@ -303,13 +300,13 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: SharedResourceSortByTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSharedReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedReportGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listsharedreportgroupspaginator)
         """
```

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/type_defs.py` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,178 +62,162 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
     "BatchGetReportGroupsInputRequestTypeDef",
     "BatchGetReportsInputRequestTypeDef",
     "BatchRestrictionsOutputTypeDef",
     "BatchRestrictionsTypeDef",
     "BuildArtifactsTypeDef",
     "BuildBatchFilterTypeDef",
     "PhaseContextTypeDef",
     "ProjectCacheOutputTypeDef",
-    "ProjectFileSystemLocationOutputTypeDef",
-    "ProjectSourceVersionOutputTypeDef",
+    "ProjectFileSystemLocationTypeDef",
+    "ProjectSourceVersionTypeDef",
     "VpcConfigOutputTypeDef",
-    "BuildStatusConfigOutputTypeDef",
     "BuildStatusConfigTypeDef",
     "ResolvedArtifactTypeDef",
     "DebugSessionTypeDef",
     "ExportedEnvironmentVariableTypeDef",
     "NetworkInterfaceTypeDef",
-    "CloudWatchLogsConfigOutputTypeDef",
     "CloudWatchLogsConfigTypeDef",
     "CodeCoverageReportSummaryTypeDef",
     "CodeCoverageTypeDef",
     "ProjectArtifactsTypeDef",
     "ProjectCacheTypeDef",
-    "ProjectFileSystemLocationTypeDef",
-    "ProjectSourceVersionTypeDef",
     "TagTypeDef",
     "VpcConfigTypeDef",
     "WebhookFilterTypeDef",
     "DeleteBuildBatchInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteReportGroupInputRequestTypeDef",
     "DeleteReportInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteSourceCredentialsInputRequestTypeDef",
-    "DeleteSourceCredentialsOutputTypeDef",
     "DeleteWebhookInputRequestTypeDef",
-    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCodeCoveragesInputRequestTypeDef",
     "TestCaseFilterTypeDef",
     "TestCaseTypeDef",
     "EnvironmentImageTypeDef",
-    "EnvironmentVariableOutputTypeDef",
     "EnvironmentVariableTypeDef",
     "GetReportGroupTrendInputRequestTypeDef",
     "ReportGroupTrendStatsTypeDef",
     "ReportWithRawDataTypeDef",
     "GetResourcePolicyInputRequestTypeDef",
-    "GetResourcePolicyOutputTypeDef",
-    "GitSubmodulesConfigOutputTypeDef",
     "GitSubmodulesConfigTypeDef",
     "ImportSourceCredentialsInputRequestTypeDef",
-    "ImportSourceCredentialsOutputTypeDef",
     "InvalidateProjectCacheInputRequestTypeDef",
-    "ListBuildBatchesForProjectOutputTypeDef",
-    "ListBuildBatchesOutputTypeDef",
-    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
     "ListBuildsForProjectInputRequestTypeDef",
-    "ListBuildsForProjectOutputTypeDef",
-    "ListBuildsInputListBuildsPaginateTypeDef",
     "ListBuildsInputRequestTypeDef",
-    "ListBuildsOutputTypeDef",
-    "ListProjectsInputListProjectsPaginateTypeDef",
     "ListProjectsInputRequestTypeDef",
-    "ListProjectsOutputTypeDef",
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
     "ListReportGroupsInputRequestTypeDef",
-    "ListReportGroupsOutputTypeDef",
     "ReportFilterTypeDef",
-    "ListReportsForReportGroupOutputTypeDef",
-    "ListReportsOutputTypeDef",
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
     "ListSharedProjectsInputRequestTypeDef",
-    "ListSharedProjectsOutputTypeDef",
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "ListSharedReportGroupsInputRequestTypeDef",
-    "ListSharedReportGroupsOutputTypeDef",
     "SourceCredentialsInfoTypeDef",
-    "S3LogsConfigOutputTypeDef",
     "S3LogsConfigTypeDef",
-    "PaginatorConfigTypeDef",
-    "ProjectArtifactsOutputTypeDef",
     "ProjectBadgeTypeDef",
-    "RegistryCredentialOutputTypeDef",
     "RegistryCredentialTypeDef",
-    "SourceAuthOutputTypeDef",
     "SourceAuthTypeDef",
-    "TagOutputTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
-    "PutResourcePolicyOutputTypeDef",
-    "S3ReportExportConfigOutputTypeDef",
     "S3ReportExportConfigTypeDef",
     "TestReportSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryBuildBatchInputRequestTypeDef",
     "RetryBuildInputRequestTypeDef",
     "StopBuildBatchInputRequestTypeDef",
     "StopBuildInputRequestTypeDef",
     "UpdateProjectVisibilityInputRequestTypeDef",
-    "UpdateProjectVisibilityOutputTypeDef",
-    "WebhookFilterOutputTypeDef",
     "BatchDeleteBuildsOutputTypeDef",
     "DeleteBuildBatchOutputTypeDef",
+    "DeleteSourceCredentialsOutputTypeDef",
+    "GetResourcePolicyOutputTypeDef",
+    "ImportSourceCredentialsOutputTypeDef",
+    "ListBuildBatchesForProjectOutputTypeDef",
+    "ListBuildBatchesOutputTypeDef",
+    "ListBuildsForProjectOutputTypeDef",
+    "ListBuildsOutputTypeDef",
+    "ListProjectsOutputTypeDef",
+    "ListReportGroupsOutputTypeDef",
+    "ListReportsForReportGroupOutputTypeDef",
+    "ListReportsOutputTypeDef",
+    "ListSharedProjectsOutputTypeDef",
+    "ListSharedReportGroupsOutputTypeDef",
+    "PutResourcePolicyOutputTypeDef",
+    "UpdateProjectVisibilityOutputTypeDef",
     "ProjectBuildBatchConfigOutputTypeDef",
     "ProjectBuildBatchConfigTypeDef",
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
+    "WebhookTypeDef",
+    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
+    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    "ListBuildsInputListBuildsPaginateTypeDef",
+    "ListProjectsInputListProjectsPaginateTypeDef",
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "DescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     "DescribeTestCasesInputRequestTypeDef",
     "DescribeTestCasesOutputTypeDef",
     "EnvironmentLanguageTypeDef",
     "GetReportGroupTrendOutputTypeDef",
     "ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     "ListReportsForReportGroupInputRequestTypeDef",
     "ListReportsInputListReportsPaginateTypeDef",
     "ListReportsInputRequestTypeDef",
     "ListSourceCredentialsOutputTypeDef",
-    "LogsConfigOutputTypeDef",
-    "LogsLocationTypeDef",
     "LogsConfigTypeDef",
+    "LogsLocationTypeDef",
     "ProjectEnvironmentOutputTypeDef",
     "ProjectEnvironmentTypeDef",
-    "ProjectSourceOutputTypeDef",
     "ProjectSourceTypeDef",
-    "ReportExportConfigOutputTypeDef",
     "ReportExportConfigTypeDef",
-    "WebhookTypeDef",
     "BuildGroupTypeDef",
+    "CreateWebhookOutputTypeDef",
+    "UpdateWebhookOutputTypeDef",
     "EnvironmentPlatformTypeDef",
     "BuildTypeDef",
     "CreateProjectInputRequestTypeDef",
+    "ProjectTypeDef",
     "StartBuildBatchInputRequestTypeDef",
     "StartBuildInputRequestTypeDef",
     "UpdateProjectInputRequestTypeDef",
+    "CreateReportGroupInputRequestTypeDef",
     "ReportGroupTypeDef",
     "ReportTypeDef",
-    "CreateReportGroupInputRequestTypeDef",
     "UpdateReportGroupInputRequestTypeDef",
-    "CreateWebhookOutputTypeDef",
-    "ProjectTypeDef",
-    "UpdateWebhookOutputTypeDef",
     "BuildBatchTypeDef",
     "ListCuratedEnvironmentImagesOutputTypeDef",
     "BatchGetBuildsOutputTypeDef",
     "RetryBuildOutputTypeDef",
     "StartBuildOutputTypeDef",
     "StopBuildOutputTypeDef",
+    "BatchGetProjectsOutputTypeDef",
+    "CreateProjectOutputTypeDef",
+    "UpdateProjectOutputTypeDef",
     "BatchGetReportGroupsOutputTypeDef",
     "CreateReportGroupOutputTypeDef",
     "UpdateReportGroupOutputTypeDef",
     "BatchGetReportsOutputTypeDef",
-    "BatchGetProjectsOutputTypeDef",
-    "CreateProjectOutputTypeDef",
-    "UpdateProjectOutputTypeDef",
     "BatchGetBuildBatchesOutputTypeDef",
     "RetryBuildBatchOutputTypeDef",
     "StartBuildBatchOutputTypeDef",
     "StopBuildBatchOutputTypeDef",
 )
 
 BatchDeleteBuildsInputRequestTypeDef = TypedDict(
@@ -248,14 +232,25 @@
     {
         "id": str,
         "statusCode": str,
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
 BatchGetBuildBatchesInputRequestTypeDef = TypedDict(
     "BatchGetBuildBatchesInputRequestTypeDef",
     {
         "ids": Sequence[str],
     },
 )
 
@@ -354,28 +349,28 @@
 
 class ProjectCacheOutputTypeDef(
     _RequiredProjectCacheOutputTypeDef, _OptionalProjectCacheOutputTypeDef
 ):
     pass
 
 
-ProjectFileSystemLocationOutputTypeDef = TypedDict(
-    "ProjectFileSystemLocationOutputTypeDef",
+ProjectFileSystemLocationTypeDef = TypedDict(
+    "ProjectFileSystemLocationTypeDef",
     {
         "type": Literal["EFS"],
         "location": str,
         "mountPoint": str,
         "identifier": str,
         "mountOptions": str,
     },
     total=False,
 )
 
-ProjectSourceVersionOutputTypeDef = TypedDict(
-    "ProjectSourceVersionOutputTypeDef",
+ProjectSourceVersionTypeDef = TypedDict(
+    "ProjectSourceVersionTypeDef",
     {
         "sourceIdentifier": str,
         "sourceVersion": str,
     },
 )
 
 VpcConfigOutputTypeDef = TypedDict(
@@ -384,23 +379,14 @@
         "vpcId": str,
         "subnets": List[str],
         "securityGroupIds": List[str],
     },
     total=False,
 )
 
-BuildStatusConfigOutputTypeDef = TypedDict(
-    "BuildStatusConfigOutputTypeDef",
-    {
-        "context": str,
-        "targetUrl": str,
-    },
-    total=False,
-)
-
 BuildStatusConfigTypeDef = TypedDict(
     "BuildStatusConfigTypeDef",
     {
         "context": str,
         "targetUrl": str,
     },
     total=False,
@@ -439,36 +425,14 @@
     {
         "subnetId": str,
         "networkInterfaceId": str,
     },
     total=False,
 )
 
-_RequiredCloudWatchLogsConfigOutputTypeDef = TypedDict(
-    "_RequiredCloudWatchLogsConfigOutputTypeDef",
-    {
-        "status": LogsConfigStatusTypeType,
-    },
-)
-_OptionalCloudWatchLogsConfigOutputTypeDef = TypedDict(
-    "_OptionalCloudWatchLogsConfigOutputTypeDef",
-    {
-        "groupName": str,
-        "streamName": str,
-    },
-    total=False,
-)
-
-
-class CloudWatchLogsConfigOutputTypeDef(
-    _RequiredCloudWatchLogsConfigOutputTypeDef, _OptionalCloudWatchLogsConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredCloudWatchLogsConfigTypeDef = TypedDict(
     "_RequiredCloudWatchLogsConfigTypeDef",
     {
         "status": LogsConfigStatusTypeType,
     },
 )
 _OptionalCloudWatchLogsConfigTypeDef = TypedDict(
@@ -560,34 +524,14 @@
 )
 
 
 class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
     pass
 
 
-ProjectFileSystemLocationTypeDef = TypedDict(
-    "ProjectFileSystemLocationTypeDef",
-    {
-        "type": Literal["EFS"],
-        "location": str,
-        "mountPoint": str,
-        "identifier": str,
-        "mountOptions": str,
-    },
-    total=False,
-)
-
-ProjectSourceVersionTypeDef = TypedDict(
-    "ProjectSourceVersionTypeDef",
-    {
-        "sourceIdentifier": str,
-        "sourceVersion": str,
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -675,55 +619,31 @@
 DeleteSourceCredentialsInputRequestTypeDef = TypedDict(
     "DeleteSourceCredentialsInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DeleteSourceCredentialsOutputTypeDef = TypedDict(
-    "DeleteSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWebhookInputRequestTypeDef = TypedDict(
     "DeleteWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
-    {
-        "reportArn": str,
-    },
-)
-_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportCodeCoverageSortByTypeType,
-        "minLineCoveragePercentage": float,
-        "maxLineCoveragePercentage": float,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
-    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeCodeCoveragesInputRequestTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
@@ -777,36 +697,14 @@
         "name": str,
         "description": str,
         "versions": List[str],
     },
     total=False,
 )
 
-_RequiredEnvironmentVariableOutputTypeDef = TypedDict(
-    "_RequiredEnvironmentVariableOutputTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-)
-_OptionalEnvironmentVariableOutputTypeDef = TypedDict(
-    "_OptionalEnvironmentVariableOutputTypeDef",
-    {
-        "type": EnvironmentVariableTypeType,
-    },
-    total=False,
-)
-
-
-class EnvironmentVariableOutputTypeDef(
-    _RequiredEnvironmentVariableOutputTypeDef, _OptionalEnvironmentVariableOutputTypeDef
-):
-    pass
-
-
 _RequiredEnvironmentVariableTypeDef = TypedDict(
     "_RequiredEnvironmentVariableTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
@@ -869,29 +767,14 @@
 GetResourcePolicyInputRequestTypeDef = TypedDict(
     "GetResourcePolicyInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetResourcePolicyOutputTypeDef = TypedDict(
-    "GetResourcePolicyOutputTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GitSubmodulesConfigOutputTypeDef = TypedDict(
-    "GitSubmodulesConfigOutputTypeDef",
-    {
-        "fetchSubmodules": bool,
-    },
-)
-
 GitSubmodulesConfigTypeDef = TypedDict(
     "GitSubmodulesConfigTypeDef",
     {
         "fetchSubmodules": bool,
     },
 )
 
@@ -916,70 +799,21 @@
 class ImportSourceCredentialsInputRequestTypeDef(
     _RequiredImportSourceCredentialsInputRequestTypeDef,
     _OptionalImportSourceCredentialsInputRequestTypeDef,
 ):
     pass
 
 
-ImportSourceCredentialsOutputTypeDef = TypedDict(
-    "ImportSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InvalidateProjectCacheInputRequestTypeDef = TypedDict(
     "InvalidateProjectCacheInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-ListBuildBatchesForProjectOutputTypeDef = TypedDict(
-    "ListBuildBatchesForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBuildBatchesOutputTypeDef = TypedDict(
-    "ListBuildBatchesOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
-    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBuildsForProjectInputRequestTypeDef = TypedDict(
     "_RequiredListBuildsForProjectInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListBuildsForProjectInputRequestTypeDef = TypedDict(
@@ -995,228 +829,84 @@
 class ListBuildsForProjectInputRequestTypeDef(
     _RequiredListBuildsForProjectInputRequestTypeDef,
     _OptionalListBuildsForProjectInputRequestTypeDef,
 ):
     pass
 
 
-ListBuildsForProjectOutputTypeDef = TypedDict(
-    "ListBuildsForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
-    "ListBuildsInputListBuildsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBuildsInputRequestTypeDef = TypedDict(
     "ListBuildsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListBuildsOutputTypeDef = TypedDict(
-    "ListBuildsOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsInputListProjectsPaginateTypeDef",
-    {
-        "sortBy": ProjectSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsInputRequestTypeDef = TypedDict(
     "ListProjectsInputRequestTypeDef",
     {
         "sortBy": ProjectSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListProjectsOutputTypeDef = TypedDict(
-    "ListProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportGroupSortByTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReportGroupsInputRequestTypeDef = TypedDict(
     "ListReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": ReportGroupSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListReportGroupsOutputTypeDef = TypedDict(
-    "ListReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReportFilterTypeDef = TypedDict(
     "ReportFilterTypeDef",
     {
         "status": ReportStatusTypeType,
     },
     total=False,
 )
 
-ListReportsForReportGroupOutputTypeDef = TypedDict(
-    "ListReportsForReportGroupOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportsOutputTypeDef = TypedDict(
-    "ListReportsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
-    {
-        "sortBy": SharedResourceSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSharedProjectsInputRequestTypeDef = TypedDict(
     "ListSharedProjectsInputRequestTypeDef",
     {
         "sortBy": SharedResourceSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListSharedProjectsOutputTypeDef = TypedDict(
-    "ListSharedProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": SharedResourceSortByTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSharedReportGroupsInputRequestTypeDef = TypedDict(
     "ListSharedReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": SharedResourceSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListSharedReportGroupsOutputTypeDef = TypedDict(
-    "ListSharedReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SourceCredentialsInfoTypeDef = TypedDict(
     "SourceCredentialsInfoTypeDef",
     {
         "arn": str,
         "serverType": ServerTypeType,
         "authType": AuthTypeType,
     },
     total=False,
 )
 
-_RequiredS3LogsConfigOutputTypeDef = TypedDict(
-    "_RequiredS3LogsConfigOutputTypeDef",
-    {
-        "status": LogsConfigStatusTypeType,
-    },
-)
-_OptionalS3LogsConfigOutputTypeDef = TypedDict(
-    "_OptionalS3LogsConfigOutputTypeDef",
-    {
-        "location": str,
-        "encryptionDisabled": bool,
-        "bucketOwnerAccess": BucketOwnerAccessType,
-    },
-    total=False,
-)
-
-
-class S3LogsConfigOutputTypeDef(
-    _RequiredS3LogsConfigOutputTypeDef, _OptionalS3LogsConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredS3LogsConfigTypeDef = TypedDict(
     "_RequiredS3LogsConfigTypeDef",
     {
         "status": LogsConfigStatusTypeType,
     },
 )
 _OptionalS3LogsConfigTypeDef = TypedDict(
@@ -1230,97 +920,31 @@
 )
 
 
 class S3LogsConfigTypeDef(_RequiredS3LogsConfigTypeDef, _OptionalS3LogsConfigTypeDef):
     pass
 
 
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
-_RequiredProjectArtifactsOutputTypeDef = TypedDict(
-    "_RequiredProjectArtifactsOutputTypeDef",
-    {
-        "type": ArtifactsTypeType,
-    },
-)
-_OptionalProjectArtifactsOutputTypeDef = TypedDict(
-    "_OptionalProjectArtifactsOutputTypeDef",
-    {
-        "location": str,
-        "path": str,
-        "namespaceType": ArtifactNamespaceType,
-        "name": str,
-        "packaging": ArtifactPackagingType,
-        "overrideArtifactName": bool,
-        "encryptionDisabled": bool,
-        "artifactIdentifier": str,
-        "bucketOwnerAccess": BucketOwnerAccessType,
-    },
-    total=False,
-)
-
-
-class ProjectArtifactsOutputTypeDef(
-    _RequiredProjectArtifactsOutputTypeDef, _OptionalProjectArtifactsOutputTypeDef
-):
-    pass
-
-
 ProjectBadgeTypeDef = TypedDict(
     "ProjectBadgeTypeDef",
     {
         "badgeEnabled": bool,
         "badgeRequestUrl": str,
     },
     total=False,
 )
 
-RegistryCredentialOutputTypeDef = TypedDict(
-    "RegistryCredentialOutputTypeDef",
-    {
-        "credential": str,
-        "credentialProvider": Literal["SECRETS_MANAGER"],
-    },
-)
-
 RegistryCredentialTypeDef = TypedDict(
     "RegistryCredentialTypeDef",
     {
         "credential": str,
         "credentialProvider": Literal["SECRETS_MANAGER"],
     },
 )
 
-_RequiredSourceAuthOutputTypeDef = TypedDict(
-    "_RequiredSourceAuthOutputTypeDef",
-    {
-        "type": Literal["OAUTH"],
-    },
-)
-_OptionalSourceAuthOutputTypeDef = TypedDict(
-    "_OptionalSourceAuthOutputTypeDef",
-    {
-        "resource": str,
-    },
-    total=False,
-)
-
-
-class SourceAuthOutputTypeDef(_RequiredSourceAuthOutputTypeDef, _OptionalSourceAuthOutputTypeDef):
-    pass
-
-
 _RequiredSourceAuthTypeDef = TypedDict(
     "_RequiredSourceAuthTypeDef",
     {
         "type": Literal["OAUTH"],
     },
 )
 _OptionalSourceAuthTypeDef = TypedDict(
@@ -1332,52 +956,22 @@
 )
 
 
 class SourceAuthTypeDef(_RequiredSourceAuthTypeDef, _OptionalSourceAuthTypeDef):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
 
-PutResourcePolicyOutputTypeDef = TypedDict(
-    "PutResourcePolicyOutputTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-S3ReportExportConfigOutputTypeDef = TypedDict(
-    "S3ReportExportConfigOutputTypeDef",
-    {
-        "bucket": str,
-        "bucketOwner": str,
-        "path": str,
-        "packaging": ReportPackagingTypeType,
-        "encryptionKey": str,
-        "encryptionDisabled": bool,
-    },
-    total=False,
-)
-
 S3ReportExportConfigTypeDef = TypedDict(
     "S3ReportExportConfigTypeDef",
     {
         "bucket": str,
         "bucketOwner": str,
         "path": str,
         "packaging": ReportPackagingTypeType,
@@ -1392,25 +986,14 @@
     {
         "total": int,
         "statusCounts": Dict[str, int],
         "durationInNanoSeconds": int,
     },
 )
 
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
 RetryBuildBatchInputRequestTypeDef = TypedDict(
     "RetryBuildBatchInputRequestTypeDef",
     {
         "id": str,
         "idempotencyToken": str,
         "retryType": RetryBuildBatchTypeType,
     },
@@ -1459,62 +1042,162 @@
 class UpdateProjectVisibilityInputRequestTypeDef(
     _RequiredUpdateProjectVisibilityInputRequestTypeDef,
     _OptionalUpdateProjectVisibilityInputRequestTypeDef,
 ):
     pass
 
 
-UpdateProjectVisibilityOutputTypeDef = TypedDict(
-    "UpdateProjectVisibilityOutputTypeDef",
+BatchDeleteBuildsOutputTypeDef = TypedDict(
+    "BatchDeleteBuildsOutputTypeDef",
     {
-        "projectArn": str,
-        "publicProjectAlias": str,
-        "projectVisibility": ProjectVisibilityTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "buildsDeleted": List[str],
+        "buildsNotDeleted": List[BuildNotDeletedTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredWebhookFilterOutputTypeDef = TypedDict(
-    "_RequiredWebhookFilterOutputTypeDef",
+DeleteBuildBatchOutputTypeDef = TypedDict(
+    "DeleteBuildBatchOutputTypeDef",
     {
-        "type": WebhookFilterTypeType,
-        "pattern": str,
+        "statusCode": str,
+        "buildsDeleted": List[str],
+        "buildsNotDeleted": List[BuildNotDeletedTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalWebhookFilterOutputTypeDef = TypedDict(
-    "_OptionalWebhookFilterOutputTypeDef",
+
+DeleteSourceCredentialsOutputTypeDef = TypedDict(
+    "DeleteSourceCredentialsOutputTypeDef",
     {
-        "excludeMatchedPattern": bool,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetResourcePolicyOutputTypeDef = TypedDict(
+    "GetResourcePolicyOutputTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class WebhookFilterOutputTypeDef(
-    _RequiredWebhookFilterOutputTypeDef, _OptionalWebhookFilterOutputTypeDef
-):
-    pass
+ImportSourceCredentialsOutputTypeDef = TypedDict(
+    "ImportSourceCredentialsOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListBuildBatchesForProjectOutputTypeDef = TypedDict(
+    "ListBuildBatchesForProjectOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-BatchDeleteBuildsOutputTypeDef = TypedDict(
-    "BatchDeleteBuildsOutputTypeDef",
+ListBuildBatchesOutputTypeDef = TypedDict(
+    "ListBuildBatchesOutputTypeDef",
     {
-        "buildsDeleted": List[str],
-        "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteBuildBatchOutputTypeDef = TypedDict(
-    "DeleteBuildBatchOutputTypeDef",
+ListBuildsForProjectOutputTypeDef = TypedDict(
+    "ListBuildsForProjectOutputTypeDef",
     {
-        "statusCode": str,
-        "buildsDeleted": List[str],
-        "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildsOutputTypeDef = TypedDict(
+    "ListBuildsOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProjectsOutputTypeDef = TypedDict(
+    "ListProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportGroupsOutputTypeDef = TypedDict(
+    "ListReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportsForReportGroupOutputTypeDef = TypedDict(
+    "ListReportsForReportGroupOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportsOutputTypeDef = TypedDict(
+    "ListReportsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSharedProjectsOutputTypeDef = TypedDict(
+    "ListSharedProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSharedReportGroupsOutputTypeDef = TypedDict(
+    "ListSharedReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyOutputTypeDef = TypedDict(
+    "PutResourcePolicyOutputTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectVisibilityOutputTypeDef = TypedDict(
+    "UpdateProjectVisibilityOutputTypeDef",
+    {
+        "projectArn": str,
+        "publicProjectAlias": str,
+        "projectVisibility": ProjectVisibilityTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProjectBuildBatchConfigOutputTypeDef = TypedDict(
     "ProjectBuildBatchConfigOutputTypeDef",
     {
         "serviceRole": str,
@@ -1534,47 +1217,26 @@
         "restrictions": BatchRestrictionsTypeDef,
         "timeoutInMins": int,
         "batchReportMode": BatchReportModeTypeType,
     },
     total=False,
 )
 
-ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
-    {
-        "projectName": str,
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBuildBatchesForProjectInputRequestTypeDef = TypedDict(
     "ListBuildBatchesForProjectInputRequestTypeDef",
     {
         "projectName": str,
         "filter": BuildBatchFilterTypeDef,
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
-    {
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBuildBatchesInputRequestTypeDef = TypedDict(
     "ListBuildBatchesInputRequestTypeDef",
     {
         "filter": BuildBatchFilterTypeDef,
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
@@ -1621,15 +1283,15 @@
 )
 
 DescribeCodeCoveragesOutputTypeDef = TypedDict(
     "DescribeCodeCoveragesOutputTypeDef",
     {
         "nextToken": str,
         "codeCoverages": List[CodeCoverageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredCreateWebhookInputRequestTypeDef",
     {
         "projectName": str,
@@ -1672,25 +1334,158 @@
 
 class UpdateWebhookInputRequestTypeDef(
     _RequiredUpdateWebhookInputRequestTypeDef, _OptionalUpdateWebhookInputRequestTypeDef
 ):
     pass
 
 
+WebhookTypeDef = TypedDict(
+    "WebhookTypeDef",
+    {
+        "url": str,
+        "payloadUrl": str,
+        "secret": str,
+        "branchFilter": str,
+        "filterGroups": List[List[WebhookFilterTypeDef]],
+        "buildType": WebhookBuildTypeType,
+        "lastModifiedSecret": datetime,
+    },
+    total=False,
+)
+
+_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    {
+        "reportArn": str,
+    },
+)
+_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportCodeCoverageSortByTypeType,
+        "minLineCoveragePercentage": float,
+        "maxLineCoveragePercentage": float,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
+    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+):
+    pass
+
+
+ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
+    {
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
+    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+):
+    pass
+
+
+ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
+    "ListBuildsInputListBuildsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsInputListProjectsPaginateTypeDef",
+    {
+        "sortBy": ProjectSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportGroupSortByTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
+    {
+        "sortBy": SharedResourceSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": SharedResourceSortByTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "filter": TestCaseFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeTestCasesInputDescribeTestCasesPaginateTypeDef(
     _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
@@ -1723,15 +1518,15 @@
 
 
 DescribeTestCasesOutputTypeDef = TypedDict(
     "DescribeTestCasesOutputTypeDef",
     {
         "nextToken": str,
         "testCases": List[TestCaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentLanguageTypeDef = TypedDict(
     "EnvironmentLanguageTypeDef",
     {
         "language": LanguageTypeType,
@@ -1741,30 +1536,30 @@
 )
 
 GetReportGroupTrendOutputTypeDef = TypedDict(
     "GetReportGroupTrendOutputTypeDef",
     {
         "stats": ReportGroupTrendStatsTypeDef,
         "rawData": List[ReportWithRawDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "reportGroupArn": str,
     },
 )
 _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef(
     _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
@@ -1799,15 +1594,15 @@
 
 
 ListReportsInputListReportsPaginateTypeDef = TypedDict(
     "ListReportsInputListReportsPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListReportsInputRequestTypeDef = TypedDict(
     "ListReportsInputRequestTypeDef",
     {
@@ -1819,45 +1614,36 @@
     total=False,
 )
 
 ListSourceCredentialsOutputTypeDef = TypedDict(
     "ListSourceCredentialsOutputTypeDef",
     {
         "sourceCredentialsInfos": List[SourceCredentialsInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LogsConfigOutputTypeDef = TypedDict(
-    "LogsConfigOutputTypeDef",
+LogsConfigTypeDef = TypedDict(
+    "LogsConfigTypeDef",
     {
-        "cloudWatchLogs": CloudWatchLogsConfigOutputTypeDef,
-        "s3Logs": S3LogsConfigOutputTypeDef,
+        "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
+        "s3Logs": S3LogsConfigTypeDef,
     },
     total=False,
 )
 
 LogsLocationTypeDef = TypedDict(
     "LogsLocationTypeDef",
     {
         "groupName": str,
         "streamName": str,
         "deepLink": str,
         "s3DeepLink": str,
         "cloudWatchLogsArn": str,
         "s3LogsArn": str,
-        "cloudWatchLogs": CloudWatchLogsConfigOutputTypeDef,
-        "s3Logs": S3LogsConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-LogsConfigTypeDef = TypedDict(
-    "LogsConfigTypeDef",
-    {
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
         "s3Logs": S3LogsConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredProjectEnvironmentOutputTypeDef = TypedDict(
@@ -1867,18 +1653,18 @@
         "image": str,
         "computeType": ComputeTypeType,
     },
 )
 _OptionalProjectEnvironmentOutputTypeDef = TypedDict(
     "_OptionalProjectEnvironmentOutputTypeDef",
     {
-        "environmentVariables": List[EnvironmentVariableOutputTypeDef],
+        "environmentVariables": List[EnvironmentVariableTypeDef],
         "privilegedMode": bool,
         "certificate": str,
-        "registryCredential": RegistryCredentialOutputTypeDef,
+        "registryCredential": RegistryCredentialTypeDef,
         "imagePullCredentialsType": ImagePullCredentialsTypeType,
     },
     total=False,
 )
 
 
 class ProjectEnvironmentOutputTypeDef(
@@ -1910,43 +1696,14 @@
 
 class ProjectEnvironmentTypeDef(
     _RequiredProjectEnvironmentTypeDef, _OptionalProjectEnvironmentTypeDef
 ):
     pass
 
 
-_RequiredProjectSourceOutputTypeDef = TypedDict(
-    "_RequiredProjectSourceOutputTypeDef",
-    {
-        "type": SourceTypeType,
-    },
-)
-_OptionalProjectSourceOutputTypeDef = TypedDict(
-    "_OptionalProjectSourceOutputTypeDef",
-    {
-        "location": str,
-        "gitCloneDepth": int,
-        "gitSubmodulesConfig": GitSubmodulesConfigOutputTypeDef,
-        "buildspec": str,
-        "auth": SourceAuthOutputTypeDef,
-        "reportBuildStatus": bool,
-        "buildStatusConfig": BuildStatusConfigOutputTypeDef,
-        "insecureSsl": bool,
-        "sourceIdentifier": str,
-    },
-    total=False,
-)
-
-
-class ProjectSourceOutputTypeDef(
-    _RequiredProjectSourceOutputTypeDef, _OptionalProjectSourceOutputTypeDef
-):
-    pass
-
-
 _RequiredProjectSourceTypeDef = TypedDict(
     "_RequiredProjectSourceTypeDef",
     {
         "type": SourceTypeType,
     },
 )
 _OptionalProjectSourceTypeDef = TypedDict(
@@ -1966,58 +1723,51 @@
 )
 
 
 class ProjectSourceTypeDef(_RequiredProjectSourceTypeDef, _OptionalProjectSourceTypeDef):
     pass
 
 
-ReportExportConfigOutputTypeDef = TypedDict(
-    "ReportExportConfigOutputTypeDef",
-    {
-        "exportConfigType": ReportExportConfigTypeType,
-        "s3Destination": S3ReportExportConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ReportExportConfigTypeDef = TypedDict(
     "ReportExportConfigTypeDef",
     {
         "exportConfigType": ReportExportConfigTypeType,
         "s3Destination": S3ReportExportConfigTypeDef,
     },
     total=False,
 )
 
-WebhookTypeDef = TypedDict(
-    "WebhookTypeDef",
-    {
-        "url": str,
-        "payloadUrl": str,
-        "secret": str,
-        "branchFilter": str,
-        "filterGroups": List[List[WebhookFilterOutputTypeDef]],
-        "buildType": WebhookBuildTypeType,
-        "lastModifiedSecret": datetime,
-    },
-    total=False,
-)
-
 BuildGroupTypeDef = TypedDict(
     "BuildGroupTypeDef",
     {
         "identifier": str,
         "dependsOn": List[str],
         "ignoreFailure": bool,
         "currentBuildSummary": BuildSummaryTypeDef,
         "priorBuildSummaryList": List[BuildSummaryTypeDef],
     },
     total=False,
 )
 
+CreateWebhookOutputTypeDef = TypedDict(
+    "CreateWebhookOutputTypeDef",
+    {
+        "webhook": WebhookTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWebhookOutputTypeDef = TypedDict(
+    "UpdateWebhookOutputTypeDef",
+    {
+        "webhook": WebhookTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EnvironmentPlatformTypeDef = TypedDict(
     "EnvironmentPlatformTypeDef",
     {
         "platform": PlatformTypeType,
         "languages": List[EnvironmentLanguageTypeDef],
     },
     total=False,
@@ -2033,17 +1783,17 @@
         "endTime": datetime,
         "currentPhase": str,
         "buildStatus": StatusTypeType,
         "sourceVersion": str,
         "resolvedSourceVersion": str,
         "projectName": str,
         "phases": List[BuildPhaseTypeDef],
-        "source": ProjectSourceOutputTypeDef,
-        "secondarySources": List[ProjectSourceOutputTypeDef],
-        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
+        "source": ProjectSourceTypeDef,
+        "secondarySources": List[ProjectSourceTypeDef],
+        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
         "cache": ProjectCacheOutputTypeDef,
         "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
         "logs": LogsLocationTypeDef,
         "timeoutInMinutes": int,
@@ -2051,15 +1801,15 @@
         "buildComplete": bool,
         "initiator": str,
         "vpcConfig": VpcConfigOutputTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "encryptionKey": str,
         "exportedEnvironmentVariables": List[ExportedEnvironmentVariableTypeDef],
         "reportArns": List[str],
-        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
+        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
         "debugSession": DebugSessionTypeDef,
         "buildBatchArn": str,
     },
     total=False,
 )
 
 _RequiredCreateProjectInputRequestTypeDef = TypedDict(
@@ -2098,14 +1848,49 @@
 
 class CreateProjectInputRequestTypeDef(
     _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
 ):
     pass
 
 
+ProjectTypeDef = TypedDict(
+    "ProjectTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "source": ProjectSourceTypeDef,
+        "secondarySources": List[ProjectSourceTypeDef],
+        "sourceVersion": str,
+        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
+        "artifacts": ProjectArtifactsTypeDef,
+        "secondaryArtifacts": List[ProjectArtifactsTypeDef],
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
+        "serviceRole": str,
+        "timeoutInMinutes": int,
+        "queuedTimeoutInMinutes": int,
+        "encryptionKey": str,
+        "tags": List[TagTypeDef],
+        "created": datetime,
+        "lastModified": datetime,
+        "webhook": WebhookTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
+        "badge": ProjectBadgeTypeDef,
+        "logsConfig": LogsConfigTypeDef,
+        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
+        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
+        "concurrentBuildLimit": int,
+        "projectVisibility": ProjectVisibilityTypeType,
+        "publicProjectAlias": str,
+        "resourceAccessRole": str,
+    },
+    total=False,
+)
+
 _RequiredStartBuildBatchInputRequestTypeDef = TypedDict(
     "_RequiredStartBuildBatchInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalStartBuildBatchInputRequestTypeDef = TypedDict(
@@ -2238,24 +2023,47 @@
 
 class UpdateProjectInputRequestTypeDef(
     _RequiredUpdateProjectInputRequestTypeDef, _OptionalUpdateProjectInputRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateReportGroupInputRequestTypeDef",
+    {
+        "name": str,
+        "type": ReportTypeType,
+        "exportConfig": ReportExportConfigTypeDef,
+    },
+)
+_OptionalCreateReportGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateReportGroupInputRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateReportGroupInputRequestTypeDef(
+    _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
+):
+    pass
+
+
 ReportGroupTypeDef = TypedDict(
     "ReportGroupTypeDef",
     {
         "arn": str,
         "name": str,
         "type": ReportTypeType,
-        "exportConfig": ReportExportConfigOutputTypeDef,
+        "exportConfig": ReportExportConfigTypeDef,
         "created": datetime,
         "lastModified": datetime,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "status": ReportGroupStatusTypeType,
     },
     total=False,
 )
 
 ReportTypeDef = TypedDict(
     "ReportTypeDef",
@@ -2264,45 +2072,22 @@
         "type": ReportTypeType,
         "name": str,
         "reportGroupArn": str,
         "executionId": str,
         "status": ReportStatusTypeType,
         "created": datetime,
         "expired": datetime,
-        "exportConfig": ReportExportConfigOutputTypeDef,
+        "exportConfig": ReportExportConfigTypeDef,
         "truncated": bool,
         "testSummary": TestReportSummaryTypeDef,
         "codeCoverageSummary": CodeCoverageReportSummaryTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateReportGroupInputRequestTypeDef",
-    {
-        "name": str,
-        "type": ReportTypeType,
-        "exportConfig": ReportExportConfigTypeDef,
-    },
-)
-_OptionalCreateReportGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateReportGroupInputRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateReportGroupInputRequestTypeDef(
-    _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReportGroupInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateReportGroupInputRequestTypeDef = TypedDict(
@@ -2317,227 +2102,176 @@
 
 class UpdateReportGroupInputRequestTypeDef(
     _RequiredUpdateReportGroupInputRequestTypeDef, _OptionalUpdateReportGroupInputRequestTypeDef
 ):
     pass
 
 
-CreateWebhookOutputTypeDef = TypedDict(
-    "CreateWebhookOutputTypeDef",
-    {
-        "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ProjectTypeDef = TypedDict(
-    "ProjectTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "source": ProjectSourceOutputTypeDef,
-        "secondarySources": List[ProjectSourceOutputTypeDef],
-        "sourceVersion": str,
-        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
-        "artifacts": ProjectArtifactsOutputTypeDef,
-        "secondaryArtifacts": List[ProjectArtifactsOutputTypeDef],
-        "cache": ProjectCacheOutputTypeDef,
-        "environment": ProjectEnvironmentOutputTypeDef,
-        "serviceRole": str,
-        "timeoutInMinutes": int,
-        "queuedTimeoutInMinutes": int,
-        "encryptionKey": str,
-        "tags": List[TagOutputTypeDef],
-        "created": datetime,
-        "lastModified": datetime,
-        "webhook": WebhookTypeDef,
-        "vpcConfig": VpcConfigOutputTypeDef,
-        "badge": ProjectBadgeTypeDef,
-        "logsConfig": LogsConfigOutputTypeDef,
-        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
-        "concurrentBuildLimit": int,
-        "projectVisibility": ProjectVisibilityTypeType,
-        "publicProjectAlias": str,
-        "resourceAccessRole": str,
-    },
-    total=False,
-)
-
-UpdateWebhookOutputTypeDef = TypedDict(
-    "UpdateWebhookOutputTypeDef",
-    {
-        "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BuildBatchTypeDef = TypedDict(
     "BuildBatchTypeDef",
     {
         "id": str,
         "arn": str,
         "startTime": datetime,
         "endTime": datetime,
         "currentPhase": str,
         "buildBatchStatus": StatusTypeType,
         "sourceVersion": str,
         "resolvedSourceVersion": str,
         "projectName": str,
         "phases": List[BuildBatchPhaseTypeDef],
-        "source": ProjectSourceOutputTypeDef,
-        "secondarySources": List[ProjectSourceOutputTypeDef],
-        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
+        "source": ProjectSourceTypeDef,
+        "secondarySources": List[ProjectSourceTypeDef],
+        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
         "cache": ProjectCacheOutputTypeDef,
         "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
-        "logConfig": LogsConfigOutputTypeDef,
+        "logConfig": LogsConfigTypeDef,
         "buildTimeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "complete": bool,
         "initiator": str,
         "vpcConfig": VpcConfigOutputTypeDef,
         "encryptionKey": str,
         "buildBatchNumber": int,
-        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
+        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
         "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
         "buildGroups": List[BuildGroupTypeDef],
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
 ListCuratedEnvironmentImagesOutputTypeDef = TypedDict(
     "ListCuratedEnvironmentImagesOutputTypeDef",
     {
         "platforms": List[EnvironmentPlatformTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetBuildsOutputTypeDef = TypedDict(
     "BatchGetBuildsOutputTypeDef",
     {
         "builds": List[BuildTypeDef],
         "buildsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RetryBuildOutputTypeDef = TypedDict(
     "RetryBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBuildOutputTypeDef = TypedDict(
     "StartBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBuildOutputTypeDef = TypedDict(
     "StopBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchGetProjectsOutputTypeDef = TypedDict(
+    "BatchGetProjectsOutputTypeDef",
+    {
+        "projects": List[ProjectTypeDef],
+        "projectsNotFound": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectOutputTypeDef = TypedDict(
+    "CreateProjectOutputTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectOutputTypeDef = TypedDict(
+    "UpdateProjectOutputTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetReportGroupsOutputTypeDef = TypedDict(
     "BatchGetReportGroupsOutputTypeDef",
     {
         "reportGroups": List[ReportGroupTypeDef],
         "reportGroupsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReportGroupOutputTypeDef = TypedDict(
     "CreateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateReportGroupOutputTypeDef = TypedDict(
     "UpdateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetReportsOutputTypeDef = TypedDict(
     "BatchGetReportsOutputTypeDef",
     {
         "reports": List[ReportTypeDef],
         "reportsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchGetProjectsOutputTypeDef = TypedDict(
-    "BatchGetProjectsOutputTypeDef",
-    {
-        "projects": List[ProjectTypeDef],
-        "projectsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProjectOutputTypeDef = TypedDict(
-    "CreateProjectOutputTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateProjectOutputTypeDef = TypedDict(
-    "UpdateProjectOutputTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetBuildBatchesOutputTypeDef = TypedDict(
     "BatchGetBuildBatchesOutputTypeDef",
     {
         "buildBatches": List[BuildBatchTypeDef],
         "buildBatchesNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RetryBuildBatchOutputTypeDef = TypedDict(
     "RetryBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBuildBatchOutputTypeDef = TypedDict(
     "StartBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBuildBatchOutputTypeDef = TypedDict(
     "StopBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/type_defs.pyi` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -61,178 +61,162 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
     "BatchGetReportGroupsInputRequestTypeDef",
     "BatchGetReportsInputRequestTypeDef",
     "BatchRestrictionsOutputTypeDef",
     "BatchRestrictionsTypeDef",
     "BuildArtifactsTypeDef",
     "BuildBatchFilterTypeDef",
     "PhaseContextTypeDef",
     "ProjectCacheOutputTypeDef",
-    "ProjectFileSystemLocationOutputTypeDef",
-    "ProjectSourceVersionOutputTypeDef",
+    "ProjectFileSystemLocationTypeDef",
+    "ProjectSourceVersionTypeDef",
     "VpcConfigOutputTypeDef",
-    "BuildStatusConfigOutputTypeDef",
     "BuildStatusConfigTypeDef",
     "ResolvedArtifactTypeDef",
     "DebugSessionTypeDef",
     "ExportedEnvironmentVariableTypeDef",
     "NetworkInterfaceTypeDef",
-    "CloudWatchLogsConfigOutputTypeDef",
     "CloudWatchLogsConfigTypeDef",
     "CodeCoverageReportSummaryTypeDef",
     "CodeCoverageTypeDef",
     "ProjectArtifactsTypeDef",
     "ProjectCacheTypeDef",
-    "ProjectFileSystemLocationTypeDef",
-    "ProjectSourceVersionTypeDef",
     "TagTypeDef",
     "VpcConfigTypeDef",
     "WebhookFilterTypeDef",
     "DeleteBuildBatchInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteReportGroupInputRequestTypeDef",
     "DeleteReportInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteSourceCredentialsInputRequestTypeDef",
-    "DeleteSourceCredentialsOutputTypeDef",
     "DeleteWebhookInputRequestTypeDef",
-    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCodeCoveragesInputRequestTypeDef",
     "TestCaseFilterTypeDef",
     "TestCaseTypeDef",
     "EnvironmentImageTypeDef",
-    "EnvironmentVariableOutputTypeDef",
     "EnvironmentVariableTypeDef",
     "GetReportGroupTrendInputRequestTypeDef",
     "ReportGroupTrendStatsTypeDef",
     "ReportWithRawDataTypeDef",
     "GetResourcePolicyInputRequestTypeDef",
-    "GetResourcePolicyOutputTypeDef",
-    "GitSubmodulesConfigOutputTypeDef",
     "GitSubmodulesConfigTypeDef",
     "ImportSourceCredentialsInputRequestTypeDef",
-    "ImportSourceCredentialsOutputTypeDef",
     "InvalidateProjectCacheInputRequestTypeDef",
-    "ListBuildBatchesForProjectOutputTypeDef",
-    "ListBuildBatchesOutputTypeDef",
-    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
     "ListBuildsForProjectInputRequestTypeDef",
-    "ListBuildsForProjectOutputTypeDef",
-    "ListBuildsInputListBuildsPaginateTypeDef",
     "ListBuildsInputRequestTypeDef",
-    "ListBuildsOutputTypeDef",
-    "ListProjectsInputListProjectsPaginateTypeDef",
     "ListProjectsInputRequestTypeDef",
-    "ListProjectsOutputTypeDef",
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
     "ListReportGroupsInputRequestTypeDef",
-    "ListReportGroupsOutputTypeDef",
     "ReportFilterTypeDef",
-    "ListReportsForReportGroupOutputTypeDef",
-    "ListReportsOutputTypeDef",
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
     "ListSharedProjectsInputRequestTypeDef",
-    "ListSharedProjectsOutputTypeDef",
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "ListSharedReportGroupsInputRequestTypeDef",
-    "ListSharedReportGroupsOutputTypeDef",
     "SourceCredentialsInfoTypeDef",
-    "S3LogsConfigOutputTypeDef",
     "S3LogsConfigTypeDef",
-    "PaginatorConfigTypeDef",
-    "ProjectArtifactsOutputTypeDef",
     "ProjectBadgeTypeDef",
-    "RegistryCredentialOutputTypeDef",
     "RegistryCredentialTypeDef",
-    "SourceAuthOutputTypeDef",
     "SourceAuthTypeDef",
-    "TagOutputTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
-    "PutResourcePolicyOutputTypeDef",
-    "S3ReportExportConfigOutputTypeDef",
     "S3ReportExportConfigTypeDef",
     "TestReportSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryBuildBatchInputRequestTypeDef",
     "RetryBuildInputRequestTypeDef",
     "StopBuildBatchInputRequestTypeDef",
     "StopBuildInputRequestTypeDef",
     "UpdateProjectVisibilityInputRequestTypeDef",
-    "UpdateProjectVisibilityOutputTypeDef",
-    "WebhookFilterOutputTypeDef",
     "BatchDeleteBuildsOutputTypeDef",
     "DeleteBuildBatchOutputTypeDef",
+    "DeleteSourceCredentialsOutputTypeDef",
+    "GetResourcePolicyOutputTypeDef",
+    "ImportSourceCredentialsOutputTypeDef",
+    "ListBuildBatchesForProjectOutputTypeDef",
+    "ListBuildBatchesOutputTypeDef",
+    "ListBuildsForProjectOutputTypeDef",
+    "ListBuildsOutputTypeDef",
+    "ListProjectsOutputTypeDef",
+    "ListReportGroupsOutputTypeDef",
+    "ListReportsForReportGroupOutputTypeDef",
+    "ListReportsOutputTypeDef",
+    "ListSharedProjectsOutputTypeDef",
+    "ListSharedReportGroupsOutputTypeDef",
+    "PutResourcePolicyOutputTypeDef",
+    "UpdateProjectVisibilityOutputTypeDef",
     "ProjectBuildBatchConfigOutputTypeDef",
     "ProjectBuildBatchConfigTypeDef",
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
+    "WebhookTypeDef",
+    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
+    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    "ListBuildsInputListBuildsPaginateTypeDef",
+    "ListProjectsInputListProjectsPaginateTypeDef",
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "DescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     "DescribeTestCasesInputRequestTypeDef",
     "DescribeTestCasesOutputTypeDef",
     "EnvironmentLanguageTypeDef",
     "GetReportGroupTrendOutputTypeDef",
     "ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     "ListReportsForReportGroupInputRequestTypeDef",
     "ListReportsInputListReportsPaginateTypeDef",
     "ListReportsInputRequestTypeDef",
     "ListSourceCredentialsOutputTypeDef",
-    "LogsConfigOutputTypeDef",
-    "LogsLocationTypeDef",
     "LogsConfigTypeDef",
+    "LogsLocationTypeDef",
     "ProjectEnvironmentOutputTypeDef",
     "ProjectEnvironmentTypeDef",
-    "ProjectSourceOutputTypeDef",
     "ProjectSourceTypeDef",
-    "ReportExportConfigOutputTypeDef",
     "ReportExportConfigTypeDef",
-    "WebhookTypeDef",
     "BuildGroupTypeDef",
+    "CreateWebhookOutputTypeDef",
+    "UpdateWebhookOutputTypeDef",
     "EnvironmentPlatformTypeDef",
     "BuildTypeDef",
     "CreateProjectInputRequestTypeDef",
+    "ProjectTypeDef",
     "StartBuildBatchInputRequestTypeDef",
     "StartBuildInputRequestTypeDef",
     "UpdateProjectInputRequestTypeDef",
+    "CreateReportGroupInputRequestTypeDef",
     "ReportGroupTypeDef",
     "ReportTypeDef",
-    "CreateReportGroupInputRequestTypeDef",
     "UpdateReportGroupInputRequestTypeDef",
-    "CreateWebhookOutputTypeDef",
-    "ProjectTypeDef",
-    "UpdateWebhookOutputTypeDef",
     "BuildBatchTypeDef",
     "ListCuratedEnvironmentImagesOutputTypeDef",
     "BatchGetBuildsOutputTypeDef",
     "RetryBuildOutputTypeDef",
     "StartBuildOutputTypeDef",
     "StopBuildOutputTypeDef",
+    "BatchGetProjectsOutputTypeDef",
+    "CreateProjectOutputTypeDef",
+    "UpdateProjectOutputTypeDef",
     "BatchGetReportGroupsOutputTypeDef",
     "CreateReportGroupOutputTypeDef",
     "UpdateReportGroupOutputTypeDef",
     "BatchGetReportsOutputTypeDef",
-    "BatchGetProjectsOutputTypeDef",
-    "CreateProjectOutputTypeDef",
-    "UpdateProjectOutputTypeDef",
     "BatchGetBuildBatchesOutputTypeDef",
     "RetryBuildBatchOutputTypeDef",
     "StartBuildBatchOutputTypeDef",
     "StopBuildBatchOutputTypeDef",
 )
 
 BatchDeleteBuildsInputRequestTypeDef = TypedDict(
@@ -247,14 +231,25 @@
     {
         "id": str,
         "statusCode": str,
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
 BatchGetBuildBatchesInputRequestTypeDef = TypedDict(
     "BatchGetBuildBatchesInputRequestTypeDef",
     {
         "ids": Sequence[str],
     },
 )
 
@@ -351,28 +346,28 @@
 )
 
 class ProjectCacheOutputTypeDef(
     _RequiredProjectCacheOutputTypeDef, _OptionalProjectCacheOutputTypeDef
 ):
     pass
 
-ProjectFileSystemLocationOutputTypeDef = TypedDict(
-    "ProjectFileSystemLocationOutputTypeDef",
+ProjectFileSystemLocationTypeDef = TypedDict(
+    "ProjectFileSystemLocationTypeDef",
     {
         "type": Literal["EFS"],
         "location": str,
         "mountPoint": str,
         "identifier": str,
         "mountOptions": str,
     },
     total=False,
 )
 
-ProjectSourceVersionOutputTypeDef = TypedDict(
-    "ProjectSourceVersionOutputTypeDef",
+ProjectSourceVersionTypeDef = TypedDict(
+    "ProjectSourceVersionTypeDef",
     {
         "sourceIdentifier": str,
         "sourceVersion": str,
     },
 )
 
 VpcConfigOutputTypeDef = TypedDict(
@@ -381,23 +376,14 @@
         "vpcId": str,
         "subnets": List[str],
         "securityGroupIds": List[str],
     },
     total=False,
 )
 
-BuildStatusConfigOutputTypeDef = TypedDict(
-    "BuildStatusConfigOutputTypeDef",
-    {
-        "context": str,
-        "targetUrl": str,
-    },
-    total=False,
-)
-
 BuildStatusConfigTypeDef = TypedDict(
     "BuildStatusConfigTypeDef",
     {
         "context": str,
         "targetUrl": str,
     },
     total=False,
@@ -436,34 +422,14 @@
     {
         "subnetId": str,
         "networkInterfaceId": str,
     },
     total=False,
 )
 
-_RequiredCloudWatchLogsConfigOutputTypeDef = TypedDict(
-    "_RequiredCloudWatchLogsConfigOutputTypeDef",
-    {
-        "status": LogsConfigStatusTypeType,
-    },
-)
-_OptionalCloudWatchLogsConfigOutputTypeDef = TypedDict(
-    "_OptionalCloudWatchLogsConfigOutputTypeDef",
-    {
-        "groupName": str,
-        "streamName": str,
-    },
-    total=False,
-)
-
-class CloudWatchLogsConfigOutputTypeDef(
-    _RequiredCloudWatchLogsConfigOutputTypeDef, _OptionalCloudWatchLogsConfigOutputTypeDef
-):
-    pass
-
 _RequiredCloudWatchLogsConfigTypeDef = TypedDict(
     "_RequiredCloudWatchLogsConfigTypeDef",
     {
         "status": LogsConfigStatusTypeType,
     },
 )
 _OptionalCloudWatchLogsConfigTypeDef = TypedDict(
@@ -549,34 +515,14 @@
     },
     total=False,
 )
 
 class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
     pass
 
-ProjectFileSystemLocationTypeDef = TypedDict(
-    "ProjectFileSystemLocationTypeDef",
-    {
-        "type": Literal["EFS"],
-        "location": str,
-        "mountPoint": str,
-        "identifier": str,
-        "mountOptions": str,
-    },
-    total=False,
-)
-
-ProjectSourceVersionTypeDef = TypedDict(
-    "ProjectSourceVersionTypeDef",
-    {
-        "sourceIdentifier": str,
-        "sourceVersion": str,
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -660,53 +606,31 @@
 DeleteSourceCredentialsInputRequestTypeDef = TypedDict(
     "DeleteSourceCredentialsInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DeleteSourceCredentialsOutputTypeDef = TypedDict(
-    "DeleteSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWebhookInputRequestTypeDef = TypedDict(
     "DeleteWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
-    {
-        "reportArn": str,
-    },
-)
-_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportCodeCoverageSortByTypeType,
-        "minLineCoveragePercentage": float,
-        "maxLineCoveragePercentage": float,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
-    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeCodeCoveragesInputRequestTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
@@ -758,34 +682,14 @@
         "name": str,
         "description": str,
         "versions": List[str],
     },
     total=False,
 )
 
-_RequiredEnvironmentVariableOutputTypeDef = TypedDict(
-    "_RequiredEnvironmentVariableOutputTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-)
-_OptionalEnvironmentVariableOutputTypeDef = TypedDict(
-    "_OptionalEnvironmentVariableOutputTypeDef",
-    {
-        "type": EnvironmentVariableTypeType,
-    },
-    total=False,
-)
-
-class EnvironmentVariableOutputTypeDef(
-    _RequiredEnvironmentVariableOutputTypeDef, _OptionalEnvironmentVariableOutputTypeDef
-):
-    pass
-
 _RequiredEnvironmentVariableTypeDef = TypedDict(
     "_RequiredEnvironmentVariableTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
@@ -844,29 +748,14 @@
 GetResourcePolicyInputRequestTypeDef = TypedDict(
     "GetResourcePolicyInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetResourcePolicyOutputTypeDef = TypedDict(
-    "GetResourcePolicyOutputTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GitSubmodulesConfigOutputTypeDef = TypedDict(
-    "GitSubmodulesConfigOutputTypeDef",
-    {
-        "fetchSubmodules": bool,
-    },
-)
-
 GitSubmodulesConfigTypeDef = TypedDict(
     "GitSubmodulesConfigTypeDef",
     {
         "fetchSubmodules": bool,
     },
 )
 
@@ -889,68 +778,21 @@
 
 class ImportSourceCredentialsInputRequestTypeDef(
     _RequiredImportSourceCredentialsInputRequestTypeDef,
     _OptionalImportSourceCredentialsInputRequestTypeDef,
 ):
     pass
 
-ImportSourceCredentialsOutputTypeDef = TypedDict(
-    "ImportSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InvalidateProjectCacheInputRequestTypeDef = TypedDict(
     "InvalidateProjectCacheInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-ListBuildBatchesForProjectOutputTypeDef = TypedDict(
-    "ListBuildBatchesForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBuildBatchesOutputTypeDef = TypedDict(
-    "ListBuildBatchesOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
-    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-):
-    pass
-
 _RequiredListBuildsForProjectInputRequestTypeDef = TypedDict(
     "_RequiredListBuildsForProjectInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListBuildsForProjectInputRequestTypeDef = TypedDict(
@@ -964,226 +806,84 @@
 
 class ListBuildsForProjectInputRequestTypeDef(
     _RequiredListBuildsForProjectInputRequestTypeDef,
     _OptionalListBuildsForProjectInputRequestTypeDef,
 ):
     pass
 
-ListBuildsForProjectOutputTypeDef = TypedDict(
-    "ListBuildsForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
-    "ListBuildsInputListBuildsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBuildsInputRequestTypeDef = TypedDict(
     "ListBuildsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListBuildsOutputTypeDef = TypedDict(
-    "ListBuildsOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsInputListProjectsPaginateTypeDef",
-    {
-        "sortBy": ProjectSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsInputRequestTypeDef = TypedDict(
     "ListProjectsInputRequestTypeDef",
     {
         "sortBy": ProjectSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListProjectsOutputTypeDef = TypedDict(
-    "ListProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportGroupSortByTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReportGroupsInputRequestTypeDef = TypedDict(
     "ListReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": ReportGroupSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListReportGroupsOutputTypeDef = TypedDict(
-    "ListReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReportFilterTypeDef = TypedDict(
     "ReportFilterTypeDef",
     {
         "status": ReportStatusTypeType,
     },
     total=False,
 )
 
-ListReportsForReportGroupOutputTypeDef = TypedDict(
-    "ListReportsForReportGroupOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportsOutputTypeDef = TypedDict(
-    "ListReportsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
-    {
-        "sortBy": SharedResourceSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSharedProjectsInputRequestTypeDef = TypedDict(
     "ListSharedProjectsInputRequestTypeDef",
     {
         "sortBy": SharedResourceSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListSharedProjectsOutputTypeDef = TypedDict(
-    "ListSharedProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": SharedResourceSortByTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSharedReportGroupsInputRequestTypeDef = TypedDict(
     "ListSharedReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": SharedResourceSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListSharedReportGroupsOutputTypeDef = TypedDict(
-    "ListSharedReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SourceCredentialsInfoTypeDef = TypedDict(
     "SourceCredentialsInfoTypeDef",
     {
         "arn": str,
         "serverType": ServerTypeType,
         "authType": AuthTypeType,
     },
     total=False,
 )
 
-_RequiredS3LogsConfigOutputTypeDef = TypedDict(
-    "_RequiredS3LogsConfigOutputTypeDef",
-    {
-        "status": LogsConfigStatusTypeType,
-    },
-)
-_OptionalS3LogsConfigOutputTypeDef = TypedDict(
-    "_OptionalS3LogsConfigOutputTypeDef",
-    {
-        "location": str,
-        "encryptionDisabled": bool,
-        "bucketOwnerAccess": BucketOwnerAccessType,
-    },
-    total=False,
-)
-
-class S3LogsConfigOutputTypeDef(
-    _RequiredS3LogsConfigOutputTypeDef, _OptionalS3LogsConfigOutputTypeDef
-):
-    pass
-
 _RequiredS3LogsConfigTypeDef = TypedDict(
     "_RequiredS3LogsConfigTypeDef",
     {
         "status": LogsConfigStatusTypeType,
     },
 )
 _OptionalS3LogsConfigTypeDef = TypedDict(
@@ -1195,93 +895,31 @@
     },
     total=False,
 )
 
 class S3LogsConfigTypeDef(_RequiredS3LogsConfigTypeDef, _OptionalS3LogsConfigTypeDef):
     pass
 
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
-_RequiredProjectArtifactsOutputTypeDef = TypedDict(
-    "_RequiredProjectArtifactsOutputTypeDef",
-    {
-        "type": ArtifactsTypeType,
-    },
-)
-_OptionalProjectArtifactsOutputTypeDef = TypedDict(
-    "_OptionalProjectArtifactsOutputTypeDef",
-    {
-        "location": str,
-        "path": str,
-        "namespaceType": ArtifactNamespaceType,
-        "name": str,
-        "packaging": ArtifactPackagingType,
-        "overrideArtifactName": bool,
-        "encryptionDisabled": bool,
-        "artifactIdentifier": str,
-        "bucketOwnerAccess": BucketOwnerAccessType,
-    },
-    total=False,
-)
-
-class ProjectArtifactsOutputTypeDef(
-    _RequiredProjectArtifactsOutputTypeDef, _OptionalProjectArtifactsOutputTypeDef
-):
-    pass
-
 ProjectBadgeTypeDef = TypedDict(
     "ProjectBadgeTypeDef",
     {
         "badgeEnabled": bool,
         "badgeRequestUrl": str,
     },
     total=False,
 )
 
-RegistryCredentialOutputTypeDef = TypedDict(
-    "RegistryCredentialOutputTypeDef",
-    {
-        "credential": str,
-        "credentialProvider": Literal["SECRETS_MANAGER"],
-    },
-)
-
 RegistryCredentialTypeDef = TypedDict(
     "RegistryCredentialTypeDef",
     {
         "credential": str,
         "credentialProvider": Literal["SECRETS_MANAGER"],
     },
 )
 
-_RequiredSourceAuthOutputTypeDef = TypedDict(
-    "_RequiredSourceAuthOutputTypeDef",
-    {
-        "type": Literal["OAUTH"],
-    },
-)
-_OptionalSourceAuthOutputTypeDef = TypedDict(
-    "_OptionalSourceAuthOutputTypeDef",
-    {
-        "resource": str,
-    },
-    total=False,
-)
-
-class SourceAuthOutputTypeDef(_RequiredSourceAuthOutputTypeDef, _OptionalSourceAuthOutputTypeDef):
-    pass
-
 _RequiredSourceAuthTypeDef = TypedDict(
     "_RequiredSourceAuthTypeDef",
     {
         "type": Literal["OAUTH"],
     },
 )
 _OptionalSourceAuthTypeDef = TypedDict(
@@ -1291,52 +929,22 @@
     },
     total=False,
 )
 
 class SourceAuthTypeDef(_RequiredSourceAuthTypeDef, _OptionalSourceAuthTypeDef):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
 
-PutResourcePolicyOutputTypeDef = TypedDict(
-    "PutResourcePolicyOutputTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-S3ReportExportConfigOutputTypeDef = TypedDict(
-    "S3ReportExportConfigOutputTypeDef",
-    {
-        "bucket": str,
-        "bucketOwner": str,
-        "path": str,
-        "packaging": ReportPackagingTypeType,
-        "encryptionKey": str,
-        "encryptionDisabled": bool,
-    },
-    total=False,
-)
-
 S3ReportExportConfigTypeDef = TypedDict(
     "S3ReportExportConfigTypeDef",
     {
         "bucket": str,
         "bucketOwner": str,
         "path": str,
         "packaging": ReportPackagingTypeType,
@@ -1351,25 +959,14 @@
     {
         "total": int,
         "statusCounts": Dict[str, int],
         "durationInNanoSeconds": int,
     },
 )
 
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
 RetryBuildBatchInputRequestTypeDef = TypedDict(
     "RetryBuildBatchInputRequestTypeDef",
     {
         "id": str,
         "idempotencyToken": str,
         "retryType": RetryBuildBatchTypeType,
     },
@@ -1416,60 +1013,162 @@
 
 class UpdateProjectVisibilityInputRequestTypeDef(
     _RequiredUpdateProjectVisibilityInputRequestTypeDef,
     _OptionalUpdateProjectVisibilityInputRequestTypeDef,
 ):
     pass
 
-UpdateProjectVisibilityOutputTypeDef = TypedDict(
-    "UpdateProjectVisibilityOutputTypeDef",
+BatchDeleteBuildsOutputTypeDef = TypedDict(
+    "BatchDeleteBuildsOutputTypeDef",
     {
-        "projectArn": str,
-        "publicProjectAlias": str,
-        "projectVisibility": ProjectVisibilityTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "buildsDeleted": List[str],
+        "buildsNotDeleted": List[BuildNotDeletedTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredWebhookFilterOutputTypeDef = TypedDict(
-    "_RequiredWebhookFilterOutputTypeDef",
+DeleteBuildBatchOutputTypeDef = TypedDict(
+    "DeleteBuildBatchOutputTypeDef",
     {
-        "type": WebhookFilterTypeType,
-        "pattern": str,
+        "statusCode": str,
+        "buildsDeleted": List[str],
+        "buildsNotDeleted": List[BuildNotDeletedTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalWebhookFilterOutputTypeDef = TypedDict(
-    "_OptionalWebhookFilterOutputTypeDef",
+
+DeleteSourceCredentialsOutputTypeDef = TypedDict(
+    "DeleteSourceCredentialsOutputTypeDef",
     {
-        "excludeMatchedPattern": bool,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class WebhookFilterOutputTypeDef(
-    _RequiredWebhookFilterOutputTypeDef, _OptionalWebhookFilterOutputTypeDef
-):
-    pass
+GetResourcePolicyOutputTypeDef = TypedDict(
+    "GetResourcePolicyOutputTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-BatchDeleteBuildsOutputTypeDef = TypedDict(
-    "BatchDeleteBuildsOutputTypeDef",
+ImportSourceCredentialsOutputTypeDef = TypedDict(
+    "ImportSourceCredentialsOutputTypeDef",
     {
-        "buildsDeleted": List[str],
-        "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteBuildBatchOutputTypeDef = TypedDict(
-    "DeleteBuildBatchOutputTypeDef",
+ListBuildBatchesForProjectOutputTypeDef = TypedDict(
+    "ListBuildBatchesForProjectOutputTypeDef",
     {
-        "statusCode": str,
-        "buildsDeleted": List[str],
-        "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildBatchesOutputTypeDef = TypedDict(
+    "ListBuildBatchesOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildsForProjectOutputTypeDef = TypedDict(
+    "ListBuildsForProjectOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildsOutputTypeDef = TypedDict(
+    "ListBuildsOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProjectsOutputTypeDef = TypedDict(
+    "ListProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportGroupsOutputTypeDef = TypedDict(
+    "ListReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportsForReportGroupOutputTypeDef = TypedDict(
+    "ListReportsForReportGroupOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportsOutputTypeDef = TypedDict(
+    "ListReportsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSharedProjectsOutputTypeDef = TypedDict(
+    "ListSharedProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSharedReportGroupsOutputTypeDef = TypedDict(
+    "ListSharedReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyOutputTypeDef = TypedDict(
+    "PutResourcePolicyOutputTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectVisibilityOutputTypeDef = TypedDict(
+    "UpdateProjectVisibilityOutputTypeDef",
+    {
+        "projectArn": str,
+        "publicProjectAlias": str,
+        "projectVisibility": ProjectVisibilityTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProjectBuildBatchConfigOutputTypeDef = TypedDict(
     "ProjectBuildBatchConfigOutputTypeDef",
     {
         "serviceRole": str,
@@ -1489,47 +1188,26 @@
         "restrictions": BatchRestrictionsTypeDef,
         "timeoutInMins": int,
         "batchReportMode": BatchReportModeTypeType,
     },
     total=False,
 )
 
-ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
-    {
-        "projectName": str,
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBuildBatchesForProjectInputRequestTypeDef = TypedDict(
     "ListBuildBatchesForProjectInputRequestTypeDef",
     {
         "projectName": str,
         "filter": BuildBatchFilterTypeDef,
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
-    {
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBuildBatchesInputRequestTypeDef = TypedDict(
     "ListBuildBatchesInputRequestTypeDef",
     {
         "filter": BuildBatchFilterTypeDef,
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
@@ -1576,15 +1254,15 @@
 )
 
 DescribeCodeCoveragesOutputTypeDef = TypedDict(
     "DescribeCodeCoveragesOutputTypeDef",
     {
         "nextToken": str,
         "codeCoverages": List[CodeCoverageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredCreateWebhookInputRequestTypeDef",
     {
         "projectName": str,
@@ -1623,25 +1301,154 @@
 )
 
 class UpdateWebhookInputRequestTypeDef(
     _RequiredUpdateWebhookInputRequestTypeDef, _OptionalUpdateWebhookInputRequestTypeDef
 ):
     pass
 
+WebhookTypeDef = TypedDict(
+    "WebhookTypeDef",
+    {
+        "url": str,
+        "payloadUrl": str,
+        "secret": str,
+        "branchFilter": str,
+        "filterGroups": List[List[WebhookFilterTypeDef]],
+        "buildType": WebhookBuildTypeType,
+        "lastModifiedSecret": datetime,
+    },
+    total=False,
+)
+
+_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    {
+        "reportArn": str,
+    },
+)
+_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportCodeCoverageSortByTypeType,
+        "minLineCoveragePercentage": float,
+        "maxLineCoveragePercentage": float,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
+    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+):
+    pass
+
+ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
+    {
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
+    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+):
+    pass
+
+ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
+    "ListBuildsInputListBuildsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsInputListProjectsPaginateTypeDef",
+    {
+        "sortBy": ProjectSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportGroupSortByTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
+    {
+        "sortBy": SharedResourceSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": SharedResourceSortByTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "filter": TestCaseFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeTestCasesInputDescribeTestCasesPaginateTypeDef(
     _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
@@ -1670,15 +1477,15 @@
     pass
 
 DescribeTestCasesOutputTypeDef = TypedDict(
     "DescribeTestCasesOutputTypeDef",
     {
         "nextToken": str,
         "testCases": List[TestCaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentLanguageTypeDef = TypedDict(
     "EnvironmentLanguageTypeDef",
     {
         "language": LanguageTypeType,
@@ -1688,30 +1495,30 @@
 )
 
 GetReportGroupTrendOutputTypeDef = TypedDict(
     "GetReportGroupTrendOutputTypeDef",
     {
         "stats": ReportGroupTrendStatsTypeDef,
         "rawData": List[ReportWithRawDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "reportGroupArn": str,
     },
 )
 _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef(
     _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
@@ -1742,15 +1549,15 @@
     pass
 
 ListReportsInputListReportsPaginateTypeDef = TypedDict(
     "ListReportsInputListReportsPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListReportsInputRequestTypeDef = TypedDict(
     "ListReportsInputRequestTypeDef",
     {
@@ -1762,45 +1569,36 @@
     total=False,
 )
 
 ListSourceCredentialsOutputTypeDef = TypedDict(
     "ListSourceCredentialsOutputTypeDef",
     {
         "sourceCredentialsInfos": List[SourceCredentialsInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LogsConfigOutputTypeDef = TypedDict(
-    "LogsConfigOutputTypeDef",
+LogsConfigTypeDef = TypedDict(
+    "LogsConfigTypeDef",
     {
-        "cloudWatchLogs": CloudWatchLogsConfigOutputTypeDef,
-        "s3Logs": S3LogsConfigOutputTypeDef,
+        "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
+        "s3Logs": S3LogsConfigTypeDef,
     },
     total=False,
 )
 
 LogsLocationTypeDef = TypedDict(
     "LogsLocationTypeDef",
     {
         "groupName": str,
         "streamName": str,
         "deepLink": str,
         "s3DeepLink": str,
         "cloudWatchLogsArn": str,
         "s3LogsArn": str,
-        "cloudWatchLogs": CloudWatchLogsConfigOutputTypeDef,
-        "s3Logs": S3LogsConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-LogsConfigTypeDef = TypedDict(
-    "LogsConfigTypeDef",
-    {
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
         "s3Logs": S3LogsConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredProjectEnvironmentOutputTypeDef = TypedDict(
@@ -1810,18 +1608,18 @@
         "image": str,
         "computeType": ComputeTypeType,
     },
 )
 _OptionalProjectEnvironmentOutputTypeDef = TypedDict(
     "_OptionalProjectEnvironmentOutputTypeDef",
     {
-        "environmentVariables": List[EnvironmentVariableOutputTypeDef],
+        "environmentVariables": List[EnvironmentVariableTypeDef],
         "privilegedMode": bool,
         "certificate": str,
-        "registryCredential": RegistryCredentialOutputTypeDef,
+        "registryCredential": RegistryCredentialTypeDef,
         "imagePullCredentialsType": ImagePullCredentialsTypeType,
     },
     total=False,
 )
 
 class ProjectEnvironmentOutputTypeDef(
     _RequiredProjectEnvironmentOutputTypeDef, _OptionalProjectEnvironmentOutputTypeDef
@@ -1849,41 +1647,14 @@
 )
 
 class ProjectEnvironmentTypeDef(
     _RequiredProjectEnvironmentTypeDef, _OptionalProjectEnvironmentTypeDef
 ):
     pass
 
-_RequiredProjectSourceOutputTypeDef = TypedDict(
-    "_RequiredProjectSourceOutputTypeDef",
-    {
-        "type": SourceTypeType,
-    },
-)
-_OptionalProjectSourceOutputTypeDef = TypedDict(
-    "_OptionalProjectSourceOutputTypeDef",
-    {
-        "location": str,
-        "gitCloneDepth": int,
-        "gitSubmodulesConfig": GitSubmodulesConfigOutputTypeDef,
-        "buildspec": str,
-        "auth": SourceAuthOutputTypeDef,
-        "reportBuildStatus": bool,
-        "buildStatusConfig": BuildStatusConfigOutputTypeDef,
-        "insecureSsl": bool,
-        "sourceIdentifier": str,
-    },
-    total=False,
-)
-
-class ProjectSourceOutputTypeDef(
-    _RequiredProjectSourceOutputTypeDef, _OptionalProjectSourceOutputTypeDef
-):
-    pass
-
 _RequiredProjectSourceTypeDef = TypedDict(
     "_RequiredProjectSourceTypeDef",
     {
         "type": SourceTypeType,
     },
 )
 _OptionalProjectSourceTypeDef = TypedDict(
@@ -1901,58 +1672,51 @@
     },
     total=False,
 )
 
 class ProjectSourceTypeDef(_RequiredProjectSourceTypeDef, _OptionalProjectSourceTypeDef):
     pass
 
-ReportExportConfigOutputTypeDef = TypedDict(
-    "ReportExportConfigOutputTypeDef",
-    {
-        "exportConfigType": ReportExportConfigTypeType,
-        "s3Destination": S3ReportExportConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ReportExportConfigTypeDef = TypedDict(
     "ReportExportConfigTypeDef",
     {
         "exportConfigType": ReportExportConfigTypeType,
         "s3Destination": S3ReportExportConfigTypeDef,
     },
     total=False,
 )
 
-WebhookTypeDef = TypedDict(
-    "WebhookTypeDef",
-    {
-        "url": str,
-        "payloadUrl": str,
-        "secret": str,
-        "branchFilter": str,
-        "filterGroups": List[List[WebhookFilterOutputTypeDef]],
-        "buildType": WebhookBuildTypeType,
-        "lastModifiedSecret": datetime,
-    },
-    total=False,
-)
-
 BuildGroupTypeDef = TypedDict(
     "BuildGroupTypeDef",
     {
         "identifier": str,
         "dependsOn": List[str],
         "ignoreFailure": bool,
         "currentBuildSummary": BuildSummaryTypeDef,
         "priorBuildSummaryList": List[BuildSummaryTypeDef],
     },
     total=False,
 )
 
+CreateWebhookOutputTypeDef = TypedDict(
+    "CreateWebhookOutputTypeDef",
+    {
+        "webhook": WebhookTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWebhookOutputTypeDef = TypedDict(
+    "UpdateWebhookOutputTypeDef",
+    {
+        "webhook": WebhookTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EnvironmentPlatformTypeDef = TypedDict(
     "EnvironmentPlatformTypeDef",
     {
         "platform": PlatformTypeType,
         "languages": List[EnvironmentLanguageTypeDef],
     },
     total=False,
@@ -1968,17 +1732,17 @@
         "endTime": datetime,
         "currentPhase": str,
         "buildStatus": StatusTypeType,
         "sourceVersion": str,
         "resolvedSourceVersion": str,
         "projectName": str,
         "phases": List[BuildPhaseTypeDef],
-        "source": ProjectSourceOutputTypeDef,
-        "secondarySources": List[ProjectSourceOutputTypeDef],
-        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
+        "source": ProjectSourceTypeDef,
+        "secondarySources": List[ProjectSourceTypeDef],
+        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
         "cache": ProjectCacheOutputTypeDef,
         "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
         "logs": LogsLocationTypeDef,
         "timeoutInMinutes": int,
@@ -1986,15 +1750,15 @@
         "buildComplete": bool,
         "initiator": str,
         "vpcConfig": VpcConfigOutputTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "encryptionKey": str,
         "exportedEnvironmentVariables": List[ExportedEnvironmentVariableTypeDef],
         "reportArns": List[str],
-        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
+        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
         "debugSession": DebugSessionTypeDef,
         "buildBatchArn": str,
     },
     total=False,
 )
 
 _RequiredCreateProjectInputRequestTypeDef = TypedDict(
@@ -2031,14 +1795,49 @@
 )
 
 class CreateProjectInputRequestTypeDef(
     _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
 ):
     pass
 
+ProjectTypeDef = TypedDict(
+    "ProjectTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "source": ProjectSourceTypeDef,
+        "secondarySources": List[ProjectSourceTypeDef],
+        "sourceVersion": str,
+        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
+        "artifacts": ProjectArtifactsTypeDef,
+        "secondaryArtifacts": List[ProjectArtifactsTypeDef],
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
+        "serviceRole": str,
+        "timeoutInMinutes": int,
+        "queuedTimeoutInMinutes": int,
+        "encryptionKey": str,
+        "tags": List[TagTypeDef],
+        "created": datetime,
+        "lastModified": datetime,
+        "webhook": WebhookTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
+        "badge": ProjectBadgeTypeDef,
+        "logsConfig": LogsConfigTypeDef,
+        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
+        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
+        "concurrentBuildLimit": int,
+        "projectVisibility": ProjectVisibilityTypeType,
+        "publicProjectAlias": str,
+        "resourceAccessRole": str,
+    },
+    total=False,
+)
+
 _RequiredStartBuildBatchInputRequestTypeDef = TypedDict(
     "_RequiredStartBuildBatchInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalStartBuildBatchInputRequestTypeDef = TypedDict(
@@ -2165,24 +1964,45 @@
 )
 
 class UpdateProjectInputRequestTypeDef(
     _RequiredUpdateProjectInputRequestTypeDef, _OptionalUpdateProjectInputRequestTypeDef
 ):
     pass
 
+_RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateReportGroupInputRequestTypeDef",
+    {
+        "name": str,
+        "type": ReportTypeType,
+        "exportConfig": ReportExportConfigTypeDef,
+    },
+)
+_OptionalCreateReportGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateReportGroupInputRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateReportGroupInputRequestTypeDef(
+    _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
+):
+    pass
+
 ReportGroupTypeDef = TypedDict(
     "ReportGroupTypeDef",
     {
         "arn": str,
         "name": str,
         "type": ReportTypeType,
-        "exportConfig": ReportExportConfigOutputTypeDef,
+        "exportConfig": ReportExportConfigTypeDef,
         "created": datetime,
         "lastModified": datetime,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "status": ReportGroupStatusTypeType,
     },
     total=False,
 )
 
 ReportTypeDef = TypedDict(
     "ReportTypeDef",
@@ -2191,43 +2011,22 @@
         "type": ReportTypeType,
         "name": str,
         "reportGroupArn": str,
         "executionId": str,
         "status": ReportStatusTypeType,
         "created": datetime,
         "expired": datetime,
-        "exportConfig": ReportExportConfigOutputTypeDef,
+        "exportConfig": ReportExportConfigTypeDef,
         "truncated": bool,
         "testSummary": TestReportSummaryTypeDef,
         "codeCoverageSummary": CodeCoverageReportSummaryTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateReportGroupInputRequestTypeDef",
-    {
-        "name": str,
-        "type": ReportTypeType,
-        "exportConfig": ReportExportConfigTypeDef,
-    },
-)
-_OptionalCreateReportGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateReportGroupInputRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateReportGroupInputRequestTypeDef(
-    _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
-):
-    pass
-
 _RequiredUpdateReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReportGroupInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateReportGroupInputRequestTypeDef = TypedDict(
@@ -2240,227 +2039,176 @@
 )
 
 class UpdateReportGroupInputRequestTypeDef(
     _RequiredUpdateReportGroupInputRequestTypeDef, _OptionalUpdateReportGroupInputRequestTypeDef
 ):
     pass
 
-CreateWebhookOutputTypeDef = TypedDict(
-    "CreateWebhookOutputTypeDef",
-    {
-        "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ProjectTypeDef = TypedDict(
-    "ProjectTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "source": ProjectSourceOutputTypeDef,
-        "secondarySources": List[ProjectSourceOutputTypeDef],
-        "sourceVersion": str,
-        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
-        "artifacts": ProjectArtifactsOutputTypeDef,
-        "secondaryArtifacts": List[ProjectArtifactsOutputTypeDef],
-        "cache": ProjectCacheOutputTypeDef,
-        "environment": ProjectEnvironmentOutputTypeDef,
-        "serviceRole": str,
-        "timeoutInMinutes": int,
-        "queuedTimeoutInMinutes": int,
-        "encryptionKey": str,
-        "tags": List[TagOutputTypeDef],
-        "created": datetime,
-        "lastModified": datetime,
-        "webhook": WebhookTypeDef,
-        "vpcConfig": VpcConfigOutputTypeDef,
-        "badge": ProjectBadgeTypeDef,
-        "logsConfig": LogsConfigOutputTypeDef,
-        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
-        "concurrentBuildLimit": int,
-        "projectVisibility": ProjectVisibilityTypeType,
-        "publicProjectAlias": str,
-        "resourceAccessRole": str,
-    },
-    total=False,
-)
-
-UpdateWebhookOutputTypeDef = TypedDict(
-    "UpdateWebhookOutputTypeDef",
-    {
-        "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BuildBatchTypeDef = TypedDict(
     "BuildBatchTypeDef",
     {
         "id": str,
         "arn": str,
         "startTime": datetime,
         "endTime": datetime,
         "currentPhase": str,
         "buildBatchStatus": StatusTypeType,
         "sourceVersion": str,
         "resolvedSourceVersion": str,
         "projectName": str,
         "phases": List[BuildBatchPhaseTypeDef],
-        "source": ProjectSourceOutputTypeDef,
-        "secondarySources": List[ProjectSourceOutputTypeDef],
-        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
+        "source": ProjectSourceTypeDef,
+        "secondarySources": List[ProjectSourceTypeDef],
+        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
         "cache": ProjectCacheOutputTypeDef,
         "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
-        "logConfig": LogsConfigOutputTypeDef,
+        "logConfig": LogsConfigTypeDef,
         "buildTimeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "complete": bool,
         "initiator": str,
         "vpcConfig": VpcConfigOutputTypeDef,
         "encryptionKey": str,
         "buildBatchNumber": int,
-        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
+        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
         "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
         "buildGroups": List[BuildGroupTypeDef],
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
 ListCuratedEnvironmentImagesOutputTypeDef = TypedDict(
     "ListCuratedEnvironmentImagesOutputTypeDef",
     {
         "platforms": List[EnvironmentPlatformTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetBuildsOutputTypeDef = TypedDict(
     "BatchGetBuildsOutputTypeDef",
     {
         "builds": List[BuildTypeDef],
         "buildsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RetryBuildOutputTypeDef = TypedDict(
     "RetryBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBuildOutputTypeDef = TypedDict(
     "StartBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBuildOutputTypeDef = TypedDict(
     "StopBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchGetProjectsOutputTypeDef = TypedDict(
+    "BatchGetProjectsOutputTypeDef",
+    {
+        "projects": List[ProjectTypeDef],
+        "projectsNotFound": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectOutputTypeDef = TypedDict(
+    "CreateProjectOutputTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectOutputTypeDef = TypedDict(
+    "UpdateProjectOutputTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetReportGroupsOutputTypeDef = TypedDict(
     "BatchGetReportGroupsOutputTypeDef",
     {
         "reportGroups": List[ReportGroupTypeDef],
         "reportGroupsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReportGroupOutputTypeDef = TypedDict(
     "CreateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateReportGroupOutputTypeDef = TypedDict(
     "UpdateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetReportsOutputTypeDef = TypedDict(
     "BatchGetReportsOutputTypeDef",
     {
         "reports": List[ReportTypeDef],
         "reportsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchGetProjectsOutputTypeDef = TypedDict(
-    "BatchGetProjectsOutputTypeDef",
-    {
-        "projects": List[ProjectTypeDef],
-        "projectsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProjectOutputTypeDef = TypedDict(
-    "CreateProjectOutputTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateProjectOutputTypeDef = TypedDict(
-    "UpdateProjectOutputTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetBuildBatchesOutputTypeDef = TypedDict(
     "BatchGetBuildBatchesOutputTypeDef",
     {
         "buildBatches": List[BuildBatchTypeDef],
         "buildBatchesNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RetryBuildBatchOutputTypeDef = TypedDict(
     "RetryBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBuildBatchOutputTypeDef = TypedDict(
     "StartBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBuildBatchOutputTypeDef = TypedDict(
     "StopBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/PKG-INFO` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codebuild
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeBuild 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeBuild 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,178 +407,162 @@
 `mypy_boto3_codebuild.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
     BatchRestrictionsOutputTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
     BuildBatchFilterTypeDef,
     PhaseContextTypeDef,
     ProjectCacheOutputTypeDef,
-    ProjectFileSystemLocationOutputTypeDef,
-    ProjectSourceVersionOutputTypeDef,
+    ProjectFileSystemLocationTypeDef,
+    ProjectSourceVersionTypeDef,
     VpcConfigOutputTypeDef,
-    BuildStatusConfigOutputTypeDef,
     BuildStatusConfigTypeDef,
     ResolvedArtifactTypeDef,
     DebugSessionTypeDef,
     ExportedEnvironmentVariableTypeDef,
     NetworkInterfaceTypeDef,
-    CloudWatchLogsConfigOutputTypeDef,
     CloudWatchLogsConfigTypeDef,
     CodeCoverageReportSummaryTypeDef,
     CodeCoverageTypeDef,
     ProjectArtifactsTypeDef,
     ProjectCacheTypeDef,
-    ProjectFileSystemLocationTypeDef,
-    ProjectSourceVersionTypeDef,
     TagTypeDef,
     VpcConfigTypeDef,
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
-    DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
-    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
-    EnvironmentVariableOutputTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
-    GetResourcePolicyOutputTypeDef,
-    GitSubmodulesConfigOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
-    ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
-    ListBuildBatchesForProjectOutputTypeDef,
-    ListBuildBatchesOutputTypeDef,
-    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     ListBuildsForProjectInputRequestTypeDef,
-    ListBuildsForProjectOutputTypeDef,
-    ListBuildsInputListBuildsPaginateTypeDef,
     ListBuildsInputRequestTypeDef,
-    ListBuildsOutputTypeDef,
-    ListProjectsInputListProjectsPaginateTypeDef,
     ListProjectsInputRequestTypeDef,
-    ListProjectsOutputTypeDef,
-    ListReportGroupsInputListReportGroupsPaginateTypeDef,
     ListReportGroupsInputRequestTypeDef,
-    ListReportGroupsOutputTypeDef,
     ReportFilterTypeDef,
-    ListReportsForReportGroupOutputTypeDef,
-    ListReportsOutputTypeDef,
-    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
-    ListSharedProjectsOutputTypeDef,
-    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
-    ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
-    S3LogsConfigOutputTypeDef,
     S3LogsConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ProjectArtifactsOutputTypeDef,
     ProjectBadgeTypeDef,
-    RegistryCredentialOutputTypeDef,
     RegistryCredentialTypeDef,
-    SourceAuthOutputTypeDef,
     SourceAuthTypeDef,
-    TagOutputTypeDef,
     PutResourcePolicyInputRequestTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    S3ReportExportConfigOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
-    UpdateProjectVisibilityOutputTypeDef,
-    WebhookFilterOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
+    DeleteSourceCredentialsOutputTypeDef,
+    GetResourcePolicyOutputTypeDef,
+    ImportSourceCredentialsOutputTypeDef,
+    ListBuildBatchesForProjectOutputTypeDef,
+    ListBuildBatchesOutputTypeDef,
+    ListBuildsForProjectOutputTypeDef,
+    ListBuildsOutputTypeDef,
+    ListProjectsOutputTypeDef,
+    ListReportGroupsOutputTypeDef,
+    ListReportsForReportGroupOutputTypeDef,
+    ListReportsOutputTypeDef,
+    ListSharedProjectsOutputTypeDef,
+    ListSharedReportGroupsOutputTypeDef,
+    PutResourcePolicyOutputTypeDef,
+    UpdateProjectVisibilityOutputTypeDef,
     ProjectBuildBatchConfigOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
-    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
-    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
+    WebhookTypeDef,
+    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
+    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
+    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    ListBuildsInputListBuildsPaginateTypeDef,
+    ListProjectsInputListProjectsPaginateTypeDef,
+    ListReportGroupsInputListReportGroupsPaginateTypeDef,
+    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
+    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
     ListReportsInputListReportsPaginateTypeDef,
     ListReportsInputRequestTypeDef,
     ListSourceCredentialsOutputTypeDef,
-    LogsConfigOutputTypeDef,
-    LogsLocationTypeDef,
     LogsConfigTypeDef,
+    LogsLocationTypeDef,
     ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
-    ProjectSourceOutputTypeDef,
     ProjectSourceTypeDef,
-    ReportExportConfigOutputTypeDef,
     ReportExportConfigTypeDef,
-    WebhookTypeDef,
     BuildGroupTypeDef,
+    CreateWebhookOutputTypeDef,
+    UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
+    ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
+    CreateReportGroupInputRequestTypeDef,
     ReportGroupTypeDef,
     ReportTypeDef,
-    CreateReportGroupInputRequestTypeDef,
     UpdateReportGroupInputRequestTypeDef,
-    CreateWebhookOutputTypeDef,
-    ProjectTypeDef,
-    UpdateWebhookOutputTypeDef,
     BuildBatchTypeDef,
     ListCuratedEnvironmentImagesOutputTypeDef,
     BatchGetBuildsOutputTypeDef,
     RetryBuildOutputTypeDef,
     StartBuildOutputTypeDef,
     StopBuildOutputTypeDef,
+    BatchGetProjectsOutputTypeDef,
+    CreateProjectOutputTypeDef,
+    UpdateProjectOutputTypeDef,
     BatchGetReportGroupsOutputTypeDef,
     CreateReportGroupOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     BatchGetReportsOutputTypeDef,
-    BatchGetProjectsOutputTypeDef,
-    CreateProjectOutputTypeDef,
-    UpdateProjectOutputTypeDef,
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
```

### Comparing `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/SOURCES.txt` & `mypy-boto3-codebuild-1.28.15/mypy_boto3_codebuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.12/setup.py` & `mypy-boto3-codebuild-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codebuild",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_codebuild"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeBuild 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CodeBuild 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

