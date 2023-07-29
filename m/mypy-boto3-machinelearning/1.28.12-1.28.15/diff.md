# Comparing `tmp/mypy-boto3-machinelearning-1.28.12.tar.gz` & `tmp/mypy-boto3-machinelearning-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-machinelearning-1.28.12.tar", last modified: Thu Jul 27 05:34:58 2023, max compression
+gzip compressed data, was "mypy-boto3-machinelearning-1.28.15.tar", last modified: Fri Jul 28 20:43:12 2023, max compression
```

## Comparing `mypy-boto3-machinelearning-1.28.12.tar` & `mypy-boto3-machinelearning-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.196452 mypy-boto3-machinelearning-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-07-27 05:34:58.196452 mypy-boto3-machinelearning-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.196452 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-07-27 05:25:44.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-07-27 05:25:44.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32223 2023-07-27 05:25:44.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.196452 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:58.000000 mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:58.196452 mypy-boto3-machinelearning-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-27 05:25:43.000000 mypy-boto3-machinelearning-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:12.025429 mypy-boto3-machinelearning-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-07-28 20:43:12.017429 mypy-boto3-machinelearning-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16717 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:12.017429 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-07-28 20:30:43.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-28 20:30:43.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-28 20:30:43.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-07-28 20:30:44.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31610 2023-07-28 20:30:43.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-28 20:30:43.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-28 20:30:43.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:12.017429 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-07-28 20:43:11.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:43:11.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:11.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:43:11.000000 mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:12.025429 mypy-boto3-machinelearning-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-28 20:30:42.000000 mypy-boto3-machinelearning-1.28.15/setup.py
```

### Comparing `mypy-boto3-machinelearning-1.28.12/LICENSE` & `mypy-boto3-machinelearning-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.12/PKG-INFO` & `mypy-boto3-machinelearning-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-machinelearning
-Version: 1.28.12
-Summary: Type annotations for boto3.MachineLearning 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MachineLearning 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-machinelearning)](https://pepy.tech/project/mypy-boto3-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MachineLearning 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[boto3.MachineLearning 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [mypy-boto3-machinelearning docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -385,86 +385,83 @@
 
 `mypy_boto3_machinelearning.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_machinelearning.type_defs import (
     TagTypeDef,
-    AddTagsOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchPredictionTypeDef,
     CreateBatchPredictionInputRequestTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
     S3DataSpecTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
     CreateEvaluationInputRequestTypeDef,
-    CreateEvaluationOutputTypeDef,
     CreateMLModelInputRequestTypeDef,
-    CreateMLModelOutputTypeDef,
     CreateRealtimeEndpointInputRequestTypeDef,
     RealtimeEndpointInfoTypeDef,
     DeleteBatchPredictionInputRequestTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
     DeleteDataSourceInputRequestTypeDef,
-    DeleteDataSourceOutputTypeDef,
     DeleteEvaluationInputRequestTypeDef,
-    DeleteEvaluationOutputTypeDef,
     DeleteMLModelInputRequestTypeDef,
-    DeleteMLModelOutputTypeDef,
     DeleteRealtimeEndpointInputRequestTypeDef,
     DeleteTagsInputRequestTypeDef,
-    DeleteTagsOutputTypeDef,
     WaiterConfigTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBatchPredictionsInputRequestTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
-    TagOutputTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
-    GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
-    RDSDatabaseOutputTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
-    RedshiftDatabaseOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
-    UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
-    UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
-    UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    AddTagsOutputTypeDef,
+    CreateBatchPredictionOutputTypeDef,
+    CreateDataSourceFromRDSOutputTypeDef,
+    CreateDataSourceFromRedshiftOutputTypeDef,
+    CreateDataSourceFromS3OutputTypeDef,
+    CreateEvaluationOutputTypeDef,
+    CreateMLModelOutputTypeDef,
+    DeleteBatchPredictionOutputTypeDef,
+    DeleteDataSourceOutputTypeDef,
+    DeleteEvaluationOutputTypeDef,
+    DeleteMLModelOutputTypeDef,
+    DeleteTagsOutputTypeDef,
+    DescribeTagsOutputTypeDef,
+    GetBatchPredictionOutputTypeDef,
+    UpdateBatchPredictionOutputTypeDef,
+    UpdateDataSourceOutputTypeDef,
+    UpdateEvaluationOutputTypeDef,
+    UpdateMLModelOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
-    DescribeTagsOutputTypeDef,
+    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
+    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
+    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
```

### Comparing `mypy-boto3-machinelearning-1.28.12/README.md` & `mypy-boto3-machinelearning-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-machinelearning)](https://pepy.tech/project/mypy-boto3-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MachineLearning 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[boto3.MachineLearning 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [mypy-boto3-machinelearning docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,86 +353,83 @@
 
 `mypy_boto3_machinelearning.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_machinelearning.type_defs import (
     TagTypeDef,
-    AddTagsOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchPredictionTypeDef,
     CreateBatchPredictionInputRequestTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
     S3DataSpecTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
     CreateEvaluationInputRequestTypeDef,
-    CreateEvaluationOutputTypeDef,
     CreateMLModelInputRequestTypeDef,
-    CreateMLModelOutputTypeDef,
     CreateRealtimeEndpointInputRequestTypeDef,
     RealtimeEndpointInfoTypeDef,
     DeleteBatchPredictionInputRequestTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
     DeleteDataSourceInputRequestTypeDef,
-    DeleteDataSourceOutputTypeDef,
     DeleteEvaluationInputRequestTypeDef,
-    DeleteEvaluationOutputTypeDef,
     DeleteMLModelInputRequestTypeDef,
-    DeleteMLModelOutputTypeDef,
     DeleteRealtimeEndpointInputRequestTypeDef,
     DeleteTagsInputRequestTypeDef,
-    DeleteTagsOutputTypeDef,
     WaiterConfigTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBatchPredictionsInputRequestTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
-    TagOutputTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
-    GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
-    RDSDatabaseOutputTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
-    RedshiftDatabaseOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
-    UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
-    UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
-    UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    AddTagsOutputTypeDef,
+    CreateBatchPredictionOutputTypeDef,
+    CreateDataSourceFromRDSOutputTypeDef,
+    CreateDataSourceFromRedshiftOutputTypeDef,
+    CreateDataSourceFromS3OutputTypeDef,
+    CreateEvaluationOutputTypeDef,
+    CreateMLModelOutputTypeDef,
+    DeleteBatchPredictionOutputTypeDef,
+    DeleteDataSourceOutputTypeDef,
+    DeleteEvaluationOutputTypeDef,
+    DeleteMLModelOutputTypeDef,
+    DeleteTagsOutputTypeDef,
+    DescribeTagsOutputTypeDef,
+    GetBatchPredictionOutputTypeDef,
+    UpdateBatchPredictionOutputTypeDef,
+    UpdateDataSourceOutputTypeDef,
+    UpdateEvaluationOutputTypeDef,
+    UpdateMLModelOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
-    DescribeTagsOutputTypeDef,
+    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
+    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
+    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
```

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__init__.py` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__init__.pyi` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/__main__.py` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MachineLearning 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MachineLearning 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning\nOther"
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

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/client.py` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/client.pyi` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/literals.py` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/literals.pyi` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/paginator.py` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBatchPredictionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeBatchPredictions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describebatchpredictionspaginator)
         """
 
 
@@ -102,15 +102,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDataSourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeDataSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describedatasourcespaginator)
         """
 
 
