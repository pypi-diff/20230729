# Comparing `tmp/mypy-boto3-codeguru-reviewer-1.28.12.tar.gz` & `tmp/mypy-boto3-codeguru-reviewer-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguru-reviewer-1.28.12.tar", last modified: Thu Jul 27 05:34:28 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguru-reviewer-1.28.15.tar", last modified: Fri Jul 28 20:42:28 2023, max compression
```

## Comparing `mypy-boto3-codeguru-reviewer-1.28.12.tar` & `mypy-boto3-codeguru-reviewer-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:28.168553 mypy-boto3-codeguru-reviewer-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-07-27 05:34:28.164553 mypy-boto3-codeguru-reviewer-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:28.160553 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:28.164553 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-07-27 05:34:27.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:28.168553 mypy-boto3-codeguru-reviewer-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.620826 mypy-boto3-codeguru-reviewer-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-07-28 20:42:28.616825 mypy-boto3-codeguru-reviewer-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.616825 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-07-28 20:21:34.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.616825 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:28.620826 mypy-boto3-codeguru-reviewer-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 20:21:33.000000 mypy-boto3-codeguru-reviewer-1.28.15/setup.py
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/LICENSE` & `mypy-boto3-codeguru-reviewer-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/PKG-INFO` & `mypy-boto3-codeguru-reviewer-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-reviewer
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeGuruReviewer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeGuruReviewer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-reviewer)](https://pepy.tech/project/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,71 +364,61 @@
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
-    BranchDiffSourceCodeTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
-    CodeArtifactsOutputTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
-    CommitDiffSourceCodeTypeOutputTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeReviewRequestRequestTypeDef,
     DescribeRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackTypeDef,
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
-    EventInfoOutputTypeDef,
     EventInfoTypeDef,
-    KMSKeyDetailsOutputTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
-    RepositoryHeadSourceCodeTypeOutputTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    S3RepositoryDetailsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
-    RequestMetadataOutputTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
+    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
-    S3BucketRepositoryOutputTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
     AssociateRepositoryResponseTypeDef,
     DescribeRepositoryAssociationResponseTypeDef,
     DisassociateRepositoryResponseTypeDef,
-    SourceCodeTypeOutputTypeDef,
     SourceCodeTypeTypeDef,
     CodeReviewSummaryTypeDef,
     CodeReviewTypeDef,
     RepositoryAnalysisTypeDef,
     ListCodeReviewsResponseTypeDef,
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/README.md` & `mypy-boto3-codeguru-reviewer-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-reviewer)](https://pepy.tech/project/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,71 +332,61 @@
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
-    BranchDiffSourceCodeTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
-    CodeArtifactsOutputTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
-    CommitDiffSourceCodeTypeOutputTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeReviewRequestRequestTypeDef,
     DescribeRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackTypeDef,
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
-    EventInfoOutputTypeDef,
     EventInfoTypeDef,
-    KMSKeyDetailsOutputTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
-    RepositoryHeadSourceCodeTypeOutputTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    S3RepositoryDetailsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
-    RequestMetadataOutputTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
+    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
-    S3BucketRepositoryOutputTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
     AssociateRepositoryResponseTypeDef,
     DescribeRepositoryAssociationResponseTypeDef,
     DisassociateRepositoryResponseTypeDef,
-    SourceCodeTypeOutputTypeDef,
     SourceCodeTypeTypeDef,
     CodeReviewSummaryTypeDef,
     CodeReviewTypeDef,
     RepositoryAnalysisTypeDef,
     ListCodeReviewsResponseTypeDef,
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__init__.py` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__init__.pyi` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__main__.py` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruReviewer 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodeGuruReviewer 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer\nOther"
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

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/client.py` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/client.pyi` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/literals.py` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/literals.pyi` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/paginator.py` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,13 +48,13 @@
     def paginate(
         self,
         *,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[RepositoryAssociationStateType] = ...,
         Names: Sequence[str] = ...,
         Owners: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRepositoryAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/paginators/#listrepositoryassociationspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/paginator.pyi` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,13 @@
     def paginate(
         self,
         *,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[RepositoryAssociationStateType] = ...,
         Names: Sequence[str] = ...,
         Owners: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRepositoryAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/paginators/#listrepositoryassociationspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/type_defs.py` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -30,74 +30,63 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "KMSKeyDetailsTypeDef",
-    "BranchDiffSourceCodeTypeOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "BranchDiffSourceCodeTypeTypeDef",
-    "CodeArtifactsOutputTypeDef",
     "CodeArtifactsTypeDef",
     "CodeCommitRepositoryTypeDef",
     "MetricsSummaryTypeDef",
     "MetricsTypeDef",
-    "CommitDiffSourceCodeTypeOutputTypeDef",
     "CommitDiffSourceCodeTypeTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCodeReviewRequestRequestTypeDef",
     "DescribeRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackTypeDef",
     "DescribeRepositoryAssociationRequestRequestTypeDef",
     "DisassociateRepositoryRequestRequestTypeDef",
-    "EventInfoOutputTypeDef",
     "EventInfoTypeDef",
-    "KMSKeyDetailsOutputTypeDef",
     "ListCodeReviewsRequestRequestTypeDef",
     "ListRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackSummaryTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRepositoryAssociationsRequestRequestTypeDef",
     "RepositoryAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutRecommendationFeedbackRequestRequestTypeDef",
     "RuleMetadataTypeDef",
     "RepositoryHeadSourceCodeTypeTypeDef",
-    "RepositoryHeadSourceCodeTypeOutputTypeDef",
     "S3RepositoryTypeDef",
     "ThirdPartySourceRepositoryTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "S3RepositoryDetailsOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "S3RepositoryDetailsTypeDef",
     "DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef",
     "DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     "DescribeRecommendationFeedbackResponseTypeDef",
-    "RequestMetadataOutputTypeDef",
     "RequestMetadataTypeDef",
     "ListRecommendationFeedbackResponseTypeDef",
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     "ListRepositoryAssociationsResponseTypeDef",
     "RecommendationSummaryTypeDef",
     "RepositoryTypeDef",
     "RepositoryAssociationTypeDef",
-    "S3BucketRepositoryOutputTypeDef",
     "S3BucketRepositoryTypeDef",
     "ListRecommendationsResponseTypeDef",
     "AssociateRepositoryRequestRequestTypeDef",
     "AssociateRepositoryResponseTypeDef",
     "DescribeRepositoryAssociationResponseTypeDef",
     "DisassociateRepositoryResponseTypeDef",
-    "SourceCodeTypeOutputTypeDef",
     "SourceCodeTypeTypeDef",
     "CodeReviewSummaryTypeDef",
     "CodeReviewTypeDef",
     "RepositoryAnalysisTypeDef",
     "ListCodeReviewsResponseTypeDef",
     "CreateCodeReviewResponseTypeDef",
     "DescribeCodeReviewResponseTypeDef",
@@ -110,70 +99,50 @@
     {
         "KMSKeyId": str,
         "EncryptionOption": EncryptionOptionType,
     },
     total=False,
 )
 
-BranchDiffSourceCodeTypeOutputTypeDef = TypedDict(
-    "BranchDiffSourceCodeTypeOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "SourceBranchName": str,
-        "DestinationBranchName": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BranchDiffSourceCodeTypeTypeDef = TypedDict(
     "BranchDiffSourceCodeTypeTypeDef",
     {
         "SourceBranchName": str,
         "DestinationBranchName": str,
     },
 )
 
-_RequiredCodeArtifactsOutputTypeDef = TypedDict(
-    "_RequiredCodeArtifactsOutputTypeDef",
-    {
-        "SourceCodeArtifactsObjectKey": str,
-    },
-)
-_OptionalCodeArtifactsOutputTypeDef = TypedDict(
-    "_OptionalCodeArtifactsOutputTypeDef",
-    {
-        "BuildArtifactsObjectKey": str,
-    },
-    total=False,
-)
-
-
-class CodeArtifactsOutputTypeDef(
-    _RequiredCodeArtifactsOutputTypeDef, _OptionalCodeArtifactsOutputTypeDef
-):
-    pass
-
-
 _RequiredCodeArtifactsTypeDef = TypedDict(
     "_RequiredCodeArtifactsTypeDef",
     {
         "SourceCodeArtifactsObjectKey": str,
     },
 )
 _OptionalCodeArtifactsTypeDef = TypedDict(
     "_OptionalCodeArtifactsTypeDef",
     {
         "BuildArtifactsObjectKey": str,
     },
     total=False,
 )
 
-
 class CodeArtifactsTypeDef(_RequiredCodeArtifactsTypeDef, _OptionalCodeArtifactsTypeDef):
     pass
 
-
 CodeCommitRepositoryTypeDef = TypedDict(
     "CodeCommitRepositoryTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -193,24 +162,14 @@
         "MeteredLinesOfCodeCount": int,
         "SuppressedLinesOfCodeCount": int,
         "FindingsCount": int,
     },
     total=False,
 )
 
-CommitDiffSourceCodeTypeOutputTypeDef = TypedDict(
-    "CommitDiffSourceCodeTypeOutputTypeDef",
-    {
-        "SourceCommit": str,
-        "DestinationCommit": str,
-        "MergeBaseCommit": str,
-    },
-    total=False,
-)
-
 CommitDiffSourceCodeTypeTypeDef = TypedDict(
     "CommitDiffSourceCodeTypeTypeDef",
     {
         "SourceCommit": str,
         "DestinationCommit": str,
         "MergeBaseCommit": str,
     },
@@ -244,22 +203,20 @@
     "_OptionalDescribeRecommendationFeedbackRequestRequestTypeDef",
     {
         "UserId": str,
     },
     total=False,
 )
 
-
 class DescribeRecommendationFeedbackRequestRequestTypeDef(
     _RequiredDescribeRecommendationFeedbackRequestRequestTypeDef,
     _OptionalDescribeRecommendationFeedbackRequestRequestTypeDef,
 ):
     pass
 
-
 RecommendationFeedbackTypeDef = TypedDict(
     "RecommendationFeedbackTypeDef",
     {
         "CodeReviewArn": str,
         "RecommendationId": str,
         "Reactions": List[ReactionType],
         "UserId": str,
@@ -279,41 +236,23 @@
 DisassociateRepositoryRequestRequestTypeDef = TypedDict(
     "DisassociateRepositoryRequestRequestTypeDef",
     {
         "AssociationArn": str,
     },
 )
 
-EventInfoOutputTypeDef = TypedDict(
-    "EventInfoOutputTypeDef",
-    {
-        "Name": str,
-        "State": str,
-    },
-    total=False,
-)
-
 EventInfoTypeDef = TypedDict(
     "EventInfoTypeDef",
     {
         "Name": str,
         "State": str,
     },
     total=False,
 )
 
-KMSKeyDetailsOutputTypeDef = TypedDict(
-    "KMSKeyDetailsOutputTypeDef",
-    {
-        "KMSKeyId": str,
-        "EncryptionOption": EncryptionOptionType,
-    },
-    total=False,
-)
-
 _RequiredListCodeReviewsRequestRequestTypeDef = TypedDict(
     "_RequiredListCodeReviewsRequestRequestTypeDef",
     {
         "Type": TypeType,
     },
 )
 _OptionalListCodeReviewsRequestRequestTypeDef = TypedDict(
@@ -324,21 +263,19 @@
         "RepositoryNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListCodeReviewsRequestRequestTypeDef(
     _RequiredListCodeReviewsRequestRequestTypeDef, _OptionalListCodeReviewsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListRecommendationFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendationFeedbackRequestRequestTypeDef",
     {
         "CodeReviewArn": str,
     },
 )
 _OptionalListRecommendationFeedbackRequestRequestTypeDef = TypedDict(
@@ -348,22 +285,20 @@
         "MaxResults": int,
         "UserIds": Sequence[str],
         "RecommendationIds": Sequence[str],
     },
     total=False,
 )
 
-
 class ListRecommendationFeedbackRequestRequestTypeDef(
     _RequiredListRecommendationFeedbackRequestRequestTypeDef,
     _OptionalListRecommendationFeedbackRequestRequestTypeDef,
 ):
     pass
 
-
 RecommendationFeedbackSummaryTypeDef = TypedDict(
     "RecommendationFeedbackSummaryTypeDef",
     {
         "RecommendationId": str,
         "Reactions": List[ReactionType],
         "UserId": str,
     },
@@ -381,30 +316,26 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-
-ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ProviderTypes": Sequence[ProviderTypeType],
-        "States": Sequence[RepositoryAssociationStateType],
-        "Names": Sequence[str],
-        "Owners": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRepositoryAssociationsRequestRequestTypeDef = TypedDict(
     "ListRepositoryAssociationsRequestRequestTypeDef",
     {
@@ -436,32 +367,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 PutRecommendationFeedbackRequestRequestTypeDef = TypedDict(
     "PutRecommendationFeedbackRequestRequestTypeDef",
     {
         "CodeReviewArn": str,
         "RecommendationId": str,
         "Reactions": Sequence[ReactionType],
     },
@@ -482,21 +395,14 @@
 RepositoryHeadSourceCodeTypeTypeDef = TypedDict(
     "RepositoryHeadSourceCodeTypeTypeDef",
     {
         "BranchName": str,
     },
 )
 
-RepositoryHeadSourceCodeTypeOutputTypeDef = TypedDict(
-    "RepositoryHeadSourceCodeTypeOutputTypeDef",
-    {
-        "BranchName": str,
-    },
-)
-
 S3RepositoryTypeDef = TypedDict(
     "S3RepositoryTypeDef",
     {
         "Name": str,
         "BucketName": str,
     },
 )
@@ -506,25 +412,14 @@
     {
         "Name": str,
         "ConnectionArn": str,
         "Owner": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -533,21 +428,20 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-S3RepositoryDetailsOutputTypeDef = TypedDict(
-    "S3RepositoryDetailsOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "BucketName": str,
-        "CodeArtifacts": CodeArtifactsOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 S3RepositoryDetailsTypeDef = TypedDict(
     "S3RepositoryDetailsTypeDef",
     {
         "BucketName": str,
         "CodeArtifacts": CodeArtifactsTypeDef,
@@ -565,63 +459,48 @@
     "_OptionalDescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef(
     _RequiredDescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     _OptionalDescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef = TypedDict(
     "_RequiredDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     {
         "AssociationArn": str,
     },
 )
 _OptionalDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef = TypedDict(
     "_OptionalDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef(
     _RequiredDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     _OptionalDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
 ):
     pass
 
-
 DescribeRecommendationFeedbackResponseTypeDef = TypedDict(
     "DescribeRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedback": RecommendationFeedbackTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RequestMetadataOutputTypeDef = TypedDict(
-    "RequestMetadataOutputTypeDef",
-    {
-        "RequestId": str,
-        "Requester": str,
-        "EventInfo": EventInfoOutputTypeDef,
-        "VendorName": VendorNameType,
-    },
-    total=False,
-)
-
 RequestMetadataTypeDef = TypedDict(
     "RequestMetadataTypeDef",
     {
         "RequestId": str,
         "Requester": str,
         "EventInfo": EventInfoTypeDef,
         "VendorName": VendorNameType,
@@ -630,24 +509,36 @@
 )
 
 ListRecommendationFeedbackResponseTypeDef = TypedDict(
     "ListRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedbackSummaries": List[RecommendationFeedbackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+    {
+        "ProviderTypes": Sequence[ProviderTypeType],
+        "States": Sequence[RepositoryAssociationStateType],
+        "Names": Sequence[str],
+        "Owners": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListRepositoryAssociationsResponseTypeDef = TypedDict(
     "ListRepositoryAssociationsResponseTypeDef",
     {
         "RepositoryAssociationSummaries": List[RepositoryAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "FilePath": str,
@@ -682,68 +573,45 @@
         "Name": str,
         "Owner": str,
         "ProviderType": ProviderTypeType,
         "State": RepositoryAssociationStateType,
         "StateReason": str,
         "LastUpdatedTimeStamp": datetime,
         "CreatedTimeStamp": datetime,
-        "KMSKeyDetails": KMSKeyDetailsOutputTypeDef,
-        "S3RepositoryDetails": S3RepositoryDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredS3BucketRepositoryOutputTypeDef = TypedDict(
-    "_RequiredS3BucketRepositoryOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalS3BucketRepositoryOutputTypeDef = TypedDict(
-    "_OptionalS3BucketRepositoryOutputTypeDef",
-    {
-        "Details": S3RepositoryDetailsOutputTypeDef,
+        "KMSKeyDetails": KMSKeyDetailsTypeDef,
+        "S3RepositoryDetails": S3RepositoryDetailsTypeDef,
     },
     total=False,
 )
 
-
-class S3BucketRepositoryOutputTypeDef(
-    _RequiredS3BucketRepositoryOutputTypeDef, _OptionalS3BucketRepositoryOutputTypeDef
-):
-    pass
-
-
 _RequiredS3BucketRepositoryTypeDef = TypedDict(
     "_RequiredS3BucketRepositoryTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalS3BucketRepositoryTypeDef = TypedDict(
     "_OptionalS3BucketRepositoryTypeDef",
     {
         "Details": S3RepositoryDetailsTypeDef,
     },
     total=False,
 )
 
-
 class S3BucketRepositoryTypeDef(
     _RequiredS3BucketRepositoryTypeDef, _OptionalS3BucketRepositoryTypeDef
 ):
     pass
 
-
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "RecommendationSummaries": List[RecommendationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateRepositoryRequestRequestTypeDef",
     {
         "Repository": RepositoryTypeDef,
@@ -755,61 +623,47 @@
         "ClientRequestToken": str,
         "Tags": Mapping[str, str],
         "KMSKeyDetails": KMSKeyDetailsTypeDef,
     },
     total=False,
 )
 
-
 class AssociateRepositoryRequestRequestTypeDef(
     _RequiredAssociateRepositoryRequestRequestTypeDef,
     _OptionalAssociateRepositoryRequestRequestTypeDef,
 ):
     pass
 
-
 AssociateRepositoryResponseTypeDef = TypedDict(
     "AssociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoryAssociationResponseTypeDef = TypedDict(
     "DescribeRepositoryAssociationResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateRepositoryResponseTypeDef = TypedDict(
     "DisassociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SourceCodeTypeOutputTypeDef = TypedDict(
-    "SourceCodeTypeOutputTypeDef",
-    {
-        "CommitDiff": CommitDiffSourceCodeTypeOutputTypeDef,
-        "RepositoryHead": RepositoryHeadSourceCodeTypeOutputTypeDef,
-        "BranchDiff": BranchDiffSourceCodeTypeOutputTypeDef,
-        "S3BucketRepository": S3BucketRepositoryOutputTypeDef,
-        "RequestMetadata": RequestMetadataOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceCodeTypeTypeDef = TypedDict(
     "SourceCodeTypeTypeDef",
     {
         "CommitDiff": CommitDiffSourceCodeTypeTypeDef,
         "RepositoryHead": RepositoryHeadSourceCodeTypeTypeDef,
         "BranchDiff": BranchDiffSourceCodeTypeTypeDef,
         "S3BucketRepository": S3BucketRepositoryTypeDef,
@@ -828,15 +682,15 @@
         "ProviderType": ProviderTypeType,
         "State": JobStateType,
         "CreatedTimeStamp": datetime,
         "LastUpdatedTimeStamp": datetime,
         "Type": TypeType,
         "PullRequestId": str,
         "MetricsSummary": MetricsSummaryTypeDef,
-        "SourceCodeType": SourceCodeTypeOutputTypeDef,
+        "SourceCodeType": SourceCodeTypeTypeDef,
     },
     total=False,
 )
 
 CodeReviewTypeDef = TypedDict(
     "CodeReviewTypeDef",
     {
@@ -847,15 +701,15 @@
         "ProviderType": ProviderTypeType,
         "State": JobStateType,
         "StateReason": str,
         "CreatedTimeStamp": datetime,
         "LastUpdatedTimeStamp": datetime,
         "Type": TypeType,
         "PullRequestId": str,
-        "SourceCodeType": SourceCodeTypeOutputTypeDef,
+        "SourceCodeType": SourceCodeTypeTypeDef,
         "AssociationArn": str,
         "Metrics": MetricsTypeDef,
         "AnalysisTypes": List[AnalysisTypeType],
         "ConfigFileState": ConfigFileStateType,
     },
     total=False,
 )
@@ -870,31 +724,31 @@
 )
 
 ListCodeReviewsResponseTypeDef = TypedDict(
     "ListCodeReviewsResponseTypeDef",
     {
         "CodeReviewSummaries": List[CodeReviewSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCodeReviewResponseTypeDef = TypedDict(
     "CreateCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCodeReviewResponseTypeDef = TypedDict(
     "DescribeCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCodeReviewTypeTypeDef = TypedDict(
     "_RequiredCodeReviewTypeTypeDef",
     {
         "RepositoryAnalysis": RepositoryAnalysisTypeDef,
@@ -904,19 +758,17 @@
     "_OptionalCodeReviewTypeTypeDef",
     {
         "AnalysisTypes": Sequence[AnalysisTypeType],
     },
     total=False,
 )
 
-
 class CodeReviewTypeTypeDef(_RequiredCodeReviewTypeTypeDef, _OptionalCodeReviewTypeTypeDef):
     pass
 
-
 _RequiredCreateCodeReviewRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCodeReviewRequestRequestTypeDef",
     {
         "Name": str,
         "RepositoryAssociationArn": str,
         "Type": CodeReviewTypeTypeDef,
     },
@@ -925,12 +777,11 @@
     "_OptionalCreateCodeReviewRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateCodeReviewRequestRequestTypeDef(
     _RequiredCreateCodeReviewRequestRequestTypeDef, _OptionalCreateCodeReviewRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/type_defs.pyi` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,73 +30,64 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "KMSKeyDetailsTypeDef",
-    "BranchDiffSourceCodeTypeOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "BranchDiffSourceCodeTypeTypeDef",
-    "CodeArtifactsOutputTypeDef",
     "CodeArtifactsTypeDef",
     "CodeCommitRepositoryTypeDef",
     "MetricsSummaryTypeDef",
     "MetricsTypeDef",
-    "CommitDiffSourceCodeTypeOutputTypeDef",
     "CommitDiffSourceCodeTypeTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCodeReviewRequestRequestTypeDef",
     "DescribeRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackTypeDef",
     "DescribeRepositoryAssociationRequestRequestTypeDef",
     "DisassociateRepositoryRequestRequestTypeDef",
-    "EventInfoOutputTypeDef",
     "EventInfoTypeDef",
-    "KMSKeyDetailsOutputTypeDef",
     "ListCodeReviewsRequestRequestTypeDef",
     "ListRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackSummaryTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRepositoryAssociationsRequestRequestTypeDef",
     "RepositoryAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutRecommendationFeedbackRequestRequestTypeDef",
     "RuleMetadataTypeDef",
     "RepositoryHeadSourceCodeTypeTypeDef",
-    "RepositoryHeadSourceCodeTypeOutputTypeDef",
     "S3RepositoryTypeDef",
     "ThirdPartySourceRepositoryTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "S3RepositoryDetailsOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "S3RepositoryDetailsTypeDef",
     "DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef",
     "DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     "DescribeRecommendationFeedbackResponseTypeDef",
-    "RequestMetadataOutputTypeDef",
     "RequestMetadataTypeDef",
     "ListRecommendationFeedbackResponseTypeDef",
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     "ListRepositoryAssociationsResponseTypeDef",
     "RecommendationSummaryTypeDef",
     "RepositoryTypeDef",
     "RepositoryAssociationTypeDef",
-    "S3BucketRepositoryOutputTypeDef",
     "S3BucketRepositoryTypeDef",
     "ListRecommendationsResponseTypeDef",
     "AssociateRepositoryRequestRequestTypeDef",
     "AssociateRepositoryResponseTypeDef",
     "DescribeRepositoryAssociationResponseTypeDef",
     "DisassociateRepositoryResponseTypeDef",
-    "SourceCodeTypeOutputTypeDef",
     "SourceCodeTypeTypeDef",
     "CodeReviewSummaryTypeDef",
     "CodeReviewTypeDef",
     "RepositoryAnalysisTypeDef",
     "ListCodeReviewsResponseTypeDef",
     "CreateCodeReviewResponseTypeDef",
     "DescribeCodeReviewResponseTypeDef",
@@ -109,66 +100,52 @@
     {
         "KMSKeyId": str,
         "EncryptionOption": EncryptionOptionType,
     },
     total=False,
 )
 
-BranchDiffSourceCodeTypeOutputTypeDef = TypedDict(
-    "BranchDiffSourceCodeTypeOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "SourceBranchName": str,
-        "DestinationBranchName": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BranchDiffSourceCodeTypeTypeDef = TypedDict(
     "BranchDiffSourceCodeTypeTypeDef",
     {
         "SourceBranchName": str,
         "DestinationBranchName": str,
     },
 )
 
-_RequiredCodeArtifactsOutputTypeDef = TypedDict(
-    "_RequiredCodeArtifactsOutputTypeDef",
-    {
-        "SourceCodeArtifactsObjectKey": str,
-    },
-)
-_OptionalCodeArtifactsOutputTypeDef = TypedDict(
-    "_OptionalCodeArtifactsOutputTypeDef",
-    {
-        "BuildArtifactsObjectKey": str,
-    },
-    total=False,
-)
-
-class CodeArtifactsOutputTypeDef(
-    _RequiredCodeArtifactsOutputTypeDef, _OptionalCodeArtifactsOutputTypeDef
-):
-    pass
-
 _RequiredCodeArtifactsTypeDef = TypedDict(
     "_RequiredCodeArtifactsTypeDef",
     {
         "SourceCodeArtifactsObjectKey": str,
     },
 )
 _OptionalCodeArtifactsTypeDef = TypedDict(
     "_OptionalCodeArtifactsTypeDef",
     {
         "BuildArtifactsObjectKey": str,
     },
     total=False,
 )
 
+
 class CodeArtifactsTypeDef(_RequiredCodeArtifactsTypeDef, _OptionalCodeArtifactsTypeDef):
     pass
 
+
 CodeCommitRepositoryTypeDef = TypedDict(
     "CodeCommitRepositoryTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -188,24 +165,14 @@
         "MeteredLinesOfCodeCount": int,
         "SuppressedLinesOfCodeCount": int,
         "FindingsCount": int,
     },
     total=False,
 )
 
-CommitDiffSourceCodeTypeOutputTypeDef = TypedDict(
-    "CommitDiffSourceCodeTypeOutputTypeDef",
-    {
-        "SourceCommit": str,
-        "DestinationCommit": str,
-        "MergeBaseCommit": str,
-    },
-    total=False,
-)
-
 CommitDiffSourceCodeTypeTypeDef = TypedDict(
     "CommitDiffSourceCodeTypeTypeDef",
     {
         "SourceCommit": str,
         "DestinationCommit": str,
         "MergeBaseCommit": str,
     },
@@ -239,20 +206,22 @@
     "_OptionalDescribeRecommendationFeedbackRequestRequestTypeDef",
     {
         "UserId": str,
     },
     total=False,
 )
 
+
 class DescribeRecommendationFeedbackRequestRequestTypeDef(
     _RequiredDescribeRecommendationFeedbackRequestRequestTypeDef,
     _OptionalDescribeRecommendationFeedbackRequestRequestTypeDef,
 ):
     pass
 
+
 RecommendationFeedbackTypeDef = TypedDict(
     "RecommendationFeedbackTypeDef",
     {
         "CodeReviewArn": str,
         "RecommendationId": str,
         "Reactions": List[ReactionType],
         "UserId": str,
@@ -272,41 +241,23 @@
 DisassociateRepositoryRequestRequestTypeDef = TypedDict(
     "DisassociateRepositoryRequestRequestTypeDef",
     {
         "AssociationArn": str,
     },
 )
 
-EventInfoOutputTypeDef = TypedDict(
-    "EventInfoOutputTypeDef",
-    {
-        "Name": str,
-        "State": str,
-    },
-    total=False,
-)
-
 EventInfoTypeDef = TypedDict(
     "EventInfoTypeDef",
     {
         "Name": str,
         "State": str,
     },
     total=False,
 )
 
-KMSKeyDetailsOutputTypeDef = TypedDict(
-    "KMSKeyDetailsOutputTypeDef",
-    {
-        "KMSKeyId": str,
-        "EncryptionOption": EncryptionOptionType,
-    },
-    total=False,
-)
-
 _RequiredListCodeReviewsRequestRequestTypeDef = TypedDict(
     "_RequiredListCodeReviewsRequestRequestTypeDef",
     {
         "Type": TypeType,
     },
 )
 _OptionalListCodeReviewsRequestRequestTypeDef = TypedDict(
@@ -317,19 +268,21 @@
         "RepositoryNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListCodeReviewsRequestRequestTypeDef(
     _RequiredListCodeReviewsRequestRequestTypeDef, _OptionalListCodeReviewsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListRecommendationFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendationFeedbackRequestRequestTypeDef",
     {
         "CodeReviewArn": str,
     },
 )
 _OptionalListRecommendationFeedbackRequestRequestTypeDef = TypedDict(
@@ -339,20 +292,22 @@
         "MaxResults": int,
         "UserIds": Sequence[str],
         "RecommendationIds": Sequence[str],
     },
     total=False,
 )
 
+
 class ListRecommendationFeedbackRequestRequestTypeDef(
     _RequiredListRecommendationFeedbackRequestRequestTypeDef,
     _OptionalListRecommendationFeedbackRequestRequestTypeDef,
 ):
     pass
 
+
 RecommendationFeedbackSummaryTypeDef = TypedDict(
     "RecommendationFeedbackSummaryTypeDef",
     {
         "RecommendationId": str,
         "Reactions": List[ReactionType],
         "UserId": str,
     },
@@ -370,28 +325,28 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ProviderTypes": Sequence[ProviderTypeType],
-        "States": Sequence[RepositoryAssociationStateType],
-        "Names": Sequence[str],
-        "Owners": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRepositoryAssociationsRequestRequestTypeDef = TypedDict(
     "ListRepositoryAssociationsRequestRequestTypeDef",
     {
@@ -423,32 +378,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 PutRecommendationFeedbackRequestRequestTypeDef = TypedDict(
     "PutRecommendationFeedbackRequestRequestTypeDef",
     {
         "CodeReviewArn": str,
         "RecommendationId": str,
         "Reactions": Sequence[ReactionType],
     },
@@ -469,21 +406,14 @@
 RepositoryHeadSourceCodeTypeTypeDef = TypedDict(
     "RepositoryHeadSourceCodeTypeTypeDef",
     {
         "BranchName": str,
     },
 )
 
-RepositoryHeadSourceCodeTypeOutputTypeDef = TypedDict(
-    "RepositoryHeadSourceCodeTypeOutputTypeDef",
-    {
-        "BranchName": str,
-    },
-)
-
 S3RepositoryTypeDef = TypedDict(
     "S3RepositoryTypeDef",
     {
         "Name": str,
         "BucketName": str,
     },
 )
@@ -493,25 +423,14 @@
     {
         "Name": str,
         "ConnectionArn": str,
         "Owner": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -520,21 +439,20 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-S3RepositoryDetailsOutputTypeDef = TypedDict(
-    "S3RepositoryDetailsOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "BucketName": str,
-        "CodeArtifacts": CodeArtifactsOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 S3RepositoryDetailsTypeDef = TypedDict(
     "S3RepositoryDetailsTypeDef",
     {
         "BucketName": str,
         "CodeArtifacts": CodeArtifactsTypeDef,
@@ -552,59 +470,52 @@
     "_OptionalDescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef(
     _RequiredDescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     _OptionalDescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef = TypedDict(
     "_RequiredDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     {
         "AssociationArn": str,
     },
 )
 _OptionalDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef = TypedDict(
     "_OptionalDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef(
     _RequiredDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     _OptionalDescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
 ):
     pass
 
+
 DescribeRecommendationFeedbackResponseTypeDef = TypedDict(
     "DescribeRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedback": RecommendationFeedbackTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RequestMetadataOutputTypeDef = TypedDict(
-    "RequestMetadataOutputTypeDef",
-    {
-        "RequestId": str,
-        "Requester": str,
-        "EventInfo": EventInfoOutputTypeDef,
-        "VendorName": VendorNameType,
-    },
-    total=False,
-)
-
 RequestMetadataTypeDef = TypedDict(
     "RequestMetadataTypeDef",
     {
         "RequestId": str,
         "Requester": str,
         "EventInfo": EventInfoTypeDef,
         "VendorName": VendorNameType,
@@ -613,24 +524,36 @@
 )
 
 ListRecommendationFeedbackResponseTypeDef = TypedDict(
     "ListRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedbackSummaries": List[RecommendationFeedbackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+    {
+        "ProviderTypes": Sequence[ProviderTypeType],
+        "States": Sequence[RepositoryAssociationStateType],
+        "Names": Sequence[str],
+        "Owners": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListRepositoryAssociationsResponseTypeDef = TypedDict(
     "ListRepositoryAssociationsResponseTypeDef",
     {
         "RepositoryAssociationSummaries": List[RepositoryAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "FilePath": str,
@@ -665,64 +588,47 @@
         "Name": str,
         "Owner": str,
         "ProviderType": ProviderTypeType,
         "State": RepositoryAssociationStateType,
         "StateReason": str,
         "LastUpdatedTimeStamp": datetime,
         "CreatedTimeStamp": datetime,
-        "KMSKeyDetails": KMSKeyDetailsOutputTypeDef,
-        "S3RepositoryDetails": S3RepositoryDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredS3BucketRepositoryOutputTypeDef = TypedDict(
-    "_RequiredS3BucketRepositoryOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalS3BucketRepositoryOutputTypeDef = TypedDict(
-    "_OptionalS3BucketRepositoryOutputTypeDef",
-    {
-        "Details": S3RepositoryDetailsOutputTypeDef,
+        "KMSKeyDetails": KMSKeyDetailsTypeDef,
+        "S3RepositoryDetails": S3RepositoryDetailsTypeDef,
     },
     total=False,
 )
 
-class S3BucketRepositoryOutputTypeDef(
-    _RequiredS3BucketRepositoryOutputTypeDef, _OptionalS3BucketRepositoryOutputTypeDef
-):
-    pass
-
 _RequiredS3BucketRepositoryTypeDef = TypedDict(
     "_RequiredS3BucketRepositoryTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalS3BucketRepositoryTypeDef = TypedDict(
     "_OptionalS3BucketRepositoryTypeDef",
     {
         "Details": S3RepositoryDetailsTypeDef,
     },
     total=False,
 )
 
+
 class S3BucketRepositoryTypeDef(
     _RequiredS3BucketRepositoryTypeDef, _OptionalS3BucketRepositoryTypeDef
 ):
     pass
 
+
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "RecommendationSummaries": List[RecommendationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateRepositoryRequestRequestTypeDef",
     {
         "Repository": RepositoryTypeDef,
@@ -734,59 +640,49 @@
         "ClientRequestToken": str,
         "Tags": Mapping[str, str],
         "KMSKeyDetails": KMSKeyDetailsTypeDef,
     },
     total=False,
 )
 
+
 class AssociateRepositoryRequestRequestTypeDef(
     _RequiredAssociateRepositoryRequestRequestTypeDef,
     _OptionalAssociateRepositoryRequestRequestTypeDef,
 ):
     pass
 
+
 AssociateRepositoryResponseTypeDef = TypedDict(
     "AssociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoryAssociationResponseTypeDef = TypedDict(
     "DescribeRepositoryAssociationResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateRepositoryResponseTypeDef = TypedDict(
     "DisassociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SourceCodeTypeOutputTypeDef = TypedDict(
-    "SourceCodeTypeOutputTypeDef",
-    {
-        "CommitDiff": CommitDiffSourceCodeTypeOutputTypeDef,
-        "RepositoryHead": RepositoryHeadSourceCodeTypeOutputTypeDef,
-        "BranchDiff": BranchDiffSourceCodeTypeOutputTypeDef,
-        "S3BucketRepository": S3BucketRepositoryOutputTypeDef,
-        "RequestMetadata": RequestMetadataOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceCodeTypeTypeDef = TypedDict(
     "SourceCodeTypeTypeDef",
     {
         "CommitDiff": CommitDiffSourceCodeTypeTypeDef,
         "RepositoryHead": RepositoryHeadSourceCodeTypeTypeDef,
         "BranchDiff": BranchDiffSourceCodeTypeTypeDef,
         "S3BucketRepository": S3BucketRepositoryTypeDef,
@@ -805,15 +701,15 @@
         "ProviderType": ProviderTypeType,
         "State": JobStateType,
         "CreatedTimeStamp": datetime,
         "LastUpdatedTimeStamp": datetime,
         "Type": TypeType,
         "PullRequestId": str,
         "MetricsSummary": MetricsSummaryTypeDef,
-        "SourceCodeType": SourceCodeTypeOutputTypeDef,
+        "SourceCodeType": SourceCodeTypeTypeDef,
     },
     total=False,
 )
 
 CodeReviewTypeDef = TypedDict(
     "CodeReviewTypeDef",
     {
@@ -824,15 +720,15 @@
         "ProviderType": ProviderTypeType,
         "State": JobStateType,
         "StateReason": str,
         "CreatedTimeStamp": datetime,
         "LastUpdatedTimeStamp": datetime,
         "Type": TypeType,
         "PullRequestId": str,
-        "SourceCodeType": SourceCodeTypeOutputTypeDef,
+        "SourceCodeType": SourceCodeTypeTypeDef,
         "AssociationArn": str,
         "Metrics": MetricsTypeDef,
         "AnalysisTypes": List[AnalysisTypeType],
         "ConfigFileState": ConfigFileStateType,
     },
     total=False,
 )
@@ -847,31 +743,31 @@
 )
 
 ListCodeReviewsResponseTypeDef = TypedDict(
     "ListCodeReviewsResponseTypeDef",
     {
         "CodeReviewSummaries": List[CodeReviewSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCodeReviewResponseTypeDef = TypedDict(
     "CreateCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCodeReviewResponseTypeDef = TypedDict(
     "DescribeCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCodeReviewTypeTypeDef = TypedDict(
     "_RequiredCodeReviewTypeTypeDef",
     {
         "RepositoryAnalysis": RepositoryAnalysisTypeDef,
@@ -881,17 +777,19 @@
     "_OptionalCodeReviewTypeTypeDef",
     {
         "AnalysisTypes": Sequence[AnalysisTypeType],
     },
     total=False,
 )
 
+
 class CodeReviewTypeTypeDef(_RequiredCodeReviewTypeTypeDef, _OptionalCodeReviewTypeTypeDef):
     pass
 
+
 _RequiredCreateCodeReviewRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCodeReviewRequestRequestTypeDef",
     {
         "Name": str,
         "RepositoryAssociationArn": str,
         "Type": CodeReviewTypeTypeDef,
     },
@@ -900,11 +798,12 @@
     "_OptionalCreateCodeReviewRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateCodeReviewRequestRequestTypeDef(
     _RequiredCreateCodeReviewRequestRequestTypeDef, _OptionalCreateCodeReviewRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/waiter.py` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/waiter.pyi` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-reviewer
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeGuruReviewer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeGuruReviewer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-reviewer)](https://pepy.tech/project/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,71 +364,61 @@
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
-    BranchDiffSourceCodeTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
-    CodeArtifactsOutputTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
-    CommitDiffSourceCodeTypeOutputTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeReviewRequestRequestTypeDef,
     DescribeRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackTypeDef,
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
-    EventInfoOutputTypeDef,
     EventInfoTypeDef,
-    KMSKeyDetailsOutputTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
-    RepositoryHeadSourceCodeTypeOutputTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    S3RepositoryDetailsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
-    RequestMetadataOutputTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
+    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
-    S3BucketRepositoryOutputTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
     AssociateRepositoryResponseTypeDef,
     DescribeRepositoryAssociationResponseTypeDef,
     DisassociateRepositoryResponseTypeDef,
-    SourceCodeTypeOutputTypeDef,
     SourceCodeTypeTypeDef,
     CodeReviewSummaryTypeDef,
     CodeReviewTypeDef,
     RepositoryAnalysisTypeDef,
     ListCodeReviewsResponseTypeDef,
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt` & `mypy-boto3-codeguru-reviewer-1.28.15/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.12/setup.py` & `mypy-boto3-codeguru-reviewer-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguru-reviewer",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_codeguru_reviewer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruReviewer 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CodeGuruReviewer 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

