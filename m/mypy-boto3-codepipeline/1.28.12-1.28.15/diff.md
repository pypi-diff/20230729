# Comparing `tmp/mypy-boto3-codepipeline-1.28.12.tar.gz` & `tmp/mypy-boto3-codepipeline-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codepipeline-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
+gzip compressed data, was "mypy-boto3-codepipeline-1.28.15.tar", last modified: Fri Jul 28 20:42:31 2023, max compression
```

## Comparing `mypy-boto3-codepipeline-1.28.12.tar` & `mypy-boto3-codepipeline-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.160550 mypy-boto3-codepipeline-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-07-27 05:34:29.160550 mypy-boto3-codepipeline-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18628 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.160550 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32307 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32255 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10845 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56295 2023-07-27 05:19:13.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56216 2023-07-27 05:19:12.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.160550 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-07-27 05:34:28.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:29.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:28.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:28.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:28.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:28.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.160550 mypy-boto3-codepipeline-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.416865 mypy-boto3-codepipeline-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:39.000000 mypy-boto3-codepipeline-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-07-28 20:42:31.416865 mypy-boto3-codepipeline-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-07-28 20:21:39.000000 mypy-boto3-codepipeline-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.412865 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-28 20:21:39.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-28 20:21:39.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:21:39.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32307 2023-07-28 20:21:39.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32255 2023-07-28 20:21:39.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10845 2023-07-28 20:21:40.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-07-28 20:21:40.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-28 20:21:40.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-07-28 20:21:40.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:39.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51067 2023-07-28 20:21:42.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50996 2023-07-28 20:21:41.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:39.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.416865 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-07-28 20:42:31.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:31.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:31.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:31.000000 mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:31.416865 mypy-boto3-codepipeline-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:21:39.000000 mypy-boto3-codepipeline-1.28.15/setup.py
```

### Comparing `mypy-boto3-codepipeline-1.28.12/LICENSE` & `mypy-boto3-codepipeline-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.12/PKG-INFO` & `mypy-boto3-codepipeline-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.28.12
-Summary: Type annotations for boto3.CodePipeline 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodePipeline 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,135 +362,118 @@
 `mypy_boto3_codepipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
-    AcknowledgeJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
-    AcknowledgeThirdPartyJobOutputTypeDef,
-    ActionConfigurationPropertyOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
-    ActionTypeIdOutputTypeDef,
-    InputArtifactOutputTypeDef,
-    OutputArtifactOutputTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
     ActionRevisionOutputTypeDef,
     ActionRevisionTypeDef,
-    ActionTypeArtifactDetailsOutputTypeDef,
     ActionTypeArtifactDetailsTypeDef,
-    ActionTypeIdentifierOutputTypeDef,
-    ActionTypePermissionsOutputTypeDef,
-    ActionTypePropertyOutputTypeDef,
-    ActionTypeUrlsOutputTypeDef,
     ActionTypeIdentifierTypeDef,
-    ActionTypePermissionsTypeDef,
+    ActionTypePermissionsOutputTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
-    ActionTypeSettingsOutputTypeDef,
+    ActionTypePermissionsTypeDef,
     ActionTypeSettingsTypeDef,
-    ArtifactDetailsOutputTypeDef,
+    ArtifactDetailsTypeDef,
     ApprovalResultTypeDef,
     S3LocationTypeDef,
-    ArtifactDetailsTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
-    EncryptionKeyOutputTypeDef,
     EncryptionKeyTypeDef,
-    BlockerDeclarationOutputTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
-    TagOutputTypeDef,
     CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
     JobWorkerExecutorConfigurationOutputTypeDef,
-    LambdaExecutorConfigurationOutputTypeDef,
-    JobWorkerExecutorConfigurationTypeDef,
     LambdaExecutorConfigurationTypeDef,
+    JobWorkerExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
     PipelineMetadataTypeDef,
     GetPipelineStateInputRequestTypeDef,
     GetThirdPartyJobDetailsInputRequestTypeDef,
-    ListActionTypesInputListActionTypesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListActionTypesInputRequestTypeDef,
-    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
     ListPipelineExecutionsInputRequestTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineSummaryTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListWebhooksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     StageContextTypeDef,
     SourceRevisionTypeDef,
     StopExecutionTriggerTypeDef,
     ThirdPartyJobTypeDef,
-    PutActionRevisionOutputTypeDef,
-    PutApprovalResultOutputTypeDef,
     RegisterWebhookWithThirdPartyInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetryStageExecutionInputRequestTypeDef,
-    RetryStageExecutionOutputTypeDef,
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
-    StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
-    StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
-    WebhookAuthConfigurationOutputTypeDef,
     WebhookAuthConfigurationTypeDef,
-    WebhookFilterRuleOutputTypeDef,
     WebhookFilterRuleTypeDef,
-    ActionDeclarationOutputTypeDef,
+    AcknowledgeJobOutputTypeDef,
+    AcknowledgeThirdPartyJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PutActionRevisionOutputTypeDef,
+    PutApprovalResultOutputTypeDef,
+    RetryStageExecutionOutputTypeDef,
+    StartPipelineExecutionOutputTypeDef,
+    StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
+    ActionDeclarationOutputTypeDef,
     ActionDeclarationTypeDef,
-    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
     PutActionRevisionInputRequestTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
-    ArtifactStoreOutputTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
+    TagResourceInputRequestTypeDef,
     PutJobSuccessResultInputRequestTypeDef,
     PutThirdPartyJobSuccessResultInputRequestTypeDef,
     ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
+    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    ListActionTypesInputListActionTypesPaginateTypeDef,
+    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
     StageDeclarationOutputTypeDef,
```

### Comparing `mypy-boto3-codepipeline-1.28.12/README.md` & `mypy-boto3-codepipeline-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,135 +330,118 @@
 `mypy_boto3_codepipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
-    AcknowledgeJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
-    AcknowledgeThirdPartyJobOutputTypeDef,
-    ActionConfigurationPropertyOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
-    ActionTypeIdOutputTypeDef,
-    InputArtifactOutputTypeDef,
-    OutputArtifactOutputTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
     ActionRevisionOutputTypeDef,
     ActionRevisionTypeDef,
-    ActionTypeArtifactDetailsOutputTypeDef,
     ActionTypeArtifactDetailsTypeDef,
-    ActionTypeIdentifierOutputTypeDef,
-    ActionTypePermissionsOutputTypeDef,
-    ActionTypePropertyOutputTypeDef,
-    ActionTypeUrlsOutputTypeDef,
     ActionTypeIdentifierTypeDef,
-    ActionTypePermissionsTypeDef,
+    ActionTypePermissionsOutputTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
-    ActionTypeSettingsOutputTypeDef,
+    ActionTypePermissionsTypeDef,
     ActionTypeSettingsTypeDef,
-    ArtifactDetailsOutputTypeDef,
+    ArtifactDetailsTypeDef,
     ApprovalResultTypeDef,
     S3LocationTypeDef,
-    ArtifactDetailsTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
-    EncryptionKeyOutputTypeDef,
     EncryptionKeyTypeDef,
-    BlockerDeclarationOutputTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
-    TagOutputTypeDef,
     CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
     JobWorkerExecutorConfigurationOutputTypeDef,
-    LambdaExecutorConfigurationOutputTypeDef,
-    JobWorkerExecutorConfigurationTypeDef,
     LambdaExecutorConfigurationTypeDef,
+    JobWorkerExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
     PipelineMetadataTypeDef,
     GetPipelineStateInputRequestTypeDef,
     GetThirdPartyJobDetailsInputRequestTypeDef,
-    ListActionTypesInputListActionTypesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListActionTypesInputRequestTypeDef,
-    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
     ListPipelineExecutionsInputRequestTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineSummaryTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListWebhooksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     StageContextTypeDef,
     SourceRevisionTypeDef,
     StopExecutionTriggerTypeDef,
     ThirdPartyJobTypeDef,
-    PutActionRevisionOutputTypeDef,
-    PutApprovalResultOutputTypeDef,
     RegisterWebhookWithThirdPartyInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetryStageExecutionInputRequestTypeDef,
-    RetryStageExecutionOutputTypeDef,
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
-    StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
-    StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
-    WebhookAuthConfigurationOutputTypeDef,
     WebhookAuthConfigurationTypeDef,
-    WebhookFilterRuleOutputTypeDef,
     WebhookFilterRuleTypeDef,
-    ActionDeclarationOutputTypeDef,
+    AcknowledgeJobOutputTypeDef,
+    AcknowledgeThirdPartyJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PutActionRevisionOutputTypeDef,
+    PutApprovalResultOutputTypeDef,
+    RetryStageExecutionOutputTypeDef,
+    StartPipelineExecutionOutputTypeDef,
+    StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
+    ActionDeclarationOutputTypeDef,
     ActionDeclarationTypeDef,
-    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
     PutActionRevisionInputRequestTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
-    ArtifactStoreOutputTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
+    TagResourceInputRequestTypeDef,
     PutJobSuccessResultInputRequestTypeDef,
     PutThirdPartyJobSuccessResultInputRequestTypeDef,
     ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
+    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    ListActionTypesInputListActionTypesPaginateTypeDef,
+    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
     StageDeclarationOutputTypeDef,
```

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__init__.py` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__init__.pyi` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__main__.py` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodePipeline 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodePipeline 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline\nOther"
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

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/client.py` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/client.pyi` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/literals.py` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/literals.pyi` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/paginator.py` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     """
 
     def paginate(
         self,
         *,
         pipelineName: str,
         filter: ActionExecutionFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListActionExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listactionexecutionspaginator)
         """
 
 