@@ -128,15 +128,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEvaluationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describeevaluationspaginator)
         """
 
 
@@ -154,13 +154,13 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMLModelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeMLModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describemlmodelspaginator)
         """
```

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/paginator.pyi` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBatchPredictionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeBatchPredictions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describebatchpredictionspaginator)
         """
 
 class DescribeDataSourcesPaginator(Paginator):
@@ -98,15 +98,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDataSourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeDataSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describedatasourcespaginator)
         """
 
 class DescribeEvaluationsPaginator(Paginator):
@@ -123,15 +123,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEvaluationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describeevaluationspaginator)
         """
 
 class DescribeMLModelsPaginator(Paginator):
@@ -148,13 +148,13 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMLModelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeMLModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/paginators/#describemlmodelspaginator)
         """
```

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/type_defs.py` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,89 +33,85 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
-    "AddTagsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchPredictionTypeDef",
     "CreateBatchPredictionInputRequestTypeDef",
-    "CreateBatchPredictionOutputTypeDef",
-    "CreateDataSourceFromRDSOutputTypeDef",
-    "CreateDataSourceFromRedshiftOutputTypeDef",
     "S3DataSpecTypeDef",
-    "CreateDataSourceFromS3OutputTypeDef",
     "CreateEvaluationInputRequestTypeDef",
-    "CreateEvaluationOutputTypeDef",
     "CreateMLModelInputRequestTypeDef",
-    "CreateMLModelOutputTypeDef",
     "CreateRealtimeEndpointInputRequestTypeDef",
     "RealtimeEndpointInfoTypeDef",
     "DeleteBatchPredictionInputRequestTypeDef",
-    "DeleteBatchPredictionOutputTypeDef",
     "DeleteDataSourceInputRequestTypeDef",
-    "DeleteDataSourceOutputTypeDef",
     "DeleteEvaluationInputRequestTypeDef",
-    "DeleteEvaluationOutputTypeDef",
     "DeleteMLModelInputRequestTypeDef",
-    "DeleteMLModelOutputTypeDef",
     "DeleteRealtimeEndpointInputRequestTypeDef",
     "DeleteTagsInputRequestTypeDef",
-    "DeleteTagsOutputTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBatchPredictionsInputRequestTypeDef",
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
     "DescribeDataSourcesInputRequestTypeDef",
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
     "DescribeEvaluationsInputRequestTypeDef",
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "DescribeMLModelsInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
-    "TagOutputTypeDef",
     "PerformanceMetricsTypeDef",
     "GetBatchPredictionInputRequestTypeDef",
-    "GetBatchPredictionOutputTypeDef",
     "GetDataSourceInputRequestTypeDef",
     "GetEvaluationInputRequestTypeDef",
     "GetMLModelInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PredictInputRequestTypeDef",
     "PredictionTypeDef",
     "RDSDatabaseCredentialsTypeDef",
     "RDSDatabaseTypeDef",
-    "RDSDatabaseOutputTypeDef",
     "RedshiftDatabaseCredentialsTypeDef",
     "RedshiftDatabaseTypeDef",
-    "RedshiftDatabaseOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateBatchPredictionInputRequestTypeDef",
-    "UpdateBatchPredictionOutputTypeDef",
     "UpdateDataSourceInputRequestTypeDef",
-    "UpdateDataSourceOutputTypeDef",
     "UpdateEvaluationInputRequestTypeDef",
-    "UpdateEvaluationOutputTypeDef",
     "UpdateMLModelInputRequestTypeDef",
-    "UpdateMLModelOutputTypeDef",
     "AddTagsInputRequestTypeDef",
+    "AddTagsOutputTypeDef",
+    "CreateBatchPredictionOutputTypeDef",
+    "CreateDataSourceFromRDSOutputTypeDef",
+    "CreateDataSourceFromRedshiftOutputTypeDef",
+    "CreateDataSourceFromS3OutputTypeDef",
+    "CreateEvaluationOutputTypeDef",
+    "CreateMLModelOutputTypeDef",
+    "DeleteBatchPredictionOutputTypeDef",
+    "DeleteDataSourceOutputTypeDef",
+    "DeleteEvaluationOutputTypeDef",
+    "DeleteMLModelOutputTypeDef",
+    "DeleteTagsOutputTypeDef",
+    "DescribeTagsOutputTypeDef",
+    "GetBatchPredictionOutputTypeDef",
+    "UpdateBatchPredictionOutputTypeDef",
+    "UpdateDataSourceOutputTypeDef",
+    "UpdateEvaluationOutputTypeDef",
+    "UpdateMLModelOutputTypeDef",
     "DescribeBatchPredictionsOutputTypeDef",
     "CreateDataSourceFromS3InputRequestTypeDef",
     "CreateRealtimeEndpointOutputTypeDef",
     "DeleteRealtimeEndpointOutputTypeDef",
     "GetMLModelOutputTypeDef",
     "MLModelTypeDef",
     "DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef",
     "DescribeDataSourcesInputDataSourceAvailableWaitTypeDef",
     "DescribeEvaluationsInputEvaluationAvailableWaitTypeDef",
     "DescribeMLModelsInputMLModelAvailableWaitTypeDef",
-    "DescribeTagsOutputTypeDef",
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "EvaluationTypeDef",
     "GetEvaluationOutputTypeDef",
     "PredictOutputTypeDef",
     "RDSDataSpecTypeDef",
     "RDSMetadataTypeDef",
     "RedshiftDataSpecTypeDef",
     "RedshiftMetadataTypeDef",
@@ -133,20 +129,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AddTagsOutputTypeDef = TypedDict(
-    "AddTagsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchPredictionTypeDef = TypedDict(
     "BatchPredictionTypeDef",
     {
         "BatchPredictionId": str,
@@ -182,46 +180,20 @@
     "_OptionalCreateBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionName": str,
     },
     total=False,
 )
 
-
 class CreateBatchPredictionInputRequestTypeDef(
     _RequiredCreateBatchPredictionInputRequestTypeDef,
     _OptionalCreateBatchPredictionInputRequestTypeDef,
 ):
     pass
 
-
-CreateBatchPredictionOutputTypeDef = TypedDict(
-    "CreateBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDataSourceFromRDSOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRDSOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRedshiftOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredS3DataSpecTypeDef = TypedDict(
     "_RequiredS3DataSpecTypeDef",
     {
         "DataLocationS3": str,
     },
 )
 _OptionalS3DataSpecTypeDef = TypedDict(
@@ -230,27 +202,17 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaLocationS3": str,
     },
     total=False,
 )
 
