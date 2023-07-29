# Comparing `tmp/mypy-boto3-comprehend-1.28.12.tar.gz` & `tmp/mypy-boto3-comprehend-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-comprehend-1.28.12.tar", last modified: Thu Jul 27 05:34:30 2023, max compression
+gzip compressed data, was "mypy-boto3-comprehend-1.28.15.tar", last modified: Fri Jul 28 20:42:31 2023, max compression
```

## Comparing `mypy-boto3-comprehend-1.28.12.tar` & `mypy-boto3-comprehend-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.268546 mypy-boto3-comprehend-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28371 2023-07-27 05:34:30.260546 mypy-boto3-comprehend-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26872 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.260546 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67084 2023-07-27 05:19:25.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66983 2023-07-27 05:19:24.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-07-27 05:19:25.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-07-27 05:19:25.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-07-27 05:19:25.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-27 05:19:25.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   107525 2023-07-27 05:19:27.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   107426 2023-07-27 05:19:26.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.260546 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28371 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:30.000000 mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:30.268546 mypy-boto3-comprehend-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:19:23.000000 mypy-boto3-comprehend-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.852872 mypy-boto3-comprehend-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:57.000000 mypy-boto3-comprehend-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28042 2023-07-28 20:42:31.848872 mypy-boto3-comprehend-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-28 20:21:57.000000 mypy-boto3-comprehend-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.844871 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-28 20:21:57.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-28 20:21:57.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:21:57.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67084 2023-07-28 20:21:58.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66983 2023-07-28 20:21:58.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-07-28 20:21:59.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-07-28 20:21:58.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-07-28 20:21:58.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-07-28 20:21:58.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:57.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   104121 2023-07-28 20:22:02.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104032 2023-07-28 20:22:00.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:57.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.848872 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28042 2023-07-28 20:42:31.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:31.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:31.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:31.000000 mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:31.852872 mypy-boto3-comprehend-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:21:56.000000 mypy-boto3-comprehend-1.28.15/setup.py
```

### Comparing `mypy-boto3-comprehend-1.28.12/LICENSE` & `mypy-boto3-comprehend-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.12/PKG-INFO` & `mypy-boto3-comprehend-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehend
-Version: 1.28.12
-Summary: Type annotations for boto3.Comprehend 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Comprehend 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehend)](https://pepy.tech/project/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -403,14 +403,15 @@
 ```python
 from mypy_boto3_comprehend.type_defs import (
     AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
+    ResponseMetadataTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
@@ -423,21 +424,16 @@
     DocumentLabelTypeDef,
     DocumentTypeListItemTypeDef,
     ErrorsListItemTypeDef,
     WarningsListItemTypeDef,
     ContainsPiiEntitiesRequestRequestTypeDef,
     EntityLabelTypeDef,
     TagTypeDef,
-    CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
-    CreateDocumentClassifierResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEntityRecognizerResponseTypeDef,
-    CreateFlywheelResponseTypeDef,
     VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
     DatasetFilterTypeDef,
@@ -457,169 +453,165 @@
     DescribeEntityRecognizerRequestRequestTypeDef,
     DescribeEventsDetectionJobRequestRequestTypeDef,
     DescribeFlywheelIterationRequestRequestTypeDef,
     DescribeFlywheelRequestRequestTypeDef,
     DescribeKeyPhrasesDetectionJobRequestRequestTypeDef,
     DescribePiiEntitiesDetectionJobRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSentimentDetectionJobRequestRequestTypeDef,
     DescribeTargetedSentimentDetectionJobRequestRequestTypeDef,
     DescribeTopicsDetectionJobRequestRequestTypeDef,
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
     DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
     DocumentClassificationJobFilterTypeDef,
-    OutputDataConfigOutputTypeDef,
-    DocumentClassifierDocumentsOutputTypeDef,
+    OutputDataConfigTypeDef,
     DocumentClassifierDocumentsTypeDef,
     DocumentClassifierFilterTypeDef,
     DocumentReaderConfigOutputTypeDef,
-    DocumentClassifierOutputDataConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
-    EntityTypesListItemOutputTypeDef,
     EntityTypesListItemTypeDef,
-    EntityRecognizerAnnotationsOutputTypeDef,
     EntityRecognizerAnnotationsTypeDef,
-    EntityRecognizerDocumentsOutputTypeDef,
     EntityRecognizerDocumentsTypeDef,
-    EntityRecognizerEntityListOutputTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
     EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
-    ImportModelResponseTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
     TopicsDetectionJobFilterTypeDef,
-    OutputDataConfigTypeDef,
-    PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
     RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RedactionConfigTypeDef,
-    ResponseMetadataTypeDef,
+    StartFlywheelIterationRequestRequestTypeDef,
+    StopDominantLanguageDetectionJobRequestRequestTypeDef,
+    StopEntitiesDetectionJobRequestRequestTypeDef,
+    StopEventsDetectionJobRequestRequestTypeDef,
+    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
+    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
+    StopSentimentDetectionJobRequestRequestTypeDef,
+    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
+    StopTrainingDocumentClassifierRequestRequestTypeDef,
+    StopTrainingEntityRecognizerRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
+    BatchDetectDominantLanguageItemResultTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateDocumentClassifierResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEntityRecognizerResponseTypeDef,
+    CreateFlywheelResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    DetectDominantLanguageResponseTypeDef,
+    ImportModelResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
-    StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
     StartPiiEntitiesDetectionJobResponseTypeDef,
     StartSentimentDetectionJobResponseTypeDef,
     StartTargetedSentimentDetectionJobResponseTypeDef,
     StartTopicsDetectionJobResponseTypeDef,
-    StopDominantLanguageDetectionJobRequestRequestTypeDef,
     StopDominantLanguageDetectionJobResponseTypeDef,
-    StopEntitiesDetectionJobRequestRequestTypeDef,
     StopEntitiesDetectionJobResponseTypeDef,
-    StopEventsDetectionJobRequestRequestTypeDef,
     StopEventsDetectionJobResponseTypeDef,
-    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
-    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
-    StopSentimentDetectionJobRequestRequestTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
-    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
-    StopTrainingDocumentClassifierRequestRequestTypeDef,
-    StopTrainingEntityRecognizerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
-    BatchDetectDominantLanguageItemResultTypeDef,
-    DetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesItemResultTypeDef,
     DetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentItemResultTypeDef,
     DetectSentimentResponseTypeDef,
     MentionSentimentTypeDef,
     BlockReferenceTypeDef,
     ClassifierMetadataTypeDef,
     ClassifyDocumentRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     InputDataConfigTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
     DataSecurityConfigOutputTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
-    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
     DocumentClassifierInputDataConfigTypeDef,
-    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
     DocumentClassifierInputDataConfigOutputTypeDef,
     InputDataConfigOutputTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
-    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
-    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
     EntityRecognitionConfigOutputTypeDef,
     EntityRecognitionConfigTypeDef,
     EntityRecognizerInputDataConfigOutputTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
-    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
     ListFlywheelIterationHistoryRequestRequestTypeDef,
     FlywheelIterationPropertiesTypeDef,
     ListFlywheelsResponseTypeDef,
     GeometryTypeDef,
-    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
+    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
+    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
+    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
+    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
+    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
```

### Comparing `mypy-boto3-comprehend-1.28.12/README.md` & `mypy-boto3-comprehend-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehend)](https://pepy.tech/project/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,14 +371,15 @@
 ```python
 from mypy_boto3_comprehend.type_defs import (
     AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
+    ResponseMetadataTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
@@ -391,21 +392,16 @@
     DocumentLabelTypeDef,
     DocumentTypeListItemTypeDef,
     ErrorsListItemTypeDef,
     WarningsListItemTypeDef,
     ContainsPiiEntitiesRequestRequestTypeDef,
     EntityLabelTypeDef,
     TagTypeDef,
-    CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
-    CreateDocumentClassifierResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEntityRecognizerResponseTypeDef,
-    CreateFlywheelResponseTypeDef,
     VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
     DatasetFilterTypeDef,
@@ -425,169 +421,165 @@
     DescribeEntityRecognizerRequestRequestTypeDef,
     DescribeEventsDetectionJobRequestRequestTypeDef,
     DescribeFlywheelIterationRequestRequestTypeDef,
     DescribeFlywheelRequestRequestTypeDef,
     DescribeKeyPhrasesDetectionJobRequestRequestTypeDef,
     DescribePiiEntitiesDetectionJobRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSentimentDetectionJobRequestRequestTypeDef,
     DescribeTargetedSentimentDetectionJobRequestRequestTypeDef,
     DescribeTopicsDetectionJobRequestRequestTypeDef,
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
     DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
     DocumentClassificationJobFilterTypeDef,
-    OutputDataConfigOutputTypeDef,
-    DocumentClassifierDocumentsOutputTypeDef,
+    OutputDataConfigTypeDef,
     DocumentClassifierDocumentsTypeDef,
     DocumentClassifierFilterTypeDef,
     DocumentReaderConfigOutputTypeDef,
-    DocumentClassifierOutputDataConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
-    EntityTypesListItemOutputTypeDef,
     EntityTypesListItemTypeDef,
-    EntityRecognizerAnnotationsOutputTypeDef,
     EntityRecognizerAnnotationsTypeDef,
-    EntityRecognizerDocumentsOutputTypeDef,
     EntityRecognizerDocumentsTypeDef,
-    EntityRecognizerEntityListOutputTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
     EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
-    ImportModelResponseTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
     TopicsDetectionJobFilterTypeDef,
-    OutputDataConfigTypeDef,
-    PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
     RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RedactionConfigTypeDef,
-    ResponseMetadataTypeDef,
+    StartFlywheelIterationRequestRequestTypeDef,
+    StopDominantLanguageDetectionJobRequestRequestTypeDef,
+    StopEntitiesDetectionJobRequestRequestTypeDef,
+    StopEventsDetectionJobRequestRequestTypeDef,
+    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
+    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
+    StopSentimentDetectionJobRequestRequestTypeDef,
+    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
+    StopTrainingDocumentClassifierRequestRequestTypeDef,
+    StopTrainingEntityRecognizerRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
+    BatchDetectDominantLanguageItemResultTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateDocumentClassifierResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEntityRecognizerResponseTypeDef,
+    CreateFlywheelResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    DetectDominantLanguageResponseTypeDef,
+    ImportModelResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
-    StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
     StartPiiEntitiesDetectionJobResponseTypeDef,
     StartSentimentDetectionJobResponseTypeDef,
     StartTargetedSentimentDetectionJobResponseTypeDef,
     StartTopicsDetectionJobResponseTypeDef,
-    StopDominantLanguageDetectionJobRequestRequestTypeDef,
     StopDominantLanguageDetectionJobResponseTypeDef,
-    StopEntitiesDetectionJobRequestRequestTypeDef,
     StopEntitiesDetectionJobResponseTypeDef,
-    StopEventsDetectionJobRequestRequestTypeDef,
     StopEventsDetectionJobResponseTypeDef,
-    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
-    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
-    StopSentimentDetectionJobRequestRequestTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
-    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
-    StopTrainingDocumentClassifierRequestRequestTypeDef,
-    StopTrainingEntityRecognizerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
-    BatchDetectDominantLanguageItemResultTypeDef,
-    DetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesItemResultTypeDef,
     DetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentItemResultTypeDef,
     DetectSentimentResponseTypeDef,
     MentionSentimentTypeDef,
     BlockReferenceTypeDef,
     ClassifierMetadataTypeDef,
     ClassifyDocumentRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     InputDataConfigTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
     DataSecurityConfigOutputTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
-    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
     DocumentClassifierInputDataConfigTypeDef,
-    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
     DocumentClassifierInputDataConfigOutputTypeDef,
     InputDataConfigOutputTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
-    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
-    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
     EntityRecognitionConfigOutputTypeDef,
     EntityRecognitionConfigTypeDef,
     EntityRecognizerInputDataConfigOutputTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
-    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
     ListFlywheelIterationHistoryRequestRequestTypeDef,
     FlywheelIterationPropertiesTypeDef,
     ListFlywheelsResponseTypeDef,
     GeometryTypeDef,
-    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
+    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
+    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
+    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
+    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
+    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
```

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__init__.py` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__init__.pyi` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/__main__.py` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Comprehend 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Comprehend 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend\nOther"
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

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/client.py` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/client.pyi` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/literals.py` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/literals.pyi` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/paginator.py` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassificationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDocumentClassificationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassificationjobspaginator)
         """
 
 
@@ -113,15 +113,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassifierspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDocumentClassifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassifierspaginator)
         """
 
 
