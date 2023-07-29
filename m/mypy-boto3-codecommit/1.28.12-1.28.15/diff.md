# Comparing `tmp/mypy-boto3-codecommit-1.28.12.tar.gz` & `tmp/mypy-boto3-codecommit-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codecommit-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
+gzip compressed data, was "mypy-boto3-codecommit-1.28.15.tar", last modified: Fri Jul 28 20:42:28 2023, max compression
```

## Comparing `mypy-boto3-codecommit-1.28.12.tar` & `mypy-boto3-codecommit-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.328555 mypy-boto3-codecommit-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-07-27 05:34:27.328555 mypy-boto3-codecommit-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.328555 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71776 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    71685 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79773 2023-07-27 05:19:03.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79676 2023-07-27 05:19:03.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.328555 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.328555 mypy-boto3-codecommit-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:19:00.000000 mypy-boto3-codecommit-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.596825 mypy-boto3-codecommit-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:24.000000 mypy-boto3-codecommit-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22934 2023-07-28 20:42:28.596825 mypy-boto3-codecommit-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21435 2023-07-28 20:21:24.000000 mypy-boto3-codecommit-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.592825 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-28 20:21:24.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-28 20:21:24.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:21:24.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71776 2023-07-28 20:21:25.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71685 2023-07-28 20:21:25.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-28 20:21:26.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-07-28 20:21:26.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-28 20:21:25.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-07-28 20:21:25.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:24.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79361 2023-07-28 20:21:29.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79264 2023-07-28 20:21:27.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:24.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.596825 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22934 2023-07-28 20:42:28.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:28.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:28.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:28.000000 mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:28.596825 mypy-boto3-codecommit-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:21:24.000000 mypy-boto3-codecommit-1.28.15/setup.py
```

### Comparing `mypy-boto3-codecommit-1.28.12/LICENSE` & `mypy-boto3-codecommit-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.12/PKG-INFO` & `mypy-boto3-codecommit-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecommit
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeCommit 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeCommit 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecommit)](https://pepy.tech/project/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,26 +368,27 @@
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
     ApprovalStateChangedEventMetadataTypeDef,
     ApprovalTypeDef,
     AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeMergeConflictsErrorTypeDef,
     BatchDescribeMergeConflictsInputRequestTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
-    LocationOutputTypeDef,
+    LocationTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
@@ -395,152 +396,150 @@
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
-    CreateUnreferencedMergeCommitOutputTypeDef,
     DeleteApprovalRuleTemplateInputRequestTypeDef,
-    DeleteApprovalRuleTemplateOutputTypeDef,
     DeleteBranchInputRequestTypeDef,
     DeleteCommentContentInputRequestTypeDef,
     DeleteFileInputRequestTypeDef,
-    DeleteFileOutputTypeDef,
     DeletePullRequestApprovalRuleInputRequestTypeDef,
-    DeletePullRequestApprovalRuleOutputTypeDef,
     DeleteRepositoryInputRequestTypeDef,
-    DeleteRepositoryOutputTypeDef,
     DescribeMergeConflictsInputRequestTypeDef,
-    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribePullRequestEventsInputRequestTypeDef,
     DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluatePullRequestApprovalRulesInputRequestTypeDef,
     EvaluationTypeDef,
     FileTypeDef,
     FolderTypeDef,
     GetApprovalRuleTemplateInputRequestTypeDef,
     GetBlobInputRequestTypeDef,
-    GetBlobOutputTypeDef,
     GetBranchInputRequestTypeDef,
     GetCommentInputRequestTypeDef,
     GetCommentReactionsInputRequestTypeDef,
-    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForComparedCommitInputRequestTypeDef,
-    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetCommentsForPullRequestInputRequestTypeDef,
     GetCommitInputRequestTypeDef,
-    GetDifferencesInputGetDifferencesPaginateTypeDef,
     GetDifferencesInputRequestTypeDef,
     GetFileInputRequestTypeDef,
-    GetFileOutputTypeDef,
     GetFolderInputRequestTypeDef,
     SubModuleTypeDef,
     SymbolicLinkTypeDef,
     GetMergeCommitInputRequestTypeDef,
-    GetMergeCommitOutputTypeDef,
     GetMergeConflictsInputRequestTypeDef,
     GetMergeOptionsInputRequestTypeDef,
-    GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
-    GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
     RepositoryTriggerOutputTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
-    ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
-    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
-    ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
-    ListBranchesOutputTypeDef,
-    ListPullRequestsInputListPullRequestsPaginateTypeDef,
     ListPullRequestsInputRequestTypeDef,
-    ListPullRequestsOutputTypeDef,
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
-    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    LocationTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
-    MergeBranchesByFastForwardOutputTypeDef,
-    MergeBranchesBySquashOutputTypeDef,
-    MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
     OverridePullRequestApprovalRulesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
     PutFileInputRequestTypeDef,
-    PutFileOutputTypeDef,
     RepositoryTriggerTypeDef,
-    PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
     UpdatePullRequestApprovalRuleContentInputRequestTypeDef,
     UpdatePullRequestApprovalStateInputRequestTypeDef,
     UpdatePullRequestDescriptionInputRequestTypeDef,
     UpdatePullRequestStatusInputRequestTypeDef,
     UpdatePullRequestTitleInputRequestTypeDef,
     UpdateRepositoryDescriptionInputRequestTypeDef,
     UpdateRepositoryNameInputRequestTypeDef,
+    ApprovalRuleTypeDef,
+    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
+    CreateUnreferencedMergeCommitOutputTypeDef,
+    DeleteApprovalRuleTemplateOutputTypeDef,
+    DeleteFileOutputTypeDef,
+    DeletePullRequestApprovalRuleOutputTypeDef,
+    DeleteRepositoryOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApprovalRuleTemplateOutputTypeDef,
+    GetBlobOutputTypeDef,
+    GetFileOutputTypeDef,
+    GetMergeCommitOutputTypeDef,
+    GetMergeOptionsOutputTypeDef,
+    GetPullRequestApprovalStatesOutputTypeDef,
+    GetPullRequestOverrideStateOutputTypeDef,
+    ListApprovalRuleTemplatesOutputTypeDef,
+    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
+    ListBranchesOutputTypeDef,
+    ListPullRequestsOutputTypeDef,
+    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    MergeBranchesByFastForwardOutputTypeDef,
+    MergeBranchesBySquashOutputTypeDef,
+    MergeBranchesByThreeWayOutputTypeDef,
+    PutFileOutputTypeDef,
+    PutRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
-    ApprovalRuleTypeDef,
-    GetPullRequestApprovalStatesOutputTypeDef,
-    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
+    PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
+    PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
     ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
+    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    GetDifferencesInputGetDifferencesPaginateTypeDef,
+    ListBranchesInputListBranchesPaginateTypeDef,
+    ListPullRequestsInputListPullRequestsPaginateTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
     ListRepositoriesOutputTypeDef,
-    PostCommentForComparedCommitInputRequestTypeDef,
-    PostCommentForPullRequestInputRequestTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
     PutRepositoryTriggersInputRequestTypeDef,
     TestRepositoryTriggersInputRequestTypeDef,
     ReactionForCommentTypeDef,
```

### Comparing `mypy-boto3-codecommit-1.28.12/README.md` & `mypy-boto3-codecommit-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecommit)](https://pepy.tech/project/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,26 +336,27 @@
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
     ApprovalStateChangedEventMetadataTypeDef,
     ApprovalTypeDef,
     AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeMergeConflictsErrorTypeDef,
     BatchDescribeMergeConflictsInputRequestTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
-    LocationOutputTypeDef,
+    LocationTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
@@ -363,152 +364,150 @@
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
-    CreateUnreferencedMergeCommitOutputTypeDef,
     DeleteApprovalRuleTemplateInputRequestTypeDef,
-    DeleteApprovalRuleTemplateOutputTypeDef,
     DeleteBranchInputRequestTypeDef,
     DeleteCommentContentInputRequestTypeDef,
     DeleteFileInputRequestTypeDef,
-    DeleteFileOutputTypeDef,
     DeletePullRequestApprovalRuleInputRequestTypeDef,
-    DeletePullRequestApprovalRuleOutputTypeDef,
     DeleteRepositoryInputRequestTypeDef,
-    DeleteRepositoryOutputTypeDef,
     DescribeMergeConflictsInputRequestTypeDef,
-    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribePullRequestEventsInputRequestTypeDef,
     DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluatePullRequestApprovalRulesInputRequestTypeDef,
     EvaluationTypeDef,
     FileTypeDef,
     FolderTypeDef,
     GetApprovalRuleTemplateInputRequestTypeDef,
     GetBlobInputRequestTypeDef,
-    GetBlobOutputTypeDef,
     GetBranchInputRequestTypeDef,
     GetCommentInputRequestTypeDef,
     GetCommentReactionsInputRequestTypeDef,
-    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForComparedCommitInputRequestTypeDef,
-    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetCommentsForPullRequestInputRequestTypeDef,
     GetCommitInputRequestTypeDef,
-    GetDifferencesInputGetDifferencesPaginateTypeDef,
     GetDifferencesInputRequestTypeDef,
     GetFileInputRequestTypeDef,
-    GetFileOutputTypeDef,
     GetFolderInputRequestTypeDef,
     SubModuleTypeDef,
     SymbolicLinkTypeDef,
     GetMergeCommitInputRequestTypeDef,
-    GetMergeCommitOutputTypeDef,
     GetMergeConflictsInputRequestTypeDef,
     GetMergeOptionsInputRequestTypeDef,
-    GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
-    GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
     RepositoryTriggerOutputTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
-    ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
-    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
-    ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
-    ListBranchesOutputTypeDef,
-    ListPullRequestsInputListPullRequestsPaginateTypeDef,
     ListPullRequestsInputRequestTypeDef,
-    ListPullRequestsOutputTypeDef,
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
-    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    LocationTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
-    MergeBranchesByFastForwardOutputTypeDef,
-    MergeBranchesBySquashOutputTypeDef,
-    MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
     OverridePullRequestApprovalRulesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
     PutFileInputRequestTypeDef,
-    PutFileOutputTypeDef,
     RepositoryTriggerTypeDef,
-    PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
     UpdatePullRequestApprovalRuleContentInputRequestTypeDef,
     UpdatePullRequestApprovalStateInputRequestTypeDef,
     UpdatePullRequestDescriptionInputRequestTypeDef,
     UpdatePullRequestStatusInputRequestTypeDef,
     UpdatePullRequestTitleInputRequestTypeDef,
     UpdateRepositoryDescriptionInputRequestTypeDef,
     UpdateRepositoryNameInputRequestTypeDef,
+    ApprovalRuleTypeDef,
+    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
+    CreateUnreferencedMergeCommitOutputTypeDef,
+    DeleteApprovalRuleTemplateOutputTypeDef,
+    DeleteFileOutputTypeDef,
+    DeletePullRequestApprovalRuleOutputTypeDef,
+    DeleteRepositoryOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApprovalRuleTemplateOutputTypeDef,
+    GetBlobOutputTypeDef,
+    GetFileOutputTypeDef,
+    GetMergeCommitOutputTypeDef,
+    GetMergeOptionsOutputTypeDef,
+    GetPullRequestApprovalStatesOutputTypeDef,
+    GetPullRequestOverrideStateOutputTypeDef,
+    ListApprovalRuleTemplatesOutputTypeDef,
+    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
+    ListBranchesOutputTypeDef,
+    ListPullRequestsOutputTypeDef,
+    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    MergeBranchesByFastForwardOutputTypeDef,
+    MergeBranchesBySquashOutputTypeDef,
+    MergeBranchesByThreeWayOutputTypeDef,
+    PutFileOutputTypeDef,
+    PutRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
-    ApprovalRuleTypeDef,
-    GetPullRequestApprovalStatesOutputTypeDef,
-    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
+    PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
+    PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
     ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
+    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    GetDifferencesInputGetDifferencesPaginateTypeDef,
+    ListBranchesInputListBranchesPaginateTypeDef,
+    ListPullRequestsInputListPullRequestsPaginateTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
     ListRepositoriesOutputTypeDef,
-    PostCommentForComparedCommitInputRequestTypeDef,
-    PostCommentForPullRequestInputRequestTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
     PutRepositoryTriggersInputRequestTypeDef,
     TestRepositoryTriggersInputRequestTypeDef,
     ReactionForCommentTypeDef,
```

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__init__.py` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__init__.pyi` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__main__.py` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeCommit 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodeCommit 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit\nOther"
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

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/client.py` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/client.pyi` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/literals.py` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/literals.pyi` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/paginator.py` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,153 +58,144 @@
     "GetCommentsForPullRequestPaginator",
     "GetDifferencesPaginator",
     "ListBranchesPaginator",
     "ListPullRequestsPaginator",
     "ListRepositoriesPaginator",
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
 class DescribePullRequestEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#describepullrequesteventspaginator)
     """
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         pullRequestEventType: PullRequestEventTypeType = ...,
         actorArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePullRequestEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#describepullrequesteventspaginator)
         """
 
-
 class GetCommentsForComparedCommitPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         beforeCommitId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetCommentsForComparedCommitOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
         """
 
-
 class GetCommentsForPullRequestPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforpullrequestpaginator)
     """
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         repositoryName: str = ...,
         beforeCommitId: str = ...,
         afterCommitId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetCommentsForPullRequestOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforpullrequestpaginator)
         """
 
-
 class GetDifferencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getdifferencespaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitSpecifier: str,
         beforeCommitSpecifier: str = ...,
         beforePath: str = ...,
         afterPath: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDifferencesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getdifferencespaginator)
         """
 
-
 class ListBranchesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listbranchespaginator)
     """
 
     def paginate(
-        self, *, repositoryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, repositoryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBranchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listbranchespaginator)
         """
 
-
 class ListPullRequestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listpullrequestspaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         authorArn: str = ...,
         pullRequestStatus: PullRequestStatusEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPullRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listpullrequestspaginator)
         """
 
-
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
         self,
         *,
         sortBy: SortByEnumType = ...,
         order: OrderEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listrepositoriespaginator)
         """
```

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/paginator.pyi` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,144 +58,153 @@
     "GetCommentsForPullRequestPaginator",
     "GetDifferencesPaginator",
     "ListBranchesPaginator",
     "ListPullRequestsPaginator",
     "ListRepositoriesPaginator",
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
 class DescribePullRequestEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#describepullrequesteventspaginator)
     """
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         pullRequestEventType: PullRequestEventTypeType = ...,
         actorArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePullRequestEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#describepullrequesteventspaginator)
         """
 
+
 class GetCommentsForComparedCommitPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         beforeCommitId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetCommentsForComparedCommitOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
         """
 
+
 class GetCommentsForPullRequestPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforpullrequestpaginator)
     """
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         repositoryName: str = ...,
         beforeCommitId: str = ...,
         afterCommitId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetCommentsForPullRequestOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforpullrequestpaginator)
         """
 
+
 class GetDifferencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getdifferencespaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitSpecifier: str,
         beforeCommitSpecifier: str = ...,
         beforePath: str = ...,
         afterPath: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDifferencesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getdifferencespaginator)
         """
 
+
 class ListBranchesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listbranchespaginator)
     """
 
     def paginate(
-        self, *, repositoryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, repositoryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBranchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listbranchespaginator)
         """
 
+
 class ListPullRequestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listpullrequestspaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         authorArn: str = ...,
         pullRequestStatus: PullRequestStatusEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPullRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listpullrequestspaginator)
         """
 
+
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
         self,
         *,
         sortBy: SortByEnumType = ...,
         order: OrderEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listrepositoriespaginator)
         """
```

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/type_defs.py` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,26 +47,27 @@
     "ApprovalRuleTemplateTypeDef",
     "OriginApprovalRuleTemplateTypeDef",
     "ApprovalStateChangedEventMetadataTypeDef",
     "ApprovalTypeDef",
     "AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDescribeMergeConflictsErrorTypeDef",
     "BatchDescribeMergeConflictsInputRequestTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef",
     "BatchGetCommitsErrorTypeDef",
     "BatchGetCommitsInputRequestTypeDef",
     "BatchGetRepositoriesInputRequestTypeDef",
     "RepositoryMetadataTypeDef",
     "BlobMetadataTypeDef",
     "BranchInfoTypeDef",
     "CommentTypeDef",
-    "LocationOutputTypeDef",
+    "LocationTypeDef",
     "UserInfoTypeDef",
     "FileModesTypeDef",
     "FileSizesTypeDef",
     "IsBinaryFileTypeDef",
     "MergeOperationsTypeDef",
     "ObjectTypesTypeDef",
     "DeleteFileEntryTypeDef",
@@ -74,152 +75,150 @@
     "SetFileModeEntryTypeDef",
     "CreateApprovalRuleTemplateInputRequestTypeDef",
     "CreateBranchInputRequestTypeDef",
     "FileMetadataTypeDef",
     "CreatePullRequestApprovalRuleInputRequestTypeDef",
     "TargetTypeDef",
     "CreateRepositoryInputRequestTypeDef",
-    "CreateUnreferencedMergeCommitOutputTypeDef",
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
-    "DeleteApprovalRuleTemplateOutputTypeDef",
     "DeleteBranchInputRequestTypeDef",
     "DeleteCommentContentInputRequestTypeDef",
     "DeleteFileInputRequestTypeDef",
-    "DeleteFileOutputTypeDef",
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
-    "DeletePullRequestApprovalRuleOutputTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
-    "DeleteRepositoryOutputTypeDef",
     "DescribeMergeConflictsInputRequestTypeDef",
-    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribePullRequestEventsInputRequestTypeDef",
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     "EvaluationTypeDef",
     "FileTypeDef",
     "FolderTypeDef",
     "GetApprovalRuleTemplateInputRequestTypeDef",
     "GetBlobInputRequestTypeDef",
-    "GetBlobOutputTypeDef",
     "GetBranchInputRequestTypeDef",
     "GetCommentInputRequestTypeDef",
     "GetCommentReactionsInputRequestTypeDef",
-    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
     "GetCommentsForComparedCommitInputRequestTypeDef",
-    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
     "GetCommentsForPullRequestInputRequestTypeDef",
     "GetCommitInputRequestTypeDef",
-    "GetDifferencesInputGetDifferencesPaginateTypeDef",
     "GetDifferencesInputRequestTypeDef",
     "GetFileInputRequestTypeDef",
-    "GetFileOutputTypeDef",
     "GetFolderInputRequestTypeDef",
     "SubModuleTypeDef",
     "SymbolicLinkTypeDef",
     "GetMergeCommitInputRequestTypeDef",
-    "GetMergeCommitOutputTypeDef",
     "GetMergeConflictsInputRequestTypeDef",
     "GetMergeOptionsInputRequestTypeDef",
-    "GetMergeOptionsOutputTypeDef",
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     "GetPullRequestInputRequestTypeDef",
     "GetPullRequestOverrideStateInputRequestTypeDef",
-    "GetPullRequestOverrideStateOutputTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositoryTriggersInputRequestTypeDef",
     "RepositoryTriggerOutputTypeDef",
     "ListApprovalRuleTemplatesInputRequestTypeDef",
-    "ListApprovalRuleTemplatesOutputTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    "ListBranchesInputListBranchesPaginateTypeDef",
     "ListBranchesInputRequestTypeDef",
-    "ListBranchesOutputTypeDef",
-    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
     "ListPullRequestsInputRequestTypeDef",
-    "ListPullRequestsOutputTypeDef",
     "ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositoryNameIdPairTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "LocationTypeDef",
     "MergeBranchesByFastForwardInputRequestTypeDef",
-    "MergeBranchesByFastForwardOutputTypeDef",
-    "MergeBranchesBySquashOutputTypeDef",
-    "MergeBranchesByThreeWayOutputTypeDef",
     "MergeHunkDetailTypeDef",
     "MergeMetadataTypeDef",
     "MergePullRequestByFastForwardInputRequestTypeDef",
     "OverridePullRequestApprovalRulesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PostCommentReplyInputRequestTypeDef",
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
     "PutFileInputRequestTypeDef",
-    "PutFileOutputTypeDef",
     "RepositoryTriggerTypeDef",
-    "PutRepositoryTriggersOutputTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
     "UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef",
     "UpdateApprovalRuleTemplateNameInputRequestTypeDef",
     "UpdateCommentInputRequestTypeDef",
     "UpdateDefaultBranchInputRequestTypeDef",
     "UpdatePullRequestApprovalRuleContentInputRequestTypeDef",
     "UpdatePullRequestApprovalStateInputRequestTypeDef",
     "UpdatePullRequestDescriptionInputRequestTypeDef",
     "UpdatePullRequestStatusInputRequestTypeDef",
     "UpdatePullRequestTitleInputRequestTypeDef",
     "UpdateRepositoryDescriptionInputRequestTypeDef",
     "UpdateRepositoryNameInputRequestTypeDef",
+    "ApprovalRuleTypeDef",
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "CreateApprovalRuleTemplateOutputTypeDef",
+    "CreateUnreferencedMergeCommitOutputTypeDef",
+    "DeleteApprovalRuleTemplateOutputTypeDef",
+    "DeleteFileOutputTypeDef",
+    "DeletePullRequestApprovalRuleOutputTypeDef",
+    "DeleteRepositoryOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetApprovalRuleTemplateOutputTypeDef",
+    "GetBlobOutputTypeDef",
+    "GetFileOutputTypeDef",
+    "GetMergeCommitOutputTypeDef",
+    "GetMergeOptionsOutputTypeDef",
+    "GetPullRequestApprovalStatesOutputTypeDef",
+    "GetPullRequestOverrideStateOutputTypeDef",
+    "ListApprovalRuleTemplatesOutputTypeDef",
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    "ListBranchesOutputTypeDef",
+    "ListPullRequestsOutputTypeDef",
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "MergeBranchesByFastForwardOutputTypeDef",
+    "MergeBranchesBySquashOutputTypeDef",
+    "MergeBranchesByThreeWayOutputTypeDef",
+    "PutFileOutputTypeDef",
+    "PutRepositoryTriggersOutputTypeDef",
     "UpdateApprovalRuleTemplateContentOutputTypeDef",
     "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
     "UpdateApprovalRuleTemplateNameOutputTypeDef",
-    "ApprovalRuleTypeDef",
-    "GetPullRequestApprovalStatesOutputTypeDef",
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     "BatchGetRepositoriesOutputTypeDef",
     "CreateRepositoryOutputTypeDef",
     "GetRepositoryOutputTypeDef",
     "DifferenceTypeDef",
     "DeleteBranchOutputTypeDef",
     "GetBranchOutputTypeDef",
     "DeleteCommentContentOutputTypeDef",
     "GetCommentOutputTypeDef",
     "PostCommentReplyOutputTypeDef",
     "UpdateCommentOutputTypeDef",
     "CommentsForComparedCommitTypeDef",
     "CommentsForPullRequestTypeDef",
+    "PostCommentForComparedCommitInputRequestTypeDef",
     "PostCommentForComparedCommitOutputTypeDef",
+    "PostCommentForPullRequestInputRequestTypeDef",
     "PostCommentForPullRequestOutputTypeDef",
     "CommitTypeDef",
     "ConflictMetadataTypeDef",
     "ConflictResolutionTypeDef",
     "CreateCommitOutputTypeDef",
     "CreatePullRequestInputRequestTypeDef",
+    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    "GetDifferencesInputGetDifferencesPaginateTypeDef",
+    "ListBranchesInputListBranchesPaginateTypeDef",
+    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
     "ListRepositoriesOutputTypeDef",
-    "PostCommentForComparedCommitInputRequestTypeDef",
-    "PostCommentForPullRequestInputRequestTypeDef",
     "MergeHunkTypeDef",
     "PullRequestMergedStateChangedEventMetadataTypeDef",
     "PullRequestTargetTypeDef",
     "PutFileEntryTypeDef",
     "PutRepositoryTriggersInputRequestTypeDef",
     "TestRepositoryTriggersInputRequestTypeDef",
     "ReactionForCommentTypeDef",
@@ -338,14 +337,25 @@
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryNames": Sequence[str],
     },
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
 BatchDescribeMergeConflictsErrorTypeDef = TypedDict(
     "BatchDescribeMergeConflictsErrorTypeDef",
     {
         "filePath": str,
         "exceptionName": str,
         "message": str,
     },
@@ -473,16 +483,16 @@
         "clientRequestToken": str,
         "callerReactions": List[str],
         "reactionCounts": Dict[str, int],
     },
     total=False,
 )
 
-LocationOutputTypeDef = TypedDict(
-    "LocationOutputTypeDef",
+LocationTypeDef = TypedDict(
+    "LocationTypeDef",
     {
         "filePath": str,
         "filePosition": int,
         "relativeFileVersion": RelativeFileVersionEnumType,
     },
     total=False,
 )
@@ -673,38 +683,21 @@
 
 class CreateRepositoryInputRequestTypeDef(
     _RequiredCreateRepositoryInputRequestTypeDef, _OptionalCreateRepositoryInputRequestTypeDef
 ):
     pass
 
 
-CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
-    "CreateUnreferencedMergeCommitOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 
-DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "DeleteApprovalRuleTemplateOutputTypeDef",
-    {
-        "approvalRuleTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBranchInputRequestTypeDef = TypedDict(
     "DeleteBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
 )
@@ -739,56 +732,29 @@
 
 class DeleteFileInputRequestTypeDef(
     _RequiredDeleteFileInputRequestTypeDef, _OptionalDeleteFileInputRequestTypeDef
 ):
     pass
 
 
-DeleteFileOutputTypeDef = TypedDict(
-    "DeleteFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "filePath": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePullRequestApprovalRuleInputRequestTypeDef = TypedDict(
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
     {
         "pullRequestId": str,
         "approvalRuleName": str,
     },
 )
 
-DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
-    "DeletePullRequestApprovalRuleOutputTypeDef",
-    {
-        "approvalRuleId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRepositoryInputRequestTypeDef = TypedDict(
     "DeleteRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
-DeleteRepositoryOutputTypeDef = TypedDict(
-    "DeleteRepositoryOutputTypeDef",
-    {
-        "repositoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -810,38 +776,24 @@
 class DescribeMergeConflictsInputRequestTypeDef(
     _RequiredDescribeMergeConflictsInputRequestTypeDef,
     _OptionalDescribeMergeConflictsInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "pullRequestEventType": PullRequestEventTypeType,
-        "actorArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
-    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribePullRequestEventsInputRequestTypeDef = TypedDict(
     "_RequiredDescribePullRequestEventsInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalDescribePullRequestEventsInputRequestTypeDef = TypedDict(
@@ -867,21 +819,14 @@
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluatePullRequestApprovalRulesInputRequestTypeDef = TypedDict(
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -929,22 +874,14 @@
     "GetBlobInputRequestTypeDef",
     {
         "repositoryName": str,
         "blobId": str,
     },
 )
 
-GetBlobOutputTypeDef = TypedDict(
-    "GetBlobOutputTypeDef",
-    {
-        "content": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBranchInputRequestTypeDef = TypedDict(
     "GetBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
     total=False,
@@ -976,38 +913,14 @@
 
 class GetCommentReactionsInputRequestTypeDef(
     _RequiredGetCommentReactionsInputRequestTypeDef, _OptionalGetCommentReactionsInputRequestTypeDef
 ):
     pass
 
 
-_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitId": str,
-    },
-)
-_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "beforeCommitId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
-    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetCommentsForComparedCommitInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForComparedCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitId": str,
     },
 )
@@ -1025,39 +938,14 @@
 class GetCommentsForComparedCommitInputRequestTypeDef(
     _RequiredGetCommentsForComparedCommitInputRequestTypeDef,
     _OptionalGetCommentsForComparedCommitInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "beforeCommitId": str,
-        "afterCommitId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
-    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForPullRequestInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
@@ -1084,40 +972,14 @@
     "GetCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "commitId": str,
     },
 )
 
-_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitSpecifier": str,
-    },
-)
-_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "beforeCommitSpecifier": str,
-        "beforePath": str,
-        "afterPath": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetDifferencesInputGetDifferencesPaginateTypeDef(
-    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
-    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetDifferencesInputRequestTypeDef = TypedDict(
     "_RequiredGetDifferencesInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitSpecifier": str,
     },
 )
@@ -1158,27 +1020,14 @@
 
 class GetFileInputRequestTypeDef(
     _RequiredGetFileInputRequestTypeDef, _OptionalGetFileInputRequestTypeDef
 ):
     pass
 
 
-GetFileOutputTypeDef = TypedDict(
-    "GetFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "filePath": str,
-        "fileMode": FileModeTypeEnumType,
-        "fileSize": int,
-        "fileContent": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetFolderInputRequestTypeDef = TypedDict(
     "_RequiredGetFolderInputRequestTypeDef",
     {
         "repositoryName": str,
         "folderPath": str,
     },
 )
@@ -1238,25 +1087,14 @@
 
 class GetMergeCommitInputRequestTypeDef(
     _RequiredGetMergeCommitInputRequestTypeDef, _OptionalGetMergeCommitInputRequestTypeDef
 ):
     pass
 
 
-GetMergeCommitOutputTypeDef = TypedDict(
-    "GetMergeCommitOutputTypeDef",
-    {
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "mergedCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredGetMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -1300,25 +1138,14 @@
 
 class GetMergeOptionsInputRequestTypeDef(
     _RequiredGetMergeOptionsInputRequestTypeDef, _OptionalGetMergeOptionsInputRequestTypeDef
 ):
     pass
 
 
-GetMergeOptionsOutputTypeDef = TypedDict(
-    "GetMergeOptionsOutputTypeDef",
-    {
-        "mergeOptions": List[MergeOptionTypeEnumType],
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPullRequestApprovalStatesInputRequestTypeDef = TypedDict(
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -1334,23 +1161,14 @@
     "GetPullRequestOverrideStateInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
 
-GetPullRequestOverrideStateOutputTypeDef = TypedDict(
-    "GetPullRequestOverrideStateOutputTypeDef",
-    {
-        "overridden": bool,
-        "overrider": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRepositoryInputRequestTypeDef = TypedDict(
     "GetRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
@@ -1390,23 +1208,14 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
-    "ListApprovalRuleTemplatesOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
     "_RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
@@ -1422,45 +1231,14 @@
 class ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef(
     _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
     _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
 ):
     pass
 
 
-ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListBranchesInputListBranchesPaginateTypeDef(
-    _RequiredListBranchesInputListBranchesPaginateTypeDef,
-    _OptionalListBranchesInputListBranchesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBranchesInputRequestTypeDef = TypedDict(
     "_RequiredListBranchesInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListBranchesInputRequestTypeDef = TypedDict(
@@ -1474,47 +1252,14 @@
 
 class ListBranchesInputRequestTypeDef(
     _RequiredListBranchesInputRequestTypeDef, _OptionalListBranchesInputRequestTypeDef
 ):
     pass
 
 
-ListBranchesOutputTypeDef = TypedDict(
-    "ListBranchesOutputTypeDef",
-    {
-        "branches": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "authorArn": str,
-        "pullRequestStatus": PullRequestStatusEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPullRequestsInputListPullRequestsPaginateTypeDef(
-    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
-    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPullRequestsInputRequestTypeDef = TypedDict(
     "_RequiredListPullRequestsInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListPullRequestsInputRequestTypeDef = TypedDict(
@@ -1531,23 +1276,14 @@
 
 class ListPullRequestsInputRequestTypeDef(
     _RequiredListPullRequestsInputRequestTypeDef, _OptionalListPullRequestsInputRequestTypeDef
 ):
     pass
 
 
-ListPullRequestsOutputTypeDef = TypedDict(
-    "ListPullRequestsOutputTypeDef",
-    {
-        "pullRequestIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
@@ -1563,33 +1299,14 @@
 class ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef(
     _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
     _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
 ):
     pass
 
 
-ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    {
-        "repositoryNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
-    {
-        "sortBy": SortByEnumType,
-        "order": OrderEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRepositoriesInputRequestTypeDef = TypedDict(
     "ListRepositoriesInputRequestTypeDef",
     {
         "nextToken": str,
         "sortBy": SortByEnumType,
         "order": OrderEnumType,
     },
@@ -1622,33 +1339,14 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LocationTypeDef = TypedDict(
-    "LocationTypeDef",
-    {
-        "filePath": str,
-        "filePosition": int,
-        "relativeFileVersion": RelativeFileVersionEnumType,
-    },
-    total=False,
-)
-
 _RequiredMergeBranchesByFastForwardInputRequestTypeDef = TypedDict(
     "_RequiredMergeBranchesByFastForwardInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
     },
@@ -1665,41 +1363,14 @@
 class MergeBranchesByFastForwardInputRequestTypeDef(
     _RequiredMergeBranchesByFastForwardInputRequestTypeDef,
     _OptionalMergeBranchesByFastForwardInputRequestTypeDef,
 ):
     pass
 
 
-MergeBranchesByFastForwardOutputTypeDef = TypedDict(
-    "MergeBranchesByFastForwardOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MergeBranchesBySquashOutputTypeDef = TypedDict(
-    "MergeBranchesBySquashOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MergeBranchesByThreeWayOutputTypeDef = TypedDict(
-    "MergeBranchesByThreeWayOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MergeHunkDetailTypeDef = TypedDict(
     "MergeHunkDetailTypeDef",
     {
         "startLine": int,
         "endLine": int,
         "hunkContent": str,
     },
@@ -1745,24 +1416,14 @@
     {
         "pullRequestId": str,
         "revisionId": str,
         "overrideStatus": OverrideStatusType,
     },
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
 _RequiredPostCommentReplyInputRequestTypeDef = TypedDict(
     "_RequiredPostCommentReplyInputRequestTypeDef",
     {
         "inReplyTo": str,
         "content": str,
     },
 )
@@ -1864,24 +1525,14 @@
 
 class PutFileInputRequestTypeDef(
     _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
 ):
     pass
 
 
-PutFileOutputTypeDef = TypedDict(
-    "PutFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRepositoryTriggerTypeDef = TypedDict(
     "_RequiredRepositoryTriggerTypeDef",
     {
         "name": str,
         "destinationArn": str,
         "events": Sequence[RepositoryTriggerEventEnumType],
     },
@@ -1898,22 +1549,14 @@
 
 class RepositoryTriggerTypeDef(
     _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
 ):
     pass
 
 
-PutRepositoryTriggersOutputTypeDef = TypedDict(
-    "PutRepositoryTriggersOutputTypeDef",
-    {
-        "configurationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReactionValueFormatsTypeDef = TypedDict(
     "ReactionValueFormatsTypeDef",
     {
         "emoji": str,
         "shortCode": str,
         "unicode": str,
     },
@@ -1925,25 +1568,14 @@
     {
         "trigger": str,
         "failureMessage": str,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -2094,117 +1726,319 @@
     "UpdateRepositoryNameInputRequestTypeDef",
     {
         "oldName": str,
         "newName": str,
     },
 )
 
+ApprovalRuleTypeDef = TypedDict(
+    "ApprovalRuleTypeDef",
+    {
+        "approvalRuleId": str,
+        "approvalRuleName": str,
+        "approvalRuleContent": str,
+        "ruleContentSha256": str,
+        "lastModifiedDate": datetime,
+        "creationDate": datetime,
+        "lastModifiedUser": str,
+        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
+    },
+    total=False,
+)
+
+BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
+    {
+        "associatedRepositoryNames": List[str],
+        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApprovalRuleTemplateOutputTypeDef = TypedDict(
     "CreateApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
+    "CreateUnreferencedMergeCommitOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "DeleteApprovalRuleTemplateOutputTypeDef",
+    {
+        "approvalRuleTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFileOutputTypeDef = TypedDict(
+    "DeleteFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "filePath": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
+    "DeletePullRequestApprovalRuleOutputTypeDef",
+    {
+        "approvalRuleId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRepositoryOutputTypeDef = TypedDict(
+    "DeleteRepositoryOutputTypeDef",
+    {
+        "repositoryId": str,
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
 
 GetApprovalRuleTemplateOutputTypeDef = TypedDict(
     "GetApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateContentOutputTypeDef",
+GetBlobOutputTypeDef = TypedDict(
+    "GetBlobOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "content": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
+GetFileOutputTypeDef = TypedDict(
+    "GetFileOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "commitId": str,
+        "blobId": str,
+        "filePath": str,
+        "fileMode": FileModeTypeEnumType,
+        "fileSize": int,
+        "fileContent": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateNameOutputTypeDef",
+GetMergeCommitOutputTypeDef = TypedDict(
+    "GetMergeCommitOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "mergedCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ApprovalRuleTypeDef = TypedDict(
-    "ApprovalRuleTypeDef",
+GetMergeOptionsOutputTypeDef = TypedDict(
+    "GetMergeOptionsOutputTypeDef",
     {
-        "approvalRuleId": str,
-        "approvalRuleName": str,
-        "approvalRuleContent": str,
-        "ruleContentSha256": str,
-        "lastModifiedDate": datetime,
-        "creationDate": datetime,
-        "lastModifiedUser": str,
-        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
+        "mergeOptions": List[MergeOptionTypeEnumType],
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetPullRequestApprovalStatesOutputTypeDef = TypedDict(
     "GetPullRequestApprovalStatesOutputTypeDef",
     {
         "approvals": List[ApprovalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
+GetPullRequestOverrideStateOutputTypeDef = TypedDict(
+    "GetPullRequestOverrideStateOutputTypeDef",
     {
-        "associatedRepositoryNames": List[str],
-        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "overridden": bool,
+        "overrider": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
+    "ListApprovalRuleTemplatesOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBranchesOutputTypeDef = TypedDict(
+    "ListBranchesOutputTypeDef",
+    {
+        "branches": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPullRequestsOutputTypeDef = TypedDict(
+    "ListPullRequestsOutputTypeDef",
+    {
+        "pullRequestIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    {
+        "repositoryNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesByFastForwardOutputTypeDef = TypedDict(
+    "MergeBranchesByFastForwardOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesBySquashOutputTypeDef = TypedDict(
+    "MergeBranchesBySquashOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesByThreeWayOutputTypeDef = TypedDict(
+    "MergeBranchesByThreeWayOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutFileOutputTypeDef = TypedDict(
+    "PutFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRepositoryTriggersOutputTypeDef = TypedDict(
+    "PutRepositoryTriggersOutputTypeDef",
+    {
+        "configurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateContentOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateNameOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef = TypedDict(
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     {
         "disassociatedRepositoryNames": List[str],
         "errors": List[BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetRepositoriesOutputTypeDef = TypedDict(
     "BatchGetRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryMetadataTypeDef],
         "repositoriesNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryOutputTypeDef = TypedDict(
     "CreateRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRepositoryOutputTypeDef = TypedDict(
     "GetRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DifferenceTypeDef = TypedDict(
     "DifferenceTypeDef",
     {
         "beforeBlob": BlobMetadataTypeDef,
@@ -2214,113 +2048,166 @@
     total=False,
 )
 
 DeleteBranchOutputTypeDef = TypedDict(
     "DeleteBranchOutputTypeDef",
     {
         "deletedBranch": BranchInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBranchOutputTypeDef = TypedDict(
     "GetBranchOutputTypeDef",
     {
         "branch": BranchInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCommentContentOutputTypeDef = TypedDict(
     "DeleteCommentContentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommentOutputTypeDef = TypedDict(
     "GetCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PostCommentReplyOutputTypeDef = TypedDict(
     "PostCommentReplyOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCommentOutputTypeDef = TypedDict(
     "UpdateCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommentsForComparedCommitTypeDef = TypedDict(
     "CommentsForComparedCommitTypeDef",
     {
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationOutputTypeDef,
+        "location": LocationTypeDef,
         "comments": List[CommentTypeDef],
     },
     total=False,
 )
 
 CommentsForPullRequestTypeDef = TypedDict(
     "CommentsForPullRequestTypeDef",
     {
         "pullRequestId": str,
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationOutputTypeDef,
+        "location": LocationTypeDef,
         "comments": List[CommentTypeDef],
     },
     total=False,
 )
 
+_RequiredPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
+    "_RequiredPostCommentForComparedCommitInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "afterCommitId": str,
+        "content": str,
+    },
+)
+_OptionalPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
+    "_OptionalPostCommentForComparedCommitInputRequestTypeDef",
+    {
+        "beforeCommitId": str,
+        "location": LocationTypeDef,
+        "clientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class PostCommentForComparedCommitInputRequestTypeDef(
+    _RequiredPostCommentForComparedCommitInputRequestTypeDef,
+    _OptionalPostCommentForComparedCommitInputRequestTypeDef,
+):
+    pass
+
+
 PostCommentForComparedCommitOutputTypeDef = TypedDict(
     "PostCommentForComparedCommitOutputTypeDef",
     {
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationOutputTypeDef,
+        "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
+    "_RequiredPostCommentForPullRequestInputRequestTypeDef",
+    {
+        "pullRequestId": str,
+        "repositoryName": str,
+        "beforeCommitId": str,
+        "afterCommitId": str,
+        "content": str,
+    },
+)
+_OptionalPostCommentForPullRequestInputRequestTypeDef = TypedDict(
+    "_OptionalPostCommentForPullRequestInputRequestTypeDef",
+    {
+        "location": LocationTypeDef,
+        "clientRequestToken": str,
     },
+    total=False,
 )
 
+
+class PostCommentForPullRequestInputRequestTypeDef(
+    _RequiredPostCommentForPullRequestInputRequestTypeDef,
+    _OptionalPostCommentForPullRequestInputRequestTypeDef,
+):
+    pass
+
+
 PostCommentForPullRequestOutputTypeDef = TypedDict(
     "PostCommentForPullRequestOutputTypeDef",
     {
         "repositoryName": str,
         "pullRequestId": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationOutputTypeDef,
+        "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommitTypeDef = TypedDict(
     "CommitTypeDef",
     {
         "commitId": str,
@@ -2365,15 +2252,15 @@
     "CreateCommitOutputTypeDef",
     {
         "commitId": str,
         "treeId": str,
         "filesAdded": List[FileMetadataTypeDef],
         "filesUpdated": List[FileMetadataTypeDef],
         "filesDeleted": List[FileMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePullRequestInputRequestTypeDef = TypedDict(
     "_RequiredCreatePullRequestInputRequestTypeDef",
     {
         "title": str,
@@ -2392,107 +2279,209 @@
 
 class CreatePullRequestInputRequestTypeDef(
     _RequiredCreatePullRequestInputRequestTypeDef, _OptionalCreatePullRequestInputRequestTypeDef
 ):
     pass
 
 
-EvaluatePullRequestApprovalRulesOutputTypeDef = TypedDict(
-    "EvaluatePullRequestApprovalRulesOutputTypeDef",
+_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
     {
-        "evaluation": EvaluationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "pullRequestId": str,
+    },
+)
+_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    {
+        "pullRequestEventType": PullRequestEventTypeType,
+        "actorArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetFolderOutputTypeDef = TypedDict(
-    "GetFolderOutputTypeDef",
+
+class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
+    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
     {
-        "commitId": str,
-        "folderPath": str,
-        "treeId": str,
-        "subFolders": List[FolderTypeDef],
-        "files": List[FileTypeDef],
-        "symbolicLinks": List[SymbolicLinkTypeDef],
-        "subModules": List[SubModuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "repositoryName": str,
+        "afterCommitId": str,
+    },
+)
+_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    {
+        "beforeCommitId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetRepositoryTriggersOutputTypeDef = TypedDict(
-    "GetRepositoryTriggersOutputTypeDef",
+
+class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
+    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
     {
-        "configurationId": str,
-        "triggers": List[RepositoryTriggerOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "pullRequestId": str,
     },
 )
+_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "beforeCommitId": str,
+        "afterCommitId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ListRepositoriesOutputTypeDef = TypedDict(
-    "ListRepositoriesOutputTypeDef",
+
+class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
+    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
     {
-        "repositories": List[RepositoryNameIdPairTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "repositoryName": str,
+        "afterCommitSpecifier": str,
     },
 )
+_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
+    {
+        "beforeCommitSpecifier": str,
+        "beforePath": str,
+        "afterPath": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-_RequiredPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
-    "_RequiredPostCommentForComparedCommitInputRequestTypeDef",
+
+class GetDifferencesInputGetDifferencesPaginateTypeDef(
+    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
+    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
     {
         "repositoryName": str,
-        "afterCommitId": str,
-        "content": str,
     },
 )
-_OptionalPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
-    "_OptionalPostCommentForComparedCommitInputRequestTypeDef",
+_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
     {
-        "beforeCommitId": str,
-        "location": LocationTypeDef,
-        "clientRequestToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class PostCommentForComparedCommitInputRequestTypeDef(
-    _RequiredPostCommentForComparedCommitInputRequestTypeDef,
-    _OptionalPostCommentForComparedCommitInputRequestTypeDef,
+class ListBranchesInputListBranchesPaginateTypeDef(
+    _RequiredListBranchesInputListBranchesPaginateTypeDef,
+    _OptionalListBranchesInputListBranchesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
-    "_RequiredPostCommentForPullRequestInputRequestTypeDef",
+_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
     {
-        "pullRequestId": str,
         "repositoryName": str,
-        "beforeCommitId": str,
-        "afterCommitId": str,
-        "content": str,
     },
 )
-_OptionalPostCommentForPullRequestInputRequestTypeDef = TypedDict(
-    "_OptionalPostCommentForPullRequestInputRequestTypeDef",
+_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
     {
-        "location": LocationTypeDef,
-        "clientRequestToken": str,
+        "authorArn": str,
+        "pullRequestStatus": PullRequestStatusEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class PostCommentForPullRequestInputRequestTypeDef(
-    _RequiredPostCommentForPullRequestInputRequestTypeDef,
-    _OptionalPostCommentForPullRequestInputRequestTypeDef,
+class ListPullRequestsInputListPullRequestsPaginateTypeDef(
+    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
+    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
 ):
     pass
 
 
+ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
+    {
+        "sortBy": SortByEnumType,
+        "order": OrderEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+EvaluatePullRequestApprovalRulesOutputTypeDef = TypedDict(
+    "EvaluatePullRequestApprovalRulesOutputTypeDef",
+    {
+        "evaluation": EvaluationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFolderOutputTypeDef = TypedDict(
+    "GetFolderOutputTypeDef",
+    {
+        "commitId": str,
+        "folderPath": str,
+        "treeId": str,
+        "subFolders": List[FolderTypeDef],
+        "files": List[FileTypeDef],
+        "symbolicLinks": List[SymbolicLinkTypeDef],
+        "subModules": List[SubModuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRepositoryTriggersOutputTypeDef = TypedDict(
+    "GetRepositoryTriggersOutputTypeDef",
+    {
+        "configurationId": str,
+        "triggers": List[RepositoryTriggerOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRepositoriesOutputTypeDef = TypedDict(
+    "ListRepositoriesOutputTypeDef",
+    {
+        "repositories": List[RepositoryNameIdPairTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 MergeHunkTypeDef = TypedDict(
     "MergeHunkTypeDef",
     {
         "isConflict": bool,
         "source": MergeHunkDetailTypeDef,
         "destination": MergeHunkDetailTypeDef,
         "base": MergeHunkDetailTypeDef,
@@ -2572,88 +2561,88 @@
 )
 
 TestRepositoryTriggersOutputTypeDef = TypedDict(
     "TestRepositoryTriggersOutputTypeDef",
     {
         "successfulExecutions": List[str],
         "failedExecutions": List[RepositoryTriggerExecutionFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePullRequestApprovalRuleOutputTypeDef = TypedDict(
     "CreatePullRequestApprovalRuleOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestApprovalRuleContentOutputTypeDef = TypedDict(
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDifferencesOutputTypeDef = TypedDict(
     "GetDifferencesOutputTypeDef",
     {
         "differences": List[DifferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommentsForComparedCommitOutputTypeDef = TypedDict(
     "GetCommentsForComparedCommitOutputTypeDef",
     {
         "commentsForComparedCommitData": List[CommentsForComparedCommitTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommentsForPullRequestOutputTypeDef = TypedDict(
     "GetCommentsForPullRequestOutputTypeDef",
     {
         "commentsForPullRequestData": List[CommentsForPullRequestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetCommitsOutputTypeDef = TypedDict(
     "BatchGetCommitsOutputTypeDef",
     {
         "commits": List[CommitTypeDef],
         "errors": List[BatchGetCommitsErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommitOutputTypeDef = TypedDict(
     "GetCommitOutputTypeDef",
     {
         "commit": CommitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMergeConflictsOutputTypeDef = TypedDict(
     "GetMergeConflictsOutputTypeDef",
     {
         "mergeable": bool,
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
         "conflictMetadataList": List[ConflictMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUnreferencedMergeCommitInputRequestTypeDef = TypedDict(
     "_RequiredCreateUnreferencedMergeCommitInputRequestTypeDef",
     {
         "repositoryName": str,
@@ -2820,15 +2809,15 @@
     {
         "conflictMetadata": ConflictMetadataTypeDef,
         "mergeHunks": List[MergeHunkTypeDef],
         "nextToken": str,
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PullRequestEventTypeDef = TypedDict(
     "PullRequestEventTypeDef",
     {
         "pullRequestId": str,
@@ -2898,96 +2887,96 @@
 
 
 GetCommentReactionsOutputTypeDef = TypedDict(
     "GetCommentReactionsOutputTypeDef",
     {
         "reactionsForComment": List[ReactionForCommentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDescribeMergeConflictsOutputTypeDef = TypedDict(
     "BatchDescribeMergeConflictsOutputTypeDef",
     {
         "conflicts": List[ConflictTypeDef],
         "nextToken": str,
         "errors": List[BatchDescribeMergeConflictsErrorTypeDef],
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePullRequestEventsOutputTypeDef = TypedDict(
     "DescribePullRequestEventsOutputTypeDef",
     {
         "pullRequestEvents": List[PullRequestEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePullRequestOutputTypeDef = TypedDict(
     "CreatePullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPullRequestOutputTypeDef = TypedDict(
     "GetPullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestByFastForwardOutputTypeDef = TypedDict(
     "MergePullRequestByFastForwardOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestBySquashOutputTypeDef = TypedDict(
     "MergePullRequestBySquashOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestByThreeWayOutputTypeDef = TypedDict(
     "MergePullRequestByThreeWayOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestDescriptionOutputTypeDef = TypedDict(
     "UpdatePullRequestDescriptionOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestStatusOutputTypeDef = TypedDict(
     "UpdatePullRequestStatusOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestTitleOutputTypeDef = TypedDict(
     "UpdatePullRequestTitleOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/type_defs.pyi` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,27 @@
     "ApprovalRuleTemplateTypeDef",
     "OriginApprovalRuleTemplateTypeDef",
     "ApprovalStateChangedEventMetadataTypeDef",
     "ApprovalTypeDef",
     "AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDescribeMergeConflictsErrorTypeDef",
     "BatchDescribeMergeConflictsInputRequestTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef",
     "BatchGetCommitsErrorTypeDef",
     "BatchGetCommitsInputRequestTypeDef",
     "BatchGetRepositoriesInputRequestTypeDef",
     "RepositoryMetadataTypeDef",
     "BlobMetadataTypeDef",
     "BranchInfoTypeDef",
     "CommentTypeDef",
-    "LocationOutputTypeDef",
+    "LocationTypeDef",
     "UserInfoTypeDef",
     "FileModesTypeDef",
     "FileSizesTypeDef",
     "IsBinaryFileTypeDef",
     "MergeOperationsTypeDef",
     "ObjectTypesTypeDef",
     "DeleteFileEntryTypeDef",
@@ -73,152 +74,150 @@
     "SetFileModeEntryTypeDef",
     "CreateApprovalRuleTemplateInputRequestTypeDef",
     "CreateBranchInputRequestTypeDef",
     "FileMetadataTypeDef",
     "CreatePullRequestApprovalRuleInputRequestTypeDef",
     "TargetTypeDef",
     "CreateRepositoryInputRequestTypeDef",
-    "CreateUnreferencedMergeCommitOutputTypeDef",
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
-    "DeleteApprovalRuleTemplateOutputTypeDef",
     "DeleteBranchInputRequestTypeDef",
     "DeleteCommentContentInputRequestTypeDef",
     "DeleteFileInputRequestTypeDef",
-    "DeleteFileOutputTypeDef",
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
-    "DeletePullRequestApprovalRuleOutputTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
-    "DeleteRepositoryOutputTypeDef",
     "DescribeMergeConflictsInputRequestTypeDef",
-    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribePullRequestEventsInputRequestTypeDef",
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     "EvaluationTypeDef",
     "FileTypeDef",
     "FolderTypeDef",
     "GetApprovalRuleTemplateInputRequestTypeDef",
     "GetBlobInputRequestTypeDef",
-    "GetBlobOutputTypeDef",
     "GetBranchInputRequestTypeDef",
     "GetCommentInputRequestTypeDef",
     "GetCommentReactionsInputRequestTypeDef",
-    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
     "GetCommentsForComparedCommitInputRequestTypeDef",
-    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
     "GetCommentsForPullRequestInputRequestTypeDef",
     "GetCommitInputRequestTypeDef",
-    "GetDifferencesInputGetDifferencesPaginateTypeDef",
     "GetDifferencesInputRequestTypeDef",
     "GetFileInputRequestTypeDef",
-    "GetFileOutputTypeDef",
     "GetFolderInputRequestTypeDef",
     "SubModuleTypeDef",
     "SymbolicLinkTypeDef",
     "GetMergeCommitInputRequestTypeDef",
-    "GetMergeCommitOutputTypeDef",
     "GetMergeConflictsInputRequestTypeDef",
     "GetMergeOptionsInputRequestTypeDef",
-    "GetMergeOptionsOutputTypeDef",
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     "GetPullRequestInputRequestTypeDef",
     "GetPullRequestOverrideStateInputRequestTypeDef",
-    "GetPullRequestOverrideStateOutputTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositoryTriggersInputRequestTypeDef",
     "RepositoryTriggerOutputTypeDef",
     "ListApprovalRuleTemplatesInputRequestTypeDef",
-    "ListApprovalRuleTemplatesOutputTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    "ListBranchesInputListBranchesPaginateTypeDef",
     "ListBranchesInputRequestTypeDef",
-    "ListBranchesOutputTypeDef",
-    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
     "ListPullRequestsInputRequestTypeDef",
-    "ListPullRequestsOutputTypeDef",
     "ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositoryNameIdPairTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "LocationTypeDef",
     "MergeBranchesByFastForwardInputRequestTypeDef",
-    "MergeBranchesByFastForwardOutputTypeDef",
-    "MergeBranchesBySquashOutputTypeDef",
-    "MergeBranchesByThreeWayOutputTypeDef",
     "MergeHunkDetailTypeDef",
     "MergeMetadataTypeDef",
     "MergePullRequestByFastForwardInputRequestTypeDef",
     "OverridePullRequestApprovalRulesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PostCommentReplyInputRequestTypeDef",
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
     "PutFileInputRequestTypeDef",
-    "PutFileOutputTypeDef",
     "RepositoryTriggerTypeDef",
-    "PutRepositoryTriggersOutputTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
     "UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef",
     "UpdateApprovalRuleTemplateNameInputRequestTypeDef",
     "UpdateCommentInputRequestTypeDef",
     "UpdateDefaultBranchInputRequestTypeDef",
     "UpdatePullRequestApprovalRuleContentInputRequestTypeDef",
     "UpdatePullRequestApprovalStateInputRequestTypeDef",
     "UpdatePullRequestDescriptionInputRequestTypeDef",
     "UpdatePullRequestStatusInputRequestTypeDef",
     "UpdatePullRequestTitleInputRequestTypeDef",
     "UpdateRepositoryDescriptionInputRequestTypeDef",
     "UpdateRepositoryNameInputRequestTypeDef",
+    "ApprovalRuleTypeDef",
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "CreateApprovalRuleTemplateOutputTypeDef",
+    "CreateUnreferencedMergeCommitOutputTypeDef",
+    "DeleteApprovalRuleTemplateOutputTypeDef",
+    "DeleteFileOutputTypeDef",
+    "DeletePullRequestApprovalRuleOutputTypeDef",
+    "DeleteRepositoryOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetApprovalRuleTemplateOutputTypeDef",
+    "GetBlobOutputTypeDef",
+    "GetFileOutputTypeDef",
+    "GetMergeCommitOutputTypeDef",
+    "GetMergeOptionsOutputTypeDef",
+    "GetPullRequestApprovalStatesOutputTypeDef",
+    "GetPullRequestOverrideStateOutputTypeDef",
+    "ListApprovalRuleTemplatesOutputTypeDef",
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    "ListBranchesOutputTypeDef",
+    "ListPullRequestsOutputTypeDef",
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "MergeBranchesByFastForwardOutputTypeDef",
+    "MergeBranchesBySquashOutputTypeDef",
+    "MergeBranchesByThreeWayOutputTypeDef",
+    "PutFileOutputTypeDef",
+    "PutRepositoryTriggersOutputTypeDef",
     "UpdateApprovalRuleTemplateContentOutputTypeDef",
     "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
     "UpdateApprovalRuleTemplateNameOutputTypeDef",
-    "ApprovalRuleTypeDef",
-    "GetPullRequestApprovalStatesOutputTypeDef",
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     "BatchGetRepositoriesOutputTypeDef",
     "CreateRepositoryOutputTypeDef",
     "GetRepositoryOutputTypeDef",
     "DifferenceTypeDef",
     "DeleteBranchOutputTypeDef",
     "GetBranchOutputTypeDef",
     "DeleteCommentContentOutputTypeDef",
     "GetCommentOutputTypeDef",
     "PostCommentReplyOutputTypeDef",
     "UpdateCommentOutputTypeDef",
     "CommentsForComparedCommitTypeDef",
     "CommentsForPullRequestTypeDef",
+    "PostCommentForComparedCommitInputRequestTypeDef",
     "PostCommentForComparedCommitOutputTypeDef",
+    "PostCommentForPullRequestInputRequestTypeDef",
     "PostCommentForPullRequestOutputTypeDef",
     "CommitTypeDef",
     "ConflictMetadataTypeDef",
     "ConflictResolutionTypeDef",
     "CreateCommitOutputTypeDef",
     "CreatePullRequestInputRequestTypeDef",
+    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    "GetDifferencesInputGetDifferencesPaginateTypeDef",
+    "ListBranchesInputListBranchesPaginateTypeDef",
+    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
     "ListRepositoriesOutputTypeDef",
-    "PostCommentForComparedCommitInputRequestTypeDef",
-    "PostCommentForPullRequestInputRequestTypeDef",
     "MergeHunkTypeDef",
     "PullRequestMergedStateChangedEventMetadataTypeDef",
     "PullRequestTargetTypeDef",
     "PutFileEntryTypeDef",
     "PutRepositoryTriggersInputRequestTypeDef",
     "TestRepositoryTriggersInputRequestTypeDef",
     "ReactionForCommentTypeDef",
@@ -337,14 +336,25 @@
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryNames": Sequence[str],
     },
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
 BatchDescribeMergeConflictsErrorTypeDef = TypedDict(
     "BatchDescribeMergeConflictsErrorTypeDef",
     {
         "filePath": str,
         "exceptionName": str,
         "message": str,
     },
@@ -470,16 +480,16 @@
         "clientRequestToken": str,
         "callerReactions": List[str],
         "reactionCounts": Dict[str, int],
     },
     total=False,
 )
 