-
 class S3DataSpecTypeDef(_RequiredS3DataSpecTypeDef, _OptionalS3DataSpecTypeDef):
     pass
 
-
-CreateDataSourceFromS3OutputTypeDef = TypedDict(
-    "CreateDataSourceFromS3OutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateEvaluationInputRequestTypeDef = TypedDict(
     "_RequiredCreateEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
     },
@@ -259,29 +221,19 @@
     "_OptionalCreateEvaluationInputRequestTypeDef",
     {
         "EvaluationName": str,
     },
     total=False,
 )
 
-
 class CreateEvaluationInputRequestTypeDef(
     _RequiredCreateEvaluationInputRequestTypeDef, _OptionalCreateEvaluationInputRequestTypeDef
 ):
     pass
 
-
-CreateEvaluationOutputTypeDef = TypedDict(
-    "CreateEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateMLModelInputRequestTypeDef = TypedDict(
     "_RequiredCreateMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
         "MLModelType": MLModelTypeType,
         "TrainingDataSourceId": str,
     },
@@ -293,29 +245,19 @@
         "Parameters": Mapping[str, str],
         "Recipe": str,
         "RecipeUri": str,
     },
     total=False,
 )
 
-
 class CreateMLModelInputRequestTypeDef(
     _RequiredCreateMLModelInputRequestTypeDef, _OptionalCreateMLModelInputRequestTypeDef
 ):
     pass
 