@@ -131,33 +131,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDominantLanguageDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
         """
 
 
 class ListEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listendpointspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Filter: EndpointFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Filter: EndpointFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listendpointspaginator)
         """
 
 
@@ -167,15 +164,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentitiesdetectionjobspaginator)
         """
 
 
@@ -185,15 +182,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentityrecognizerspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEntityRecognizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentityrecognizerspaginator)
         """
 
 
@@ -203,15 +200,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeyPhrasesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
         """
 
 
@@ -221,15 +218,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPiiEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListPiiEntitiesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
         """
 
 
@@ -239,15 +236,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listsentimentdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSentimentDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listsentimentdetectionjobspaginator)
         """
 
 
@@ -257,13 +254,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listtopicsdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTopicsDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listtopicsdetectionjobspaginator)
         """
```

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/paginator.pyi` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassificationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDocumentClassificationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassificationjobspaginator)
         """
 
 class ListDocumentClassifiersPaginator(Paginator):
@@ -109,15 +109,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassifierspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDocumentClassifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdocumentclassifierspaginator)
         """
 
 class ListDominantLanguageDetectionJobsPaginator(Paginator):
@@ -126,32 +126,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDominantLanguageDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
         """
 
 class ListEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listendpointspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Filter: EndpointFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Filter: EndpointFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listendpointspaginator)
         """
 
 class ListEntitiesDetectionJobsPaginator(Paginator):
@@ -160,15 +157,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentitiesdetectionjobspaginator)
         """
 
 class ListEntityRecognizersPaginator(Paginator):
@@ -177,15 +174,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentityrecognizerspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEntityRecognizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listentityrecognizerspaginator)
         """
 
 class ListKeyPhrasesDetectionJobsPaginator(Paginator):
@@ -194,15 +191,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeyPhrasesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
         """
 
 class ListPiiEntitiesDetectionJobsPaginator(Paginator):
@@ -211,15 +208,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPiiEntitiesDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListPiiEntitiesDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
         """
 
 class ListSentimentDetectionJobsPaginator(Paginator):
@@ -228,15 +225,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listsentimentdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSentimentDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listsentimentdetectionjobspaginator)
         """
 
 class ListTopicsDetectionJobsPaginator(Paginator):
@@ -245,13 +242,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listtopicsdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTopicsDetectionJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/paginators/#listtopicsdetectionjobspaginator)
         """