-LocationOutputTypeDef = TypedDict(
-    "LocationOutputTypeDef",
+LocationTypeDef = TypedDict(
+    "LocationTypeDef",
     {
         "filePath": str,
         "filePosition": int,
         "relativeFileVersion": RelativeFileVersionEnumType,
     },
     total=False,
 )
@@ -662,38 +672,21 @@
 )
 
 class CreateRepositoryInputRequestTypeDef(
     _RequiredCreateRepositoryInputRequestTypeDef, _OptionalCreateRepositoryInputRequestTypeDef
 ):
     pass
 
-CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
-    "CreateUnreferencedMergeCommitOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 
-DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "DeleteApprovalRuleTemplateOutputTypeDef",
-    {
-        "approvalRuleTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBranchInputRequestTypeDef = TypedDict(
     "DeleteBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
 )
@@ -726,56 +719,29 @@
 )
 
 class DeleteFileInputRequestTypeDef(
     _RequiredDeleteFileInputRequestTypeDef, _OptionalDeleteFileInputRequestTypeDef
 ):
     pass
 
-DeleteFileOutputTypeDef = TypedDict(
-    "DeleteFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "filePath": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePullRequestApprovalRuleInputRequestTypeDef = TypedDict(
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
     {
         "pullRequestId": str,
         "approvalRuleName": str,
     },
 )
 
-DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
-    "DeletePullRequestApprovalRuleOutputTypeDef",
-    {
-        "approvalRuleId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRepositoryInputRequestTypeDef = TypedDict(
     "DeleteRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
-DeleteRepositoryOutputTypeDef = TypedDict(
-    "DeleteRepositoryOutputTypeDef",
-    {
-        "repositoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -795,36 +761,24 @@
 
 class DescribeMergeConflictsInputRequestTypeDef(
     _RequiredDescribeMergeConflictsInputRequestTypeDef,
     _OptionalDescribeMergeConflictsInputRequestTypeDef,
 ):
     pass
 
-_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "pullRequestEventType": PullRequestEventTypeType,
-        "actorArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
-    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribePullRequestEventsInputRequestTypeDef = TypedDict(
     "_RequiredDescribePullRequestEventsInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalDescribePullRequestEventsInputRequestTypeDef = TypedDict(
@@ -848,21 +802,14 @@
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluatePullRequestApprovalRulesInputRequestTypeDef = TypedDict(
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -910,22 +857,14 @@
     "GetBlobInputRequestTypeDef",
     {
         "repositoryName": str,
         "blobId": str,
     },
 )
 
-GetBlobOutputTypeDef = TypedDict(
-    "GetBlobOutputTypeDef",
-    {
-        "content": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBranchInputRequestTypeDef = TypedDict(
     "GetBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
     total=False,
@@ -955,36 +894,14 @@
 )
 
 class GetCommentReactionsInputRequestTypeDef(
     _RequiredGetCommentReactionsInputRequestTypeDef, _OptionalGetCommentReactionsInputRequestTypeDef
 ):
     pass
 
-_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitId": str,
-    },
-)
-_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "beforeCommitId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
-    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-):
-    pass
-
 _RequiredGetCommentsForComparedCommitInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForComparedCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitId": str,
     },
 )
@@ -1000,37 +917,14 @@
 
 class GetCommentsForComparedCommitInputRequestTypeDef(
     _RequiredGetCommentsForComparedCommitInputRequestTypeDef,
     _OptionalGetCommentsForComparedCommitInputRequestTypeDef,
 ):
     pass
 
-_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "beforeCommitId": str,
-        "afterCommitId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
-    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-):
-    pass
-
 _RequiredGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForPullRequestInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