-
-CreateMLModelOutputTypeDef = TypedDict(
-    "CreateMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateRealtimeEndpointInputRequestTypeDef = TypedDict(
     "CreateRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
@@ -333,67 +275,35 @@
 DeleteBatchPredictionInputRequestTypeDef = TypedDict(
     "DeleteBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
-DeleteBatchPredictionOutputTypeDef = TypedDict(
-    "DeleteBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDataSourceInputRequestTypeDef = TypedDict(
     "DeleteDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 
-DeleteDataSourceOutputTypeDef = TypedDict(
-    "DeleteDataSourceOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEvaluationInputRequestTypeDef = TypedDict(
     "DeleteEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
     },
 )
 
-DeleteEvaluationOutputTypeDef = TypedDict(
-    "DeleteEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteMLModelInputRequestTypeDef = TypedDict(
     "DeleteMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
-DeleteMLModelOutputTypeDef = TypedDict(
-    "DeleteMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRealtimeEndpointInputRequestTypeDef = TypedDict(
     "DeleteRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
@@ -402,45 +312,29 @@
     {
         "TagKeys": Sequence[str],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
-DeleteTagsOutputTypeDef = TypedDict(
-    "DeleteTagsOutputTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "FilterVariable": BatchPredictionFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeBatchPredictionsInputRequestTypeDef = TypedDict(
     "DescribeBatchPredictionsInputRequestTypeDef",
     {
@@ -455,31 +349,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
-    {
-        "FilterVariable": DataSourceFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSourcesInputRequestTypeDef = TypedDict(
     "DescribeDataSourcesInputRequestTypeDef",
     {
         "FilterVariable": DataSourceFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -490,31 +367,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
-    {
-        "FilterVariable": EvaluationFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEvaluationsInputRequestTypeDef = TypedDict(
     "DescribeEvaluationsInputRequestTypeDef",
     {
         "FilterVariable": EvaluationFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -525,31 +385,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
-    {
-        "FilterVariable": MLModelFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeMLModelsInputRequestTypeDef = TypedDict(
     "DescribeMLModelsInputRequestTypeDef",
     {
         "FilterVariable": MLModelFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -568,23 +411,14 @@
     "DescribeTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 PerformanceMetricsTypeDef = TypedDict(
     "PerformanceMetricsTypeDef",
     {
         "Properties": Dict[str, str],
     },
     total=False,
 )
@@ -592,59 +426,33 @@
 GetBatchPredictionInputRequestTypeDef = TypedDict(
     "GetBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
-GetBatchPredictionOutputTypeDef = TypedDict(
-    "GetBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "MLModelId": str,
-        "BatchPredictionDataSourceId": str,
-        "InputDataLocationS3": str,
-        "CreatedByIamUser": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Name": str,
-        "Status": EntityStatusType,
-        "OutputUri": str,
-        "LogUri": str,
-        "Message": str,
-        "ComputeTime": int,
-        "FinishedAt": datetime,
-        "StartedAt": datetime,
-        "TotalRecordCount": int,
-        "InvalidRecordCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDataSourceInputRequestTypeDef = TypedDict(
     "_RequiredGetDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 _OptionalGetDataSourceInputRequestTypeDef = TypedDict(
     "_OptionalGetDataSourceInputRequestTypeDef",
     {
         "Verbose": bool,
     },
     total=False,
 )
 
-
 class GetDataSourceInputRequestTypeDef(
     _RequiredGetDataSourceInputRequestTypeDef, _OptionalGetDataSourceInputRequestTypeDef
 ):
     pass
 
-
 GetEvaluationInputRequestTypeDef = TypedDict(
     "GetEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
     },
 )
 
@@ -658,31 +466,19 @@
     "_OptionalGetMLModelInputRequestTypeDef",
     {
         "Verbose": bool,
     },
     total=False,
 )
 
-
 class GetMLModelInputRequestTypeDef(
     _RequiredGetMLModelInputRequestTypeDef, _OptionalGetMLModelInputRequestTypeDef
 ):
     pass
 
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
 PredictInputRequestTypeDef = TypedDict(
     "PredictInputRequestTypeDef",
     {
         "MLModelId": str,
         "Record": Mapping[str, str],
         "PredictEndpoint": str,
     },
@@ -711,22 +507,14 @@
     "RDSDatabaseTypeDef",
     {
         "InstanceIdentifier": str,
         "DatabaseName": str,
     },
 )
 
-RDSDatabaseOutputTypeDef = TypedDict(
-    "RDSDatabaseOutputTypeDef",
-    {
-        "InstanceIdentifier": str,
-        "DatabaseName": str,
-    },
-)
-
 RedshiftDatabaseCredentialsTypeDef = TypedDict(
     "RedshiftDatabaseCredentialsTypeDef",
     {
         "Username": str,
         "Password": str,
     },
 )
@@ -735,126 +523,237 @@
     "RedshiftDatabaseTypeDef",
     {
         "DatabaseName": str,
         "ClusterIdentifier": str,
     },
 )
 
-RedshiftDatabaseOutputTypeDef = TypedDict(
-    "RedshiftDatabaseOutputTypeDef",
+UpdateBatchPredictionInputRequestTypeDef = TypedDict(
+    "UpdateBatchPredictionInputRequestTypeDef",
     {
-        "DatabaseName": str,
-        "ClusterIdentifier": str,
+        "BatchPredictionId": str,
+        "BatchPredictionName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UpdateDataSourceInputRequestTypeDef = TypedDict(
+    "UpdateDataSourceInputRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DataSourceId": str,
+        "DataSourceName": str,
     },
 )
 
-UpdateBatchPredictionInputRequestTypeDef = TypedDict(
-    "UpdateBatchPredictionInputRequestTypeDef",
+UpdateEvaluationInputRequestTypeDef = TypedDict(
+    "UpdateEvaluationInputRequestTypeDef",
     {
-        "BatchPredictionId": str,
-        "BatchPredictionName": str,
+        "EvaluationId": str,
+        "EvaluationName": str,
     },
 )
 
-UpdateBatchPredictionOutputTypeDef = TypedDict(
-    "UpdateBatchPredictionOutputTypeDef",
+_RequiredUpdateMLModelInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateMLModelInputRequestTypeDef",
+    {
+        "MLModelId": str,
+    },
+)
+_OptionalUpdateMLModelInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateMLModelInputRequestTypeDef",
+    {
+        "MLModelName": str,
+        "ScoreThreshold": float,
+    },
+    total=False,
+)
+
+class UpdateMLModelInputRequestTypeDef(
+    _RequiredUpdateMLModelInputRequestTypeDef, _OptionalUpdateMLModelInputRequestTypeDef
+):
+    pass
+
+AddTagsInputRequestTypeDef = TypedDict(
+    "AddTagsInputRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+    },
+)
+
+AddTagsOutputTypeDef = TypedDict(
+    "AddTagsOutputTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBatchPredictionOutputTypeDef = TypedDict(
+    "CreateBatchPredictionOutputTypeDef",
     {
         "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDataSourceInputRequestTypeDef = TypedDict(
-    "UpdateDataSourceInputRequestTypeDef",
+CreateDataSourceFromRDSOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRDSOutputTypeDef",
     {
         "DataSourceId": str,
-        "DataSourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDataSourceOutputTypeDef = TypedDict(
-    "UpdateDataSourceOutputTypeDef",
+CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRedshiftOutputTypeDef",
     {
         "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateEvaluationInputRequestTypeDef = TypedDict(
-    "UpdateEvaluationInputRequestTypeDef",
+CreateDataSourceFromS3OutputTypeDef = TypedDict(
+    "CreateDataSourceFromS3OutputTypeDef",
     {
-        "EvaluationId": str,
-        "EvaluationName": str,
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateEvaluationOutputTypeDef = TypedDict(
-    "UpdateEvaluationOutputTypeDef",
+CreateEvaluationOutputTypeDef = TypedDict(
+    "CreateEvaluationOutputTypeDef",
     {
         "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateMLModelInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateMLModelInputRequestTypeDef",
+CreateMLModelOutputTypeDef = TypedDict(
+    "CreateMLModelOutputTypeDef",
     {
         "MLModelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateMLModelInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateMLModelInputRequestTypeDef",
+
+DeleteBatchPredictionOutputTypeDef = TypedDict(
+    "DeleteBatchPredictionOutputTypeDef",
     {
-        "MLModelName": str,
-        "ScoreThreshold": float,
+        "BatchPredictionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+DeleteDataSourceOutputTypeDef = TypedDict(
+    "DeleteDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateMLModelInputRequestTypeDef(
-    _RequiredUpdateMLModelInputRequestTypeDef, _OptionalUpdateMLModelInputRequestTypeDef
-):
-    pass
-
+DeleteEvaluationOutputTypeDef = TypedDict(
+    "DeleteEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateMLModelOutputTypeDef = TypedDict(
-    "UpdateMLModelOutputTypeDef",
+DeleteMLModelOutputTypeDef = TypedDict(
+    "DeleteMLModelOutputTypeDef",
     {
         "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddTagsInputRequestTypeDef = TypedDict(
-    "AddTagsInputRequestTypeDef",
+DeleteTagsOutputTypeDef = TypedDict(
+    "DeleteTagsOutputTypeDef",
     {
-        "Tags": Sequence[TagTypeDef],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBatchPredictionOutputTypeDef = TypedDict(
+    "GetBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "MLModelId": str,
+        "BatchPredictionDataSourceId": str,
+        "InputDataLocationS3": str,
+        "CreatedByIamUser": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Name": str,
+        "Status": EntityStatusType,
+        "OutputUri": str,
+        "LogUri": str,
+        "Message": str,
+        "ComputeTime": int,
+        "FinishedAt": datetime,
+        "StartedAt": datetime,
+        "TotalRecordCount": int,
+        "InvalidRecordCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBatchPredictionOutputTypeDef = TypedDict(
+    "UpdateBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDataSourceOutputTypeDef = TypedDict(
+    "UpdateDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEvaluationOutputTypeDef = TypedDict(
+    "UpdateEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMLModelOutputTypeDef = TypedDict(
+    "UpdateMLModelOutputTypeDef",
+    {
+        "MLModelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBatchPredictionsOutputTypeDef = TypedDict(
     "DescribeBatchPredictionsOutputTypeDef",
     {
         "Results": List[BatchPredictionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceFromS3InputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromS3InputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -866,37 +765,35 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
-
 class CreateDataSourceFromS3InputRequestTypeDef(
     _RequiredCreateDataSourceFromS3InputRequestTypeDef,
     _OptionalCreateDataSourceFromS3InputRequestTypeDef,
 ):
     pass
 
-
 CreateRealtimeEndpointOutputTypeDef = TypedDict(
     "CreateRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRealtimeEndpointOutputTypeDef = TypedDict(
     "DeleteRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMLModelOutputTypeDef = TypedDict(
     "GetMLModelOutputTypeDef",
     {
         "MLModelId": str,
@@ -916,15 +813,15 @@
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "Recipe": str,
         "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MLModelTypeDef = TypedDict(
     "MLModelTypeDef",
     {
         "MLModelId": str,
@@ -1022,22 +919,80 @@
         "NextToken": str,
         "Limit": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
+DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
     {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FilterVariable": BatchPredictionFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
+    {
+        "FilterVariable": DataSourceFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
+    {
+        "FilterVariable": EvaluationFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
+    {
+        "FilterVariable": MLModelFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 EvaluationTypeDef = TypedDict(
     "EvaluationTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
@@ -1071,23 +1026,23 @@
         "Status": EntityStatusType,
         "PerformanceMetrics": PerformanceMetricsTypeDef,
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictOutputTypeDef = TypedDict(
     "PredictOutputTypeDef",
     {
         "Prediction": PredictionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRDSDataSpecTypeDef = TypedDict(
     "_RequiredRDSDataSpecTypeDef",
     {
         "DatabaseInformation": RDSDatabaseTypeDef,
@@ -1106,23 +1061,21 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaUri": str,
     },
     total=False,
 )
 
-
 class RDSDataSpecTypeDef(_RequiredRDSDataSpecTypeDef, _OptionalRDSDataSpecTypeDef):
     pass
 
-
 RDSMetadataTypeDef = TypedDict(
     "RDSMetadataTypeDef",
     {
-        "Database": RDSDatabaseOutputTypeDef,
+        "Database": RDSDatabaseTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
         "ResourceRole": str,
         "ServiceRole": str,
         "DataPipelineId": str,
     },
     total=False,
@@ -1143,44 +1096,42 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaUri": str,
     },
     total=False,
 )
 
-
 class RedshiftDataSpecTypeDef(_RequiredRedshiftDataSpecTypeDef, _OptionalRedshiftDataSpecTypeDef):
     pass
 
-
 RedshiftMetadataTypeDef = TypedDict(
     "RedshiftMetadataTypeDef",
     {
-        "RedshiftDatabase": RedshiftDatabaseOutputTypeDef,
+        "RedshiftDatabase": RedshiftDatabaseTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
     },
     total=False,
 )
 
 DescribeMLModelsOutputTypeDef = TypedDict(
     "DescribeMLModelsOutputTypeDef",
     {
         "Results": List[MLModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEvaluationsOutputTypeDef = TypedDict(
     "DescribeEvaluationsOutputTypeDef",
     {
         "Results": List[EvaluationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceFromRDSInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromRDSInputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -1193,22 +1144,20 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
-
 class CreateDataSourceFromRDSInputRequestTypeDef(
     _RequiredCreateDataSourceFromRDSInputRequestTypeDef,
     _OptionalCreateDataSourceFromRDSInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDataSourceFromRedshiftInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromRedshiftInputRequestTypeDef",
     {
         "DataSourceId": str,
         "DataSpec": RedshiftDataSpecTypeDef,
         "RoleARN": str,
     },
@@ -1218,22 +1167,20 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
-
 class CreateDataSourceFromRedshiftInputRequestTypeDef(
     _RequiredCreateDataSourceFromRedshiftInputRequestTypeDef,
     _OptionalCreateDataSourceFromRedshiftInputRequestTypeDef,
 ):
     pass
 
-
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "DataSourceId": str,
         "DataLocationS3": str,
         "DataRearrangement": str,
         "CreatedByIamUser": str,
@@ -1274,19 +1221,19 @@
         "RDSMetadata": RDSMetadataTypeDef,
         "RoleARN": str,
         "ComputeStatistics": bool,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "DataSourceSchema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSourcesOutputTypeDef = TypedDict(
     "DescribeDataSourcesOutputTypeDef",
     {
         "Results": List[DataSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/type_defs.pyi` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,88 +33,86 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
-    "AddTagsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchPredictionTypeDef",
     "CreateBatchPredictionInputRequestTypeDef",
-    "CreateBatchPredictionOutputTypeDef",
-    "CreateDataSourceFromRDSOutputTypeDef",
-    "CreateDataSourceFromRedshiftOutputTypeDef",
     "S3DataSpecTypeDef",
-    "CreateDataSourceFromS3OutputTypeDef",
     "CreateEvaluationInputRequestTypeDef",
-    "CreateEvaluationOutputTypeDef",
     "CreateMLModelInputRequestTypeDef",
-    "CreateMLModelOutputTypeDef",
     "CreateRealtimeEndpointInputRequestTypeDef",
     "RealtimeEndpointInfoTypeDef",
     "DeleteBatchPredictionInputRequestTypeDef",
-    "DeleteBatchPredictionOutputTypeDef",
     "DeleteDataSourceInputRequestTypeDef",
-    "DeleteDataSourceOutputTypeDef",
     "DeleteEvaluationInputRequestTypeDef",
-    "DeleteEvaluationOutputTypeDef",
     "DeleteMLModelInputRequestTypeDef",
-    "DeleteMLModelOutputTypeDef",
     "DeleteRealtimeEndpointInputRequestTypeDef",
     "DeleteTagsInputRequestTypeDef",
-    "DeleteTagsOutputTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBatchPredictionsInputRequestTypeDef",
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
     "DescribeDataSourcesInputRequestTypeDef",
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
     "DescribeEvaluationsInputRequestTypeDef",
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "DescribeMLModelsInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
-    "TagOutputTypeDef",
     "PerformanceMetricsTypeDef",
     "GetBatchPredictionInputRequestTypeDef",
-    "GetBatchPredictionOutputTypeDef",
     "GetDataSourceInputRequestTypeDef",
     "GetEvaluationInputRequestTypeDef",
     "GetMLModelInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PredictInputRequestTypeDef",
     "PredictionTypeDef",
     "RDSDatabaseCredentialsTypeDef",
     "RDSDatabaseTypeDef",
-    "RDSDatabaseOutputTypeDef",
     "RedshiftDatabaseCredentialsTypeDef",
     "RedshiftDatabaseTypeDef",
-    "RedshiftDatabaseOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateBatchPredictionInputRequestTypeDef",
-    "UpdateBatchPredictionOutputTypeDef",
     "UpdateDataSourceInputRequestTypeDef",
-    "UpdateDataSourceOutputTypeDef",
     "UpdateEvaluationInputRequestTypeDef",
-    "UpdateEvaluationOutputTypeDef",
     "UpdateMLModelInputRequestTypeDef",
-    "UpdateMLModelOutputTypeDef",
     "AddTagsInputRequestTypeDef",
+    "AddTagsOutputTypeDef",
+    "CreateBatchPredictionOutputTypeDef",
+    "CreateDataSourceFromRDSOutputTypeDef",
+    "CreateDataSourceFromRedshiftOutputTypeDef",
+    "CreateDataSourceFromS3OutputTypeDef",
+    "CreateEvaluationOutputTypeDef",
+    "CreateMLModelOutputTypeDef",
+    "DeleteBatchPredictionOutputTypeDef",
+    "DeleteDataSourceOutputTypeDef",
+    "DeleteEvaluationOutputTypeDef",
+    "DeleteMLModelOutputTypeDef",
+    "DeleteTagsOutputTypeDef",
+    "DescribeTagsOutputTypeDef",
+    "GetBatchPredictionOutputTypeDef",
+    "UpdateBatchPredictionOutputTypeDef",
+    "UpdateDataSourceOutputTypeDef",
+    "UpdateEvaluationOutputTypeDef",
+    "UpdateMLModelOutputTypeDef",
     "DescribeBatchPredictionsOutputTypeDef",
     "CreateDataSourceFromS3InputRequestTypeDef",
     "CreateRealtimeEndpointOutputTypeDef",
     "DeleteRealtimeEndpointOutputTypeDef",
     "GetMLModelOutputTypeDef",
     "MLModelTypeDef",
     "DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef",
     "DescribeDataSourcesInputDataSourceAvailableWaitTypeDef",
     "DescribeEvaluationsInputEvaluationAvailableWaitTypeDef",
     "DescribeMLModelsInputMLModelAvailableWaitTypeDef",
-    "DescribeTagsOutputTypeDef",
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "EvaluationTypeDef",
     "GetEvaluationOutputTypeDef",
     "PredictOutputTypeDef",
     "RDSDataSpecTypeDef",
     "RDSMetadataTypeDef",
     "RedshiftDataSpecTypeDef",
     "RedshiftMetadataTypeDef",
@@ -132,20 +130,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AddTagsOutputTypeDef = TypedDict(
-    "AddTagsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchPredictionTypeDef = TypedDict(
     "BatchPredictionTypeDef",
     {
         "BatchPredictionId": str,
@@ -181,43 +181,21 @@
     "_OptionalCreateBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionName": str,
     },
     total=False,
 )
 
+
 class CreateBatchPredictionInputRequestTypeDef(
     _RequiredCreateBatchPredictionInputRequestTypeDef,
     _OptionalCreateBatchPredictionInputRequestTypeDef,
 ):
     pass
 
-CreateBatchPredictionOutputTypeDef = TypedDict(
-    "CreateBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDataSourceFromRDSOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRDSOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRedshiftOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredS3DataSpecTypeDef = TypedDict(
     "_RequiredS3DataSpecTypeDef",
     {
         "DataLocationS3": str,
     },
 )
@@ -227,24 +205,18 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaLocationS3": str,
     },
     total=False,
 )
 
+
 class S3DataSpecTypeDef(_RequiredS3DataSpecTypeDef, _OptionalS3DataSpecTypeDef):
     pass
 
-CreateDataSourceFromS3OutputTypeDef = TypedDict(
-    "CreateDataSourceFromS3OutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateEvaluationInputRequestTypeDef = TypedDict(
     "_RequiredCreateEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
@@ -254,26 +226,20 @@
     "_OptionalCreateEvaluationInputRequestTypeDef",
     {
         "EvaluationName": str,
     },
     total=False,
 )
 
+
 class CreateEvaluationInputRequestTypeDef(
     _RequiredCreateEvaluationInputRequestTypeDef, _OptionalCreateEvaluationInputRequestTypeDef
 ):
     pass
 
-CreateEvaluationOutputTypeDef = TypedDict(
-    "CreateEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateMLModelInputRequestTypeDef = TypedDict(
     "_RequiredCreateMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
         "MLModelType": MLModelTypeType,
         "TrainingDataSourceId": str,
@@ -286,26 +252,20 @@
         "Parameters": Mapping[str, str],
         "Recipe": str,
         "RecipeUri": str,
     },
     total=False,
 )
 
+
 class CreateMLModelInputRequestTypeDef(
     _RequiredCreateMLModelInputRequestTypeDef, _OptionalCreateMLModelInputRequestTypeDef
 ):
     pass
 
-CreateMLModelOutputTypeDef = TypedDict(
-    "CreateMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 CreateRealtimeEndpointInputRequestTypeDef = TypedDict(
     "CreateRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
@@ -324,67 +284,35 @@
 DeleteBatchPredictionInputRequestTypeDef = TypedDict(
     "DeleteBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
-DeleteBatchPredictionOutputTypeDef = TypedDict(
-    "DeleteBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDataSourceInputRequestTypeDef = TypedDict(
     "DeleteDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 
-DeleteDataSourceOutputTypeDef = TypedDict(
-    "DeleteDataSourceOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEvaluationInputRequestTypeDef = TypedDict(
     "DeleteEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
     },
 )
 
-DeleteEvaluationOutputTypeDef = TypedDict(
-    "DeleteEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteMLModelInputRequestTypeDef = TypedDict(
     "DeleteMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
-DeleteMLModelOutputTypeDef = TypedDict(
-    "DeleteMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRealtimeEndpointInputRequestTypeDef = TypedDict(
     "DeleteRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
@@ -393,45 +321,29 @@
     {
         "TagKeys": Sequence[str],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
-DeleteTagsOutputTypeDef = TypedDict(
-    "DeleteTagsOutputTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "FilterVariable": BatchPredictionFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeBatchPredictionsInputRequestTypeDef = TypedDict(
     "DescribeBatchPredictionsInputRequestTypeDef",
     {
@@ -446,31 +358,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
-    {
-        "FilterVariable": DataSourceFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSourcesInputRequestTypeDef = TypedDict(
     "DescribeDataSourcesInputRequestTypeDef",
     {
         "FilterVariable": DataSourceFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -481,31 +376,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
-    {
-        "FilterVariable": EvaluationFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEvaluationsInputRequestTypeDef = TypedDict(
     "DescribeEvaluationsInputRequestTypeDef",
     {
         "FilterVariable": EvaluationFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -516,31 +394,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
-    {
-        "FilterVariable": MLModelFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeMLModelsInputRequestTypeDef = TypedDict(
     "DescribeMLModelsInputRequestTypeDef",
     {
         "FilterVariable": MLModelFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -559,23 +420,14 @@
     "DescribeTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 PerformanceMetricsTypeDef = TypedDict(
     "PerformanceMetricsTypeDef",
     {
         "Properties": Dict[str, str],
     },
     total=False,
 )
@@ -583,57 +435,35 @@
 GetBatchPredictionInputRequestTypeDef = TypedDict(
     "GetBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
-GetBatchPredictionOutputTypeDef = TypedDict(
-    "GetBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "MLModelId": str,
-        "BatchPredictionDataSourceId": str,
-        "InputDataLocationS3": str,
-        "CreatedByIamUser": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Name": str,
-        "Status": EntityStatusType,
-        "OutputUri": str,
-        "LogUri": str,
-        "Message": str,
-        "ComputeTime": int,
-        "FinishedAt": datetime,
-        "StartedAt": datetime,
-        "TotalRecordCount": int,
-        "InvalidRecordCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDataSourceInputRequestTypeDef = TypedDict(
     "_RequiredGetDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 _OptionalGetDataSourceInputRequestTypeDef = TypedDict(
     "_OptionalGetDataSourceInputRequestTypeDef",
     {
         "Verbose": bool,
     },
     total=False,
 )
 
+
 class GetDataSourceInputRequestTypeDef(
     _RequiredGetDataSourceInputRequestTypeDef, _OptionalGetDataSourceInputRequestTypeDef
 ):
     pass
 
+
 GetEvaluationInputRequestTypeDef = TypedDict(
     "GetEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
     },
 )
 
@@ -647,28 +477,20 @@
     "_OptionalGetMLModelInputRequestTypeDef",
     {
         "Verbose": bool,
     },
     total=False,
 )
 
+
 class GetMLModelInputRequestTypeDef(
     _RequiredGetMLModelInputRequestTypeDef, _OptionalGetMLModelInputRequestTypeDef
 ):
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
 
 PredictInputRequestTypeDef = TypedDict(
     "PredictInputRequestTypeDef",
     {
         "MLModelId": str,
         "Record": Mapping[str, str],
         "PredictEndpoint": str,
@@ -698,22 +520,14 @@
     "RDSDatabaseTypeDef",
     {
         "InstanceIdentifier": str,
         "DatabaseName": str,
     },
 )
 
-RDSDatabaseOutputTypeDef = TypedDict(
-    "RDSDatabaseOutputTypeDef",
-    {
-        "InstanceIdentifier": str,
-        "DatabaseName": str,
-    },
-)
-
 RedshiftDatabaseCredentialsTypeDef = TypedDict(
     "RedshiftDatabaseCredentialsTypeDef",
     {
         "Username": str,
         "Password": str,
     },
 )
@@ -722,124 +536,239 @@
     "RedshiftDatabaseTypeDef",
     {
         "DatabaseName": str,
         "ClusterIdentifier": str,
     },
 )
 
-RedshiftDatabaseOutputTypeDef = TypedDict(
-    "RedshiftDatabaseOutputTypeDef",
+UpdateBatchPredictionInputRequestTypeDef = TypedDict(
+    "UpdateBatchPredictionInputRequestTypeDef",
     {
-        "DatabaseName": str,
-        "ClusterIdentifier": str,
+        "BatchPredictionId": str,
+        "BatchPredictionName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UpdateDataSourceInputRequestTypeDef = TypedDict(
+    "UpdateDataSourceInputRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DataSourceId": str,
+        "DataSourceName": str,
     },
 )
 
-UpdateBatchPredictionInputRequestTypeDef = TypedDict(
-    "UpdateBatchPredictionInputRequestTypeDef",
+UpdateEvaluationInputRequestTypeDef = TypedDict(
+    "UpdateEvaluationInputRequestTypeDef",
     {
-        "BatchPredictionId": str,
-        "BatchPredictionName": str,
+        "EvaluationId": str,
+        "EvaluationName": str,
     },
 )
 
-UpdateBatchPredictionOutputTypeDef = TypedDict(
-    "UpdateBatchPredictionOutputTypeDef",
+_RequiredUpdateMLModelInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateMLModelInputRequestTypeDef",
+    {
+        "MLModelId": str,
+    },
+)
+_OptionalUpdateMLModelInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateMLModelInputRequestTypeDef",
+    {
+        "MLModelName": str,
+        "ScoreThreshold": float,
+    },
+    total=False,
+)
+
+
+class UpdateMLModelInputRequestTypeDef(
+    _RequiredUpdateMLModelInputRequestTypeDef, _OptionalUpdateMLModelInputRequestTypeDef
+):
+    pass
+
+
+AddTagsInputRequestTypeDef = TypedDict(
+    "AddTagsInputRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+    },
+)
+
+AddTagsOutputTypeDef = TypedDict(
+    "AddTagsOutputTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBatchPredictionOutputTypeDef = TypedDict(
+    "CreateBatchPredictionOutputTypeDef",
     {
         "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDataSourceInputRequestTypeDef = TypedDict(
-    "UpdateDataSourceInputRequestTypeDef",
+CreateDataSourceFromRDSOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRDSOutputTypeDef",
     {
         "DataSourceId": str,
-        "DataSourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDataSourceOutputTypeDef = TypedDict(
-    "UpdateDataSourceOutputTypeDef",
+CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRedshiftOutputTypeDef",
     {
         "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateEvaluationInputRequestTypeDef = TypedDict(
-    "UpdateEvaluationInputRequestTypeDef",
+CreateDataSourceFromS3OutputTypeDef = TypedDict(
+    "CreateDataSourceFromS3OutputTypeDef",
     {
-        "EvaluationId": str,
-        "EvaluationName": str,
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateEvaluationOutputTypeDef = TypedDict(
-    "UpdateEvaluationOutputTypeDef",
+CreateEvaluationOutputTypeDef = TypedDict(
+    "CreateEvaluationOutputTypeDef",
     {
         "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateMLModelInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateMLModelInputRequestTypeDef",
+CreateMLModelOutputTypeDef = TypedDict(
+    "CreateMLModelOutputTypeDef",
     {
         "MLModelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateMLModelInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateMLModelInputRequestTypeDef",
+
+DeleteBatchPredictionOutputTypeDef = TypedDict(
+    "DeleteBatchPredictionOutputTypeDef",
     {
-        "MLModelName": str,
-        "ScoreThreshold": float,
+        "BatchPredictionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateMLModelInputRequestTypeDef(
-    _RequiredUpdateMLModelInputRequestTypeDef, _OptionalUpdateMLModelInputRequestTypeDef
-):
-    pass
+DeleteDataSourceOutputTypeDef = TypedDict(
+    "DeleteDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateMLModelOutputTypeDef = TypedDict(
-    "UpdateMLModelOutputTypeDef",
+DeleteEvaluationOutputTypeDef = TypedDict(
+    "DeleteEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteMLModelOutputTypeDef = TypedDict(
+    "DeleteMLModelOutputTypeDef",
     {
         "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddTagsInputRequestTypeDef = TypedDict(
-    "AddTagsInputRequestTypeDef",
+DeleteTagsOutputTypeDef = TypedDict(
+    "DeleteTagsOutputTypeDef",
     {
-        "Tags": Sequence[TagTypeDef],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBatchPredictionOutputTypeDef = TypedDict(
+    "GetBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "MLModelId": str,
+        "BatchPredictionDataSourceId": str,
+        "InputDataLocationS3": str,
+        "CreatedByIamUser": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Name": str,
+        "Status": EntityStatusType,
+        "OutputUri": str,
+        "LogUri": str,
+        "Message": str,
+        "ComputeTime": int,
+        "FinishedAt": datetime,
+        "StartedAt": datetime,
+        "TotalRecordCount": int,
+        "InvalidRecordCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBatchPredictionOutputTypeDef = TypedDict(
+    "UpdateBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDataSourceOutputTypeDef = TypedDict(
+    "UpdateDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEvaluationOutputTypeDef = TypedDict(
+    "UpdateEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMLModelOutputTypeDef = TypedDict(
+    "UpdateMLModelOutputTypeDef",
+    {
+        "MLModelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBatchPredictionsOutputTypeDef = TypedDict(
     "DescribeBatchPredictionsOutputTypeDef",
     {
         "Results": List[BatchPredictionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceFromS3InputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromS3InputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -851,35 +780,37 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
+
 class CreateDataSourceFromS3InputRequestTypeDef(
     _RequiredCreateDataSourceFromS3InputRequestTypeDef,
     _OptionalCreateDataSourceFromS3InputRequestTypeDef,
 ):
     pass
 
+
 CreateRealtimeEndpointOutputTypeDef = TypedDict(
     "CreateRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRealtimeEndpointOutputTypeDef = TypedDict(
     "DeleteRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMLModelOutputTypeDef = TypedDict(
     "GetMLModelOutputTypeDef",
     {
         "MLModelId": str,
@@ -899,15 +830,15 @@
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "Recipe": str,
         "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MLModelTypeDef = TypedDict(
     "MLModelTypeDef",
     {
         "MLModelId": str,
@@ -1005,22 +936,80 @@
         "NextToken": str,
         "Limit": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
+DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
     {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FilterVariable": BatchPredictionFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
+    {
+        "FilterVariable": DataSourceFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
+    {
+        "FilterVariable": EvaluationFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
+    {
+        "FilterVariable": MLModelFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 EvaluationTypeDef = TypedDict(
     "EvaluationTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
@@ -1054,23 +1043,23 @@
         "Status": EntityStatusType,
         "PerformanceMetrics": PerformanceMetricsTypeDef,
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictOutputTypeDef = TypedDict(
     "PredictOutputTypeDef",
     {
         "Prediction": PredictionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRDSDataSpecTypeDef = TypedDict(
     "_RequiredRDSDataSpecTypeDef",
     {
         "DatabaseInformation": RDSDatabaseTypeDef,
@@ -1089,21 +1078,23 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaUri": str,
     },
     total=False,
 )
 
+
 class RDSDataSpecTypeDef(_RequiredRDSDataSpecTypeDef, _OptionalRDSDataSpecTypeDef):
     pass
 
+
 RDSMetadataTypeDef = TypedDict(
     "RDSMetadataTypeDef",
     {
-        "Database": RDSDatabaseOutputTypeDef,
+        "Database": RDSDatabaseTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
         "ResourceRole": str,
         "ServiceRole": str,
         "DataPipelineId": str,
     },
     total=False,
@@ -1124,42 +1115,44 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaUri": str,
     },
     total=False,
 )
 
+
 class RedshiftDataSpecTypeDef(_RequiredRedshiftDataSpecTypeDef, _OptionalRedshiftDataSpecTypeDef):
     pass
 
+
 RedshiftMetadataTypeDef = TypedDict(
     "RedshiftMetadataTypeDef",
     {
-        "RedshiftDatabase": RedshiftDatabaseOutputTypeDef,
+        "RedshiftDatabase": RedshiftDatabaseTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
     },
     total=False,
 )
 
 DescribeMLModelsOutputTypeDef = TypedDict(
     "DescribeMLModelsOutputTypeDef",
     {
         "Results": List[MLModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEvaluationsOutputTypeDef = TypedDict(
     "DescribeEvaluationsOutputTypeDef",
     {
         "Results": List[EvaluationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceFromRDSInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromRDSInputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -1172,20 +1165,22 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
+
 class CreateDataSourceFromRDSInputRequestTypeDef(
     _RequiredCreateDataSourceFromRDSInputRequestTypeDef,
     _OptionalCreateDataSourceFromRDSInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDataSourceFromRedshiftInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromRedshiftInputRequestTypeDef",
     {
         "DataSourceId": str,
         "DataSpec": RedshiftDataSpecTypeDef,
         "RoleARN": str,
     },
@@ -1195,20 +1190,22 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
+
 class CreateDataSourceFromRedshiftInputRequestTypeDef(
     _RequiredCreateDataSourceFromRedshiftInputRequestTypeDef,
     _OptionalCreateDataSourceFromRedshiftInputRequestTypeDef,
 ):
     pass
 
+
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "DataSourceId": str,
         "DataLocationS3": str,
         "DataRearrangement": str,
         "CreatedByIamUser": str,
@@ -1249,19 +1246,19 @@
         "RDSMetadata": RDSMetadataTypeDef,
         "RoleARN": str,
         "ComputeStatistics": bool,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "DataSourceSchema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSourcesOutputTypeDef = TypedDict(
     "DescribeDataSourcesOutputTypeDef",
     {
         "Results": List[DataSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/waiter.py` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning/waiter.pyi` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/PKG-INFO` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-machinelearning
-Version: 1.28.12
-Summary: Type annotations for boto3.MachineLearning 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MachineLearning 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-machinelearning.svg?color=blue)](https://pypi.org/project/mypy-boto3-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-machinelearning)](https://pepy.tech/project/mypy-boto3-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MachineLearning 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[boto3.MachineLearning 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [mypy-boto3-machinelearning docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -385,86 +385,83 @@
 
 `mypy_boto3_machinelearning.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_machinelearning.type_defs import (
     TagTypeDef,
-    AddTagsOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchPredictionTypeDef,
     CreateBatchPredictionInputRequestTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
     S3DataSpecTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
     CreateEvaluationInputRequestTypeDef,
-    CreateEvaluationOutputTypeDef,
     CreateMLModelInputRequestTypeDef,
-    CreateMLModelOutputTypeDef,
     CreateRealtimeEndpointInputRequestTypeDef,
     RealtimeEndpointInfoTypeDef,
     DeleteBatchPredictionInputRequestTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
     DeleteDataSourceInputRequestTypeDef,
-    DeleteDataSourceOutputTypeDef,
     DeleteEvaluationInputRequestTypeDef,
-    DeleteEvaluationOutputTypeDef,
     DeleteMLModelInputRequestTypeDef,
-    DeleteMLModelOutputTypeDef,
     DeleteRealtimeEndpointInputRequestTypeDef,
     DeleteTagsInputRequestTypeDef,
-    DeleteTagsOutputTypeDef,
     WaiterConfigTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBatchPredictionsInputRequestTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
-    TagOutputTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
-    GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
-    RDSDatabaseOutputTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
-    RedshiftDatabaseOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
-    UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
-    UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
-    UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    AddTagsOutputTypeDef,
+    CreateBatchPredictionOutputTypeDef,
+    CreateDataSourceFromRDSOutputTypeDef,
+    CreateDataSourceFromRedshiftOutputTypeDef,
+    CreateDataSourceFromS3OutputTypeDef,
+    CreateEvaluationOutputTypeDef,
+    CreateMLModelOutputTypeDef,
+    DeleteBatchPredictionOutputTypeDef,
+    DeleteDataSourceOutputTypeDef,
+    DeleteEvaluationOutputTypeDef,
+    DeleteMLModelOutputTypeDef,
+    DeleteTagsOutputTypeDef,
+    DescribeTagsOutputTypeDef,
+    GetBatchPredictionOutputTypeDef,
+    UpdateBatchPredictionOutputTypeDef,
+    UpdateDataSourceOutputTypeDef,
+    UpdateEvaluationOutputTypeDef,
+    UpdateMLModelOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
-    DescribeTagsOutputTypeDef,
+    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
+    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
+    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
```

### Comparing `mypy-boto3-machinelearning-1.28.12/mypy_boto3_machinelearning.egg-info/SOURCES.txt` & `mypy-boto3-machinelearning-1.28.15/mypy_boto3_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-machinelearning-1.28.12/setup.py` & `mypy-boto3-machinelearning-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-machinelearning",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_machinelearning"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MachineLearning 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MachineLearning 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