```

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/type_defs.py` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
 __all__ = (
     "AugmentedManifestsListItemOutputTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
     "BatchDetectKeyPhrasesRequestRequestTypeDef",
     "SentimentScoreTypeDef",
     "BatchDetectSentimentRequestRequestTypeDef",
     "BatchDetectSyntaxRequestRequestTypeDef",
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
@@ -84,21 +85,16 @@
     "DocumentLabelTypeDef",
     "DocumentTypeListItemTypeDef",
     "ErrorsListItemTypeDef",
     "WarningsListItemTypeDef",
     "ContainsPiiEntitiesRequestRequestTypeDef",
     "EntityLabelTypeDef",
     "TagTypeDef",
-    "CreateDatasetResponseTypeDef",
     "DocumentClassifierOutputDataConfigTypeDef",
     "VpcConfigTypeDef",
-    "CreateDocumentClassifierResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
-    "CreateEntityRecognizerResponseTypeDef",
-    "CreateFlywheelResponseTypeDef",
     "VpcConfigOutputTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
     "DatasetFilterTypeDef",
@@ -118,169 +114,165 @@
     "DescribeEntityRecognizerRequestRequestTypeDef",
     "DescribeEventsDetectionJobRequestRequestTypeDef",
     "DescribeFlywheelIterationRequestRequestTypeDef",
     "DescribeFlywheelRequestRequestTypeDef",
     "DescribeKeyPhrasesDetectionJobRequestRequestTypeDef",
     "DescribePiiEntitiesDetectionJobRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTargetedSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTopicsDetectionJobRequestRequestTypeDef",
     "DetectDominantLanguageRequestRequestTypeDef",
     "DetectKeyPhrasesRequestRequestTypeDef",
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
     "DocumentClassificationConfigOutputTypeDef",
     "DocumentClassificationConfigTypeDef",
     "DocumentClassificationJobFilterTypeDef",
-    "OutputDataConfigOutputTypeDef",
-    "DocumentClassifierDocumentsOutputTypeDef",
+    "OutputDataConfigTypeDef",
     "DocumentClassifierDocumentsTypeDef",
     "DocumentClassifierFilterTypeDef",
     "DocumentReaderConfigOutputTypeDef",
-    "DocumentClassifierOutputDataConfigOutputTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
     "DominantLanguageDetectionJobFilterTypeDef",
     "EndpointFilterTypeDef",
     "EntitiesDetectionJobFilterTypeDef",
-    "EntityTypesListItemOutputTypeDef",
     "EntityTypesListItemTypeDef",
-    "EntityRecognizerAnnotationsOutputTypeDef",
     "EntityRecognizerAnnotationsTypeDef",
-    "EntityRecognizerDocumentsOutputTypeDef",
     "EntityRecognizerDocumentsTypeDef",
-    "EntityRecognizerEntityListOutputTypeDef",
     "EntityRecognizerEntityListTypeDef",
     "EntityRecognizerEvaluationMetricsTypeDef",
     "EntityRecognizerFilterTypeDef",
     "EntityTypesEvaluationMetricsTypeDef",
     "EntityRecognizerOutputDataConfigTypeDef",
     "EntityRecognizerSummaryTypeDef",
     "EventsDetectionJobFilterTypeDef",
     "FlywheelFilterTypeDef",
     "FlywheelIterationFilterTypeDef",
     "FlywheelModelEvaluationMetricsTypeDef",
     "FlywheelSummaryTypeDef",
     "PointTypeDef",
-    "ImportModelResponseTypeDef",
     "KeyPhrasesDetectionJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
     "PiiEntitiesDetectionJobFilterTypeDef",
     "SentimentDetectionJobFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "TargetedSentimentDetectionJobFilterTypeDef",
     "TopicsDetectionJobFilterTypeDef",
-    "OutputDataConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
     "RedactionConfigOutputTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
     "RedactionConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "StartFlywheelIterationRequestRequestTypeDef",
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
+    "StopEventsDetectionJobRequestRequestTypeDef",
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
+    "StopSentimentDetectionJobRequestRequestTypeDef",
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "UpdateEndpointRequestRequestTypeDef",
+    "BatchDetectDominantLanguageItemResultTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateDocumentClassifierResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
+    "CreateEntityRecognizerResponseTypeDef",
+    "CreateFlywheelResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "DetectDominantLanguageResponseTypeDef",
+    "ImportModelResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
     "StartDocumentClassificationJobResponseTypeDef",
     "StartDominantLanguageDetectionJobResponseTypeDef",
     "StartEntitiesDetectionJobResponseTypeDef",
     "StartEventsDetectionJobResponseTypeDef",
-    "StartFlywheelIterationRequestRequestTypeDef",
     "StartFlywheelIterationResponseTypeDef",
     "StartKeyPhrasesDetectionJobResponseTypeDef",
     "StartPiiEntitiesDetectionJobResponseTypeDef",
     "StartSentimentDetectionJobResponseTypeDef",
     "StartTargetedSentimentDetectionJobResponseTypeDef",
     "StartTopicsDetectionJobResponseTypeDef",
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     "StopDominantLanguageDetectionJobResponseTypeDef",
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
     "StopEntitiesDetectionJobResponseTypeDef",
-    "StopEventsDetectionJobRequestRequestTypeDef",
     "StopEventsDetectionJobResponseTypeDef",
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StopKeyPhrasesDetectionJobResponseTypeDef",
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StopPiiEntitiesDetectionJobResponseTypeDef",
-    "StopSentimentDetectionJobRequestRequestTypeDef",
     "StopSentimentDetectionJobResponseTypeDef",
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StopTargetedSentimentDetectionJobResponseTypeDef",
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
-    "BatchDetectDominantLanguageItemResultTypeDef",
-    "DetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesItemResultTypeDef",
     "DetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentItemResultTypeDef",
     "DetectSentimentResponseTypeDef",
     "MentionSentimentTypeDef",
     "BlockReferenceTypeDef",
     "ClassifierMetadataTypeDef",
     "ClassifyDocumentRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "ContainsPiiEntitiesResponseTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "ImportModelRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DataSecurityConfigTypeDef",
     "UpdateDataSecurityConfigTypeDef",
     "DataSecurityConfigOutputTypeDef",
     "DatasetEntityRecognizerInputDataConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
     "ListDocumentClassificationJobsRequestRequestTypeDef",
     "DocumentClassifierInputDataConfigTypeDef",
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
     "ListDocumentClassifiersRequestRequestTypeDef",
     "DocumentClassifierInputDataConfigOutputTypeDef",
     "InputDataConfigOutputTypeDef",
     "ListDocumentClassifierSummariesResponseTypeDef",
     "DocumentMetadataTypeDef",
-    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
     "ListEndpointsRequestRequestTypeDef",
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
     "EntityRecognitionConfigOutputTypeDef",
     "EntityRecognitionConfigTypeDef",
     "EntityRecognizerInputDataConfigOutputTypeDef",
     "EntityRecognizerInputDataConfigTypeDef",
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     "ListEntityRecognizersRequestRequestTypeDef",
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     "ListEntityRecognizerSummariesResponseTypeDef",
     "ListEventsDetectionJobsRequestRequestTypeDef",
     "ListFlywheelsRequestRequestTypeDef",
     "ListFlywheelIterationHistoryRequestRequestTypeDef",
     "FlywheelIterationPropertiesTypeDef",
     "ListFlywheelsResponseTypeDef",
     "GeometryTypeDef",
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     "ListSentimentDetectionJobsRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     "SyntaxTokenTypeDef",
     "BatchDetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentResponseTypeDef",
@@ -429,14 +421,25 @@
         "Index": int,
         "ErrorCode": str,
         "ErrorMessage": str,
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
 BatchDetectEntitiesRequestRequestTypeDef = TypedDict(
     "BatchDetectEntitiesRequestRequestTypeDef",
     {
         "TextList": Sequence[str],
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -643,22 +646,14 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DocumentClassifierOutputDataConfigTypeDef = TypedDict(
     "DocumentClassifierOutputDataConfigTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
         "FlywheelStatsS3Prefix": str,
     },
@@ -669,48 +664,14 @@
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
 
-CreateDocumentClassifierResponseTypeDef = TypedDict(
-    "CreateDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
-    {
-        "EndpointArn": str,
-        "ModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEntityRecognizerResponseTypeDef = TypedDict(
-    "CreateEntityRecognizerResponseTypeDef",
-    {
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFlywheelResponseTypeDef = TypedDict(
-    "CreateFlywheelResponseTypeDef",
-    {
-        "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VpcConfigOutputTypeDef = TypedDict(
     "VpcConfigOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "Subnets": List[str],
     },
 )
@@ -983,25 +944,14 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "ResourcePolicy": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "PolicyRevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -1127,54 +1077,30 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredOutputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredOutputDataConfigOutputTypeDef",
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
-_OptionalOutputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalOutputDataConfigOutputTypeDef",
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
 
-class OutputDataConfigOutputTypeDef(
-    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
-):
-    pass
-
-
-_RequiredDocumentClassifierDocumentsOutputTypeDef = TypedDict(
-    "_RequiredDocumentClassifierDocumentsOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalDocumentClassifierDocumentsOutputTypeDef = TypedDict(
-    "_OptionalDocumentClassifierDocumentsOutputTypeDef",
-    {
-        "TestS3Uri": str,
-    },
-    total=False,
-)
-
-
-class DocumentClassifierDocumentsOutputTypeDef(
-    _RequiredDocumentClassifierDocumentsOutputTypeDef,
-    _OptionalDocumentClassifierDocumentsOutputTypeDef,
-):
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
 
 _RequiredDocumentClassifierDocumentsTypeDef = TypedDict(
     "_RequiredDocumentClassifierDocumentsTypeDef",
     {
         "S3Uri": str,
@@ -1224,24 +1150,14 @@
 
 class DocumentReaderConfigOutputTypeDef(
     _RequiredDocumentReaderConfigOutputTypeDef, _OptionalDocumentReaderConfigOutputTypeDef
 ):
     pass
 
 
-DocumentClassifierOutputDataConfigOutputTypeDef = TypedDict(
-    "DocumentClassifierOutputDataConfigOutputTypeDef",
-    {
-        "S3Uri": str,
-        "KmsKeyId": str,
-        "FlywheelStatsS3Prefix": str,
-    },
-    total=False,
-)
-
 DocumentClassifierSummaryTypeDef = TypedDict(
     "DocumentClassifierSummaryTypeDef",
     {
         "DocumentClassifierName": str,
         "NumberOfVersions": int,
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
@@ -1288,50 +1204,21 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-EntityTypesListItemOutputTypeDef = TypedDict(
-    "EntityTypesListItemOutputTypeDef",
-    {
-        "Type": str,
-    },
-)
-
 EntityTypesListItemTypeDef = TypedDict(
     "EntityTypesListItemTypeDef",
     {
         "Type": str,
     },
 )
 
-_RequiredEntityRecognizerAnnotationsOutputTypeDef = TypedDict(
-    "_RequiredEntityRecognizerAnnotationsOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalEntityRecognizerAnnotationsOutputTypeDef = TypedDict(
-    "_OptionalEntityRecognizerAnnotationsOutputTypeDef",
-    {
-        "TestS3Uri": str,
-    },
-    total=False,
-)
-
-
-class EntityRecognizerAnnotationsOutputTypeDef(
-    _RequiredEntityRecognizerAnnotationsOutputTypeDef,
-    _OptionalEntityRecognizerAnnotationsOutputTypeDef,
-):
-    pass
-
-
 _RequiredEntityRecognizerAnnotationsTypeDef = TypedDict(
     "_RequiredEntityRecognizerAnnotationsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalEntityRecognizerAnnotationsTypeDef = TypedDict(
@@ -1345,36 +1232,14 @@
 
 class EntityRecognizerAnnotationsTypeDef(
     _RequiredEntityRecognizerAnnotationsTypeDef, _OptionalEntityRecognizerAnnotationsTypeDef
 ):
     pass
 
 
-_RequiredEntityRecognizerDocumentsOutputTypeDef = TypedDict(
-    "_RequiredEntityRecognizerDocumentsOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalEntityRecognizerDocumentsOutputTypeDef = TypedDict(
-    "_OptionalEntityRecognizerDocumentsOutputTypeDef",
-    {
-        "TestS3Uri": str,
-        "InputFormat": InputFormatType,
-    },
-    total=False,
-)
-
-
-class EntityRecognizerDocumentsOutputTypeDef(
-    _RequiredEntityRecognizerDocumentsOutputTypeDef, _OptionalEntityRecognizerDocumentsOutputTypeDef
-):
-    pass
-
-
 _RequiredEntityRecognizerDocumentsTypeDef = TypedDict(
     "_RequiredEntityRecognizerDocumentsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalEntityRecognizerDocumentsTypeDef = TypedDict(
@@ -1389,21 +1254,14 @@
 
 class EntityRecognizerDocumentsTypeDef(
     _RequiredEntityRecognizerDocumentsTypeDef, _OptionalEntityRecognizerDocumentsTypeDef
 ):
     pass
 
 
-EntityRecognizerEntityListOutputTypeDef = TypedDict(
-    "EntityRecognizerEntityListOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-
 EntityRecognizerEntityListTypeDef = TypedDict(
     "EntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -1520,33 +1378,35 @@
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
-ImportModelResponseTypeDef = TypedDict(
-    "ImportModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
     "KeyPhrasesDetectionJobFilterTypeDef",
     {
         "JobName": str,
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ListDocumentClassifierSummariesRequestRequestTypeDef = TypedDict(
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1586,33 +1446,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-
 TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
     "TargetedSentimentDetectionJobFilterTypeDef",
     {
         "JobName": str,
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
@@ -1627,43 +1468,14 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredOutputDataConfigTypeDef = TypedDict(
-    "_RequiredOutputDataConfigTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalOutputDataConfigTypeDef = TypedDict(
-    "_OptionalOutputDataConfigTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
-    pass
-
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
 PartOfSpeechTagTypeDef = TypedDict(
     "PartOfSpeechTagTypeDef",
     {
         "Tag": PartOfSpeechTagTypeType,
         "Score": float,
     },
     total=False,
@@ -1718,346 +1530,396 @@
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "PolicyRevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RedactionConfigTypeDef = TypedDict(
     "RedactionConfigTypeDef",
     {
         "PiiEntityTypes": Sequence[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FlywheelArn": str,
     },
 )
+_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
 
-StartDocumentClassificationJobResponseTypeDef = TypedDict(
-    "StartDocumentClassificationJobResponseTypeDef",
+
+class StartFlywheelIterationRequestRequestTypeDef(
+    _RequiredStartFlywheelIterationRequestRequestTypeDef,
+    _OptionalStartFlywheelIterationRequestRequestTypeDef,
+):
+    pass
+
+
+StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StartDominantLanguageDetectionJobResponseTypeDef",
+StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionJobResponseTypeDef",
+StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEventsDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartEventsDetectionJobResponseTypeDef = TypedDict(
-    "StartEventsDetectionJobResponseTypeDef",
+StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
+StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     {
-        "FlywheelArn": str,
+        "JobId": str,
     },
 )
-_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
+
+StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopSentimentDetectionJobRequestRequestTypeDef",
     {
-        "ClientRequestToken": str,
+        "JobId": str,
+    },
+)
+
+StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+    {
+        "JobId": str,
+    },
+)
+
+StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+    {
+        "DocumentClassifierArn": str,
+    },
+)
+
+StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+    {
+        "EntityRecognizerArn": str,
+    },
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
+_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEndpointRequestRequestTypeDef",
+    {
+        "EndpointArn": str,
+    },
+)
+_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEndpointRequestRequestTypeDef",
+    {
+        "DesiredModelArn": str,
+        "DesiredInferenceUnits": int,
+        "DesiredDataAccessRoleArn": str,
+        "FlywheelArn": str,
     },
     total=False,
 )
 
 
-class StartFlywheelIterationRequestRequestTypeDef(
-    _RequiredStartFlywheelIterationRequestRequestTypeDef,
-    _OptionalStartFlywheelIterationRequestRequestTypeDef,
+class UpdateEndpointRequestRequestTypeDef(
+    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
 ):
     pass
 
 
-StartFlywheelIterationResponseTypeDef = TypedDict(
-    "StartFlywheelIterationResponseTypeDef",
+BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
+    "BatchDetectDominantLanguageItemResultTypeDef",
     {
-        "FlywheelArn": str,
-        "FlywheelIterationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Index": int,
+        "Languages": List[DominantLanguageTypeDef],
     },
+    total=False,
 )
 
-StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StartKeyPhrasesDetectionJobResponseTypeDef",
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartPiiEntitiesDetectionJobResponseTypeDef",
+CreateDocumentClassifierResponseTypeDef = TypedDict(
+    "CreateDocumentClassifierResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartSentimentDetectionJobResponseTypeDef",
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EndpointArn": str,
+        "ModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartTargetedSentimentDetectionJobResponseTypeDef",
+CreateEntityRecognizerResponseTypeDef = TypedDict(
+    "CreateEntityRecognizerResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EntityRecognizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTopicsDetectionJobResponseTypeDef = TypedDict(
-    "StartTopicsDetectionJobResponseTypeDef",
+CreateFlywheelResponseTypeDef = TypedDict(
+    "CreateFlywheelResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FlywheelArn": str,
+        "ActiveModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
     {
-        "JobId": str,
+        "ResourcePolicy": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobResponseTypeDef",
+DetectDominantLanguageResponseTypeDef = TypedDict(
+    "DetectDominantLanguageResponseTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Languages": List[DominantLanguageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
+ImportModelResponseTypeDef = TypedDict(
+    "ImportModelResponseTypeDef",
     {
-        "JobId": str,
+        "ModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionJobResponseTypeDef",
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEventsDetectionJobRequestRequestTypeDef",
+StartDocumentClassificationJobResponseTypeDef = TypedDict(
+    "StartDocumentClassificationJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEventsDetectionJobResponseTypeDef = TypedDict(
-    "StopEventsDetectionJobResponseTypeDef",
+StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StartDominantLanguageDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
+StartEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "EntityRecognizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobResponseTypeDef",
+StartEventsDetectionJobResponseTypeDef = TypedDict(
+    "StartEventsDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
+StartFlywheelIterationResponseTypeDef = TypedDict(
+    "StartFlywheelIterationResponseTypeDef",
     {
-        "JobId": str,
+        "FlywheelArn": str,
+        "FlywheelIterationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobResponseTypeDef",
+StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StartKeyPhrasesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopSentimentDetectionJobRequestRequestTypeDef",
+StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartPiiEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopSentimentDetectionJobResponseTypeDef",
+StartSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartTargetedSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobResponseTypeDef",
+StartTopicsDetectionJobResponseTypeDef = TypedDict(
+    "StartTopicsDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobResponseTypeDef",
     {
-        "DocumentClassifierArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+StopEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionJobResponseTypeDef",
     {
-        "EntityRecognizerArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StopEventsDetectionJobResponseTypeDef = TypedDict(
+    "StopEventsDetectionJobResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEndpointRequestRequestTypeDef",
+StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobResponseTypeDef",
     {
-        "EndpointArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEndpointRequestRequestTypeDef",
+
+StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobResponseTypeDef",
     {
-        "DesiredModelArn": str,
-        "DesiredInferenceUnits": int,
-        "DesiredDataAccessRoleArn": str,
-        "FlywheelArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateEndpointRequestRequestTypeDef(
-    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
-):
-    pass
-
-
-UpdateEndpointResponseTypeDef = TypedDict(
-    "UpdateEndpointResponseTypeDef",
+StopSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopSentimentDetectionJobResponseTypeDef",
     {
-        "DesiredModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
-    "BatchDetectDominantLanguageItemResultTypeDef",
+StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobResponseTypeDef",
     {
-        "Index": int,
-        "Languages": List[DominantLanguageTypeDef],
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-DetectDominantLanguageResponseTypeDef = TypedDict(
-    "DetectDominantLanguageResponseTypeDef",
+UpdateEndpointResponseTypeDef = TypedDict(
+    "UpdateEndpointResponseTypeDef",
     {
-        "Languages": List[DominantLanguageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DesiredModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectKeyPhrasesItemResultTypeDef = TypedDict(
     "BatchDetectKeyPhrasesItemResultTypeDef",
     {
         "Index": int,
@@ -2066,15 +1928,15 @@
     total=False,
 )
 
 DetectKeyPhrasesResponseTypeDef = TypedDict(
     "DetectKeyPhrasesResponseTypeDef",
     {
         "KeyPhrases": List[KeyPhraseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSentimentItemResultTypeDef = TypedDict(
     "BatchDetectSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -2085,15 +1947,15 @@
 )
 
 DetectSentimentResponseTypeDef = TypedDict(
     "DetectSentimentResponseTypeDef",
     {
         "Sentiment": SentimentTypeType,
         "SentimentScore": SentimentScoreTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MentionSentimentTypeDef = TypedDict(
     "MentionSentimentTypeDef",
     {
         "Sentiment": SentimentTypeType,
@@ -2179,15 +2041,15 @@
     pass
 
 
 ContainsPiiEntitiesResponseTypeDef = TypedDict(
     "ContainsPiiEntitiesResponseTypeDef",
     {
         "Labels": List[EntityLabelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
@@ -2234,14 +2096,23 @@
 
 class ImportModelRequestRequestTypeDef(
     _RequiredImportModelRequestRequestTypeDef, _OptionalImportModelRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2312,59 +2183,50 @@
     total=False,
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetProperties": DatasetPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "DatasetPropertiesList": List[DatasetPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "EndpointProperties": EndpointPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "EndpointPropertiesList": List[EndpointPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectPiiEntitiesResponseTypeDef = TypedDict(
     "DetectPiiEntitiesResponseTypeDef",
     {
         "Entities": List[PiiEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
     "ListDocumentClassificationJobsRequestRequestTypeDef",
     {
         "Filter": DocumentClassificationJobFilterTypeDef,
         "NextToken": str,
@@ -2384,23 +2246,14 @@
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
         "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
-    {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
     "ListDocumentClassifiersRequestRequestTypeDef",
     {
         "Filter": DocumentClassifierFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2412,15 +2265,15 @@
     {
         "DataFormat": DocumentClassifierDataFormatType,
         "S3Uri": str,
         "TestS3Uri": str,
         "LabelDelimiter": str,
         "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
-        "Documents": DocumentClassifierDocumentsOutputTypeDef,
+        "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredInputDataConfigOutputTypeDef = TypedDict(
     "_RequiredInputDataConfigOutputTypeDef",
@@ -2445,113 +2298,84 @@
 
 
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Pages": int,
         "ExtractedCharacters": List[ExtractedCharactersListItemTypeDef],
     },
     total=False,
 )
 
-ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
-    TypedDict(
-        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-        {
-            "Filter": DominantLanguageDetectionJobFilterTypeDef,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
     {
         "Filter": DominantLanguageDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    {
-        "Filter": EndpointFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEndpointsRequestRequestTypeDef = TypedDict(
     "ListEndpointsRequestRequestTypeDef",
     {
         "Filter": EndpointFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
     {
         "Filter": EntitiesDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 EntityRecognitionConfigOutputTypeDef = TypedDict(
     "EntityRecognitionConfigOutputTypeDef",
     {
-        "EntityTypes": List[EntityTypesListItemOutputTypeDef],
+        "EntityTypes": List[EntityTypesListItemTypeDef],
     },
 )
 
 EntityRecognitionConfigTypeDef = TypedDict(
     "EntityRecognitionConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 
 _RequiredEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
     "_RequiredEntityRecognizerInputDataConfigOutputTypeDef",
     {
-        "EntityTypes": List[EntityTypesListItemOutputTypeDef],
+        "EntityTypes": List[EntityTypesListItemTypeDef],
     },
 )
 _OptionalEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
     "_OptionalEntityRecognizerInputDataConfigOutputTypeDef",
     {
         "DataFormat": EntityRecognizerDataFormatType,
-        "Documents": EntityRecognizerDocumentsOutputTypeDef,
-        "Annotations": EntityRecognizerAnnotationsOutputTypeDef,
-        "EntityList": EntityRecognizerEntityListOutputTypeDef,
+        "Documents": EntityRecognizerDocumentsTypeDef,
+        "Annotations": EntityRecognizerAnnotationsTypeDef,
+        "EntityList": EntityRecognizerEntityListTypeDef,
         "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
     },
     total=False,
 )
 
 
 class EntityRecognizerInputDataConfigOutputTypeDef(
@@ -2582,23 +2406,14 @@
 
 class EntityRecognizerInputDataConfigTypeDef(
     _RequiredEntityRecognizerInputDataConfigTypeDef, _OptionalEntityRecognizerInputDataConfigTypeDef
 ):
     pass
 
 
-ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEntityRecognizersRequestRequestTypeDef = TypedDict(
     "ListEntityRecognizersRequestRequestTypeDef",
     {
         "Filter": EntityRecognizerFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2616,15 +2431,15 @@
 )
 
 ListEntityRecognizerSummariesResponseTypeDef = TypedDict(
     "ListEntityRecognizerSummariesResponseTypeDef",
     {
         "EntityRecognizerSummariesList": List[EntityRecognizerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListEventsDetectionJobsRequestRequestTypeDef",
     {
         "Filter": EventsDetectionJobFilterTypeDef,
@@ -2687,51 +2502,107 @@
 )
 
 ListFlywheelsResponseTypeDef = TypedDict(
     "ListFlywheelsResponseTypeDef",
     {
         "FlywheelSummaryList": List[FlywheelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
     {
         "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
-ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
+    TypedDict(
+        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+        {
+            "Filter": DominantLanguageDetectionJobFilterTypeDef,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     {
         "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     {
         "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     {
@@ -2742,53 +2613,44 @@
     total=False,
 )
 
 ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     {
         "Filter": SentimentDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListSentimentDetectionJobsRequestRequestTypeDef",
     {
         "Filter": SentimentDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     {
         "Filter": TargetedSentimentDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     {
         "Filter": TopicsDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     {
@@ -2812,33 +2674,33 @@
 )
 
 BatchDetectDominantLanguageResponseTypeDef = TypedDict(
     "BatchDetectDominantLanguageResponseTypeDef",
     {
         "ResultList": List[BatchDetectDominantLanguageItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectKeyPhrasesResponseTypeDef = TypedDict(
     "BatchDetectKeyPhrasesResponseTypeDef",
     {
         "ResultList": List[BatchDetectKeyPhrasesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSentimentResponseTypeDef = TypedDict(
     "BatchDetectSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetedSentimentMentionTypeDef = TypedDict(
     "TargetedSentimentMentionTypeDef",
     {
         "Score": float,
@@ -3202,15 +3064,15 @@
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
         "InputDataConfig": DocumentClassifierInputDataConfigOutputTypeDef,
-        "OutputDataConfig": DocumentClassifierOutputDataConfigOutputTypeDef,
+        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
         "ClassifierMetadata": ClassifierMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "VersionName": str,
@@ -3228,15 +3090,15 @@
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "DocumentClassifierArn": str,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
         "FlywheelArn": str,
     },
     total=False,
 )
@@ -3248,15 +3110,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
@@ -3268,15 +3130,15 @@
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "EntityRecognizerArn": str,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
         "FlywheelArn": str,
     },
     total=False,
@@ -3289,15 +3151,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "TargetEventTypes": List[str],
     },
     total=False,
 )
 
@@ -3308,15 +3170,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
@@ -3348,15 +3210,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
@@ -3368,15 +3230,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
@@ -3388,15 +3250,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "NumberOfTopics": int,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
@@ -3406,15 +3268,15 @@
     {
         "Classes": List[DocumentClassTypeDef],
         "Labels": List[DocumentLabelTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
         "Warnings": List[WarningsListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTaskConfigOutputTypeDef = TypedDict(
     "_RequiredTaskConfigOutputTypeDef",
     {
         "LanguageCode": LanguageCodeType,
@@ -3496,24 +3358,24 @@
     total=False,
 )
 
 DescribeFlywheelIterationResponseTypeDef = TypedDict(
     "DescribeFlywheelIterationResponseTypeDef",
     {
         "FlywheelIterationProperties": FlywheelIterationPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFlywheelIterationHistoryResponseTypeDef = TypedDict(
     "ListFlywheelIterationHistoryResponseTypeDef",
     {
         "FlywheelIterationPropertiesList": List[FlywheelIterationPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
         "Id": str,
@@ -3535,15 +3397,15 @@
     total=False,
 )
 
 DetectSyntaxResponseTypeDef = TypedDict(
     "DetectSyntaxResponseTypeDef",
     {
         "SyntaxTokens": List[SyntaxTokenTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetedSentimentEntityTypeDef = TypedDict(
     "TargetedSentimentEntityTypeDef",
     {
         "DescriptiveMentionIndex": List[int],
@@ -3587,181 +3449,181 @@
     pass
 
 
 DescribeDocumentClassifierResponseTypeDef = TypedDict(
     "DescribeDocumentClassifierResponseTypeDef",
     {
         "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDocumentClassifiersResponseTypeDef = TypedDict(
     "ListDocumentClassifiersResponseTypeDef",
     {
         "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDocumentClassificationJobResponseTypeDef = TypedDict(
     "DescribeDocumentClassificationJobResponseTypeDef",
     {
         "DocumentClassificationJobProperties": DocumentClassificationJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDocumentClassificationJobsResponseTypeDef = TypedDict(
     "ListDocumentClassificationJobsResponseTypeDef",
     {
         "DocumentClassificationJobPropertiesList": List[DocumentClassificationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDominantLanguageDetectionJobResponseTypeDef = TypedDict(
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     {
         "DominantLanguageDetectionJobProperties": DominantLanguageDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDominantLanguageDetectionJobsResponseTypeDef = TypedDict(
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     {
         "DominantLanguageDetectionJobPropertiesList": List[
             DominantLanguageDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionJobResponseTypeDef",
     {
         "EntitiesDetectionJobProperties": EntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionJobsResponseTypeDef",
     {
         "EntitiesDetectionJobPropertiesList": List[EntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsDetectionJobResponseTypeDef = TypedDict(
     "DescribeEventsDetectionJobResponseTypeDef",
     {
         "EventsDetectionJobProperties": EventsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventsDetectionJobsResponseTypeDef = TypedDict(
     "ListEventsDetectionJobsResponseTypeDef",
     {
         "EventsDetectionJobPropertiesList": List[EventsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
     "DescribeKeyPhrasesDetectionJobResponseTypeDef",
     {
         "KeyPhrasesDetectionJobProperties": KeyPhrasesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKeyPhrasesDetectionJobsResponseTypeDef = TypedDict(
     "ListKeyPhrasesDetectionJobsResponseTypeDef",
     {
         "KeyPhrasesDetectionJobPropertiesList": List[KeyPhrasesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePiiEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribePiiEntitiesDetectionJobResponseTypeDef",
     {
         "PiiEntitiesDetectionJobProperties": PiiEntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPiiEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     {
         "PiiEntitiesDetectionJobPropertiesList": List[PiiEntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeSentimentDetectionJobResponseTypeDef",
     {
         "SentimentDetectionJobProperties": SentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListSentimentDetectionJobsResponseTypeDef",
     {
         "SentimentDetectionJobPropertiesList": List[SentimentDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     {
         "TargetedSentimentDetectionJobProperties": TargetedSentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetedSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     {
         "TargetedSentimentDetectionJobPropertiesList": List[
             TargetedSentimentDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTopicsDetectionJobResponseTypeDef = TypedDict(
     "DescribeTopicsDetectionJobResponseTypeDef",
     {
         "TopicsDetectionJobProperties": TopicsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTopicsDetectionJobsResponseTypeDef = TypedDict(
     "ListTopicsDetectionJobsResponseTypeDef",
     {
         "TopicsDetectionJobPropertiesList": List[TopicsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FlywheelPropertiesTypeDef = TypedDict(
     "FlywheelPropertiesTypeDef",
     {
         "FlywheelArn": str,
@@ -3837,24 +3699,24 @@
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Blocks": List[BlockTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSyntaxResponseTypeDef = TypedDict(
     "BatchDetectSyntaxResponseTypeDef",
     {
         "ResultList": List[BatchDetectSyntaxItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectTargetedSentimentItemResultTypeDef = TypedDict(
     "BatchDetectTargetedSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -3863,61 +3725,61 @@
     total=False,
 )
 
 DetectTargetedSentimentResponseTypeDef = TypedDict(
     "DetectTargetedSentimentResponseTypeDef",
     {
         "Entities": List[TargetedSentimentEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectEntitiesResponseTypeDef = TypedDict(
     "BatchDetectEntitiesResponseTypeDef",
     {
         "ResultList": List[BatchDetectEntitiesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFlywheelResponseTypeDef = TypedDict(
     "DescribeFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlywheelResponseTypeDef = TypedDict(
     "UpdateFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntityRecognizerResponseTypeDef = TypedDict(
     "DescribeEntityRecognizerResponseTypeDef",
     {
         "EntityRecognizerProperties": EntityRecognizerPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntityRecognizersResponseTypeDef = TypedDict(
     "ListEntityRecognizersResponseTypeDef",
     {
         "EntityRecognizerPropertiesList": List[EntityRecognizerPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectTargetedSentimentResponseTypeDef = TypedDict(
     "BatchDetectTargetedSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectTargetedSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend/type_defs.pyi` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
 __all__ = (
     "AugmentedManifestsListItemOutputTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
     "BatchDetectKeyPhrasesRequestRequestTypeDef",
     "SentimentScoreTypeDef",
     "BatchDetectSentimentRequestRequestTypeDef",
     "BatchDetectSyntaxRequestRequestTypeDef",
     "BatchDetectTargetedSentimentRequestRequestTypeDef",
@@ -83,21 +84,16 @@
     "DocumentLabelTypeDef",
     "DocumentTypeListItemTypeDef",
     "ErrorsListItemTypeDef",
     "WarningsListItemTypeDef",
     "ContainsPiiEntitiesRequestRequestTypeDef",
     "EntityLabelTypeDef",
     "TagTypeDef",
-    "CreateDatasetResponseTypeDef",
     "DocumentClassifierOutputDataConfigTypeDef",
     "VpcConfigTypeDef",
-    "CreateDocumentClassifierResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
-    "CreateEntityRecognizerResponseTypeDef",
-    "CreateFlywheelResponseTypeDef",
     "VpcConfigOutputTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
     "DatasetFilterTypeDef",
@@ -117,169 +113,165 @@
     "DescribeEntityRecognizerRequestRequestTypeDef",
     "DescribeEventsDetectionJobRequestRequestTypeDef",
     "DescribeFlywheelIterationRequestRequestTypeDef",
     "DescribeFlywheelRequestRequestTypeDef",
     "DescribeKeyPhrasesDetectionJobRequestRequestTypeDef",
     "DescribePiiEntitiesDetectionJobRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTargetedSentimentDetectionJobRequestRequestTypeDef",
     "DescribeTopicsDetectionJobRequestRequestTypeDef",
     "DetectDominantLanguageRequestRequestTypeDef",
     "DetectKeyPhrasesRequestRequestTypeDef",
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
     "DocumentClassificationConfigOutputTypeDef",
     "DocumentClassificationConfigTypeDef",
     "DocumentClassificationJobFilterTypeDef",
-    "OutputDataConfigOutputTypeDef",
-    "DocumentClassifierDocumentsOutputTypeDef",
+    "OutputDataConfigTypeDef",
     "DocumentClassifierDocumentsTypeDef",
     "DocumentClassifierFilterTypeDef",
     "DocumentReaderConfigOutputTypeDef",
-    "DocumentClassifierOutputDataConfigOutputTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
     "DominantLanguageDetectionJobFilterTypeDef",
     "EndpointFilterTypeDef",
     "EntitiesDetectionJobFilterTypeDef",
-    "EntityTypesListItemOutputTypeDef",
     "EntityTypesListItemTypeDef",
-    "EntityRecognizerAnnotationsOutputTypeDef",
     "EntityRecognizerAnnotationsTypeDef",
-    "EntityRecognizerDocumentsOutputTypeDef",
     "EntityRecognizerDocumentsTypeDef",
-    "EntityRecognizerEntityListOutputTypeDef",
     "EntityRecognizerEntityListTypeDef",
     "EntityRecognizerEvaluationMetricsTypeDef",
     "EntityRecognizerFilterTypeDef",
     "EntityTypesEvaluationMetricsTypeDef",
     "EntityRecognizerOutputDataConfigTypeDef",
     "EntityRecognizerSummaryTypeDef",
     "EventsDetectionJobFilterTypeDef",
     "FlywheelFilterTypeDef",
     "FlywheelIterationFilterTypeDef",
     "FlywheelModelEvaluationMetricsTypeDef",
     "FlywheelSummaryTypeDef",
     "PointTypeDef",
-    "ImportModelResponseTypeDef",
     "KeyPhrasesDetectionJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
     "PiiEntitiesDetectionJobFilterTypeDef",
     "SentimentDetectionJobFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "TargetedSentimentDetectionJobFilterTypeDef",
     "TopicsDetectionJobFilterTypeDef",
-    "OutputDataConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
     "RedactionConfigOutputTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
     "RedactionConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "StartFlywheelIterationRequestRequestTypeDef",
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
+    "StopEventsDetectionJobRequestRequestTypeDef",
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
+    "StopSentimentDetectionJobRequestRequestTypeDef",
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "UpdateEndpointRequestRequestTypeDef",
+    "BatchDetectDominantLanguageItemResultTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateDocumentClassifierResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
+    "CreateEntityRecognizerResponseTypeDef",
+    "CreateFlywheelResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "DetectDominantLanguageResponseTypeDef",
+    "ImportModelResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
     "StartDocumentClassificationJobResponseTypeDef",
     "StartDominantLanguageDetectionJobResponseTypeDef",
     "StartEntitiesDetectionJobResponseTypeDef",
     "StartEventsDetectionJobResponseTypeDef",
-    "StartFlywheelIterationRequestRequestTypeDef",
     "StartFlywheelIterationResponseTypeDef",
     "StartKeyPhrasesDetectionJobResponseTypeDef",
     "StartPiiEntitiesDetectionJobResponseTypeDef",
     "StartSentimentDetectionJobResponseTypeDef",
     "StartTargetedSentimentDetectionJobResponseTypeDef",
     "StartTopicsDetectionJobResponseTypeDef",
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     "StopDominantLanguageDetectionJobResponseTypeDef",
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
     "StopEntitiesDetectionJobResponseTypeDef",
-    "StopEventsDetectionJobRequestRequestTypeDef",
     "StopEventsDetectionJobResponseTypeDef",
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StopKeyPhrasesDetectionJobResponseTypeDef",
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StopPiiEntitiesDetectionJobResponseTypeDef",
-    "StopSentimentDetectionJobRequestRequestTypeDef",
     "StopSentimentDetectionJobResponseTypeDef",
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StopTargetedSentimentDetectionJobResponseTypeDef",
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
-    "BatchDetectDominantLanguageItemResultTypeDef",
-    "DetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesItemResultTypeDef",
     "DetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentItemResultTypeDef",
     "DetectSentimentResponseTypeDef",
     "MentionSentimentTypeDef",
     "BlockReferenceTypeDef",
     "ClassifierMetadataTypeDef",
     "ClassifyDocumentRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "ContainsPiiEntitiesResponseTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "ImportModelRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DataSecurityConfigTypeDef",
     "UpdateDataSecurityConfigTypeDef",
     "DataSecurityConfigOutputTypeDef",
     "DatasetEntityRecognizerInputDataConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
     "ListDocumentClassificationJobsRequestRequestTypeDef",
     "DocumentClassifierInputDataConfigTypeDef",
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
     "ListDocumentClassifiersRequestRequestTypeDef",
     "DocumentClassifierInputDataConfigOutputTypeDef",
     "InputDataConfigOutputTypeDef",
     "ListDocumentClassifierSummariesResponseTypeDef",
     "DocumentMetadataTypeDef",
-    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
     "ListEndpointsRequestRequestTypeDef",
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
     "EntityRecognitionConfigOutputTypeDef",
     "EntityRecognitionConfigTypeDef",
     "EntityRecognizerInputDataConfigOutputTypeDef",
     "EntityRecognizerInputDataConfigTypeDef",
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
     "ListEntityRecognizersRequestRequestTypeDef",
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     "ListEntityRecognizerSummariesResponseTypeDef",
     "ListEventsDetectionJobsRequestRequestTypeDef",
     "ListFlywheelsRequestRequestTypeDef",
     "ListFlywheelIterationHistoryRequestRequestTypeDef",
     "FlywheelIterationPropertiesTypeDef",
     "ListFlywheelsResponseTypeDef",
     "GeometryTypeDef",
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     "ListSentimentDetectionJobsRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     "SyntaxTokenTypeDef",
     "BatchDetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentResponseTypeDef",
@@ -424,14 +416,25 @@
         "Index": int,
         "ErrorCode": str,
         "ErrorMessage": str,
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
 BatchDetectEntitiesRequestRequestTypeDef = TypedDict(
     "BatchDetectEntitiesRequestRequestTypeDef",
     {
         "TextList": Sequence[str],
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -634,22 +637,14 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DocumentClassifierOutputDataConfigTypeDef = TypedDict(
     "DocumentClassifierOutputDataConfigTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
         "FlywheelStatsS3Prefix": str,
     },
@@ -660,48 +655,14 @@
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
 
-CreateDocumentClassifierResponseTypeDef = TypedDict(
-    "CreateDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
-    {
-        "EndpointArn": str,
-        "ModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEntityRecognizerResponseTypeDef = TypedDict(
-    "CreateEntityRecognizerResponseTypeDef",
-    {
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFlywheelResponseTypeDef = TypedDict(
-    "CreateFlywheelResponseTypeDef",
-    {
-        "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VpcConfigOutputTypeDef = TypedDict(
     "VpcConfigOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "Subnets": List[str],
     },
 )
@@ -966,25 +927,14 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "ResourcePolicy": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "PolicyRevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSentimentDetectionJobRequestRequestTypeDef = TypedDict(
     "DescribeSentimentDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -1106,51 +1056,29 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredOutputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredOutputDataConfigOutputTypeDef",
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
-_OptionalOutputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalOutputDataConfigOutputTypeDef",
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-class OutputDataConfigOutputTypeDef(
-    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
-):
-    pass
-
-_RequiredDocumentClassifierDocumentsOutputTypeDef = TypedDict(
-    "_RequiredDocumentClassifierDocumentsOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalDocumentClassifierDocumentsOutputTypeDef = TypedDict(
-    "_OptionalDocumentClassifierDocumentsOutputTypeDef",
-    {
-        "TestS3Uri": str,
-    },
-    total=False,
-)
-
-class DocumentClassifierDocumentsOutputTypeDef(
-    _RequiredDocumentClassifierDocumentsOutputTypeDef,
-    _OptionalDocumentClassifierDocumentsOutputTypeDef,
-):
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
 _RequiredDocumentClassifierDocumentsTypeDef = TypedDict(
     "_RequiredDocumentClassifierDocumentsTypeDef",
     {
         "S3Uri": str,
     },
@@ -1195,24 +1123,14 @@
 )
 
 class DocumentReaderConfigOutputTypeDef(
     _RequiredDocumentReaderConfigOutputTypeDef, _OptionalDocumentReaderConfigOutputTypeDef
 ):
     pass
 
-DocumentClassifierOutputDataConfigOutputTypeDef = TypedDict(
-    "DocumentClassifierOutputDataConfigOutputTypeDef",
-    {
-        "S3Uri": str,
-        "KmsKeyId": str,
-        "FlywheelStatsS3Prefix": str,
-    },
-    total=False,
-)
-
 DocumentClassifierSummaryTypeDef = TypedDict(
     "DocumentClassifierSummaryTypeDef",
     {
         "DocumentClassifierName": str,
         "NumberOfVersions": int,
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
@@ -1259,48 +1177,21 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-EntityTypesListItemOutputTypeDef = TypedDict(
-    "EntityTypesListItemOutputTypeDef",
-    {
-        "Type": str,
-    },
-)
-
 EntityTypesListItemTypeDef = TypedDict(
     "EntityTypesListItemTypeDef",
     {
         "Type": str,
     },
 )
 
-_RequiredEntityRecognizerAnnotationsOutputTypeDef = TypedDict(
-    "_RequiredEntityRecognizerAnnotationsOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalEntityRecognizerAnnotationsOutputTypeDef = TypedDict(
-    "_OptionalEntityRecognizerAnnotationsOutputTypeDef",
-    {
-        "TestS3Uri": str,
-    },
-    total=False,
-)
-
-class EntityRecognizerAnnotationsOutputTypeDef(
-    _RequiredEntityRecognizerAnnotationsOutputTypeDef,
-    _OptionalEntityRecognizerAnnotationsOutputTypeDef,
-):
-    pass
-
 _RequiredEntityRecognizerAnnotationsTypeDef = TypedDict(
     "_RequiredEntityRecognizerAnnotationsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalEntityRecognizerAnnotationsTypeDef = TypedDict(
@@ -1312,34 +1203,14 @@
 )
 
 class EntityRecognizerAnnotationsTypeDef(
     _RequiredEntityRecognizerAnnotationsTypeDef, _OptionalEntityRecognizerAnnotationsTypeDef
 ):
     pass
 
-_RequiredEntityRecognizerDocumentsOutputTypeDef = TypedDict(
-    "_RequiredEntityRecognizerDocumentsOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalEntityRecognizerDocumentsOutputTypeDef = TypedDict(
-    "_OptionalEntityRecognizerDocumentsOutputTypeDef",
-    {
-        "TestS3Uri": str,
-        "InputFormat": InputFormatType,
-    },
-    total=False,
-)
-
-class EntityRecognizerDocumentsOutputTypeDef(
-    _RequiredEntityRecognizerDocumentsOutputTypeDef, _OptionalEntityRecognizerDocumentsOutputTypeDef
-):
-    pass
-
 _RequiredEntityRecognizerDocumentsTypeDef = TypedDict(
     "_RequiredEntityRecognizerDocumentsTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalEntityRecognizerDocumentsTypeDef = TypedDict(
@@ -1352,21 +1223,14 @@
 )
 
 class EntityRecognizerDocumentsTypeDef(
     _RequiredEntityRecognizerDocumentsTypeDef, _OptionalEntityRecognizerDocumentsTypeDef
 ):
     pass
 
-EntityRecognizerEntityListOutputTypeDef = TypedDict(
-    "EntityRecognizerEntityListOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-
 EntityRecognizerEntityListTypeDef = TypedDict(
     "EntityRecognizerEntityListTypeDef",
     {
         "S3Uri": str,
     },
 )
 
@@ -1483,33 +1347,35 @@
     {
         "X": float,
         "Y": float,
     },
     total=False,
 )
 
-ImportModelResponseTypeDef = TypedDict(
-    "ImportModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 KeyPhrasesDetectionJobFilterTypeDef = TypedDict(
     "KeyPhrasesDetectionJobFilterTypeDef",
     {
         "JobName": str,
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ListDocumentClassifierSummariesRequestRequestTypeDef = TypedDict(
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1549,31 +1415,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
 TargetedSentimentDetectionJobFilterTypeDef = TypedDict(
     "TargetedSentimentDetectionJobFilterTypeDef",
     {
         "JobName": str,
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
@@ -1588,41 +1437,14 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredOutputDataConfigTypeDef = TypedDict(
-    "_RequiredOutputDataConfigTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalOutputDataConfigTypeDef = TypedDict(
-    "_OptionalOutputDataConfigTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
-    pass
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
 PartOfSpeechTagTypeDef = TypedDict(
     "PartOfSpeechTagTypeDef",
     {
         "Tag": PartOfSpeechTagTypeType,
         "Score": float,
     },
     total=False,
@@ -1673,342 +1495,392 @@
 )
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "PolicyRevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RedactionConfigTypeDef = TypedDict(
     "RedactionConfigTypeDef",
     {
         "PiiEntityTypes": Sequence[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "FlywheelArn": str,
     },
 )
+_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
 
-StartDocumentClassificationJobResponseTypeDef = TypedDict(
-    "StartDocumentClassificationJobResponseTypeDef",
+class StartFlywheelIterationRequestRequestTypeDef(
+    _RequiredStartFlywheelIterationRequestRequestTypeDef,
+    _OptionalStartFlywheelIterationRequestRequestTypeDef,
+):
+    pass
+
+StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "DocumentClassifierArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StartDominantLanguageDetectionJobResponseTypeDef",
+StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEntitiesDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionJobResponseTypeDef",
+StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopEventsDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "EntityRecognizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartEventsDetectionJobResponseTypeDef = TypedDict(
-    "StartEventsDetectionJobResponseTypeDef",
+StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFlywheelIterationRequestRequestTypeDef",
+StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     {
-        "FlywheelArn": str,
+        "JobId": str,
     },
 )
-_OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFlywheelIterationRequestRequestTypeDef",
+
+StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopSentimentDetectionJobRequestRequestTypeDef",
     {
-        "ClientRequestToken": str,
+        "JobId": str,
+    },
+)
+
+StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+    {
+        "JobId": str,
+    },
+)
+
+StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
+    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+    {
+        "DocumentClassifierArn": str,
+    },
+)
+
+StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
+    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+    {
+        "EntityRecognizerArn": str,
+    },
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
+_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEndpointRequestRequestTypeDef",
+    {
+        "EndpointArn": str,
+    },
+)
+_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEndpointRequestRequestTypeDef",
+    {
+        "DesiredModelArn": str,
+        "DesiredInferenceUnits": int,
+        "DesiredDataAccessRoleArn": str,
+        "FlywheelArn": str,
     },
     total=False,
 )
 
-class StartFlywheelIterationRequestRequestTypeDef(
-    _RequiredStartFlywheelIterationRequestRequestTypeDef,
-    _OptionalStartFlywheelIterationRequestRequestTypeDef,
+class UpdateEndpointRequestRequestTypeDef(
+    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
 ):
     pass
 
-StartFlywheelIterationResponseTypeDef = TypedDict(
-    "StartFlywheelIterationResponseTypeDef",
+BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
+    "BatchDetectDominantLanguageItemResultTypeDef",
     {
-        "FlywheelArn": str,
-        "FlywheelIterationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Index": int,
+        "Languages": List[DominantLanguageTypeDef],
     },
+    total=False,
 )
 
-StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StartKeyPhrasesDetectionJobResponseTypeDef",
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StartPiiEntitiesDetectionJobResponseTypeDef",
+CreateDocumentClassifierResponseTypeDef = TypedDict(
+    "CreateDocumentClassifierResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartSentimentDetectionJobResponseTypeDef",
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EndpointArn": str,
+        "ModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StartTargetedSentimentDetectionJobResponseTypeDef",
+CreateEntityRecognizerResponseTypeDef = TypedDict(
+    "CreateEntityRecognizerResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EntityRecognizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTopicsDetectionJobResponseTypeDef = TypedDict(
-    "StartTopicsDetectionJobResponseTypeDef",
+CreateFlywheelResponseTypeDef = TypedDict(
+    "CreateFlywheelResponseTypeDef",
     {
-        "JobId": str,
-        "JobArn": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FlywheelArn": str,
+        "ActiveModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDominantLanguageDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobRequestRequestTypeDef",
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
     {
-        "JobId": str,
+        "ResourcePolicy": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
-    "StopDominantLanguageDetectionJobResponseTypeDef",
+DetectDominantLanguageResponseTypeDef = TypedDict(
+    "DetectDominantLanguageResponseTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Languages": List[DominantLanguageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEntitiesDetectionJobRequestRequestTypeDef",
+ImportModelResponseTypeDef = TypedDict(
+    "ImportModelResponseTypeDef",
     {
-        "JobId": str,
+        "ModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionJobResponseTypeDef",
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEventsDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopEventsDetectionJobRequestRequestTypeDef",
+StartDocumentClassificationJobResponseTypeDef = TypedDict(
+    "StartDocumentClassificationJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "DocumentClassifierArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopEventsDetectionJobResponseTypeDef = TypedDict(
-    "StopEventsDetectionJobResponseTypeDef",
+StartDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StartDominantLanguageDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopKeyPhrasesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
+StartEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "EntityRecognizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
-    "StopKeyPhrasesDetectionJobResponseTypeDef",
+StartEventsDetectionJobResponseTypeDef = TypedDict(
+    "StartEventsDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopPiiEntitiesDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
+StartFlywheelIterationResponseTypeDef = TypedDict(
+    "StartFlywheelIterationResponseTypeDef",
     {
-        "JobId": str,
+        "FlywheelArn": str,
+        "FlywheelIterationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
-    "StopPiiEntitiesDetectionJobResponseTypeDef",
+StartKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StartKeyPhrasesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopSentimentDetectionJobRequestRequestTypeDef",
+StartPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StartPiiEntitiesDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopSentimentDetectionJobResponseTypeDef",
+StartSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTargetedSentimentDetectionJobRequestRequestTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobRequestRequestTypeDef",
+StartTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StartTargetedSentimentDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
-    "StopTargetedSentimentDetectionJobResponseTypeDef",
+StartTopicsDetectionJobResponseTypeDef = TypedDict(
+    "StartTopicsDetectionJobResponseTypeDef",
     {
         "JobId": str,
+        "JobArn": str,
         "JobStatus": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTrainingDocumentClassifierRequestRequestTypeDef = TypedDict(
-    "StopTrainingDocumentClassifierRequestRequestTypeDef",
+StopDominantLanguageDetectionJobResponseTypeDef = TypedDict(
+    "StopDominantLanguageDetectionJobResponseTypeDef",
     {
-        "DocumentClassifierArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopTrainingEntityRecognizerRequestRequestTypeDef = TypedDict(
-    "StopTrainingEntityRecognizerRequestRequestTypeDef",
+StopEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionJobResponseTypeDef",
     {
-        "EntityRecognizerArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StopEventsDetectionJobResponseTypeDef = TypedDict(
+    "StopEventsDetectionJobResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEndpointRequestRequestTypeDef",
+StopKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
+    "StopKeyPhrasesDetectionJobResponseTypeDef",
     {
-        "EndpointArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEndpointRequestRequestTypeDef",
+
+StopPiiEntitiesDetectionJobResponseTypeDef = TypedDict(
+    "StopPiiEntitiesDetectionJobResponseTypeDef",
     {
-        "DesiredModelArn": str,
-        "DesiredInferenceUnits": int,
-        "DesiredDataAccessRoleArn": str,
-        "FlywheelArn": str,
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateEndpointRequestRequestTypeDef(
-    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
-):
-    pass
-
-UpdateEndpointResponseTypeDef = TypedDict(
-    "UpdateEndpointResponseTypeDef",
+StopSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopSentimentDetectionJobResponseTypeDef",
     {
-        "DesiredModelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDetectDominantLanguageItemResultTypeDef = TypedDict(
-    "BatchDetectDominantLanguageItemResultTypeDef",
+StopTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
+    "StopTargetedSentimentDetectionJobResponseTypeDef",
     {
-        "Index": int,
-        "Languages": List[DominantLanguageTypeDef],
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-DetectDominantLanguageResponseTypeDef = TypedDict(
-    "DetectDominantLanguageResponseTypeDef",
+UpdateEndpointResponseTypeDef = TypedDict(
+    "UpdateEndpointResponseTypeDef",
     {
-        "Languages": List[DominantLanguageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DesiredModelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectKeyPhrasesItemResultTypeDef = TypedDict(
     "BatchDetectKeyPhrasesItemResultTypeDef",
     {
         "Index": int,
@@ -2017,15 +1889,15 @@
     total=False,
 )
 
 DetectKeyPhrasesResponseTypeDef = TypedDict(
     "DetectKeyPhrasesResponseTypeDef",
     {
         "KeyPhrases": List[KeyPhraseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSentimentItemResultTypeDef = TypedDict(
     "BatchDetectSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -2036,15 +1908,15 @@
 )
 
 DetectSentimentResponseTypeDef = TypedDict(
     "DetectSentimentResponseTypeDef",
     {
         "Sentiment": SentimentTypeType,
         "SentimentScore": SentimentScoreTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MentionSentimentTypeDef = TypedDict(
     "MentionSentimentTypeDef",
     {
         "Sentiment": SentimentTypeType,
@@ -2126,15 +1998,15 @@
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
 ContainsPiiEntitiesResponseTypeDef = TypedDict(
     "ContainsPiiEntitiesResponseTypeDef",
     {
         "Labels": List[EntityLabelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
@@ -2177,14 +2049,23 @@
 )
 
 class ImportModelRequestRequestTypeDef(
     _RequiredImportModelRequestRequestTypeDef, _OptionalImportModelRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2253,61 +2134,52 @@
     total=False,
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetProperties": DatasetPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "DatasetPropertiesList": List[DatasetPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "EndpointProperties": EndpointPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "EndpointPropertiesList": List[EndpointPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectPiiEntitiesResponseTypeDef = TypedDict(
     "DetectPiiEntitiesResponseTypeDef",
     {
         "Entities": List[PiiEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
-    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
-    {
-        "Filter": DocumentClassificationJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDocumentClassificationJobsRequestRequestTypeDef = TypedDict(
     "ListDocumentClassificationJobsRequestRequestTypeDef",
     {
         "Filter": DocumentClassificationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2325,23 +2197,14 @@
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
         "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
-    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
-    {
-        "Filter": DocumentClassifierFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDocumentClassifiersRequestRequestTypeDef = TypedDict(
     "ListDocumentClassifiersRequestRequestTypeDef",
     {
         "Filter": DocumentClassifierFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2353,15 +2216,15 @@
     {
         "DataFormat": DocumentClassifierDataFormatType,
         "S3Uri": str,
         "TestS3Uri": str,
         "LabelDelimiter": str,
         "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
-        "Documents": DocumentClassifierDocumentsOutputTypeDef,
+        "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredInputDataConfigOutputTypeDef = TypedDict(
     "_RequiredInputDataConfigOutputTypeDef",
@@ -2384,113 +2247,84 @@
     pass
 
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Pages": int,
         "ExtractedCharacters": List[ExtractedCharactersListItemTypeDef],
     },
     total=False,
 )
 
-ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
-    TypedDict(
-        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
-        {
-            "Filter": DominantLanguageDetectionJobFilterTypeDef,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 ListDominantLanguageDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListDominantLanguageDetectionJobsRequestRequestTypeDef",
     {
         "Filter": DominantLanguageDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
-    "ListEndpointsRequestListEndpointsPaginateTypeDef",
-    {
-        "Filter": EndpointFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEndpointsRequestRequestTypeDef = TypedDict(
     "ListEndpointsRequestRequestTypeDef",
     {
         "Filter": EndpointFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
-    {
-        "Filter": EntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListEntitiesDetectionJobsRequestRequestTypeDef",
     {
         "Filter": EntitiesDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 EntityRecognitionConfigOutputTypeDef = TypedDict(
     "EntityRecognitionConfigOutputTypeDef",
     {
-        "EntityTypes": List[EntityTypesListItemOutputTypeDef],
+        "EntityTypes": List[EntityTypesListItemTypeDef],
     },
 )
 
 EntityRecognitionConfigTypeDef = TypedDict(
     "EntityRecognitionConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 
 _RequiredEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
     "_RequiredEntityRecognizerInputDataConfigOutputTypeDef",
     {
-        "EntityTypes": List[EntityTypesListItemOutputTypeDef],
+        "EntityTypes": List[EntityTypesListItemTypeDef],
     },
 )
 _OptionalEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
     "_OptionalEntityRecognizerInputDataConfigOutputTypeDef",
     {
         "DataFormat": EntityRecognizerDataFormatType,
-        "Documents": EntityRecognizerDocumentsOutputTypeDef,
-        "Annotations": EntityRecognizerAnnotationsOutputTypeDef,
-        "EntityList": EntityRecognizerEntityListOutputTypeDef,
+        "Documents": EntityRecognizerDocumentsTypeDef,
+        "Annotations": EntityRecognizerAnnotationsTypeDef,
+        "EntityList": EntityRecognizerEntityListTypeDef,
         "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
     },
     total=False,
 )
 
 class EntityRecognizerInputDataConfigOutputTypeDef(
     _RequiredEntityRecognizerInputDataConfigOutputTypeDef,
@@ -2517,23 +2351,14 @@
 )
 
 class EntityRecognizerInputDataConfigTypeDef(
     _RequiredEntityRecognizerInputDataConfigTypeDef, _OptionalEntityRecognizerInputDataConfigTypeDef
 ):
     pass
 
-ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
-    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
-    {
-        "Filter": EntityRecognizerFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEntityRecognizersRequestRequestTypeDef = TypedDict(
     "ListEntityRecognizersRequestRequestTypeDef",
     {
         "Filter": EntityRecognizerFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2551,15 +2376,15 @@
 )
 
 ListEntityRecognizerSummariesResponseTypeDef = TypedDict(
     "ListEntityRecognizerSummariesResponseTypeDef",
     {
         "EntityRecognizerSummariesList": List[EntityRecognizerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventsDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListEventsDetectionJobsRequestRequestTypeDef",
     {
         "Filter": EventsDetectionJobFilterTypeDef,
@@ -2620,51 +2445,107 @@
 )
 
 ListFlywheelsResponseTypeDef = TypedDict(
     "ListFlywheelsResponseTypeDef",
     {
         "FlywheelSummaryList": List[FlywheelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
+ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
     {
         "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
-ListKeyPhrasesDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListKeyPhrasesDetectionJobsRequestRequestTypeDef",
+ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = TypedDict(
+    "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
+    {
+        "Filter": DocumentClassificationJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = TypedDict(
+    "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
+    {
+        "Filter": DocumentClassifierFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = (
+    TypedDict(
+        "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
+        {
+            "Filter": DominantLanguageDetectionJobFilterTypeDef,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListEndpointsRequestListEndpointsPaginateTypeDef = TypedDict(
+    "ListEndpointsRequestListEndpointsPaginateTypeDef",
+    {
+        "Filter": EndpointFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef",
+    {
+        "Filter": EntitiesDetectionJobFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = TypedDict(
+    "ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef",
+    {
+        "Filter": EntityRecognizerFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = TypedDict(
+    "ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef",
     {
         "Filter": KeyPhrasesDetectionJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef",
     {
         "Filter": PiiEntitiesDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPiiEntitiesDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     {
@@ -2675,53 +2556,44 @@
     total=False,
 )
 
 ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = TypedDict(
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     {
         "Filter": SentimentDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListSentimentDetectionJobsRequestRequestTypeDef",
     {
         "Filter": SentimentDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTargetedSentimentDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     {
         "Filter": TargetedSentimentDetectionJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = TypedDict(
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     {
         "Filter": TopicsDetectionJobFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTopicsDetectionJobsRequestRequestTypeDef = TypedDict(
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     {
@@ -2745,33 +2617,33 @@
 )
 
 BatchDetectDominantLanguageResponseTypeDef = TypedDict(
     "BatchDetectDominantLanguageResponseTypeDef",
     {
         "ResultList": List[BatchDetectDominantLanguageItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectKeyPhrasesResponseTypeDef = TypedDict(
     "BatchDetectKeyPhrasesResponseTypeDef",
     {
         "ResultList": List[BatchDetectKeyPhrasesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSentimentResponseTypeDef = TypedDict(
     "BatchDetectSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetedSentimentMentionTypeDef = TypedDict(
     "TargetedSentimentMentionTypeDef",
     {
         "Score": float,
@@ -3113,15 +2985,15 @@
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
         "InputDataConfig": DocumentClassifierInputDataConfigOutputTypeDef,
-        "OutputDataConfig": DocumentClassifierOutputDataConfigOutputTypeDef,
+        "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
         "ClassifierMetadata": ClassifierMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "VersionName": str,
@@ -3139,15 +3011,15 @@
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "DocumentClassifierArn": str,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
         "FlywheelArn": str,
     },
     total=False,
 )
@@ -3159,15 +3031,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
@@ -3179,15 +3051,15 @@
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "EntityRecognizerArn": str,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
         "FlywheelArn": str,
     },
     total=False,
@@ -3200,15 +3072,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "TargetEventTypes": List[str],
     },
     total=False,
 )
 
@@ -3219,15 +3091,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
@@ -3259,15 +3131,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
@@ -3279,15 +3151,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": LanguageCodeType,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
@@ -3299,15 +3171,15 @@
         "JobArn": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "NumberOfTopics": int,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
@@ -3317,15 +3189,15 @@
     {
         "Classes": List[DocumentClassTypeDef],
         "Labels": List[DocumentLabelTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
         "Warnings": List[WarningsListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTaskConfigOutputTypeDef = TypedDict(
     "_RequiredTaskConfigOutputTypeDef",
     {
         "LanguageCode": LanguageCodeType,
@@ -3401,24 +3273,24 @@
     total=False,
 )
 
 DescribeFlywheelIterationResponseTypeDef = TypedDict(
     "DescribeFlywheelIterationResponseTypeDef",
     {
         "FlywheelIterationProperties": FlywheelIterationPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFlywheelIterationHistoryResponseTypeDef = TypedDict(
     "ListFlywheelIterationHistoryResponseTypeDef",
     {
         "FlywheelIterationPropertiesList": List[FlywheelIterationPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BlockTypeDef = TypedDict(
     "BlockTypeDef",
     {
         "Id": str,
@@ -3440,15 +3312,15 @@
     total=False,
 )
 
 DetectSyntaxResponseTypeDef = TypedDict(
     "DetectSyntaxResponseTypeDef",
     {
         "SyntaxTokens": List[SyntaxTokenTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetedSentimentEntityTypeDef = TypedDict(
     "TargetedSentimentEntityTypeDef",
     {
         "DescriptiveMentionIndex": List[int],
@@ -3490,181 +3362,181 @@
 ):
     pass
 
 DescribeDocumentClassifierResponseTypeDef = TypedDict(
     "DescribeDocumentClassifierResponseTypeDef",
     {
         "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDocumentClassifiersResponseTypeDef = TypedDict(
     "ListDocumentClassifiersResponseTypeDef",
     {
         "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDocumentClassificationJobResponseTypeDef = TypedDict(
     "DescribeDocumentClassificationJobResponseTypeDef",
     {
         "DocumentClassificationJobProperties": DocumentClassificationJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDocumentClassificationJobsResponseTypeDef = TypedDict(
     "ListDocumentClassificationJobsResponseTypeDef",
     {
         "DocumentClassificationJobPropertiesList": List[DocumentClassificationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDominantLanguageDetectionJobResponseTypeDef = TypedDict(
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     {
         "DominantLanguageDetectionJobProperties": DominantLanguageDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDominantLanguageDetectionJobsResponseTypeDef = TypedDict(
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     {
         "DominantLanguageDetectionJobPropertiesList": List[
             DominantLanguageDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionJobResponseTypeDef",
     {
         "EntitiesDetectionJobProperties": EntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionJobsResponseTypeDef",
     {
         "EntitiesDetectionJobPropertiesList": List[EntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsDetectionJobResponseTypeDef = TypedDict(
     "DescribeEventsDetectionJobResponseTypeDef",
     {
         "EventsDetectionJobProperties": EventsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventsDetectionJobsResponseTypeDef = TypedDict(
     "ListEventsDetectionJobsResponseTypeDef",
     {
         "EventsDetectionJobPropertiesList": List[EventsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKeyPhrasesDetectionJobResponseTypeDef = TypedDict(
     "DescribeKeyPhrasesDetectionJobResponseTypeDef",
     {
         "KeyPhrasesDetectionJobProperties": KeyPhrasesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKeyPhrasesDetectionJobsResponseTypeDef = TypedDict(
     "ListKeyPhrasesDetectionJobsResponseTypeDef",
     {
         "KeyPhrasesDetectionJobPropertiesList": List[KeyPhrasesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePiiEntitiesDetectionJobResponseTypeDef = TypedDict(
     "DescribePiiEntitiesDetectionJobResponseTypeDef",
     {
         "PiiEntitiesDetectionJobProperties": PiiEntitiesDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPiiEntitiesDetectionJobsResponseTypeDef = TypedDict(
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     {
         "PiiEntitiesDetectionJobPropertiesList": List[PiiEntitiesDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeSentimentDetectionJobResponseTypeDef",
     {
         "SentimentDetectionJobProperties": SentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListSentimentDetectionJobsResponseTypeDef",
     {
         "SentimentDetectionJobPropertiesList": List[SentimentDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTargetedSentimentDetectionJobResponseTypeDef = TypedDict(
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     {
         "TargetedSentimentDetectionJobProperties": TargetedSentimentDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetedSentimentDetectionJobsResponseTypeDef = TypedDict(
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     {
         "TargetedSentimentDetectionJobPropertiesList": List[
             TargetedSentimentDetectionJobPropertiesTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTopicsDetectionJobResponseTypeDef = TypedDict(
     "DescribeTopicsDetectionJobResponseTypeDef",
     {
         "TopicsDetectionJobProperties": TopicsDetectionJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTopicsDetectionJobsResponseTypeDef = TypedDict(
     "ListTopicsDetectionJobsResponseTypeDef",
     {
         "TopicsDetectionJobPropertiesList": List[TopicsDetectionJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FlywheelPropertiesTypeDef = TypedDict(
     "FlywheelPropertiesTypeDef",
     {
         "FlywheelArn": str,
@@ -3738,24 +3610,24 @@
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Blocks": List[BlockTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectSyntaxResponseTypeDef = TypedDict(
     "BatchDetectSyntaxResponseTypeDef",
     {
         "ResultList": List[BatchDetectSyntaxItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectTargetedSentimentItemResultTypeDef = TypedDict(
     "BatchDetectTargetedSentimentItemResultTypeDef",
     {
         "Index": int,
@@ -3764,61 +3636,61 @@
     total=False,
 )
 
 DetectTargetedSentimentResponseTypeDef = TypedDict(
     "DetectTargetedSentimentResponseTypeDef",
     {
         "Entities": List[TargetedSentimentEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectEntitiesResponseTypeDef = TypedDict(
     "BatchDetectEntitiesResponseTypeDef",
     {
         "ResultList": List[BatchDetectEntitiesItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFlywheelResponseTypeDef = TypedDict(
     "DescribeFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlywheelResponseTypeDef = TypedDict(
     "UpdateFlywheelResponseTypeDef",
     {
         "FlywheelProperties": FlywheelPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntityRecognizerResponseTypeDef = TypedDict(
     "DescribeEntityRecognizerResponseTypeDef",
     {
         "EntityRecognizerProperties": EntityRecognizerPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntityRecognizersResponseTypeDef = TypedDict(
     "ListEntityRecognizersResponseTypeDef",
     {
         "EntityRecognizerPropertiesList": List[EntityRecognizerPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetectTargetedSentimentResponseTypeDef = TypedDict(
     "BatchDetectTargetedSentimentResponseTypeDef",
     {
         "ResultList": List[BatchDetectTargetedSentimentItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/PKG-INFO` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehend
-Version: 1.28.12
-Summary: Type annotations for boto3.Comprehend 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Comprehend 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehend.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehend)](https://pepy.tech/project/mypy-boto3-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Comprehend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[boto3.Comprehend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [mypy-boto3-comprehend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -403,14 +403,15 @@
 ```python
 from mypy_boto3_comprehend.type_defs import (
     AugmentedManifestsListItemOutputTypeDef,
     AugmentedManifestsListItemTypeDef,
     DominantLanguageTypeDef,
     BatchDetectDominantLanguageRequestRequestTypeDef,
     BatchItemErrorTypeDef,
+    ResponseMetadataTypeDef,
     BatchDetectEntitiesRequestRequestTypeDef,
     KeyPhraseTypeDef,
     BatchDetectKeyPhrasesRequestRequestTypeDef,
     SentimentScoreTypeDef,
     BatchDetectSentimentRequestRequestTypeDef,
     BatchDetectSyntaxRequestRequestTypeDef,
     BatchDetectTargetedSentimentRequestRequestTypeDef,
@@ -423,21 +424,16 @@
     DocumentLabelTypeDef,
     DocumentTypeListItemTypeDef,
     ErrorsListItemTypeDef,
     WarningsListItemTypeDef,
     ContainsPiiEntitiesRequestRequestTypeDef,
     EntityLabelTypeDef,
     TagTypeDef,
-    CreateDatasetResponseTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
     VpcConfigTypeDef,
-    CreateDocumentClassifierResponseTypeDef,
-    CreateEndpointResponseTypeDef,
-    CreateEntityRecognizerResponseTypeDef,
-    CreateFlywheelResponseTypeDef,
     VpcConfigOutputTypeDef,
     DatasetAugmentedManifestsListItemTypeDef,
     DatasetDocumentClassifierInputDataConfigTypeDef,
     DatasetEntityRecognizerAnnotationsTypeDef,
     DatasetEntityRecognizerDocumentsTypeDef,
     DatasetEntityRecognizerEntityListTypeDef,
     DatasetFilterTypeDef,
@@ -457,169 +453,165 @@
     DescribeEntityRecognizerRequestRequestTypeDef,
     DescribeEventsDetectionJobRequestRequestTypeDef,
     DescribeFlywheelIterationRequestRequestTypeDef,
     DescribeFlywheelRequestRequestTypeDef,
     DescribeKeyPhrasesDetectionJobRequestRequestTypeDef,
     DescribePiiEntitiesDetectionJobRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSentimentDetectionJobRequestRequestTypeDef,
     DescribeTargetedSentimentDetectionJobRequestRequestTypeDef,
     DescribeTopicsDetectionJobRequestRequestTypeDef,
     DetectDominantLanguageRequestRequestTypeDef,
     DetectKeyPhrasesRequestRequestTypeDef,
     DetectPiiEntitiesRequestRequestTypeDef,
     PiiEntityTypeDef,
     DetectSentimentRequestRequestTypeDef,
     DetectSyntaxRequestRequestTypeDef,
     DetectTargetedSentimentRequestRequestTypeDef,
     DocumentClassificationConfigOutputTypeDef,
     DocumentClassificationConfigTypeDef,
     DocumentClassificationJobFilterTypeDef,
-    OutputDataConfigOutputTypeDef,
-    DocumentClassifierDocumentsOutputTypeDef,
+    OutputDataConfigTypeDef,
     DocumentClassifierDocumentsTypeDef,
     DocumentClassifierFilterTypeDef,
     DocumentReaderConfigOutputTypeDef,
-    DocumentClassifierOutputDataConfigOutputTypeDef,
     DocumentClassifierSummaryTypeDef,
     ExtractedCharactersListItemTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
-    EntityTypesListItemOutputTypeDef,
     EntityTypesListItemTypeDef,
-    EntityRecognizerAnnotationsOutputTypeDef,
     EntityRecognizerAnnotationsTypeDef,
-    EntityRecognizerDocumentsOutputTypeDef,
     EntityRecognizerDocumentsTypeDef,
-    EntityRecognizerEntityListOutputTypeDef,
     EntityRecognizerEntityListTypeDef,
     EntityRecognizerEvaluationMetricsTypeDef,
     EntityRecognizerFilterTypeDef,
     EntityTypesEvaluationMetricsTypeDef,
     EntityRecognizerOutputDataConfigTypeDef,
     EntityRecognizerSummaryTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     FlywheelModelEvaluationMetricsTypeDef,
     FlywheelSummaryTypeDef,
     PointTypeDef,
-    ImportModelResponseTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListDocumentClassifierSummariesRequestRequestTypeDef,
     ListEntityRecognizerSummariesRequestRequestTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     SentimentDetectionJobFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
     TopicsDetectionJobFilterTypeDef,
-    OutputDataConfigTypeDef,
-    PaginatorConfigTypeDef,
     PartOfSpeechTagTypeDef,
     PiiOutputDataConfigTypeDef,
     RedactionConfigOutputTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RedactionConfigTypeDef,
-    ResponseMetadataTypeDef,
+    StartFlywheelIterationRequestRequestTypeDef,
+    StopDominantLanguageDetectionJobRequestRequestTypeDef,
+    StopEntitiesDetectionJobRequestRequestTypeDef,
+    StopEventsDetectionJobRequestRequestTypeDef,
+    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
+    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
+    StopSentimentDetectionJobRequestRequestTypeDef,
+    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
+    StopTrainingDocumentClassifierRequestRequestTypeDef,
+    StopTrainingEntityRecognizerRequestRequestTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
+    BatchDetectDominantLanguageItemResultTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateDocumentClassifierResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreateEntityRecognizerResponseTypeDef,
+    CreateFlywheelResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    DetectDominantLanguageResponseTypeDef,
+    ImportModelResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
-    StartFlywheelIterationRequestRequestTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
     StartPiiEntitiesDetectionJobResponseTypeDef,
     StartSentimentDetectionJobResponseTypeDef,
     StartTargetedSentimentDetectionJobResponseTypeDef,
     StartTopicsDetectionJobResponseTypeDef,
-    StopDominantLanguageDetectionJobRequestRequestTypeDef,
     StopDominantLanguageDetectionJobResponseTypeDef,
-    StopEntitiesDetectionJobRequestRequestTypeDef,
     StopEntitiesDetectionJobResponseTypeDef,
-    StopEventsDetectionJobRequestRequestTypeDef,
     StopEventsDetectionJobResponseTypeDef,
-    StopKeyPhrasesDetectionJobRequestRequestTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
-    StopPiiEntitiesDetectionJobRequestRequestTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
-    StopSentimentDetectionJobRequestRequestTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
-    StopTargetedSentimentDetectionJobRequestRequestTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
-    StopTrainingDocumentClassifierRequestRequestTypeDef,
-    StopTrainingEntityRecognizerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
-    BatchDetectDominantLanguageItemResultTypeDef,
-    DetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesItemResultTypeDef,
     DetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentItemResultTypeDef,
     DetectSentimentResponseTypeDef,
     MentionSentimentTypeDef,
     BlockReferenceTypeDef,
     ClassifierMetadataTypeDef,
     ClassifyDocumentRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     InputDataConfigTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateEndpointRequestRequestTypeDef,
     ImportModelRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DataSecurityConfigTypeDef,
     UpdateDataSecurityConfigTypeDef,
     DataSecurityConfigOutputTypeDef,
     DatasetEntityRecognizerInputDataConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     ListEndpointsResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
-    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
     ListDocumentClassificationJobsRequestRequestTypeDef,
     DocumentClassifierInputDataConfigTypeDef,
-    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
     ListDocumentClassifiersRequestRequestTypeDef,
     DocumentClassifierInputDataConfigOutputTypeDef,
     InputDataConfigOutputTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     DocumentMetadataTypeDef,
-    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
     ListDominantLanguageDetectionJobsRequestRequestTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
     ListEndpointsRequestRequestTypeDef,
-    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
     ListEntitiesDetectionJobsRequestRequestTypeDef,
     EntityRecognitionConfigOutputTypeDef,
     EntityRecognitionConfigTypeDef,
     EntityRecognizerInputDataConfigOutputTypeDef,
     EntityRecognizerInputDataConfigTypeDef,
-    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
     ListEntityRecognizersRequestRequestTypeDef,
     EntityRecognizerMetadataEntityTypesListItemTypeDef,
     ListEntityRecognizerSummariesResponseTypeDef,
     ListEventsDetectionJobsRequestRequestTypeDef,
     ListFlywheelsRequestRequestTypeDef,
     ListFlywheelIterationHistoryRequestRequestTypeDef,
     FlywheelIterationPropertiesTypeDef,
     ListFlywheelsResponseTypeDef,
     GeometryTypeDef,
-    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListKeyPhrasesDetectionJobsRequestRequestTypeDef,
+    ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef,
+    ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef,
+    ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef,
+    ListEndpointsRequestListEndpointsPaginateTypeDef,
+    ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef,
+    ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef,
+    ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef,
     ListPiiEntitiesDetectionJobsRequestRequestTypeDef,
     ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef,
     ListSentimentDetectionJobsRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsRequestRequestTypeDef,
     ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef,
     ListTopicsDetectionJobsRequestRequestTypeDef,
     SyntaxTokenTypeDef,
     BatchDetectDominantLanguageResponseTypeDef,
     BatchDetectKeyPhrasesResponseTypeDef,
     BatchDetectSentimentResponseTypeDef,
```

### Comparing `mypy-boto3-comprehend-1.28.12/mypy_boto3_comprehend.egg-info/SOURCES.txt` & `mypy-boto3-comprehend-1.28.15/mypy_boto3_comprehend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehend-1.28.12/setup.py` & `mypy-boto3-comprehend-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-comprehend",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_comprehend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Comprehend 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Comprehend 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