@@ -1055,38 +949,14 @@
     "GetCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "commitId": str,
     },
 )
 
-_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitSpecifier": str,
-    },
-)
-_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "beforeCommitSpecifier": str,
-        "beforePath": str,
-        "afterPath": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetDifferencesInputGetDifferencesPaginateTypeDef(
-    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
-    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetDifferencesInputRequestTypeDef = TypedDict(
     "_RequiredGetDifferencesInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitSpecifier": str,
     },
 )
@@ -1123,27 +993,14 @@
 )
 
 class GetFileInputRequestTypeDef(
     _RequiredGetFileInputRequestTypeDef, _OptionalGetFileInputRequestTypeDef
 ):
     pass
 
-GetFileOutputTypeDef = TypedDict(
-    "GetFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "filePath": str,
-        "fileMode": FileModeTypeEnumType,
-        "fileSize": int,
-        "fileContent": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetFolderInputRequestTypeDef = TypedDict(
     "_RequiredGetFolderInputRequestTypeDef",
     {
         "repositoryName": str,
         "folderPath": str,
     },
 )
@@ -1199,25 +1056,14 @@
 )
 
 class GetMergeCommitInputRequestTypeDef(
     _RequiredGetMergeCommitInputRequestTypeDef, _OptionalGetMergeCommitInputRequestTypeDef
 ):
     pass
 