@@ -91,73 +91,73 @@
     """
 
     def paginate(
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         regionFilter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListActionTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listactiontypespaginator)
         """
 
 
 class ListPipelineExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
     """
 
     def paginate(
-        self, *, pipelineName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pipelineName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipelineExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
         """
 
 
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelinespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListWebhooksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listwebhookspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWebhooksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listwebhookspaginator)
         """
```

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/paginator.pyi` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     """
 
     def paginate(
         self,
         *,
         pipelineName: str,
         filter: ActionExecutionFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListActionExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listactionexecutionspaginator)
         """
 
 class ListActionTypesPaginator(Paginator):
@@ -87,69 +87,69 @@
     """
 
     def paginate(
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         regionFilter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListActionTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listactiontypespaginator)
         """
 
 class ListPipelineExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
     """
 
     def paginate(
-        self, *, pipelineName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pipelineName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipelineExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelineexecutionspaginator)
         """
 
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listpipelinespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listtagsforresourcepaginator)
         """
 
 class ListWebhooksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listwebhookspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWebhooksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/paginators/#listwebhookspaginator)
         """
```

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/type_defs.py` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -36,139 +36,121 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AWSSessionCredentialsTypeDef",
     "AcknowledgeJobInputRequestTypeDef",
-    "AcknowledgeJobOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
-    "AcknowledgeThirdPartyJobOutputTypeDef",
-    "ActionConfigurationPropertyOutputTypeDef",
     "ActionConfigurationPropertyTypeDef",
     "ActionConfigurationTypeDef",
     "ActionContextTypeDef",
-    "ActionTypeIdOutputTypeDef",
-    "InputArtifactOutputTypeDef",
-    "OutputArtifactOutputTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ErrorDetailsTypeDef",
     "ActionRevisionOutputTypeDef",
     "ActionRevisionTypeDef",
-    "ActionTypeArtifactDetailsOutputTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
-    "ActionTypeIdentifierOutputTypeDef",
-    "ActionTypePermissionsOutputTypeDef",
-    "ActionTypePropertyOutputTypeDef",
-    "ActionTypeUrlsOutputTypeDef",
     "ActionTypeIdentifierTypeDef",
-    "ActionTypePermissionsTypeDef",
+    "ActionTypePermissionsOutputTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
-    "ActionTypeSettingsOutputTypeDef",
+    "ActionTypePermissionsTypeDef",
     "ActionTypeSettingsTypeDef",
-    "ArtifactDetailsOutputTypeDef",
+    "ArtifactDetailsTypeDef",
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
-    "ArtifactDetailsTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
-    "EncryptionKeyOutputTypeDef",
     "EncryptionKeyTypeDef",
-    "BlockerDeclarationOutputTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
-    "TagOutputTypeDef",
     "CurrentRevisionTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
     "JobWorkerExecutorConfigurationOutputTypeDef",
-    "LambdaExecutorConfigurationOutputTypeDef",
-    "JobWorkerExecutorConfigurationTypeDef",
     "LambdaExecutorConfigurationTypeDef",
+    "JobWorkerExecutorConfigurationTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
     "PipelineMetadataTypeDef",
     "GetPipelineStateInputRequestTypeDef",
     "GetThirdPartyJobDetailsInputRequestTypeDef",
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListActionTypesInputRequestTypeDef",
-    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     "ListPipelineExecutionsInputRequestTypeDef",
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineSummaryTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListWebhooksInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "StageContextTypeDef",
     "SourceRevisionTypeDef",
     "StopExecutionTriggerTypeDef",
     "ThirdPartyJobTypeDef",
-    "PutActionRevisionOutputTypeDef",
-    "PutApprovalResultOutputTypeDef",
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryStageExecutionInputRequestTypeDef",
-    "RetryStageExecutionOutputTypeDef",
     "StageExecutionTypeDef",
     "TransitionStateTypeDef",
     "StartPipelineExecutionInputRequestTypeDef",
-    "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionInputRequestTypeDef",
-    "StopPipelineExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "WebhookAuthConfigurationOutputTypeDef",
     "WebhookAuthConfigurationTypeDef",
-    "WebhookFilterRuleOutputTypeDef",
     "WebhookFilterRuleTypeDef",
-    "ActionDeclarationOutputTypeDef",
+    "AcknowledgeJobOutputTypeDef",
+    "AcknowledgeThirdPartyJobOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "PutActionRevisionOutputTypeDef",
+    "PutApprovalResultOutputTypeDef",
+    "RetryStageExecutionOutputTypeDef",
+    "StartPipelineExecutionOutputTypeDef",
+    "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
+    "ActionDeclarationOutputTypeDef",
     "ActionDeclarationTypeDef",
-    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
     "PutActionRevisionInputRequestTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "PipelineExecutionTypeDef",
-    "ArtifactStoreOutputTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
-    "TagResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "TagResourceInputRequestTypeDef",
     "PutJobSuccessResultInputRequestTypeDef",
     "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "ExecutorConfigurationOutputTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
+    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
+    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
     "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
     "StageDeclarationOutputTypeDef",
@@ -225,66 +207,34 @@
     "AcknowledgeJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
     },
 )
 
-AcknowledgeJobOutputTypeDef = TypedDict(
-    "AcknowledgeJobOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "status": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AcknowledgeThirdPartyJobInputRequestTypeDef = TypedDict(
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
         "clientToken": str,
     },
 )
 
-AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
-    "AcknowledgeThirdPartyJobOutputTypeDef",
-    {
-        "status": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredActionConfigurationPropertyOutputTypeDef = TypedDict(
-    "_RequiredActionConfigurationPropertyOutputTypeDef",
-    {
-        "name": str,
-        "required": bool,
-        "key": bool,
-        "secret": bool,
-    },
-)
-_OptionalActionConfigurationPropertyOutputTypeDef = TypedDict(
-    "_OptionalActionConfigurationPropertyOutputTypeDef",
-    {
-        "queryable": bool,
-        "description": str,
-        "type": ActionConfigurationPropertyTypeType,
-    },
-    total=False,
-)
-
-
-class ActionConfigurationPropertyOutputTypeDef(
-    _RequiredActionConfigurationPropertyOutputTypeDef,
-    _OptionalActionConfigurationPropertyOutputTypeDef,
-):
-    pass
-
-
 _RequiredActionConfigurationPropertyTypeDef = TypedDict(
     "_RequiredActionConfigurationPropertyTypeDef",
     {
         "name": str,
         "required": bool,
         "key": bool,
         "secret": bool,
@@ -296,21 +246,19 @@
         "queryable": bool,
         "description": str,
         "type": ActionConfigurationPropertyTypeType,
     },
     total=False,
 )
 
-
 class ActionConfigurationPropertyTypeDef(
     _RequiredActionConfigurationPropertyTypeDef, _OptionalActionConfigurationPropertyTypeDef
 ):
     pass
 
-
 ActionConfigurationTypeDef = TypedDict(
     "ActionConfigurationTypeDef",
     {
         "configuration": Dict[str, str],
     },
     total=False,
 )
@@ -320,38 +268,14 @@
     {
         "name": str,
         "actionExecutionId": str,
     },
     total=False,
 )
 
-ActionTypeIdOutputTypeDef = TypedDict(
-    "ActionTypeIdOutputTypeDef",
-    {
-        "category": ActionCategoryType,
-        "owner": ActionOwnerType,
-        "provider": str,
-        "version": str,
-    },
-)
-
-InputArtifactOutputTypeDef = TypedDict(
-    "InputArtifactOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-
-OutputArtifactOutputTypeDef = TypedDict(
-    "OutputArtifactOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-
 ActionTypeIdTypeDef = TypedDict(
     "ActionTypeIdTypeDef",
     {
         "category": ActionCategoryType,
         "owner": ActionOwnerType,
         "provider": str,
         "version": str,
@@ -413,32 +337,24 @@
     {
         "revisionId": str,
         "revisionChangeId": str,
         "created": Union[datetime, str],
     },
 )
 
-ActionTypeArtifactDetailsOutputTypeDef = TypedDict(
-    "ActionTypeArtifactDetailsOutputTypeDef",
-    {
-        "minimumCount": int,
-        "maximumCount": int,
-    },
-)
-
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
 
-ActionTypeIdentifierOutputTypeDef = TypedDict(
-    "ActionTypeIdentifierOutputTypeDef",
+ActionTypeIdentifierTypeDef = TypedDict(
+    "ActionTypeIdentifierTypeDef",
     {
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
     },
 )
@@ -446,67 +362,14 @@
 ActionTypePermissionsOutputTypeDef = TypedDict(
     "ActionTypePermissionsOutputTypeDef",
     {
         "allowedAccounts": List[str],
     },
 )
 
-_RequiredActionTypePropertyOutputTypeDef = TypedDict(
-    "_RequiredActionTypePropertyOutputTypeDef",
-    {
-        "name": str,
-        "optional": bool,
-        "key": bool,
-        "noEcho": bool,
-    },
-)
-_OptionalActionTypePropertyOutputTypeDef = TypedDict(
-    "_OptionalActionTypePropertyOutputTypeDef",
-    {
-        "queryable": bool,
-        "description": str,
-    },
-    total=False,
-)
-
-
-class ActionTypePropertyOutputTypeDef(
-    _RequiredActionTypePropertyOutputTypeDef, _OptionalActionTypePropertyOutputTypeDef
-):
-    pass
-
-
-ActionTypeUrlsOutputTypeDef = TypedDict(
-    "ActionTypeUrlsOutputTypeDef",
-    {
-        "configurationUrl": str,
-        "entityUrlTemplate": str,
-        "executionUrlTemplate": str,
-        "revisionUrlTemplate": str,
-    },
-    total=False,
-)
-
-ActionTypeIdentifierTypeDef = TypedDict(
-    "ActionTypeIdentifierTypeDef",
-    {
-        "category": ActionCategoryType,
-        "owner": str,
-        "provider": str,
-        "version": str,
-    },
-)
-
-ActionTypePermissionsTypeDef = TypedDict(
-    "ActionTypePermissionsTypeDef",
-    {
-        "allowedAccounts": Sequence[str],
-    },
-)
-
 _RequiredActionTypePropertyTypeDef = TypedDict(
     "_RequiredActionTypePropertyTypeDef",
     {
         "name": str,
         "optional": bool,
         "key": bool,
         "noEcho": bool,
@@ -517,56 +380,50 @@
     {
         "queryable": bool,
         "description": str,
     },
     total=False,
 )
 
-
 class ActionTypePropertyTypeDef(
     _RequiredActionTypePropertyTypeDef, _OptionalActionTypePropertyTypeDef
 ):
     pass
 
-
 ActionTypeUrlsTypeDef = TypedDict(
     "ActionTypeUrlsTypeDef",
     {
         "configurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
-ActionTypeSettingsOutputTypeDef = TypedDict(
-    "ActionTypeSettingsOutputTypeDef",
+ActionTypePermissionsTypeDef = TypedDict(
+    "ActionTypePermissionsTypeDef",
     {
-        "thirdPartyConfigurationUrl": str,
-        "entityUrlTemplate": str,
-        "executionUrlTemplate": str,
-        "revisionUrlTemplate": str,
+        "allowedAccounts": Sequence[str],
     },
-    total=False,
 )
 
 ActionTypeSettingsTypeDef = TypedDict(
     "ActionTypeSettingsTypeDef",
     {
         "thirdPartyConfigurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
-ArtifactDetailsOutputTypeDef = TypedDict(
-    "ArtifactDetailsOutputTypeDef",
+ArtifactDetailsTypeDef = TypedDict(
+    "ArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
 
 ApprovalResultTypeDef = TypedDict(
@@ -582,22 +439,14 @@
     {
         "bucket": str,
         "key": str,
     },
     total=False,
 )
 
-ArtifactDetailsTypeDef = TypedDict(
-    "ArtifactDetailsTypeDef",
-    {
-        "minimumCount": int,
-        "maximumCount": int,
-    },
-)
-
 S3ArtifactLocationTypeDef = TypedDict(
     "S3ArtifactLocationTypeDef",
     {
         "bucketName": str,
         "objectKey": str,
     },
 )
@@ -611,38 +460,22 @@
         "revisionSummary": str,
         "created": datetime,
         "revisionUrl": str,
     },
     total=False,
 )
 
-EncryptionKeyOutputTypeDef = TypedDict(
-    "EncryptionKeyOutputTypeDef",
-    {
-        "id": str,
-        "type": Literal["KMS"],
-    },
-)
-
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "id": str,
         "type": Literal["KMS"],
     },
 )
 
-BlockerDeclarationOutputTypeDef = TypedDict(
-    "BlockerDeclarationOutputTypeDef",
-    {
-        "name": str,
-        "type": Literal["Schedule"],
-    },
-)
-
 BlockerDeclarationTypeDef = TypedDict(
     "BlockerDeclarationTypeDef",
     {
         "name": str,
         "type": Literal["Schedule"],
     },
 )
@@ -651,22 +484,14 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 _RequiredCurrentRevisionTypeDef = TypedDict(
     "_RequiredCurrentRevisionTypeDef",
     {
         "revision": str,
         "changeIdentifier": str,
     },
 )
@@ -675,19 +500,17 @@
     {
         "created": Union[datetime, str],
         "revisionSummary": str,
     },
     total=False,
 )
 
-
 class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
     pass
 
-
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -721,21 +544,14 @@
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
         "reason": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableStageTransitionInputRequestTypeDef = TypedDict(
     "EnableStageTransitionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
     },
@@ -765,37 +581,30 @@
     {
         "pollingAccounts": List[str],
         "pollingServicePrincipals": List[str],
     },
     total=False,
 )
 
-LambdaExecutorConfigurationOutputTypeDef = TypedDict(
-    "LambdaExecutorConfigurationOutputTypeDef",
+LambdaExecutorConfigurationTypeDef = TypedDict(
+    "LambdaExecutorConfigurationTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
 
 JobWorkerExecutorConfigurationTypeDef = TypedDict(
     "JobWorkerExecutorConfigurationTypeDef",
     {
         "pollingAccounts": Sequence[str],
         "pollingServicePrincipals": Sequence[str],
     },
     total=False,
 )
 
-LambdaExecutorConfigurationTypeDef = TypedDict(
-    "LambdaExecutorConfigurationTypeDef",
-    {
-        "lambdaFunctionArn": str,
-    },
-)
-
 _RequiredFailureDetailsTypeDef = TypedDict(
     "_RequiredFailureDetailsTypeDef",
     {
         "type": FailureTypeType,
         "message": str,
     },
 )
@@ -803,19 +612,17 @@
     "_OptionalFailureDetailsTypeDef",
     {
         "externalExecutionId": str,
     },
     total=False,
 )
 
-
 class FailureDetailsTypeDef(_RequiredFailureDetailsTypeDef, _OptionalFailureDetailsTypeDef):
     pass
 
-
 GetActionTypeInputRequestTypeDef = TypedDict(
     "GetActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
@@ -847,21 +654,19 @@
     "_OptionalGetPipelineInputRequestTypeDef",
     {
         "version": int,
     },
     total=False,
 )
 
-
 class GetPipelineInputRequestTypeDef(
     _RequiredGetPipelineInputRequestTypeDef, _OptionalGetPipelineInputRequestTypeDef
 ):
     pass
 
-
 PipelineMetadataTypeDef = TypedDict(
     "PipelineMetadataTypeDef",
     {
         "pipelineArn": str,
         "created": datetime,
         "updated": datetime,
         "pollingDisabledAt": datetime,
@@ -880,56 +685,34 @@
     "GetThirdPartyJobDetailsInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
 
-ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "actionOwnerFilter": ActionOwnerType,
-        "regionFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListActionTypesInputRequestTypeDef = TypedDict(
     "ListActionTypesInputRequestTypeDef",
     {
         "actionOwnerFilter": ActionOwnerType,
         "nextToken": str,
         "regionFilter": str,
     },
     total=False,
 )
 
-_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
-    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPipelineExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListPipelineExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 _OptionalListPipelineExecutionsInputRequestTypeDef = TypedDict(
@@ -937,30 +720,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListPipelineExecutionsInputRequestTypeDef(
     _RequiredListPipelineExecutionsInputRequestTypeDef,
     _OptionalListPipelineExecutionsInputRequestTypeDef,
 ):
     pass
 
-
-ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -973,36 +746,14 @@
         "version": int,
         "created": datetime,
         "updated": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1010,48 +761,28 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-
-ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWebhooksInputRequestTypeDef = TypedDict(
     "ListWebhooksInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
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
 StageContextTypeDef = TypedDict(
     "StageContextTypeDef",
     {
         "name": str,
     },
     total=False,
 )
@@ -1068,19 +799,17 @@
         "revisionId": str,
         "revisionSummary": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
-
 class SourceRevisionTypeDef(_RequiredSourceRevisionTypeDef, _OptionalSourceRevisionTypeDef):
     pass
 
-
 StopExecutionTriggerTypeDef = TypedDict(
     "StopExecutionTriggerTypeDef",
     {
         "reason": str,
     },
     total=False,
 )
@@ -1090,68 +819,32 @@
     {
         "clientId": str,
         "jobId": str,
     },
     total=False,
 )
 
-PutActionRevisionOutputTypeDef = TypedDict(
-    "PutActionRevisionOutputTypeDef",
-    {
-        "newRevision": bool,
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutApprovalResultOutputTypeDef = TypedDict(
-    "PutApprovalResultOutputTypeDef",
-    {
-        "approvedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterWebhookWithThirdPartyInputRequestTypeDef = TypedDict(
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
     {
         "webhookName": str,
     },
     total=False,
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
 RetryStageExecutionInputRequestTypeDef = TypedDict(
     "RetryStageExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "pipelineExecutionId": str,
         "retryMode": Literal["FAILED_ACTIONS"],
     },
 )
 
-RetryStageExecutionOutputTypeDef = TypedDict(
-    "RetryStageExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StageExecutionTypeDef = TypedDict(
     "StageExecutionTypeDef",
     {
         "pipelineExecutionId": str,
         "status": StageExecutionStatusType,
     },
 )
@@ -1177,30 +870,20 @@
     "_OptionalStartPipelineExecutionInputRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class StartPipelineExecutionInputRequestTypeDef(
     _RequiredStartPipelineExecutionInputRequestTypeDef,
     _OptionalStartPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
-
-StartPipelineExecutionOutputTypeDef = TypedDict(
-    "StartPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopPipelineExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStopPipelineExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "pipelineExecutionId": str,
     },
 )
@@ -1209,125 +892,119 @@
     {
         "abandon": bool,
         "reason": str,
     },
     total=False,
 )
 
-
 class StopPipelineExecutionInputRequestTypeDef(
     _RequiredStopPipelineExecutionInputRequestTypeDef,
     _OptionalStopPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
-
-StopPipelineExecutionOutputTypeDef = TypedDict(
-    "StopPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-WebhookAuthConfigurationOutputTypeDef = TypedDict(
-    "WebhookAuthConfigurationOutputTypeDef",
-    {
-        "AllowedIPRange": str,
-        "SecretToken": str,
-    },
-    total=False,
-)
-
 WebhookAuthConfigurationTypeDef = TypedDict(
     "WebhookAuthConfigurationTypeDef",
     {
         "AllowedIPRange": str,
         "SecretToken": str,
     },
     total=False,
 )
 
-_RequiredWebhookFilterRuleOutputTypeDef = TypedDict(
-    "_RequiredWebhookFilterRuleOutputTypeDef",
+_RequiredWebhookFilterRuleTypeDef = TypedDict(
+    "_RequiredWebhookFilterRuleTypeDef",
     {
         "jsonPath": str,
     },
 )
-_OptionalWebhookFilterRuleOutputTypeDef = TypedDict(
-    "_OptionalWebhookFilterRuleOutputTypeDef",
+_OptionalWebhookFilterRuleTypeDef = TypedDict(
+    "_OptionalWebhookFilterRuleTypeDef",
     {
         "matchEquals": str,
     },
     total=False,
 )
 
-
-class WebhookFilterRuleOutputTypeDef(
-    _RequiredWebhookFilterRuleOutputTypeDef, _OptionalWebhookFilterRuleOutputTypeDef
+class WebhookFilterRuleTypeDef(
+    _RequiredWebhookFilterRuleTypeDef, _OptionalWebhookFilterRuleTypeDef
 ):
     pass
 
-
-_RequiredWebhookFilterRuleTypeDef = TypedDict(
-    "_RequiredWebhookFilterRuleTypeDef",
+AcknowledgeJobOutputTypeDef = TypedDict(
+    "AcknowledgeJobOutputTypeDef",
     {
-        "jsonPath": str,
+        "status": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalWebhookFilterRuleTypeDef = TypedDict(
-    "_OptionalWebhookFilterRuleTypeDef",
+
+AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
+    "AcknowledgeThirdPartyJobOutputTypeDef",
     {
-        "matchEquals": str,
+        "status": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class WebhookFilterRuleTypeDef(
-    _RequiredWebhookFilterRuleTypeDef, _OptionalWebhookFilterRuleTypeDef
-):
-    pass
-
-
-_RequiredActionDeclarationOutputTypeDef = TypedDict(
-    "_RequiredActionDeclarationOutputTypeDef",
+PutActionRevisionOutputTypeDef = TypedDict(
+    "PutActionRevisionOutputTypeDef",
     {
-        "name": str,
-        "actionTypeId": ActionTypeIdOutputTypeDef,
+        "newRevision": bool,
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalActionDeclarationOutputTypeDef = TypedDict(
-    "_OptionalActionDeclarationOutputTypeDef",
+
+PutApprovalResultOutputTypeDef = TypedDict(
+    "PutApprovalResultOutputTypeDef",
     {
-        "runOrder": int,
-        "configuration": Dict[str, str],
-        "outputArtifacts": List[OutputArtifactOutputTypeDef],
-        "inputArtifacts": List[InputArtifactOutputTypeDef],
-        "roleArn": str,
-        "region": str,
-        "namespace": str,
+        "approvedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+RetryStageExecutionOutputTypeDef = TypedDict(
+    "RetryStageExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ActionDeclarationOutputTypeDef(
-    _RequiredActionDeclarationOutputTypeDef, _OptionalActionDeclarationOutputTypeDef
-):
-    pass
+StartPipelineExecutionOutputTypeDef = TypedDict(
+    "StartPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+StopPipelineExecutionOutputTypeDef = TypedDict(
+    "StopPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredPollForJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
@@ -1336,94 +1013,91 @@
     {
         "maxBatchSize": int,
         "queryParam": Mapping[str, str],
     },
     total=False,
 )
 
-
 class PollForJobsInputRequestTypeDef(
     _RequiredPollForJobsInputRequestTypeDef, _OptionalPollForJobsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPollForThirdPartyJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForThirdPartyJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
 _OptionalPollForThirdPartyJobsInputRequestTypeDef = TypedDict(
     "_OptionalPollForThirdPartyJobsInputRequestTypeDef",
     {
         "maxBatchSize": int,
     },
     total=False,
 )
 
-
 class PollForThirdPartyJobsInputRequestTypeDef(
     _RequiredPollForThirdPartyJobsInputRequestTypeDef,
     _OptionalPollForThirdPartyJobsInputRequestTypeDef,
 ):
     pass
 
-
-_RequiredActionDeclarationTypeDef = TypedDict(
-    "_RequiredActionDeclarationTypeDef",
+_RequiredActionDeclarationOutputTypeDef = TypedDict(
+    "_RequiredActionDeclarationOutputTypeDef",
     {
         "name": str,
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
-_OptionalActionDeclarationTypeDef = TypedDict(
-    "_OptionalActionDeclarationTypeDef",
+_OptionalActionDeclarationOutputTypeDef = TypedDict(
+    "_OptionalActionDeclarationOutputTypeDef",
     {
         "runOrder": int,
-        "configuration": Mapping[str, str],
-        "outputArtifacts": Sequence[OutputArtifactTypeDef],
-        "inputArtifacts": Sequence[InputArtifactTypeDef],
+        "configuration": Dict[str, str],
+        "outputArtifacts": List[OutputArtifactTypeDef],
+        "inputArtifacts": List[InputArtifactTypeDef],
         "roleArn": str,
         "region": str,
         "namespace": str,
     },
     total=False,
 )
 
-
-class ActionDeclarationTypeDef(
-    _RequiredActionDeclarationTypeDef, _OptionalActionDeclarationTypeDef
+class ActionDeclarationOutputTypeDef(
+    _RequiredActionDeclarationOutputTypeDef, _OptionalActionDeclarationOutputTypeDef
 ):
     pass
 
-
-_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+_RequiredActionDeclarationTypeDef = TypedDict(
+    "_RequiredActionDeclarationTypeDef",
     {
-        "pipelineName": str,
+        "name": str,
+        "actionTypeId": ActionTypeIdTypeDef,
     },
 )
-_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+_OptionalActionDeclarationTypeDef = TypedDict(
+    "_OptionalActionDeclarationTypeDef",
     {
-        "filter": ActionExecutionFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "runOrder": int,
+        "configuration": Mapping[str, str],
+        "outputArtifacts": Sequence[OutputArtifactTypeDef],
+        "inputArtifacts": Sequence[InputArtifactTypeDef],
+        "roleArn": str,
+        "region": str,
+        "namespace": str,
     },
     total=False,
 )
 
-
-class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
-    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+class ActionDeclarationTypeDef(
+    _RequiredActionDeclarationTypeDef, _OptionalActionDeclarationTypeDef
 ):
     pass
 
-
 _RequiredListActionExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListActionExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 _OptionalListActionExecutionsInputRequestTypeDef = TypedDict(
@@ -1432,22 +1106,20 @@
         "filter": ActionExecutionFilterTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListActionExecutionsInputRequestTypeDef(
     _RequiredListActionExecutionsInputRequestTypeDef,
     _OptionalListActionExecutionsInputRequestTypeDef,
 ):
     pass
 
-
 ActionExecutionTypeDef = TypedDict(
     "ActionExecutionTypeDef",
     {
         "actionExecutionId": str,
         "status": ActionExecutionStatusType,
         "summary": str,
         "lastStatusChange": datetime,
@@ -1470,33 +1142,31 @@
         "actionRevision": ActionRevisionTypeDef,
     },
 )
 
 _RequiredActionTypeTypeDef = TypedDict(
     "_RequiredActionTypeTypeDef",
     {
-        "id": ActionTypeIdOutputTypeDef,
-        "inputArtifactDetails": ArtifactDetailsOutputTypeDef,
-        "outputArtifactDetails": ArtifactDetailsOutputTypeDef,
+        "id": ActionTypeIdTypeDef,
+        "inputArtifactDetails": ArtifactDetailsTypeDef,
+        "outputArtifactDetails": ArtifactDetailsTypeDef,
     },
 )
 _OptionalActionTypeTypeDef = TypedDict(
     "_OptionalActionTypeTypeDef",
     {
-        "settings": ActionTypeSettingsOutputTypeDef,
-        "actionConfigurationProperties": List[ActionConfigurationPropertyOutputTypeDef],
+        "settings": ActionTypeSettingsTypeDef,
+        "actionConfigurationProperties": List[ActionConfigurationPropertyTypeDef],
     },
     total=False,
 )
 
-
 class ActionTypeTypeDef(_RequiredActionTypeTypeDef, _OptionalActionTypeTypeDef):
     pass
 
-
 PutApprovalResultInputRequestTypeDef = TypedDict(
     "PutApprovalResultInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "actionName": str,
         "result": ApprovalResultTypeDef,
@@ -1531,36 +1201,14 @@
         "status": PipelineExecutionStatusType,
         "statusSummary": str,
         "artifactRevisions": List[ArtifactRevisionTypeDef],
     },
     total=False,
 )
 
-_RequiredArtifactStoreOutputTypeDef = TypedDict(
-    "_RequiredArtifactStoreOutputTypeDef",
-    {
-        "type": Literal["S3"],
-        "location": str,
-    },
-)
-_OptionalArtifactStoreOutputTypeDef = TypedDict(
-    "_OptionalArtifactStoreOutputTypeDef",
-    {
-        "encryptionKey": EncryptionKeyOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ArtifactStoreOutputTypeDef(
-    _RequiredArtifactStoreOutputTypeDef, _OptionalArtifactStoreOutputTypeDef
-):
-    pass
-
-
 _RequiredArtifactStoreTypeDef = TypedDict(
     "_RequiredArtifactStoreTypeDef",
     {
         "type": Literal["S3"],
         "location": str,
     },
 )
@@ -1568,19 +1216,17 @@
     "_OptionalArtifactStoreTypeDef",
     {
         "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
-
 class ArtifactStoreTypeDef(_RequiredArtifactStoreTypeDef, _OptionalArtifactStoreTypeDef):
     pass
 
-
 _RequiredCreateCustomActionTypeInputRequestTypeDef = TypedDict(
     "_RequiredCreateCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
@@ -1593,39 +1239,37 @@
         "settings": ActionTypeSettingsTypeDef,
         "configurationProperties": Sequence[ActionConfigurationPropertyTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCustomActionTypeInputRequestTypeDef(
     _RequiredCreateCustomActionTypeInputRequestTypeDef,
     _OptionalCreateCustomActionTypeInputRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
     "_RequiredPutJobSuccessResultInputRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
@@ -1635,21 +1279,19 @@
         "continuationToken": str,
         "executionDetails": ExecutionDetailsTypeDef,
         "outputVariables": Mapping[str, str],
     },
     total=False,
 )
 
-
 class PutJobSuccessResultInputRequestTypeDef(
     _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
     "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
@@ -1659,26 +1301,24 @@
         "currentRevision": CurrentRevisionTypeDef,
         "continuationToken": str,
         "executionDetails": ExecutionDetailsTypeDef,
     },
     total=False,
 )
 
-
 class PutThirdPartyJobSuccessResultInputRequestTypeDef(
     _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
     _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
 ):
     pass
 
-
 ExecutorConfigurationOutputTypeDef = TypedDict(
     "ExecutorConfigurationOutputTypeDef",
     {
-        "lambdaExecutorConfiguration": LambdaExecutorConfigurationOutputTypeDef,
+        "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
         "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 ExecutorConfigurationTypeDef = TypedDict(
     "ExecutorConfigurationTypeDef",
@@ -1702,20 +1342,107 @@
     {
         "jobId": str,
         "clientToken": str,
         "failureDetails": FailureDetailsTypeDef,
     },
 )
 
+_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "filter": ActionExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
+    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+):
+    pass
+
+ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
+    {
+        "actionOwnerFilter": ActionOwnerType,
+        "regionFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
+    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+):
+    pass
+
+ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelines": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PipelineContextTypeDef = TypedDict(
     "PipelineContextTypeDef",
     {
         "pipelineName": str,
@@ -1741,27 +1468,27 @@
     total=False,
 )
 
 PollForThirdPartyJobsOutputTypeDef = TypedDict(
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WebhookDefinitionOutputTypeDef = TypedDict(
     "WebhookDefinitionOutputTypeDef",
     {
         "name": str,
         "targetPipeline": str,
         "targetAction": str,
-        "filters": List[WebhookFilterRuleOutputTypeDef],
+        "filters": List[WebhookFilterRuleTypeDef],
         "authentication": WebhookAuthenticationTypeType,
-        "authenticationConfiguration": WebhookAuthConfigurationOutputTypeDef,
+        "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
 
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
@@ -1779,26 +1506,24 @@
         "name": str,
         "actions": List[ActionDeclarationOutputTypeDef],
     },
 )
 _OptionalStageDeclarationOutputTypeDef = TypedDict(
     "_OptionalStageDeclarationOutputTypeDef",
     {
-        "blockers": List[BlockerDeclarationOutputTypeDef],
+        "blockers": List[BlockerDeclarationTypeDef],
     },
     total=False,
 )
 
-
 class StageDeclarationOutputTypeDef(
     _RequiredStageDeclarationOutputTypeDef, _OptionalStageDeclarationOutputTypeDef
 ):
     pass
 
-
 _RequiredStageDeclarationTypeDef = TypedDict(
     "_RequiredStageDeclarationTypeDef",
     {
         "name": str,
         "actions": Sequence[ActionDeclarationTypeDef],
     },
 )
@@ -1806,19 +1531,17 @@
     "_OptionalStageDeclarationTypeDef",
     {
         "blockers": Sequence[BlockerDeclarationTypeDef],
     },
     total=False,
 )
 
-
 class StageDeclarationTypeDef(_RequiredStageDeclarationTypeDef, _OptionalStageDeclarationTypeDef):
     pass
 
-
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": str,
         "currentRevision": ActionRevisionOutputTypeDef,
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
@@ -1827,32 +1550,32 @@
     total=False,
 )
 
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListActionTypesOutputTypeDef = TypedDict(
     "ListActionTypesOutputTypeDef",
     {
         "actionTypes": List[ActionTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActionExecutionInputTypeDef = TypedDict(
     "ActionExecutionInputTypeDef",
     {
-        "actionTypeId": ActionTypeIdOutputTypeDef,
+        "actionTypeId": ActionTypeIdTypeDef,
         "configuration": Dict[str, str],
         "resolvedConfiguration": Dict[str, str],
         "roleArn": str,
         "region": str,
         "inputArtifacts": List[ArtifactDetailTypeDef],
         "namespace": str,
     },
@@ -1879,15 +1602,15 @@
     total=False,
 )
 
 GetPipelineExecutionOutputTypeDef = TypedDict(
     "GetPipelineExecutionOutputTypeDef",
     {
         "pipelineExecution": PipelineExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredActionTypeExecutorOutputTypeDef = TypedDict(
     "_RequiredActionTypeExecutorOutputTypeDef",
     {
         "configuration": ExecutorConfigurationOutputTypeDef,
@@ -1899,21 +1622,19 @@
     {
         "policyStatementsTemplate": str,
         "jobTimeout": int,
     },
     total=False,
 )
 
-
 class ActionTypeExecutorOutputTypeDef(
     _RequiredActionTypeExecutorOutputTypeDef, _OptionalActionTypeExecutorOutputTypeDef
 ):
     pass
 
-
 _RequiredActionTypeExecutorTypeDef = TypedDict(
     "_RequiredActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
         "type": ExecutorTypeType,
     },
 )
@@ -1922,27 +1643,25 @@
     {
         "policyStatementsTemplate": str,
         "jobTimeout": int,
     },
     total=False,
 )
 
-
 class ActionTypeExecutorTypeDef(
     _RequiredActionTypeExecutorTypeDef, _OptionalActionTypeExecutorTypeDef
 ):
     pass
 
-
 ListPipelineExecutionsOutputTypeDef = TypedDict(
     "ListPipelineExecutionsOutputTypeDef",
     {
         "pipelineExecutionSummaries": List[PipelineExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListWebhookItemTypeDef = TypedDict(
     "_RequiredListWebhookItemTypeDef",
     {
         "definition": WebhookDefinitionOutputTypeDef,
@@ -1952,70 +1671,64 @@
 _OptionalListWebhookItemTypeDef = TypedDict(
     "_OptionalListWebhookItemTypeDef",
     {
         "errorMessage": str,
         "errorCode": str,
         "lastTriggered": datetime,
         "arn": str,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class ListWebhookItemTypeDef(_RequiredListWebhookItemTypeDef, _OptionalListWebhookItemTypeDef):
     pass
 
-
 _RequiredPutWebhookInputRequestTypeDef = TypedDict(
     "_RequiredPutWebhookInputRequestTypeDef",
     {
         "webhook": WebhookDefinitionTypeDef,
     },
 )
 _OptionalPutWebhookInputRequestTypeDef = TypedDict(
     "_OptionalPutWebhookInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPipelineDeclarationOutputTypeDef = TypedDict(
     "_RequiredPipelineDeclarationOutputTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": List[StageDeclarationOutputTypeDef],
     },
 )
 _OptionalPipelineDeclarationOutputTypeDef = TypedDict(
     "_OptionalPipelineDeclarationOutputTypeDef",
     {
-        "artifactStore": ArtifactStoreOutputTypeDef,
-        "artifactStores": Dict[str, ArtifactStoreOutputTypeDef],
+        "artifactStore": ArtifactStoreTypeDef,
+        "artifactStores": Dict[str, ArtifactStoreTypeDef],
         "version": int,
     },
     total=False,
 )
 
-
 class PipelineDeclarationOutputTypeDef(
     _RequiredPipelineDeclarationOutputTypeDef, _OptionalPipelineDeclarationOutputTypeDef
 ):
     pass
 
-
 _RequiredPipelineDeclarationTypeDef = TypedDict(
     "_RequiredPipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
     },
@@ -2026,21 +1739,19 @@
         "artifactStore": ArtifactStoreTypeDef,
         "artifactStores": Mapping[str, ArtifactStoreTypeDef],
         "version": int,
     },
     total=False,
 )
 
-
 class PipelineDeclarationTypeDef(
     _RequiredPipelineDeclarationTypeDef, _OptionalPipelineDeclarationTypeDef
 ):
     pass
 
-
 StageStateTypeDef = TypedDict(
     "StageStateTypeDef",
     {
         "stageName": str,
         "inboundExecution": StageExecutionTypeDef,
         "inboundTransitionState": TransitionStateTypeDef,
         "actionStates": List[ActionStateTypeDef],
@@ -2065,68 +1776,66 @@
     },
     total=False,
 )
 
 JobDataTypeDef = TypedDict(
     "JobDataTypeDef",
     {
-        "actionTypeId": ActionTypeIdOutputTypeDef,
+        "actionTypeId": ActionTypeIdTypeDef,
         "actionConfiguration": ActionConfigurationTypeDef,
         "pipelineContext": PipelineContextTypeDef,
         "inputArtifacts": List[ArtifactTypeDef],
         "outputArtifacts": List[ArtifactTypeDef],
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
-        "encryptionKey": EncryptionKeyOutputTypeDef,
+        "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
 ThirdPartyJobDataTypeDef = TypedDict(
     "ThirdPartyJobDataTypeDef",
     {
-        "actionTypeId": ActionTypeIdOutputTypeDef,
+        "actionTypeId": ActionTypeIdTypeDef,
         "actionConfiguration": ActionConfigurationTypeDef,
         "pipelineContext": PipelineContextTypeDef,
         "inputArtifacts": List[ArtifactTypeDef],
         "outputArtifacts": List[ArtifactTypeDef],
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
-        "encryptionKey": EncryptionKeyOutputTypeDef,
+        "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
 _RequiredActionTypeDeclarationOutputTypeDef = TypedDict(
     "_RequiredActionTypeDeclarationOutputTypeDef",
     {
         "executor": ActionTypeExecutorOutputTypeDef,
-        "id": ActionTypeIdentifierOutputTypeDef,
-        "inputArtifactDetails": ActionTypeArtifactDetailsOutputTypeDef,
-        "outputArtifactDetails": ActionTypeArtifactDetailsOutputTypeDef,
+        "id": ActionTypeIdentifierTypeDef,
+        "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
+        "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
     },
 )
 _OptionalActionTypeDeclarationOutputTypeDef = TypedDict(
     "_OptionalActionTypeDeclarationOutputTypeDef",
     {
         "description": str,
         "permissions": ActionTypePermissionsOutputTypeDef,
-        "properties": List[ActionTypePropertyOutputTypeDef],
-        "urls": ActionTypeUrlsOutputTypeDef,
+        "properties": List[ActionTypePropertyTypeDef],
+        "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
-
 class ActionTypeDeclarationOutputTypeDef(
     _RequiredActionTypeDeclarationOutputTypeDef, _OptionalActionTypeDeclarationOutputTypeDef
 ):
     pass
 
-
 _RequiredActionTypeDeclarationTypeDef = TypedDict(
     "_RequiredActionTypeDeclarationTypeDef",
     {
         "executor": ActionTypeExecutorTypeDef,
         "id": ActionTypeIdentifierTypeDef,
         "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
@@ -2139,61 +1848,59 @@
         "permissions": ActionTypePermissionsTypeDef,
         "properties": Sequence[ActionTypePropertyTypeDef],
         "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
-
 class ActionTypeDeclarationTypeDef(
     _RequiredActionTypeDeclarationTypeDef, _OptionalActionTypeDeclarationTypeDef
 ):
     pass
 
-
 ListWebhooksOutputTypeDef = TypedDict(
     "ListWebhooksOutputTypeDef",
     {
         "webhooks": List[ListWebhookItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutWebhookOutputTypeDef = TypedDict(
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePipelineOutputTypeDef = TypedDict(
     "CreatePipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationOutputTypeDef,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPipelineOutputTypeDef = TypedDict(
     "GetPipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationOutputTypeDef,
         "metadata": PipelineMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineOutputTypeDef = TypedDict(
     "UpdatePipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
@@ -2203,21 +1910,19 @@
     "_OptionalCreatePipelineInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
-
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
@@ -2225,24 +1930,24 @@
     "GetPipelineStateOutputTypeDef",
     {
         "pipelineName": str,
         "pipelineVersion": int,
         "stageStates": List[StageStateTypeDef],
         "created": datetime,
         "updated": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListActionExecutionsOutputTypeDef = TypedDict(
     "ListActionExecutionsOutputTypeDef",
     {
         "actionExecutionDetails": List[ActionExecutionDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "id": str,
@@ -2273,41 +1978,41 @@
     total=False,
 )
 
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeDeclarationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
 
 GetJobDetailsOutputTypeDef = TypedDict(
     "GetJobDetailsOutputTypeDef",
     {
         "jobDetails": JobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PollForJobsOutputTypeDef = TypedDict(
     "PollForJobsOutputTypeDef",
     {
         "jobs": List[JobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetThirdPartyJobDetailsOutputTypeDef = TypedDict(
     "GetThirdPartyJobDetailsOutputTypeDef",
     {
         "jobDetails": ThirdPartyJobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/type_defs.pyi` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,138 +36,122 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AWSSessionCredentialsTypeDef",
     "AcknowledgeJobInputRequestTypeDef",
-    "AcknowledgeJobOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
-    "AcknowledgeThirdPartyJobOutputTypeDef",
-    "ActionConfigurationPropertyOutputTypeDef",
     "ActionConfigurationPropertyTypeDef",
     "ActionConfigurationTypeDef",
     "ActionContextTypeDef",
-    "ActionTypeIdOutputTypeDef",
-    "InputArtifactOutputTypeDef",
-    "OutputArtifactOutputTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ErrorDetailsTypeDef",
     "ActionRevisionOutputTypeDef",
     "ActionRevisionTypeDef",
-    "ActionTypeArtifactDetailsOutputTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
-    "ActionTypeIdentifierOutputTypeDef",
-    "ActionTypePermissionsOutputTypeDef",
-    "ActionTypePropertyOutputTypeDef",
-    "ActionTypeUrlsOutputTypeDef",
     "ActionTypeIdentifierTypeDef",
-    "ActionTypePermissionsTypeDef",
+    "ActionTypePermissionsOutputTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
-    "ActionTypeSettingsOutputTypeDef",
+    "ActionTypePermissionsTypeDef",
     "ActionTypeSettingsTypeDef",
-    "ArtifactDetailsOutputTypeDef",
+    "ArtifactDetailsTypeDef",
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
-    "ArtifactDetailsTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
-    "EncryptionKeyOutputTypeDef",
     "EncryptionKeyTypeDef",
-    "BlockerDeclarationOutputTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
-    "TagOutputTypeDef",
     "CurrentRevisionTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
     "JobWorkerExecutorConfigurationOutputTypeDef",
-    "LambdaExecutorConfigurationOutputTypeDef",
-    "JobWorkerExecutorConfigurationTypeDef",
     "LambdaExecutorConfigurationTypeDef",
+    "JobWorkerExecutorConfigurationTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
     "PipelineMetadataTypeDef",
     "GetPipelineStateInputRequestTypeDef",
     "GetThirdPartyJobDetailsInputRequestTypeDef",
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListActionTypesInputRequestTypeDef",
-    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     "ListPipelineExecutionsInputRequestTypeDef",
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineSummaryTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListWebhooksInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "StageContextTypeDef",
     "SourceRevisionTypeDef",
     "StopExecutionTriggerTypeDef",
     "ThirdPartyJobTypeDef",
-    "PutActionRevisionOutputTypeDef",
-    "PutApprovalResultOutputTypeDef",
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryStageExecutionInputRequestTypeDef",
-    "RetryStageExecutionOutputTypeDef",
     "StageExecutionTypeDef",
     "TransitionStateTypeDef",
     "StartPipelineExecutionInputRequestTypeDef",
-    "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionInputRequestTypeDef",
-    "StopPipelineExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "WebhookAuthConfigurationOutputTypeDef",
     "WebhookAuthConfigurationTypeDef",
-    "WebhookFilterRuleOutputTypeDef",
     "WebhookFilterRuleTypeDef",
-    "ActionDeclarationOutputTypeDef",
+    "AcknowledgeJobOutputTypeDef",
+    "AcknowledgeThirdPartyJobOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "PutActionRevisionOutputTypeDef",
+    "PutApprovalResultOutputTypeDef",
+    "RetryStageExecutionOutputTypeDef",
+    "StartPipelineExecutionOutputTypeDef",
+    "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
+    "ActionDeclarationOutputTypeDef",
     "ActionDeclarationTypeDef",
-    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
     "PutActionRevisionInputRequestTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "PipelineExecutionTypeDef",
-    "ArtifactStoreOutputTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
-    "TagResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "TagResourceInputRequestTypeDef",
     "PutJobSuccessResultInputRequestTypeDef",
     "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "ExecutorConfigurationOutputTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
+    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
+    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
     "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
     "StageDeclarationOutputTypeDef",
@@ -224,64 +208,34 @@
     "AcknowledgeJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
     },
 )
 
-AcknowledgeJobOutputTypeDef = TypedDict(
-    "AcknowledgeJobOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "status": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AcknowledgeThirdPartyJobInputRequestTypeDef = TypedDict(
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
         "clientToken": str,
     },
 )
 
-AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
-    "AcknowledgeThirdPartyJobOutputTypeDef",
-    {
-        "status": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredActionConfigurationPropertyOutputTypeDef = TypedDict(
-    "_RequiredActionConfigurationPropertyOutputTypeDef",
-    {
-        "name": str,
-        "required": bool,
-        "key": bool,
-        "secret": bool,
-    },
-)
-_OptionalActionConfigurationPropertyOutputTypeDef = TypedDict(
-    "_OptionalActionConfigurationPropertyOutputTypeDef",
-    {
-        "queryable": bool,
-        "description": str,
-        "type": ActionConfigurationPropertyTypeType,
-    },
-    total=False,
-)
-
-class ActionConfigurationPropertyOutputTypeDef(
-    _RequiredActionConfigurationPropertyOutputTypeDef,
-    _OptionalActionConfigurationPropertyOutputTypeDef,
-):
-    pass
-
 _RequiredActionConfigurationPropertyTypeDef = TypedDict(
     "_RequiredActionConfigurationPropertyTypeDef",
     {
         "name": str,
         "required": bool,
         "key": bool,
         "secret": bool,
@@ -293,19 +247,21 @@
         "queryable": bool,
         "description": str,
         "type": ActionConfigurationPropertyTypeType,
     },
     total=False,
 )
 
+
 class ActionConfigurationPropertyTypeDef(
     _RequiredActionConfigurationPropertyTypeDef, _OptionalActionConfigurationPropertyTypeDef
 ):
     pass
 
+
 ActionConfigurationTypeDef = TypedDict(
     "ActionConfigurationTypeDef",
     {
         "configuration": Dict[str, str],
     },
     total=False,
 )
@@ -315,38 +271,14 @@
     {
         "name": str,
         "actionExecutionId": str,
     },
     total=False,
 )
 
-ActionTypeIdOutputTypeDef = TypedDict(
-    "ActionTypeIdOutputTypeDef",
-    {
-        "category": ActionCategoryType,
-        "owner": ActionOwnerType,
-        "provider": str,
-        "version": str,
-    },
-)
-
-InputArtifactOutputTypeDef = TypedDict(
-    "InputArtifactOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-
-OutputArtifactOutputTypeDef = TypedDict(
-    "OutputArtifactOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-
 ActionTypeIdTypeDef = TypedDict(
     "ActionTypeIdTypeDef",
     {
         "category": ActionCategoryType,
         "owner": ActionOwnerType,
         "provider": str,
         "version": str,
@@ -408,32 +340,24 @@
     {
         "revisionId": str,
         "revisionChangeId": str,
         "created": Union[datetime, str],
     },
 )
 
-ActionTypeArtifactDetailsOutputTypeDef = TypedDict(
-    "ActionTypeArtifactDetailsOutputTypeDef",
-    {
-        "minimumCount": int,
-        "maximumCount": int,
-    },
-)
-
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
 
-ActionTypeIdentifierOutputTypeDef = TypedDict(
-    "ActionTypeIdentifierOutputTypeDef",
+ActionTypeIdentifierTypeDef = TypedDict(
+    "ActionTypeIdentifierTypeDef",
     {
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
     },
 )
@@ -441,65 +365,14 @@
 ActionTypePermissionsOutputTypeDef = TypedDict(
     "ActionTypePermissionsOutputTypeDef",
     {
         "allowedAccounts": List[str],
     },
 )
 
-_RequiredActionTypePropertyOutputTypeDef = TypedDict(
-    "_RequiredActionTypePropertyOutputTypeDef",
-    {
-        "name": str,
-        "optional": bool,
-        "key": bool,
-        "noEcho": bool,
-    },
-)
-_OptionalActionTypePropertyOutputTypeDef = TypedDict(
-    "_OptionalActionTypePropertyOutputTypeDef",
-    {
-        "queryable": bool,
-        "description": str,
-    },
-    total=False,
-)
-
-class ActionTypePropertyOutputTypeDef(
-    _RequiredActionTypePropertyOutputTypeDef, _OptionalActionTypePropertyOutputTypeDef
-):
-    pass
-
-ActionTypeUrlsOutputTypeDef = TypedDict(
-    "ActionTypeUrlsOutputTypeDef",
-    {
-        "configurationUrl": str,
-        "entityUrlTemplate": str,
-        "executionUrlTemplate": str,
-        "revisionUrlTemplate": str,
-    },
-    total=False,
-)
-
-ActionTypeIdentifierTypeDef = TypedDict(
-    "ActionTypeIdentifierTypeDef",
-    {
-        "category": ActionCategoryType,
-        "owner": str,
-        "provider": str,
-        "version": str,
-    },
-)
-
-ActionTypePermissionsTypeDef = TypedDict(
-    "ActionTypePermissionsTypeDef",
-    {
-        "allowedAccounts": Sequence[str],
-    },
-)
-
 _RequiredActionTypePropertyTypeDef = TypedDict(
     "_RequiredActionTypePropertyTypeDef",
     {
         "name": str,
         "optional": bool,
         "key": bool,
         "noEcho": bool,
@@ -510,54 +383,52 @@
     {
         "queryable": bool,
         "description": str,
     },
     total=False,
 )
 
+
 class ActionTypePropertyTypeDef(
     _RequiredActionTypePropertyTypeDef, _OptionalActionTypePropertyTypeDef
 ):
     pass
 
+
 ActionTypeUrlsTypeDef = TypedDict(
     "ActionTypeUrlsTypeDef",
     {
         "configurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
-ActionTypeSettingsOutputTypeDef = TypedDict(
-    "ActionTypeSettingsOutputTypeDef",
+ActionTypePermissionsTypeDef = TypedDict(
+    "ActionTypePermissionsTypeDef",
     {
-        "thirdPartyConfigurationUrl": str,
-        "entityUrlTemplate": str,
-        "executionUrlTemplate": str,
-        "revisionUrlTemplate": str,
+        "allowedAccounts": Sequence[str],
     },
-    total=False,
 )
 
 ActionTypeSettingsTypeDef = TypedDict(
     "ActionTypeSettingsTypeDef",
     {
         "thirdPartyConfigurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
-ArtifactDetailsOutputTypeDef = TypedDict(
-    "ArtifactDetailsOutputTypeDef",
+ArtifactDetailsTypeDef = TypedDict(
+    "ArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
 
 ApprovalResultTypeDef = TypedDict(
@@ -573,22 +444,14 @@
     {
         "bucket": str,
         "key": str,
     },
     total=False,
 )
 
-ArtifactDetailsTypeDef = TypedDict(
-    "ArtifactDetailsTypeDef",
-    {
-        "minimumCount": int,
-        "maximumCount": int,
-    },
-)
-
 S3ArtifactLocationTypeDef = TypedDict(
     "S3ArtifactLocationTypeDef",
     {
         "bucketName": str,
         "objectKey": str,
     },
 )
@@ -602,38 +465,22 @@
         "revisionSummary": str,
         "created": datetime,
         "revisionUrl": str,
     },
     total=False,
 )
 
-EncryptionKeyOutputTypeDef = TypedDict(
-    "EncryptionKeyOutputTypeDef",
-    {
-        "id": str,
-        "type": Literal["KMS"],
-    },
-)
-
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "id": str,
         "type": Literal["KMS"],
     },
 )
 
-BlockerDeclarationOutputTypeDef = TypedDict(
-    "BlockerDeclarationOutputTypeDef",
-    {
-        "name": str,
-        "type": Literal["Schedule"],
-    },
-)
-
 BlockerDeclarationTypeDef = TypedDict(
     "BlockerDeclarationTypeDef",
     {
         "name": str,
         "type": Literal["Schedule"],
     },
 )
@@ -642,22 +489,14 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 _RequiredCurrentRevisionTypeDef = TypedDict(
     "_RequiredCurrentRevisionTypeDef",
     {
         "revision": str,
         "changeIdentifier": str,
     },
 )
@@ -666,17 +505,19 @@
     {
         "created": Union[datetime, str],
         "revisionSummary": str,
     },
     total=False,
 )
 
+
 class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
     pass
 
+
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -710,21 +551,14 @@
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
         "reason": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableStageTransitionInputRequestTypeDef = TypedDict(
     "EnableStageTransitionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
     },
@@ -754,37 +588,30 @@
     {
         "pollingAccounts": List[str],
         "pollingServicePrincipals": List[str],
     },
     total=False,
 )
 
-LambdaExecutorConfigurationOutputTypeDef = TypedDict(
-    "LambdaExecutorConfigurationOutputTypeDef",
+LambdaExecutorConfigurationTypeDef = TypedDict(
+    "LambdaExecutorConfigurationTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
 
 JobWorkerExecutorConfigurationTypeDef = TypedDict(
     "JobWorkerExecutorConfigurationTypeDef",
     {
         "pollingAccounts": Sequence[str],
         "pollingServicePrincipals": Sequence[str],
     },
     total=False,
 )
 
-LambdaExecutorConfigurationTypeDef = TypedDict(
-    "LambdaExecutorConfigurationTypeDef",
-    {
-        "lambdaFunctionArn": str,
-    },
-)
-
 _RequiredFailureDetailsTypeDef = TypedDict(
     "_RequiredFailureDetailsTypeDef",
     {
         "type": FailureTypeType,
         "message": str,
     },
 )
@@ -792,17 +619,19 @@
     "_OptionalFailureDetailsTypeDef",
     {
         "externalExecutionId": str,
     },
     total=False,
 )
 
+
 class FailureDetailsTypeDef(_RequiredFailureDetailsTypeDef, _OptionalFailureDetailsTypeDef):
     pass
 
+
 GetActionTypeInputRequestTypeDef = TypedDict(
     "GetActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
@@ -834,19 +663,21 @@
     "_OptionalGetPipelineInputRequestTypeDef",
     {
         "version": int,
     },
     total=False,
 )
 
+
 class GetPipelineInputRequestTypeDef(
     _RequiredGetPipelineInputRequestTypeDef, _OptionalGetPipelineInputRequestTypeDef
 ):
     pass
 
+
 PipelineMetadataTypeDef = TypedDict(
     "PipelineMetadataTypeDef",
     {
         "pipelineArn": str,
         "created": datetime,
         "updated": datetime,
         "pollingDisabledAt": datetime,
@@ -865,54 +696,34 @@
     "GetThirdPartyJobDetailsInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
 
-ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "actionOwnerFilter": ActionOwnerType,
-        "regionFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListActionTypesInputRequestTypeDef = TypedDict(
     "ListActionTypesInputRequestTypeDef",
     {
         "actionOwnerFilter": ActionOwnerType,
         "nextToken": str,
         "regionFilter": str,
     },
     total=False,
 )
 
-_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
-    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPipelineExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListPipelineExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 _OptionalListPipelineExecutionsInputRequestTypeDef = TypedDict(
@@ -920,27 +731,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListPipelineExecutionsInputRequestTypeDef(
     _RequiredListPipelineExecutionsInputRequestTypeDef,
     _OptionalListPipelineExecutionsInputRequestTypeDef,
 ):
     pass
 
-ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
@@ -954,34 +759,14 @@
         "version": int,
         "created": datetime,
         "updated": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -989,46 +774,30 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListWebhooksInputRequestTypeDef = TypedDict(
     "ListWebhooksInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
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
 StageContextTypeDef = TypedDict(
     "StageContextTypeDef",
     {
         "name": str,
     },
     total=False,
 )
@@ -1045,17 +814,19 @@
         "revisionId": str,
         "revisionSummary": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
+
 class SourceRevisionTypeDef(_RequiredSourceRevisionTypeDef, _OptionalSourceRevisionTypeDef):
     pass
 
+
 StopExecutionTriggerTypeDef = TypedDict(
     "StopExecutionTriggerTypeDef",
     {
         "reason": str,
     },
     total=False,
 )
@@ -1065,68 +836,32 @@
     {
         "clientId": str,
         "jobId": str,
     },
     total=False,
 )
 
-PutActionRevisionOutputTypeDef = TypedDict(
-    "PutActionRevisionOutputTypeDef",
-    {
-        "newRevision": bool,
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutApprovalResultOutputTypeDef = TypedDict(
-    "PutApprovalResultOutputTypeDef",
-    {
-        "approvedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterWebhookWithThirdPartyInputRequestTypeDef = TypedDict(
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
     {
         "webhookName": str,
     },
     total=False,
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
 RetryStageExecutionInputRequestTypeDef = TypedDict(
     "RetryStageExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "pipelineExecutionId": str,
         "retryMode": Literal["FAILED_ACTIONS"],
     },
 )
 
-RetryStageExecutionOutputTypeDef = TypedDict(
-    "RetryStageExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StageExecutionTypeDef = TypedDict(
     "StageExecutionTypeDef",
     {
         "pipelineExecutionId": str,
         "status": StageExecutionStatusType,
     },
 )
@@ -1152,27 +887,21 @@
     "_OptionalStartPipelineExecutionInputRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class StartPipelineExecutionInputRequestTypeDef(
     _RequiredStartPipelineExecutionInputRequestTypeDef,
     _OptionalStartPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
-StartPipelineExecutionOutputTypeDef = TypedDict(
-    "StartPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStopPipelineExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStopPipelineExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "pipelineExecutionId": str,
     },
@@ -1182,117 +911,123 @@
     {
         "abandon": bool,
         "reason": str,
     },
     total=False,
 )
 
+
 class StopPipelineExecutionInputRequestTypeDef(
     _RequiredStopPipelineExecutionInputRequestTypeDef,
     _OptionalStopPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
-StopPipelineExecutionOutputTypeDef = TypedDict(
-    "StopPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-WebhookAuthConfigurationOutputTypeDef = TypedDict(
-    "WebhookAuthConfigurationOutputTypeDef",
-    {
-        "AllowedIPRange": str,
-        "SecretToken": str,
-    },
-    total=False,
-)
-
 WebhookAuthConfigurationTypeDef = TypedDict(
     "WebhookAuthConfigurationTypeDef",
     {
         "AllowedIPRange": str,
         "SecretToken": str,
     },
     total=False,
 )
 
-_RequiredWebhookFilterRuleOutputTypeDef = TypedDict(
-    "_RequiredWebhookFilterRuleOutputTypeDef",
+_RequiredWebhookFilterRuleTypeDef = TypedDict(
+    "_RequiredWebhookFilterRuleTypeDef",
     {
         "jsonPath": str,
     },
 )
-_OptionalWebhookFilterRuleOutputTypeDef = TypedDict(
-    "_OptionalWebhookFilterRuleOutputTypeDef",
+_OptionalWebhookFilterRuleTypeDef = TypedDict(
+    "_OptionalWebhookFilterRuleTypeDef",
     {
         "matchEquals": str,
     },
     total=False,
 )
 
-class WebhookFilterRuleOutputTypeDef(
-    _RequiredWebhookFilterRuleOutputTypeDef, _OptionalWebhookFilterRuleOutputTypeDef
+
+class WebhookFilterRuleTypeDef(
+    _RequiredWebhookFilterRuleTypeDef, _OptionalWebhookFilterRuleTypeDef
 ):
     pass
 
-_RequiredWebhookFilterRuleTypeDef = TypedDict(
-    "_RequiredWebhookFilterRuleTypeDef",
+
+AcknowledgeJobOutputTypeDef = TypedDict(
+    "AcknowledgeJobOutputTypeDef",
     {
-        "jsonPath": str,
+        "status": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalWebhookFilterRuleTypeDef = TypedDict(
-    "_OptionalWebhookFilterRuleTypeDef",
+
+AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
+    "AcknowledgeThirdPartyJobOutputTypeDef",
     {
-        "matchEquals": str,
+        "status": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class WebhookFilterRuleTypeDef(
-    _RequiredWebhookFilterRuleTypeDef, _OptionalWebhookFilterRuleTypeDef
-):
-    pass
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredActionDeclarationOutputTypeDef = TypedDict(
-    "_RequiredActionDeclarationOutputTypeDef",
+PutActionRevisionOutputTypeDef = TypedDict(
+    "PutActionRevisionOutputTypeDef",
     {
-        "name": str,
-        "actionTypeId": ActionTypeIdOutputTypeDef,
+        "newRevision": bool,
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalActionDeclarationOutputTypeDef = TypedDict(
-    "_OptionalActionDeclarationOutputTypeDef",
+
+PutApprovalResultOutputTypeDef = TypedDict(
+    "PutApprovalResultOutputTypeDef",
     {
-        "runOrder": int,
-        "configuration": Dict[str, str],
-        "outputArtifacts": List[OutputArtifactOutputTypeDef],
-        "inputArtifacts": List[InputArtifactOutputTypeDef],
-        "roleArn": str,
-        "region": str,
-        "namespace": str,
+        "approvedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ActionDeclarationOutputTypeDef(
-    _RequiredActionDeclarationOutputTypeDef, _OptionalActionDeclarationOutputTypeDef
-):
-    pass
+RetryStageExecutionOutputTypeDef = TypedDict(
+    "RetryStageExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartPipelineExecutionOutputTypeDef = TypedDict(
+    "StartPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopPipelineExecutionOutputTypeDef = TypedDict(
+    "StopPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredPollForJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
@@ -1301,86 +1036,99 @@
     {
         "maxBatchSize": int,
         "queryParam": Mapping[str, str],
     },
     total=False,
 )
 
+
 class PollForJobsInputRequestTypeDef(
     _RequiredPollForJobsInputRequestTypeDef, _OptionalPollForJobsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPollForThirdPartyJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForThirdPartyJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
 _OptionalPollForThirdPartyJobsInputRequestTypeDef = TypedDict(
     "_OptionalPollForThirdPartyJobsInputRequestTypeDef",
     {
         "maxBatchSize": int,
     },
     total=False,
 )
 
+
 class PollForThirdPartyJobsInputRequestTypeDef(
     _RequiredPollForThirdPartyJobsInputRequestTypeDef,
     _OptionalPollForThirdPartyJobsInputRequestTypeDef,
 ):
     pass
 
-_RequiredActionDeclarationTypeDef = TypedDict(
-    "_RequiredActionDeclarationTypeDef",
+
+_RequiredActionDeclarationOutputTypeDef = TypedDict(
+    "_RequiredActionDeclarationOutputTypeDef",
     {
         "name": str,
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
-_OptionalActionDeclarationTypeDef = TypedDict(
-    "_OptionalActionDeclarationTypeDef",
+_OptionalActionDeclarationOutputTypeDef = TypedDict(
+    "_OptionalActionDeclarationOutputTypeDef",
     {
         "runOrder": int,
-        "configuration": Mapping[str, str],
-        "outputArtifacts": Sequence[OutputArtifactTypeDef],
-        "inputArtifacts": Sequence[InputArtifactTypeDef],
+        "configuration": Dict[str, str],
+        "outputArtifacts": List[OutputArtifactTypeDef],
+        "inputArtifacts": List[InputArtifactTypeDef],
         "roleArn": str,
         "region": str,
         "namespace": str,
     },
     total=False,
 )
 
-class ActionDeclarationTypeDef(
-    _RequiredActionDeclarationTypeDef, _OptionalActionDeclarationTypeDef
+
+class ActionDeclarationOutputTypeDef(
+    _RequiredActionDeclarationOutputTypeDef, _OptionalActionDeclarationOutputTypeDef
 ):
     pass
 
-_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+
+_RequiredActionDeclarationTypeDef = TypedDict(
+    "_RequiredActionDeclarationTypeDef",
     {
-        "pipelineName": str,
+        "name": str,
+        "actionTypeId": ActionTypeIdTypeDef,
     },
 )
-_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+_OptionalActionDeclarationTypeDef = TypedDict(
+    "_OptionalActionDeclarationTypeDef",
     {
-        "filter": ActionExecutionFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "runOrder": int,
+        "configuration": Mapping[str, str],
+        "outputArtifacts": Sequence[OutputArtifactTypeDef],
+        "inputArtifacts": Sequence[InputArtifactTypeDef],
+        "roleArn": str,
+        "region": str,
+        "namespace": str,
     },
     total=False,
 )
 
-class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
-    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+
+class ActionDeclarationTypeDef(
+    _RequiredActionDeclarationTypeDef, _OptionalActionDeclarationTypeDef
 ):
     pass
 
+
 _RequiredListActionExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListActionExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 _OptionalListActionExecutionsInputRequestTypeDef = TypedDict(
@@ -1389,20 +1137,22 @@
         "filter": ActionExecutionFilterTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListActionExecutionsInputRequestTypeDef(
     _RequiredListActionExecutionsInputRequestTypeDef,
     _OptionalListActionExecutionsInputRequestTypeDef,
 ):
     pass
 
+
 ActionExecutionTypeDef = TypedDict(
     "ActionExecutionTypeDef",
     {
         "actionExecutionId": str,
         "status": ActionExecutionStatusType,
         "summary": str,
         "lastStatusChange": datetime,
@@ -1425,31 +1175,33 @@
         "actionRevision": ActionRevisionTypeDef,
     },
 )
 
 _RequiredActionTypeTypeDef = TypedDict(
     "_RequiredActionTypeTypeDef",
     {
-        "id": ActionTypeIdOutputTypeDef,
-        "inputArtifactDetails": ArtifactDetailsOutputTypeDef,
-        "outputArtifactDetails": ArtifactDetailsOutputTypeDef,
+        "id": ActionTypeIdTypeDef,
+        "inputArtifactDetails": ArtifactDetailsTypeDef,
+        "outputArtifactDetails": ArtifactDetailsTypeDef,
     },
 )
 _OptionalActionTypeTypeDef = TypedDict(
     "_OptionalActionTypeTypeDef",
     {
-        "settings": ActionTypeSettingsOutputTypeDef,
-        "actionConfigurationProperties": List[ActionConfigurationPropertyOutputTypeDef],
+        "settings": ActionTypeSettingsTypeDef,
+        "actionConfigurationProperties": List[ActionConfigurationPropertyTypeDef],
     },
     total=False,
 )
 
+
 class ActionTypeTypeDef(_RequiredActionTypeTypeDef, _OptionalActionTypeTypeDef):
     pass
 
+
 PutApprovalResultInputRequestTypeDef = TypedDict(
     "PutApprovalResultInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "actionName": str,
         "result": ApprovalResultTypeDef,
@@ -1484,34 +1236,14 @@
         "status": PipelineExecutionStatusType,
         "statusSummary": str,
         "artifactRevisions": List[ArtifactRevisionTypeDef],
     },
     total=False,
 )
 
-_RequiredArtifactStoreOutputTypeDef = TypedDict(
-    "_RequiredArtifactStoreOutputTypeDef",
-    {
-        "type": Literal["S3"],
-        "location": str,
-    },
-)
-_OptionalArtifactStoreOutputTypeDef = TypedDict(
-    "_OptionalArtifactStoreOutputTypeDef",
-    {
-        "encryptionKey": EncryptionKeyOutputTypeDef,
-    },
-    total=False,
-)
-
-class ArtifactStoreOutputTypeDef(
-    _RequiredArtifactStoreOutputTypeDef, _OptionalArtifactStoreOutputTypeDef
-):
-    pass
-
 _RequiredArtifactStoreTypeDef = TypedDict(
     "_RequiredArtifactStoreTypeDef",
     {
         "type": Literal["S3"],
         "location": str,
     },
 )
@@ -1519,17 +1251,19 @@
     "_OptionalArtifactStoreTypeDef",
     {
         "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
+
 class ArtifactStoreTypeDef(_RequiredArtifactStoreTypeDef, _OptionalArtifactStoreTypeDef):
     pass
 
+
 _RequiredCreateCustomActionTypeInputRequestTypeDef = TypedDict(
     "_RequiredCreateCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
@@ -1542,34 +1276,36 @@
         "settings": ActionTypeSettingsTypeDef,
         "configurationProperties": Sequence[ActionConfigurationPropertyTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCustomActionTypeInputRequestTypeDef(
     _RequiredCreateCustomActionTypeInputRequestTypeDef,
     _OptionalCreateCustomActionTypeInputRequestTypeDef,
 ):
     pass
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
     "_RequiredPutJobSuccessResultInputRequestTypeDef",
     {
         "jobId": str,
@@ -1582,19 +1318,21 @@
         "continuationToken": str,
         "executionDetails": ExecutionDetailsTypeDef,
         "outputVariables": Mapping[str, str],
     },
     total=False,
 )
 
+
 class PutJobSuccessResultInputRequestTypeDef(
     _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
     "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
@@ -1604,24 +1342,26 @@
         "currentRevision": CurrentRevisionTypeDef,
         "continuationToken": str,
         "executionDetails": ExecutionDetailsTypeDef,
     },
     total=False,
 )
 
+
 class PutThirdPartyJobSuccessResultInputRequestTypeDef(
     _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
     _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
 ):
     pass
 
+
 ExecutorConfigurationOutputTypeDef = TypedDict(
     "ExecutorConfigurationOutputTypeDef",
     {
-        "lambdaExecutorConfiguration": LambdaExecutorConfigurationOutputTypeDef,
+        "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
         "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 ExecutorConfigurationTypeDef = TypedDict(
     "ExecutorConfigurationTypeDef",
@@ -1645,20 +1385,113 @@
     {
         "jobId": str,
         "clientToken": str,
         "failureDetails": FailureDetailsTypeDef,
     },
 )
 
+_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "filter": ActionExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
+    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+):
+    pass
+
+
+ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
+    {
+        "actionOwnerFilter": ActionOwnerType,
+        "regionFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
+    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+):
+    pass
+
+
+ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelines": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PipelineContextTypeDef = TypedDict(
     "PipelineContextTypeDef",
     {
         "pipelineName": str,
@@ -1684,27 +1517,27 @@
     total=False,
 )
 
 PollForThirdPartyJobsOutputTypeDef = TypedDict(
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WebhookDefinitionOutputTypeDef = TypedDict(
     "WebhookDefinitionOutputTypeDef",
     {
         "name": str,
         "targetPipeline": str,
         "targetAction": str,
-        "filters": List[WebhookFilterRuleOutputTypeDef],
+        "filters": List[WebhookFilterRuleTypeDef],
         "authentication": WebhookAuthenticationTypeType,
-        "authenticationConfiguration": WebhookAuthConfigurationOutputTypeDef,
+        "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
 
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
@@ -1722,24 +1555,26 @@
         "name": str,
         "actions": List[ActionDeclarationOutputTypeDef],
     },
 )
 _OptionalStageDeclarationOutputTypeDef = TypedDict(
     "_OptionalStageDeclarationOutputTypeDef",
     {
-        "blockers": List[BlockerDeclarationOutputTypeDef],
+        "blockers": List[BlockerDeclarationTypeDef],
     },
     total=False,
 )
 
+
 class StageDeclarationOutputTypeDef(
     _RequiredStageDeclarationOutputTypeDef, _OptionalStageDeclarationOutputTypeDef
 ):
     pass
 
+
 _RequiredStageDeclarationTypeDef = TypedDict(
     "_RequiredStageDeclarationTypeDef",
     {
         "name": str,
         "actions": Sequence[ActionDeclarationTypeDef],
     },
 )
@@ -1747,17 +1582,19 @@
     "_OptionalStageDeclarationTypeDef",
     {
         "blockers": Sequence[BlockerDeclarationTypeDef],
     },
     total=False,
 )
 
+
 class StageDeclarationTypeDef(_RequiredStageDeclarationTypeDef, _OptionalStageDeclarationTypeDef):
     pass
 
+
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": str,
         "currentRevision": ActionRevisionOutputTypeDef,
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
@@ -1766,32 +1603,32 @@
     total=False,
 )
 
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListActionTypesOutputTypeDef = TypedDict(
     "ListActionTypesOutputTypeDef",
     {
         "actionTypes": List[ActionTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActionExecutionInputTypeDef = TypedDict(
     "ActionExecutionInputTypeDef",
     {
-        "actionTypeId": ActionTypeIdOutputTypeDef,
+        "actionTypeId": ActionTypeIdTypeDef,
         "configuration": Dict[str, str],
         "resolvedConfiguration": Dict[str, str],
         "roleArn": str,
         "region": str,
         "inputArtifacts": List[ArtifactDetailTypeDef],
         "namespace": str,
     },
@@ -1818,15 +1655,15 @@
     total=False,
 )
 
 GetPipelineExecutionOutputTypeDef = TypedDict(
     "GetPipelineExecutionOutputTypeDef",
     {
         "pipelineExecution": PipelineExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredActionTypeExecutorOutputTypeDef = TypedDict(
     "_RequiredActionTypeExecutorOutputTypeDef",
     {
         "configuration": ExecutorConfigurationOutputTypeDef,
@@ -1838,19 +1675,21 @@
     {
         "policyStatementsTemplate": str,
         "jobTimeout": int,
     },
     total=False,
 )
 
+
 class ActionTypeExecutorOutputTypeDef(
     _RequiredActionTypeExecutorOutputTypeDef, _OptionalActionTypeExecutorOutputTypeDef
 ):
     pass
 
+
 _RequiredActionTypeExecutorTypeDef = TypedDict(
     "_RequiredActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
         "type": ExecutorTypeType,
     },
 )
@@ -1859,25 +1698,27 @@
     {
         "policyStatementsTemplate": str,
         "jobTimeout": int,
     },
     total=False,
 )
 
+
 class ActionTypeExecutorTypeDef(
     _RequiredActionTypeExecutorTypeDef, _OptionalActionTypeExecutorTypeDef
 ):
     pass
 
+
 ListPipelineExecutionsOutputTypeDef = TypedDict(
     "ListPipelineExecutionsOutputTypeDef",
     {
         "pipelineExecutionSummaries": List[PipelineExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListWebhookItemTypeDef = TypedDict(
     "_RequiredListWebhookItemTypeDef",
     {
         "definition": WebhookDefinitionOutputTypeDef,
@@ -1887,64 +1728,70 @@
 _OptionalListWebhookItemTypeDef = TypedDict(
     "_OptionalListWebhookItemTypeDef",
     {
         "errorMessage": str,
         "errorCode": str,
         "lastTriggered": datetime,
         "arn": str,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class ListWebhookItemTypeDef(_RequiredListWebhookItemTypeDef, _OptionalListWebhookItemTypeDef):
     pass
 
+
 _RequiredPutWebhookInputRequestTypeDef = TypedDict(
     "_RequiredPutWebhookInputRequestTypeDef",
     {
         "webhook": WebhookDefinitionTypeDef,
     },
 )
 _OptionalPutWebhookInputRequestTypeDef = TypedDict(
     "_OptionalPutWebhookInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPipelineDeclarationOutputTypeDef = TypedDict(
     "_RequiredPipelineDeclarationOutputTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": List[StageDeclarationOutputTypeDef],
     },
 )
 _OptionalPipelineDeclarationOutputTypeDef = TypedDict(
     "_OptionalPipelineDeclarationOutputTypeDef",
     {
-        "artifactStore": ArtifactStoreOutputTypeDef,
-        "artifactStores": Dict[str, ArtifactStoreOutputTypeDef],
+        "artifactStore": ArtifactStoreTypeDef,
+        "artifactStores": Dict[str, ArtifactStoreTypeDef],
         "version": int,
     },
     total=False,
 )
 
+
 class PipelineDeclarationOutputTypeDef(
     _RequiredPipelineDeclarationOutputTypeDef, _OptionalPipelineDeclarationOutputTypeDef
 ):
     pass
 
+
 _RequiredPipelineDeclarationTypeDef = TypedDict(
     "_RequiredPipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
     },
@@ -1955,19 +1802,21 @@
         "artifactStore": ArtifactStoreTypeDef,
         "artifactStores": Mapping[str, ArtifactStoreTypeDef],
         "version": int,
     },
     total=False,
 )
 
+
 class PipelineDeclarationTypeDef(
     _RequiredPipelineDeclarationTypeDef, _OptionalPipelineDeclarationTypeDef
 ):
     pass
 
+
 StageStateTypeDef = TypedDict(
     "StageStateTypeDef",
     {
         "stageName": str,
         "inboundExecution": StageExecutionTypeDef,
         "inboundTransitionState": TransitionStateTypeDef,
         "actionStates": List[ActionStateTypeDef],
@@ -1992,66 +1841,68 @@
     },
     total=False,
 )
 
 JobDataTypeDef = TypedDict(
     "JobDataTypeDef",
     {
-        "actionTypeId": ActionTypeIdOutputTypeDef,
+        "actionTypeId": ActionTypeIdTypeDef,
         "actionConfiguration": ActionConfigurationTypeDef,
         "pipelineContext": PipelineContextTypeDef,
         "inputArtifacts": List[ArtifactTypeDef],
         "outputArtifacts": List[ArtifactTypeDef],
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
-        "encryptionKey": EncryptionKeyOutputTypeDef,
+        "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
 ThirdPartyJobDataTypeDef = TypedDict(
     "ThirdPartyJobDataTypeDef",
     {
-        "actionTypeId": ActionTypeIdOutputTypeDef,
+        "actionTypeId": ActionTypeIdTypeDef,
         "actionConfiguration": ActionConfigurationTypeDef,
         "pipelineContext": PipelineContextTypeDef,
         "inputArtifacts": List[ArtifactTypeDef],
         "outputArtifacts": List[ArtifactTypeDef],
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
-        "encryptionKey": EncryptionKeyOutputTypeDef,
+        "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
 _RequiredActionTypeDeclarationOutputTypeDef = TypedDict(
     "_RequiredActionTypeDeclarationOutputTypeDef",
     {
         "executor": ActionTypeExecutorOutputTypeDef,
-        "id": ActionTypeIdentifierOutputTypeDef,
-        "inputArtifactDetails": ActionTypeArtifactDetailsOutputTypeDef,
-        "outputArtifactDetails": ActionTypeArtifactDetailsOutputTypeDef,
+        "id": ActionTypeIdentifierTypeDef,
+        "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
+        "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
     },
 )
 _OptionalActionTypeDeclarationOutputTypeDef = TypedDict(
     "_OptionalActionTypeDeclarationOutputTypeDef",
     {
         "description": str,
         "permissions": ActionTypePermissionsOutputTypeDef,
-        "properties": List[ActionTypePropertyOutputTypeDef],
-        "urls": ActionTypeUrlsOutputTypeDef,
+        "properties": List[ActionTypePropertyTypeDef],
+        "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
+
 class ActionTypeDeclarationOutputTypeDef(
     _RequiredActionTypeDeclarationOutputTypeDef, _OptionalActionTypeDeclarationOutputTypeDef
 ):
     pass
 
+
 _RequiredActionTypeDeclarationTypeDef = TypedDict(
     "_RequiredActionTypeDeclarationTypeDef",
     {
         "executor": ActionTypeExecutorTypeDef,
         "id": ActionTypeIdentifierTypeDef,
         "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
@@ -2064,59 +1915,61 @@
         "permissions": ActionTypePermissionsTypeDef,
         "properties": Sequence[ActionTypePropertyTypeDef],
         "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
+
 class ActionTypeDeclarationTypeDef(
     _RequiredActionTypeDeclarationTypeDef, _OptionalActionTypeDeclarationTypeDef
 ):
     pass
 
+
 ListWebhooksOutputTypeDef = TypedDict(
     "ListWebhooksOutputTypeDef",
     {
         "webhooks": List[ListWebhookItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutWebhookOutputTypeDef = TypedDict(
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePipelineOutputTypeDef = TypedDict(
     "CreatePipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationOutputTypeDef,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPipelineOutputTypeDef = TypedDict(
     "GetPipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationOutputTypeDef,
         "metadata": PipelineMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineOutputTypeDef = TypedDict(
     "UpdatePipelineOutputTypeDef",
     {
         "pipeline": PipelineDeclarationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
@@ -2126,19 +1979,21 @@
     "_OptionalCreatePipelineInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
+
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
@@ -2146,24 +2001,24 @@
     "GetPipelineStateOutputTypeDef",
     {
         "pipelineName": str,
         "pipelineVersion": int,
         "stageStates": List[StageStateTypeDef],
         "created": datetime,
         "updated": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListActionExecutionsOutputTypeDef = TypedDict(
     "ListActionExecutionsOutputTypeDef",
     {
         "actionExecutionDetails": List[ActionExecutionDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "id": str,
@@ -2194,41 +2049,41 @@
     total=False,
 )
 
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeDeclarationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
 
 GetJobDetailsOutputTypeDef = TypedDict(
     "GetJobDetailsOutputTypeDef",
     {
         "jobDetails": JobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PollForJobsOutputTypeDef = TypedDict(
     "PollForJobsOutputTypeDef",
     {
         "jobs": List[JobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetThirdPartyJobDetailsOutputTypeDef = TypedDict(
     "GetThirdPartyJobDetailsOutputTypeDef",
     {
         "jobDetails": ThirdPartyJobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/PKG-INFO` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.28.12
-Summary: Type annotations for boto3.CodePipeline 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodePipeline 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,135 +362,118 @@
 `mypy_boto3_codepipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
-    AcknowledgeJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
-    AcknowledgeThirdPartyJobOutputTypeDef,
-    ActionConfigurationPropertyOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
-    ActionTypeIdOutputTypeDef,
-    InputArtifactOutputTypeDef,
-    OutputArtifactOutputTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
     ActionRevisionOutputTypeDef,
     ActionRevisionTypeDef,
-    ActionTypeArtifactDetailsOutputTypeDef,
     ActionTypeArtifactDetailsTypeDef,
-    ActionTypeIdentifierOutputTypeDef,
-    ActionTypePermissionsOutputTypeDef,
-    ActionTypePropertyOutputTypeDef,
-    ActionTypeUrlsOutputTypeDef,
     ActionTypeIdentifierTypeDef,
-    ActionTypePermissionsTypeDef,
+    ActionTypePermissionsOutputTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
-    ActionTypeSettingsOutputTypeDef,
+    ActionTypePermissionsTypeDef,
     ActionTypeSettingsTypeDef,
-    ArtifactDetailsOutputTypeDef,
+    ArtifactDetailsTypeDef,
     ApprovalResultTypeDef,
     S3LocationTypeDef,
-    ArtifactDetailsTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
-    EncryptionKeyOutputTypeDef,
     EncryptionKeyTypeDef,
-    BlockerDeclarationOutputTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
-    TagOutputTypeDef,
     CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
     JobWorkerExecutorConfigurationOutputTypeDef,
-    LambdaExecutorConfigurationOutputTypeDef,
-    JobWorkerExecutorConfigurationTypeDef,
     LambdaExecutorConfigurationTypeDef,
+    JobWorkerExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
     PipelineMetadataTypeDef,
     GetPipelineStateInputRequestTypeDef,
     GetThirdPartyJobDetailsInputRequestTypeDef,
-    ListActionTypesInputListActionTypesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListActionTypesInputRequestTypeDef,
-    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
     ListPipelineExecutionsInputRequestTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineSummaryTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListWebhooksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     StageContextTypeDef,
     SourceRevisionTypeDef,
     StopExecutionTriggerTypeDef,
     ThirdPartyJobTypeDef,
-    PutActionRevisionOutputTypeDef,
-    PutApprovalResultOutputTypeDef,
     RegisterWebhookWithThirdPartyInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetryStageExecutionInputRequestTypeDef,
-    RetryStageExecutionOutputTypeDef,
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
-    StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
-    StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
-    WebhookAuthConfigurationOutputTypeDef,
     WebhookAuthConfigurationTypeDef,
-    WebhookFilterRuleOutputTypeDef,
     WebhookFilterRuleTypeDef,
-    ActionDeclarationOutputTypeDef,
+    AcknowledgeJobOutputTypeDef,
+    AcknowledgeThirdPartyJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PutActionRevisionOutputTypeDef,
+    PutApprovalResultOutputTypeDef,
+    RetryStageExecutionOutputTypeDef,
+    StartPipelineExecutionOutputTypeDef,
+    StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
+    ActionDeclarationOutputTypeDef,
     ActionDeclarationTypeDef,
-    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
     PutActionRevisionInputRequestTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
-    ArtifactStoreOutputTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
+    TagResourceInputRequestTypeDef,
     PutJobSuccessResultInputRequestTypeDef,
     PutThirdPartyJobSuccessResultInputRequestTypeDef,
     ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
+    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    ListActionTypesInputListActionTypesPaginateTypeDef,
+    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
     StageDeclarationOutputTypeDef,
```

### Comparing `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/SOURCES.txt` & `mypy-boto3-codepipeline-1.28.15/mypy_boto3_codepipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.12/setup.py` & `mypy-boto3-codepipeline-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codepipeline",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_codepipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodePipeline 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CodePipeline 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