-GetMergeCommitOutputTypeDef = TypedDict(
-    "GetMergeCommitOutputTypeDef",
-    {
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "mergedCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredGetMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -1257,25 +1103,14 @@
 )
 
 class GetMergeOptionsInputRequestTypeDef(
     _RequiredGetMergeOptionsInputRequestTypeDef, _OptionalGetMergeOptionsInputRequestTypeDef
 ):
     pass
 
-GetMergeOptionsOutputTypeDef = TypedDict(
-    "GetMergeOptionsOutputTypeDef",
-    {
-        "mergeOptions": List[MergeOptionTypeEnumType],
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPullRequestApprovalStatesInputRequestTypeDef = TypedDict(
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -1291,23 +1126,14 @@
     "GetPullRequestOverrideStateInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
 
-GetPullRequestOverrideStateOutputTypeDef = TypedDict(
-    "GetPullRequestOverrideStateOutputTypeDef",
-    {
-        "overridden": bool,
-        "overrider": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRepositoryInputRequestTypeDef = TypedDict(
     "GetRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
@@ -1345,23 +1171,14 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
-    "ListApprovalRuleTemplatesOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
     "_RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
@@ -1375,43 +1192,14 @@
 
 class ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef(
     _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
     _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
 ):
     pass
 
-ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListBranchesInputListBranchesPaginateTypeDef(
-    _RequiredListBranchesInputListBranchesPaginateTypeDef,
-    _OptionalListBranchesInputListBranchesPaginateTypeDef,
-):
-    pass
-
 _RequiredListBranchesInputRequestTypeDef = TypedDict(
     "_RequiredListBranchesInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListBranchesInputRequestTypeDef = TypedDict(
@@ -1423,45 +1211,14 @@
 )
 
 class ListBranchesInputRequestTypeDef(
     _RequiredListBranchesInputRequestTypeDef, _OptionalListBranchesInputRequestTypeDef
 ):
     pass
 
-ListBranchesOutputTypeDef = TypedDict(
-    "ListBranchesOutputTypeDef",
-    {
-        "branches": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "authorArn": str,
-        "pullRequestStatus": PullRequestStatusEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPullRequestsInputListPullRequestsPaginateTypeDef(
-    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
-    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPullRequestsInputRequestTypeDef = TypedDict(
     "_RequiredListPullRequestsInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListPullRequestsInputRequestTypeDef = TypedDict(
@@ -1476,23 +1233,14 @@
 )
 
 class ListPullRequestsInputRequestTypeDef(
     _RequiredListPullRequestsInputRequestTypeDef, _OptionalListPullRequestsInputRequestTypeDef
 ):
     pass
 
-ListPullRequestsOutputTypeDef = TypedDict(
-    "ListPullRequestsOutputTypeDef",
-    {
-        "pullRequestIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
@@ -1506,33 +1254,14 @@
 
 class ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef(
     _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
     _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
 ):
     pass
 
-ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    {
-        "repositoryNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
-    {
-        "sortBy": SortByEnumType,
-        "order": OrderEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRepositoriesInputRequestTypeDef = TypedDict(
     "ListRepositoriesInputRequestTypeDef",
     {
         "nextToken": str,
         "sortBy": SortByEnumType,
         "order": OrderEnumType,
     },
@@ -1563,33 +1292,14 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LocationTypeDef = TypedDict(
-    "LocationTypeDef",
-    {
-        "filePath": str,
-        "filePosition": int,
-        "relativeFileVersion": RelativeFileVersionEnumType,
-    },
-    total=False,
-)
-
 _RequiredMergeBranchesByFastForwardInputRequestTypeDef = TypedDict(
     "_RequiredMergeBranchesByFastForwardInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
     },
@@ -1604,41 +1314,14 @@
 
 class MergeBranchesByFastForwardInputRequestTypeDef(
     _RequiredMergeBranchesByFastForwardInputRequestTypeDef,
     _OptionalMergeBranchesByFastForwardInputRequestTypeDef,
 ):
     pass
 
-MergeBranchesByFastForwardOutputTypeDef = TypedDict(
-    "MergeBranchesByFastForwardOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MergeBranchesBySquashOutputTypeDef = TypedDict(
-    "MergeBranchesBySquashOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MergeBranchesByThreeWayOutputTypeDef = TypedDict(
-    "MergeBranchesByThreeWayOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MergeHunkDetailTypeDef = TypedDict(
     "MergeHunkDetailTypeDef",
     {
         "startLine": int,
         "endLine": int,
         "hunkContent": str,
     },
@@ -1682,24 +1365,14 @@
     {
         "pullRequestId": str,
         "revisionId": str,
         "overrideStatus": OverrideStatusType,
     },
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
 _RequiredPostCommentReplyInputRequestTypeDef = TypedDict(
     "_RequiredPostCommentReplyInputRequestTypeDef",
     {
         "inReplyTo": str,
         "content": str,
     },
 )
@@ -1795,24 +1468,14 @@
 )
 
 class PutFileInputRequestTypeDef(
     _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
 ):
     pass
 
-PutFileOutputTypeDef = TypedDict(
-    "PutFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRepositoryTriggerTypeDef = TypedDict(
     "_RequiredRepositoryTriggerTypeDef",
     {
         "name": str,
         "destinationArn": str,
         "events": Sequence[RepositoryTriggerEventEnumType],
     },
@@ -1827,22 +1490,14 @@
 )
 
 class RepositoryTriggerTypeDef(
     _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
 ):
     pass
 
-PutRepositoryTriggersOutputTypeDef = TypedDict(
-    "PutRepositoryTriggersOutputTypeDef",
-    {
-        "configurationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReactionValueFormatsTypeDef = TypedDict(
     "ReactionValueFormatsTypeDef",
     {
         "emoji": str,
         "shortCode": str,
         "unicode": str,
     },
@@ -1854,25 +1509,14 @@
     {
         "trigger": str,
         "failureMessage": str,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -2017,117 +1661,319 @@
     "UpdateRepositoryNameInputRequestTypeDef",
     {
         "oldName": str,
         "newName": str,
     },
 )
 
+ApprovalRuleTypeDef = TypedDict(
+    "ApprovalRuleTypeDef",
+    {
+        "approvalRuleId": str,
+        "approvalRuleName": str,
+        "approvalRuleContent": str,
+        "ruleContentSha256": str,
+        "lastModifiedDate": datetime,
+        "creationDate": datetime,
+        "lastModifiedUser": str,
+        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
+    },
+    total=False,
+)
+
+BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
+    {
+        "associatedRepositoryNames": List[str],
+        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApprovalRuleTemplateOutputTypeDef = TypedDict(
     "CreateApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
+    "CreateUnreferencedMergeCommitOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "DeleteApprovalRuleTemplateOutputTypeDef",
+    {
+        "approvalRuleTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFileOutputTypeDef = TypedDict(
+    "DeleteFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "filePath": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
+    "DeletePullRequestApprovalRuleOutputTypeDef",
+    {
+        "approvalRuleId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRepositoryOutputTypeDef = TypedDict(
+    "DeleteRepositoryOutputTypeDef",
+    {
+        "repositoryId": str,
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
 
 GetApprovalRuleTemplateOutputTypeDef = TypedDict(
     "GetApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateContentOutputTypeDef",
+GetBlobOutputTypeDef = TypedDict(
+    "GetBlobOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "content": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
+GetFileOutputTypeDef = TypedDict(
+    "GetFileOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "commitId": str,
+        "blobId": str,
+        "filePath": str,
+        "fileMode": FileModeTypeEnumType,
+        "fileSize": int,
+        "fileContent": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateNameOutputTypeDef",
+GetMergeCommitOutputTypeDef = TypedDict(
+    "GetMergeCommitOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "mergedCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ApprovalRuleTypeDef = TypedDict(
-    "ApprovalRuleTypeDef",
+GetMergeOptionsOutputTypeDef = TypedDict(
+    "GetMergeOptionsOutputTypeDef",
     {
-        "approvalRuleId": str,
-        "approvalRuleName": str,
-        "approvalRuleContent": str,
-        "ruleContentSha256": str,
-        "lastModifiedDate": datetime,
-        "creationDate": datetime,
-        "lastModifiedUser": str,
-        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
+        "mergeOptions": List[MergeOptionTypeEnumType],
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetPullRequestApprovalStatesOutputTypeDef = TypedDict(
     "GetPullRequestApprovalStatesOutputTypeDef",
     {
         "approvals": List[ApprovalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
+GetPullRequestOverrideStateOutputTypeDef = TypedDict(
+    "GetPullRequestOverrideStateOutputTypeDef",
     {
-        "associatedRepositoryNames": List[str],
-        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "overridden": bool,
+        "overrider": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
+    "ListApprovalRuleTemplatesOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBranchesOutputTypeDef = TypedDict(
+    "ListBranchesOutputTypeDef",
+    {
+        "branches": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPullRequestsOutputTypeDef = TypedDict(
+    "ListPullRequestsOutputTypeDef",
+    {
+        "pullRequestIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    {
+        "repositoryNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesByFastForwardOutputTypeDef = TypedDict(
+    "MergeBranchesByFastForwardOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesBySquashOutputTypeDef = TypedDict(
+    "MergeBranchesBySquashOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesByThreeWayOutputTypeDef = TypedDict(
+    "MergeBranchesByThreeWayOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutFileOutputTypeDef = TypedDict(
+    "PutFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRepositoryTriggersOutputTypeDef = TypedDict(
+    "PutRepositoryTriggersOutputTypeDef",
+    {
+        "configurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateContentOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateNameOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef = TypedDict(
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     {
         "disassociatedRepositoryNames": List[str],
         "errors": List[BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetRepositoriesOutputTypeDef = TypedDict(
     "BatchGetRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryMetadataTypeDef],
         "repositoriesNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryOutputTypeDef = TypedDict(
     "CreateRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRepositoryOutputTypeDef = TypedDict(
     "GetRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DifferenceTypeDef = TypedDict(
     "DifferenceTypeDef",
     {
         "beforeBlob": BlobMetadataTypeDef,
@@ -2137,113 +1983,162 @@
     total=False,
 )
 
 DeleteBranchOutputTypeDef = TypedDict(
     "DeleteBranchOutputTypeDef",
     {
         "deletedBranch": BranchInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBranchOutputTypeDef = TypedDict(
     "GetBranchOutputTypeDef",
     {
         "branch": BranchInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCommentContentOutputTypeDef = TypedDict(
     "DeleteCommentContentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommentOutputTypeDef = TypedDict(
     "GetCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PostCommentReplyOutputTypeDef = TypedDict(
     "PostCommentReplyOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCommentOutputTypeDef = TypedDict(
     "UpdateCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommentsForComparedCommitTypeDef = TypedDict(
     "CommentsForComparedCommitTypeDef",
     {
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationOutputTypeDef,
+        "location": LocationTypeDef,
         "comments": List[CommentTypeDef],
     },
     total=False,
 )
 
 CommentsForPullRequestTypeDef = TypedDict(
     "CommentsForPullRequestTypeDef",
     {
         "pullRequestId": str,
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationOutputTypeDef,
+        "location": LocationTypeDef,
         "comments": List[CommentTypeDef],
     },
     total=False,
 )
 
+_RequiredPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
+    "_RequiredPostCommentForComparedCommitInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "afterCommitId": str,
+        "content": str,
+    },
+)
+_OptionalPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
+    "_OptionalPostCommentForComparedCommitInputRequestTypeDef",
+    {
+        "beforeCommitId": str,
+        "location": LocationTypeDef,
+        "clientRequestToken": str,
+    },
+    total=False,
+)
+
+class PostCommentForComparedCommitInputRequestTypeDef(
+    _RequiredPostCommentForComparedCommitInputRequestTypeDef,
+    _OptionalPostCommentForComparedCommitInputRequestTypeDef,
+):
+    pass
+
 PostCommentForComparedCommitOutputTypeDef = TypedDict(
     "PostCommentForComparedCommitOutputTypeDef",
     {
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationOutputTypeDef,
+        "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
+    "_RequiredPostCommentForPullRequestInputRequestTypeDef",
+    {
+        "pullRequestId": str,
+        "repositoryName": str,
+        "beforeCommitId": str,
+        "afterCommitId": str,
+        "content": str,
+    },
+)
+_OptionalPostCommentForPullRequestInputRequestTypeDef = TypedDict(
+    "_OptionalPostCommentForPullRequestInputRequestTypeDef",
+    {
+        "location": LocationTypeDef,
+        "clientRequestToken": str,
     },
+    total=False,
 )
 
+class PostCommentForPullRequestInputRequestTypeDef(
+    _RequiredPostCommentForPullRequestInputRequestTypeDef,
+    _OptionalPostCommentForPullRequestInputRequestTypeDef,
+):
+    pass
+
 PostCommentForPullRequestOutputTypeDef = TypedDict(
     "PostCommentForPullRequestOutputTypeDef",
     {
         "repositoryName": str,
         "pullRequestId": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationOutputTypeDef,
+        "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommitTypeDef = TypedDict(
     "CommitTypeDef",
     {
         "commitId": str,
@@ -2288,15 +2183,15 @@
     "CreateCommitOutputTypeDef",
     {
         "commitId": str,
         "treeId": str,
         "filesAdded": List[FileMetadataTypeDef],
         "filesUpdated": List[FileMetadataTypeDef],
         "filesDeleted": List[FileMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePullRequestInputRequestTypeDef = TypedDict(
     "_RequiredCreatePullRequestInputRequestTypeDef",
     {
         "title": str,
@@ -2313,103 +2208,197 @@
 )
 
 class CreatePullRequestInputRequestTypeDef(
     _RequiredCreatePullRequestInputRequestTypeDef, _OptionalCreatePullRequestInputRequestTypeDef
 ):
     pass
 
-EvaluatePullRequestApprovalRulesOutputTypeDef = TypedDict(
-    "EvaluatePullRequestApprovalRulesOutputTypeDef",
+_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
     {
-        "evaluation": EvaluationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "pullRequestId": str,
+    },
+)
+_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    {
+        "pullRequestEventType": PullRequestEventTypeType,
+        "actorArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetFolderOutputTypeDef = TypedDict(
-    "GetFolderOutputTypeDef",
+class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
+    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
     {
-        "commitId": str,
-        "folderPath": str,
-        "treeId": str,
-        "subFolders": List[FolderTypeDef],
-        "files": List[FileTypeDef],
-        "symbolicLinks": List[SymbolicLinkTypeDef],
-        "subModules": List[SubModuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "repositoryName": str,
+        "afterCommitId": str,
+    },
+)
+_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    {
+        "beforeCommitId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetRepositoryTriggersOutputTypeDef = TypedDict(
-    "GetRepositoryTriggersOutputTypeDef",
+class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
+    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+):
+    pass
+
+_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
     {
-        "configurationId": str,
-        "triggers": List[RepositoryTriggerOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "pullRequestId": str,
+    },
+)
+_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "beforeCommitId": str,
+        "afterCommitId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListRepositoriesOutputTypeDef = TypedDict(
-    "ListRepositoriesOutputTypeDef",
+class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
+    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+):
+    pass
+
+_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
     {
-        "repositories": List[RepositoryNameIdPairTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "repositoryName": str,
+        "afterCommitSpecifier": str,
+    },
+)
+_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
+    {
+        "beforeCommitSpecifier": str,
+        "beforePath": str,
+        "afterPath": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
-    "_RequiredPostCommentForComparedCommitInputRequestTypeDef",
+class GetDifferencesInputGetDifferencesPaginateTypeDef(
+    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
+    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
+):
+    pass
+
+_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
     {
         "repositoryName": str,
-        "afterCommitId": str,
-        "content": str,
     },
 )
-_OptionalPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
-    "_OptionalPostCommentForComparedCommitInputRequestTypeDef",
+_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
     {
-        "beforeCommitId": str,
-        "location": LocationTypeDef,
-        "clientRequestToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class PostCommentForComparedCommitInputRequestTypeDef(
-    _RequiredPostCommentForComparedCommitInputRequestTypeDef,
-    _OptionalPostCommentForComparedCommitInputRequestTypeDef,
+class ListBranchesInputListBranchesPaginateTypeDef(
+    _RequiredListBranchesInputListBranchesPaginateTypeDef,
+    _OptionalListBranchesInputListBranchesPaginateTypeDef,
 ):
     pass
 
-_RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
-    "_RequiredPostCommentForPullRequestInputRequestTypeDef",
+_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
     {
-        "pullRequestId": str,
         "repositoryName": str,
-        "beforeCommitId": str,
-        "afterCommitId": str,
-        "content": str,
     },
 )
-_OptionalPostCommentForPullRequestInputRequestTypeDef = TypedDict(
-    "_OptionalPostCommentForPullRequestInputRequestTypeDef",
+_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
     {
-        "location": LocationTypeDef,
-        "clientRequestToken": str,
+        "authorArn": str,
+        "pullRequestStatus": PullRequestStatusEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class PostCommentForPullRequestInputRequestTypeDef(
-    _RequiredPostCommentForPullRequestInputRequestTypeDef,
-    _OptionalPostCommentForPullRequestInputRequestTypeDef,
+class ListPullRequestsInputListPullRequestsPaginateTypeDef(
+    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
+    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
 ):
     pass
 
+ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
+    {
+        "sortBy": SortByEnumType,
+        "order": OrderEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+EvaluatePullRequestApprovalRulesOutputTypeDef = TypedDict(
+    "EvaluatePullRequestApprovalRulesOutputTypeDef",
+    {
+        "evaluation": EvaluationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFolderOutputTypeDef = TypedDict(
+    "GetFolderOutputTypeDef",
+    {
+        "commitId": str,
+        "folderPath": str,
+        "treeId": str,
+        "subFolders": List[FolderTypeDef],
+        "files": List[FileTypeDef],
+        "symbolicLinks": List[SymbolicLinkTypeDef],
+        "subModules": List[SubModuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRepositoryTriggersOutputTypeDef = TypedDict(
+    "GetRepositoryTriggersOutputTypeDef",
+    {
+        "configurationId": str,
+        "triggers": List[RepositoryTriggerOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRepositoriesOutputTypeDef = TypedDict(
+    "ListRepositoriesOutputTypeDef",
+    {
+        "repositories": List[RepositoryNameIdPairTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 MergeHunkTypeDef = TypedDict(
     "MergeHunkTypeDef",
     {
         "isConflict": bool,
         "source": MergeHunkDetailTypeDef,
         "destination": MergeHunkDetailTypeDef,
         "base": MergeHunkDetailTypeDef,
@@ -2487,88 +2476,88 @@
 )
 
 TestRepositoryTriggersOutputTypeDef = TypedDict(
     "TestRepositoryTriggersOutputTypeDef",
     {
         "successfulExecutions": List[str],
         "failedExecutions": List[RepositoryTriggerExecutionFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePullRequestApprovalRuleOutputTypeDef = TypedDict(
     "CreatePullRequestApprovalRuleOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestApprovalRuleContentOutputTypeDef = TypedDict(
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDifferencesOutputTypeDef = TypedDict(
     "GetDifferencesOutputTypeDef",
     {
         "differences": List[DifferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommentsForComparedCommitOutputTypeDef = TypedDict(
     "GetCommentsForComparedCommitOutputTypeDef",
     {
         "commentsForComparedCommitData": List[CommentsForComparedCommitTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommentsForPullRequestOutputTypeDef = TypedDict(
     "GetCommentsForPullRequestOutputTypeDef",
     {
         "commentsForPullRequestData": List[CommentsForPullRequestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetCommitsOutputTypeDef = TypedDict(
     "BatchGetCommitsOutputTypeDef",
     {
         "commits": List[CommitTypeDef],
         "errors": List[BatchGetCommitsErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommitOutputTypeDef = TypedDict(
     "GetCommitOutputTypeDef",
     {
         "commit": CommitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMergeConflictsOutputTypeDef = TypedDict(
     "GetMergeConflictsOutputTypeDef",
     {
         "mergeable": bool,
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
         "conflictMetadataList": List[ConflictMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUnreferencedMergeCommitInputRequestTypeDef = TypedDict(
     "_RequiredCreateUnreferencedMergeCommitInputRequestTypeDef",
     {
         "repositoryName": str,
@@ -2725,15 +2714,15 @@
     {
         "conflictMetadata": ConflictMetadataTypeDef,
         "mergeHunks": List[MergeHunkTypeDef],
         "nextToken": str,
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PullRequestEventTypeDef = TypedDict(
     "PullRequestEventTypeDef",
     {
         "pullRequestId": str,
@@ -2801,96 +2790,96 @@
     pass
 
 GetCommentReactionsOutputTypeDef = TypedDict(
     "GetCommentReactionsOutputTypeDef",
     {
         "reactionsForComment": List[ReactionForCommentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDescribeMergeConflictsOutputTypeDef = TypedDict(
     "BatchDescribeMergeConflictsOutputTypeDef",
     {
         "conflicts": List[ConflictTypeDef],
         "nextToken": str,
         "errors": List[BatchDescribeMergeConflictsErrorTypeDef],
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePullRequestEventsOutputTypeDef = TypedDict(
     "DescribePullRequestEventsOutputTypeDef",
     {
         "pullRequestEvents": List[PullRequestEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePullRequestOutputTypeDef = TypedDict(
     "CreatePullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPullRequestOutputTypeDef = TypedDict(
     "GetPullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestByFastForwardOutputTypeDef = TypedDict(
     "MergePullRequestByFastForwardOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestBySquashOutputTypeDef = TypedDict(
     "MergePullRequestBySquashOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestByThreeWayOutputTypeDef = TypedDict(
     "MergePullRequestByThreeWayOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestDescriptionOutputTypeDef = TypedDict(
     "UpdatePullRequestDescriptionOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestStatusOutputTypeDef = TypedDict(
     "UpdatePullRequestStatusOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestTitleOutputTypeDef = TypedDict(
     "UpdatePullRequestTitleOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/PKG-INFO` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecommit
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeCommit 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeCommit 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecommit)](https://pepy.tech/project/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,26 +368,27 @@
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
     ApprovalStateChangedEventMetadataTypeDef,
     ApprovalTypeDef,
     AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeMergeConflictsErrorTypeDef,
     BatchDescribeMergeConflictsInputRequestTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
-    LocationOutputTypeDef,
+    LocationTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
@@ -395,152 +396,150 @@
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
-    CreateUnreferencedMergeCommitOutputTypeDef,
     DeleteApprovalRuleTemplateInputRequestTypeDef,
-    DeleteApprovalRuleTemplateOutputTypeDef,
     DeleteBranchInputRequestTypeDef,
     DeleteCommentContentInputRequestTypeDef,
     DeleteFileInputRequestTypeDef,
-    DeleteFileOutputTypeDef,
     DeletePullRequestApprovalRuleInputRequestTypeDef,
-    DeletePullRequestApprovalRuleOutputTypeDef,
     DeleteRepositoryInputRequestTypeDef,
-    DeleteRepositoryOutputTypeDef,
     DescribeMergeConflictsInputRequestTypeDef,
-    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribePullRequestEventsInputRequestTypeDef,
     DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluatePullRequestApprovalRulesInputRequestTypeDef,
     EvaluationTypeDef,
     FileTypeDef,
     FolderTypeDef,
     GetApprovalRuleTemplateInputRequestTypeDef,
     GetBlobInputRequestTypeDef,
-    GetBlobOutputTypeDef,
     GetBranchInputRequestTypeDef,
     GetCommentInputRequestTypeDef,
     GetCommentReactionsInputRequestTypeDef,
-    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForComparedCommitInputRequestTypeDef,
-    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetCommentsForPullRequestInputRequestTypeDef,
     GetCommitInputRequestTypeDef,
-    GetDifferencesInputGetDifferencesPaginateTypeDef,
     GetDifferencesInputRequestTypeDef,
     GetFileInputRequestTypeDef,
-    GetFileOutputTypeDef,
     GetFolderInputRequestTypeDef,
     SubModuleTypeDef,
     SymbolicLinkTypeDef,
     GetMergeCommitInputRequestTypeDef,
-    GetMergeCommitOutputTypeDef,
     GetMergeConflictsInputRequestTypeDef,
     GetMergeOptionsInputRequestTypeDef,
-    GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
-    GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
     RepositoryTriggerOutputTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
-    ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
-    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
-    ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
-    ListBranchesOutputTypeDef,
-    ListPullRequestsInputListPullRequestsPaginateTypeDef,
     ListPullRequestsInputRequestTypeDef,
-    ListPullRequestsOutputTypeDef,
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
-    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    LocationTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
-    MergeBranchesByFastForwardOutputTypeDef,
-    MergeBranchesBySquashOutputTypeDef,
-    MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
     OverridePullRequestApprovalRulesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
     PutFileInputRequestTypeDef,
-    PutFileOutputTypeDef,
     RepositoryTriggerTypeDef,
-    PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
     UpdatePullRequestApprovalRuleContentInputRequestTypeDef,
     UpdatePullRequestApprovalStateInputRequestTypeDef,
     UpdatePullRequestDescriptionInputRequestTypeDef,
     UpdatePullRequestStatusInputRequestTypeDef,
     UpdatePullRequestTitleInputRequestTypeDef,
     UpdateRepositoryDescriptionInputRequestTypeDef,
     UpdateRepositoryNameInputRequestTypeDef,
+    ApprovalRuleTypeDef,
+    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
+    CreateUnreferencedMergeCommitOutputTypeDef,
+    DeleteApprovalRuleTemplateOutputTypeDef,
+    DeleteFileOutputTypeDef,
+    DeletePullRequestApprovalRuleOutputTypeDef,
+    DeleteRepositoryOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApprovalRuleTemplateOutputTypeDef,
+    GetBlobOutputTypeDef,
+    GetFileOutputTypeDef,
+    GetMergeCommitOutputTypeDef,
+    GetMergeOptionsOutputTypeDef,
+    GetPullRequestApprovalStatesOutputTypeDef,
+    GetPullRequestOverrideStateOutputTypeDef,
+    ListApprovalRuleTemplatesOutputTypeDef,
+    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
+    ListBranchesOutputTypeDef,
+    ListPullRequestsOutputTypeDef,
+    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    MergeBranchesByFastForwardOutputTypeDef,
+    MergeBranchesBySquashOutputTypeDef,
+    MergeBranchesByThreeWayOutputTypeDef,
+    PutFileOutputTypeDef,
+    PutRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
-    ApprovalRuleTypeDef,
-    GetPullRequestApprovalStatesOutputTypeDef,
-    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
+    PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
+    PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
     ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
+    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    GetDifferencesInputGetDifferencesPaginateTypeDef,
+    ListBranchesInputListBranchesPaginateTypeDef,
+    ListPullRequestsInputListPullRequestsPaginateTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
     ListRepositoriesOutputTypeDef,
-    PostCommentForComparedCommitInputRequestTypeDef,
-    PostCommentForPullRequestInputRequestTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
     PutRepositoryTriggersInputRequestTypeDef,
     TestRepositoryTriggersInputRequestTypeDef,
     ReactionForCommentTypeDef,
```

### Comparing `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/SOURCES.txt` & `mypy-boto3-codecommit-1.28.15/mypy_boto3_codecommit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.12/setup.py` & `mypy-boto3-codecommit-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codecommit",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_codecommit"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeCommit 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CodeCommit 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

