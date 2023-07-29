# Comparing `tmp/mypy-boto3-compute-optimizer-1.28.12.tar.gz` & `tmp/mypy-boto3-compute-optimizer-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-compute-optimizer-1.28.12.tar", last modified: Thu Jul 27 05:34:31 2023, max compression
+gzip compressed data, was "mypy-boto3-compute-optimizer-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
```

## Comparing `mypy-boto3-compute-optimizer-1.28.12.tar` & `mypy-boto3-compute-optimizer-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.136544 mypy-boto3-compute-optimizer-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-27 05:34:31.136544 mypy-boto3-compute-optimizer-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.136544 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-07-27 05:19:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    23987 2023-07-27 05:19:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42449 2023-07-27 05:19:31.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42426 2023-07-27 05:19:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.136544 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:30.000000 mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:31.136544 mypy-boto3-compute-optimizer-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:19:29.000000 mypy-boto3-compute-optimizer-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.116904 mypy-boto3-compute-optimizer-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:05.000000 mypy-boto3-compute-optimizer-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-07-28 20:42:34.108904 mypy-boto3-compute-optimizer-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-28 20:22:05.000000 mypy-boto3-compute-optimizer-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.096904 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-28 20:22:05.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-28 20:22:05.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:22:05.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-07-28 20:22:06.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-07-28 20:22:06.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-07-28 20:22:06.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23987 2023-07-28 20:22:06.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-28 20:22:06.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-07-28 20:22:06.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:05.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41985 2023-07-28 20:22:07.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41962 2023-07-28 20:22:07.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:05.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.108904 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-07-28 20:42:33.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:42:33.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:33.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:33.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:33.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:33.000000 mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.116904 mypy-boto3-compute-optimizer-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 20:22:05.000000 mypy-boto3-compute-optimizer-1.28.15/setup.py
```

### Comparing `mypy-boto3-compute-optimizer-1.28.12/LICENSE` & `mypy-boto3-compute-optimizer-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.12/PKG-INFO` & `mypy-boto3-compute-optimizer-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-compute-optimizer
-Version: 1.28.12
-Summary: Type annotations for boto3.ComputeOptimizer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ComputeOptimizer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-compute-optimizer)](https://pepy.tech/project/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,61 +399,61 @@
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
     CurrentPerformanceRiskRatingsTypeDef,
     ScopeTypeDef,
     JobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
     TagTypeDef,
-    ExternalMetricsPreferenceOutputTypeDef,
+    ExternalMetricsPreferenceTypeDef,
     EnrollmentFilterTypeDef,
     EstimatedMonthlySavingsTypeDef,
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
-    ExternalMetricsPreferenceTypeDef,
     GetRecommendationErrorTypeDef,
     GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
-    GetEnrollmentStatusResponseTypeDef,
-    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
-    PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
-    ScopeOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
-    UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
-    GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
     DeleteRecommendationPreferencesRequestRequestTypeDef,
-    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
     GetRecommendationPreferencesRequestRequestTypeDef,
-    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
     DescribeRecommendationExportJobsRequestRequestTypeDef,
+    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
+    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
+    GetEnrollmentStatusResponseTypeDef,
+    GetEnrollmentStatusesForOrganizationResponseTypeDef,
+    UpdateEnrollmentStatusResponseTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
+    PutRecommendationPreferencesRequestRequestTypeDef,
+    RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
     GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
@@ -466,29 +466,27 @@
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
-    PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
-    RecommendationPreferencesDetailTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
+    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
     InstanceRecommendationOptionTypeDef,
     LambdaFunctionMemoryRecommendationOptionTypeDef,
     VolumeRecommendationOptionTypeDef,
     RecommendationExportJobTypeDef,
     GetEC2RecommendationProjectedMetricsResponseTypeDef,
     RecommendationSummaryTypeDef,
-    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationTypeDef,
     ECSServiceRecommendationTypeDef,
     InstanceRecommendationTypeDef,
     LambdaFunctionRecommendationTypeDef,
     VolumeRecommendationTypeDef,
     DescribeRecommendationExportJobsResponseTypeDef,
     GetRecommendationSummariesResponseTypeDef,
```

### Comparing `mypy-boto3-compute-optimizer-1.28.12/README.md` & `mypy-boto3-compute-optimizer-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-compute-optimizer)](https://pepy.tech/project/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,61 +367,61 @@
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
     CurrentPerformanceRiskRatingsTypeDef,
     ScopeTypeDef,
     JobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
     TagTypeDef,
-    ExternalMetricsPreferenceOutputTypeDef,
+    ExternalMetricsPreferenceTypeDef,
     EnrollmentFilterTypeDef,
     EstimatedMonthlySavingsTypeDef,
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
-    ExternalMetricsPreferenceTypeDef,
     GetRecommendationErrorTypeDef,
     GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
-    GetEnrollmentStatusResponseTypeDef,
-    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
-    PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
-    ScopeOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
-    UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
-    GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
     DeleteRecommendationPreferencesRequestRequestTypeDef,
-    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
     GetRecommendationPreferencesRequestRequestTypeDef,
-    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
     DescribeRecommendationExportJobsRequestRequestTypeDef,
+    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
+    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
+    GetEnrollmentStatusResponseTypeDef,
+    GetEnrollmentStatusesForOrganizationResponseTypeDef,
+    UpdateEnrollmentStatusResponseTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
+    PutRecommendationPreferencesRequestRequestTypeDef,
+    RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
     GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
@@ -434,29 +434,27 @@
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
-    PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
-    RecommendationPreferencesDetailTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
+    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
     InstanceRecommendationOptionTypeDef,
     LambdaFunctionMemoryRecommendationOptionTypeDef,
     VolumeRecommendationOptionTypeDef,
     RecommendationExportJobTypeDef,
     GetEC2RecommendationProjectedMetricsResponseTypeDef,
     RecommendationSummaryTypeDef,
-    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationTypeDef,
     ECSServiceRecommendationTypeDef,
     InstanceRecommendationTypeDef,
     LambdaFunctionRecommendationTypeDef,
     VolumeRecommendationTypeDef,
     DescribeRecommendationExportJobsResponseTypeDef,
     GetRecommendationSummariesResponseTypeDef,
```

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__init__.py` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__init__.pyi` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/__main__.py` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ComputeOptimizer 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ComputeOptimizer 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer\nOther"
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

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/client.py` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/client.pyi` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/literals.py` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/literals.pyi` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/paginator.py` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,107 +49,100 @@
     "DescribeRecommendationExportJobsPaginator",
     "GetEnrollmentStatusesForOrganizationPaginator",
     "GetLambdaFunctionRecommendationsPaginator",
     "GetRecommendationPreferencesPaginator",
     "GetRecommendationSummariesPaginator",
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
 class DescribeRecommendationExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#describerecommendationexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRecommendationExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#describerecommendationexportjobspaginator)
         """
 
-
 class GetEnrollmentStatusesForOrganizationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetEnrollmentStatusesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
         """
 
-
 class GetLambdaFunctionRecommendationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getlambdafunctionrecommendationspaginator)
     """
 
     def paginate(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetLambdaFunctionRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getlambdafunctionrecommendationspaginator)
         """
 
-
 class GetRecommendationPreferencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationPreferences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationpreferencespaginator)
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRecommendationPreferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationPreferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationpreferencespaginator)
         """
 
-
 class GetRecommendationSummariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationsummariespaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRecommendationSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationsummariespaginator)
         """
```

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/paginator.pyi` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,100 +49,107 @@
     "DescribeRecommendationExportJobsPaginator",
     "GetEnrollmentStatusesForOrganizationPaginator",
     "GetLambdaFunctionRecommendationsPaginator",
     "GetRecommendationPreferencesPaginator",
     "GetRecommendationSummariesPaginator",
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
 class DescribeRecommendationExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#describerecommendationexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRecommendationExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#describerecommendationexportjobspaginator)
         """
 
+
 class GetEnrollmentStatusesForOrganizationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetEnrollmentStatusesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
         """
 
+
 class GetLambdaFunctionRecommendationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getlambdafunctionrecommendationspaginator)
     """
 
     def paginate(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetLambdaFunctionRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getlambdafunctionrecommendationspaginator)
         """
 
+
 class GetRecommendationPreferencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationPreferences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationpreferencespaginator)
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRecommendationPreferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationPreferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationpreferencespaginator)
         """
 
+
 class GetRecommendationSummariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationsummariespaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRecommendationSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/paginators/#getrecommendationsummariespaginator)
         """
```

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/type_defs.py` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,61 +76,61 @@
     "AccountEnrollmentStatusTypeDef",
     "AutoScalingGroupConfigurationTypeDef",
     "UtilizationMetricTypeDef",
     "MemorySizeConfigurationTypeDef",
     "CurrentPerformanceRiskRatingsTypeDef",
     "ScopeTypeDef",
     "JobFilterTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "EBSFilterTypeDef",
     "EBSUtilizationMetricTypeDef",
     "ECSServiceProjectedMetricTypeDef",
     "ECSServiceProjectedUtilizationMetricTypeDef",
     "ECSServiceRecommendationFilterTypeDef",
     "ECSServiceUtilizationMetricTypeDef",
     "TagTypeDef",
-    "ExternalMetricsPreferenceOutputTypeDef",
+    "ExternalMetricsPreferenceTypeDef",
     "EnrollmentFilterTypeDef",
     "EstimatedMonthlySavingsTypeDef",
     "FilterTypeDef",
     "RecommendationPreferencesTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "LambdaFunctionRecommendationFilterTypeDef",
     "ExternalMetricStatusTypeDef",
-    "ExternalMetricsPreferenceTypeDef",
     "GetRecommendationErrorTypeDef",
     "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
-    "GetEnrollmentStatusResponseTypeDef",
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
     "GetRecommendationSummariesRequestRequestTypeDef",
     "RecommendationSourceTypeDef",
     "LambdaFunctionMemoryProjectedMetricTypeDef",
     "LambdaFunctionUtilizationMetricTypeDef",
-    "PaginatorConfigTypeDef",
     "ProjectedMetricTypeDef",
     "ReasonCodeSummaryTypeDef",
-    "ScopeOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateEnrollmentStatusRequestRequestTypeDef",
-    "UpdateEnrollmentStatusResponseTypeDef",
     "VolumeConfigurationTypeDef",
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
     "ContainerConfigurationTypeDef",
     "ContainerRecommendationTypeDef",
     "DeleteRecommendationPreferencesRequestRequestTypeDef",
-    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     "GetRecommendationPreferencesRequestRequestTypeDef",
-    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
     "DescribeRecommendationExportJobsRequestRequestTypeDef",
+    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
+    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
+    "GetEnrollmentStatusResponseTypeDef",
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+    "UpdateEnrollmentStatusResponseTypeDef",
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     "ECSServiceRecommendedOptionProjectedMetricTypeDef",
     "GetECSServiceRecommendationsRequestRequestTypeDef",
     "EffectiveRecommendationPreferencesTypeDef",
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
+    "PutRecommendationPreferencesRequestRequestTypeDef",
+    "RecommendationPreferencesDetailTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     "InferredWorkloadSavingTypeDef",
     "SavingsOpportunityTypeDef",
     "GetAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "GetEC2InstanceRecommendationsRequestRequestTypeDef",
     "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
@@ -143,29 +143,27 @@
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     "ExportECSServiceRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
-    "PutRecommendationPreferencesRequestRequestTypeDef",
     "RecommendedOptionProjectedMetricTypeDef",
     "SummaryTypeDef",
-    "RecommendationPreferencesDetailTypeDef",
     "ServiceConfigurationTypeDef",
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
+    "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationOptionTypeDef",
     "ECSServiceRecommendationOptionTypeDef",
     "InstanceRecommendationOptionTypeDef",
     "LambdaFunctionMemoryRecommendationOptionTypeDef",
     "VolumeRecommendationOptionTypeDef",
     "RecommendationExportJobTypeDef",
     "GetEC2RecommendationProjectedMetricsResponseTypeDef",
     "RecommendationSummaryTypeDef",
-    "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationTypeDef",
     "ECSServiceRecommendationTypeDef",
     "InstanceRecommendationTypeDef",
     "LambdaFunctionRecommendationTypeDef",
     "VolumeRecommendationTypeDef",
     "DescribeRecommendationExportJobsResponseTypeDef",
     "GetRecommendationSummariesResponseTypeDef",
@@ -242,14 +240,35 @@
     {
         "name": JobFilterNameType,
         "values": Sequence[str],
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
 EBSFilterTypeDef = TypedDict(
     "EBSFilterTypeDef",
     {
         "name": Literal["Finding"],
         "values": Sequence[str],
     },
     total=False,
@@ -311,16 +330,16 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-ExternalMetricsPreferenceOutputTypeDef = TypedDict(
-    "ExternalMetricsPreferenceOutputTypeDef",
+ExternalMetricsPreferenceTypeDef = TypedDict(
+    "ExternalMetricsPreferenceTypeDef",
     {
         "source": ExternalMetricsSourceType,
     },
     total=False,
 )
 
 EnrollmentFilterTypeDef = TypedDict(
@@ -391,22 +410,14 @@
     {
         "statusCode": ExternalMetricStatusCodeType,
         "statusReason": str,
     },
     total=False,
 )
 
-ExternalMetricsPreferenceTypeDef = TypedDict(
-    "ExternalMetricsPreferenceTypeDef",
-    {
-        "source": ExternalMetricsSourceType,
-    },
-    total=False,
-)
-
 GetRecommendationErrorTypeDef = TypedDict(
     "GetRecommendationErrorTypeDef",
     {
         "identifier": str,
         "code": str,
         "message": str,
     },
@@ -427,35 +438,14 @@
 GetEffectiveRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetEnrollmentStatusResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "memberAccountsEnrolled": bool,
-        "lastUpdatedTimestamp": datetime,
-        "numberOfMemberAccountsOptedIn": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
-    {
-        "accountIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRecommendationSummariesRequestRequestTypeDef = TypedDict(
     "GetRecommendationSummariesRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -487,24 +477,14 @@
         "name": LambdaFunctionMetricNameType,
         "statistic": LambdaFunctionMetricStatisticType,
         "value": float,
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
 ProjectedMetricTypeDef = TypedDict(
     "ProjectedMetricTypeDef",
     {
         "name": MetricNameType,
         "timestamps": List[datetime],
         "values": List[float],
     },
@@ -516,34 +496,14 @@
     {
         "name": FindingReasonCodeType,
         "value": float,
     },
     total=False,
 )
 
-ScopeOutputTypeDef = TypedDict(
-    "ScopeOutputTypeDef",
-    {
-        "name": ScopeNameType,
-        "value": str,
-    },
-    total=False,
-)
-
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
 _RequiredUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnrollmentStatusRequestRequestTypeDef",
     {
         "status": StatusType,
     },
 )
 _OptionalUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
@@ -558,46 +518,28 @@
 class UpdateEnrollmentStatusRequestRequestTypeDef(
     _RequiredUpdateEnrollmentStatusRequestRequestTypeDef,
     _OptionalUpdateEnrollmentStatusRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateEnrollmentStatusResponseTypeDef = TypedDict(
-    "UpdateEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VolumeConfigurationTypeDef = TypedDict(
     "VolumeConfigurationTypeDef",
     {
         "volumeType": str,
         "volumeSize": int,
         "volumeBaselineIOPS": int,
         "volumeBurstIOPS": int,
         "volumeBaselineThroughput": int,
         "volumeBurstThroughput": int,
         "rootVolume": bool,
     },
     total=False,
 )
 
-GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
-    {
-        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ContainerConfigurationTypeDef = TypedDict(
     "ContainerConfigurationTypeDef",
     {
         "containerName": str,
         "memorySizeConfiguration": MemorySizeConfigurationTypeDef,
         "cpu": int,
     },
@@ -633,80 +575,119 @@
 class DeleteRecommendationPreferencesRequestRequestTypeDef(
     _RequiredDeleteRecommendationPreferencesRequestRequestTypeDef,
     _OptionalDeleteRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+_RequiredGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
-_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+_OptionalGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetRecommendationPreferencesRequestRequestTypeDef",
     {
         "scope": ScopeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
-class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
-    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+class GetRecommendationPreferencesRequestRequestTypeDef(
+    _RequiredGetRecommendationPreferencesRequestRequestTypeDef,
+    _OptionalGetRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetRecommendationPreferencesRequestRequestTypeDef",
+DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestRequestTypeDef",
+    {
+        "jobIds": Sequence[str],
+        "filters": Sequence[JobFilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
+    {
+        "jobIds": Sequence[str],
+        "filters": Sequence[JobFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
-_OptionalGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetRecommendationPreferencesRequestRequestTypeDef",
+_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     {
         "scope": ScopeTypeDef,
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class GetRecommendationPreferencesRequestRequestTypeDef(
-    _RequiredGetRecommendationPreferencesRequestRequestTypeDef,
-    _OptionalGetRecommendationPreferencesRequestRequestTypeDef,
+class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
+    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
 ):
     pass
 
 
-DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
+GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
     {
-        "jobIds": Sequence[str],
-        "filters": Sequence[JobFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "accountIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestRequestTypeDef",
+GetEnrollmentStatusResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusResponseTypeDef",
     {
-        "jobIds": Sequence[str],
-        "filters": Sequence[JobFilterTypeDef],
+        "status": StatusType,
+        "statusReason": str,
+        "memberAccountsEnrolled": bool,
+        "lastUpdatedTimestamp": datetime,
+        "numberOfMemberAccountsOptedIn": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+    {
+        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
         "nextToken": str,
-        "maxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEnrollmentStatusResponseTypeDef = TypedDict(
+    "UpdateEnrollmentStatusResponseTypeDef",
+    {
+        "status": StatusType,
+        "statusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetEBSVolumeRecommendationsRequestRequestTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     {
         "volumeArns": Sequence[str],
         "nextToken": str,
@@ -741,33 +722,70 @@
 
 EffectiveRecommendationPreferencesTypeDef = TypedDict(
     "EffectiveRecommendationPreferencesTypeDef",
     {
         "cpuVendorArchitectures": List[CpuVendorArchitectureType],
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
         "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
+        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
     },
     total=False,
 )
 
 GetEffectiveRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     {
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+    },
+)
+_OptionalPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRecommendationPreferencesRequestRequestTypeDef",
+    {
+        "scope": ScopeTypeDef,
+        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
+        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
+        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+    },
+    total=False,
+)
+
+
+class PutRecommendationPreferencesRequestRequestTypeDef(
+    _RequiredPutRecommendationPreferencesRequestRequestTypeDef,
+    _OptionalPutRecommendationPreferencesRequestRequestTypeDef,
+):
+    pass
+
+
+RecommendationPreferencesDetailTypeDef = TypedDict(
+    "RecommendationPreferencesDetailTypeDef",
+    {
+        "scope": ScopeTypeDef,
+        "resourceType": ResourceTypeType,
+        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
+        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
+        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+    },
+    total=False,
+)
+
 GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     {
         "filters": Sequence[EnrollmentFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetEnrollmentStatusesForOrganizationRequestRequestTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     {
@@ -955,15 +973,15 @@
 
 
 ExportAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "ExportAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportDestinationTypeDef = TypedDict(
     "ExportDestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
@@ -972,42 +990,42 @@
 )
 
 ExportEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportECSServiceRecommendationsResponseTypeDef = TypedDict(
     "ExportECSServiceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
         "s3DestinationConfig": S3DestinationConfigTypeDef,
@@ -1035,15 +1053,15 @@
 
 GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     {
         "functionArns": Sequence[str],
         "accountIds": Sequence[str],
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
@@ -1052,39 +1070,14 @@
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-    },
-)
-_OptionalPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRecommendationPreferencesRequestRequestTypeDef",
-    {
-        "scope": ScopeTypeDef,
-        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
-    },
-    total=False,
-)
-
-
-class PutRecommendationPreferencesRequestRequestTypeDef(
-    _RequiredPutRecommendationPreferencesRequestRequestTypeDef,
-    _OptionalPutRecommendationPreferencesRequestRequestTypeDef,
-):
-    pass
-
-
 RecommendedOptionProjectedMetricTypeDef = TypedDict(
     "RecommendedOptionProjectedMetricTypeDef",
     {
         "recommendedInstanceType": str,
         "rank": int,
         "projectedMetrics": List[ProjectedMetricTypeDef],
     },
@@ -1097,26 +1090,14 @@
         "name": FindingType,
         "value": float,
         "reasonCodeSummaries": List[ReasonCodeSummaryTypeDef],
     },
     total=False,
 )
 
-RecommendationPreferencesDetailTypeDef = TypedDict(
-    "RecommendationPreferencesDetailTypeDef",
-    {
-        "scope": ScopeOutputTypeDef,
-        "resourceType": ResourceTypeType,
-        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
-    },
-    total=False,
-)
-
 ServiceConfigurationTypeDef = TypedDict(
     "ServiceConfigurationTypeDef",
     {
         "memory": int,
         "cpu": int,
         "containerConfigurations": List[ContainerConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationType,
@@ -1127,15 +1108,24 @@
 
 GetECSServiceRecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[
             ECSServiceRecommendedOptionProjectedMetricTypeDef
         ],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRecommendationPreferencesResponseTypeDef = TypedDict(
+    "GetRecommendationPreferencesResponseTypeDef",
+    {
+        "nextToken": str,
+        "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoScalingGroupRecommendationOptionTypeDef = TypedDict(
     "AutoScalingGroupRecommendationOptionTypeDef",
     {
         "configuration": AutoScalingGroupConfigurationTypeDef,
@@ -1210,15 +1200,15 @@
     total=False,
 )
 
 GetEC2RecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetEC2RecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[RecommendedOptionProjectedMetricTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "summaries": List[SummaryTypeDef],
@@ -1227,23 +1217,14 @@
         "savingsOpportunity": SavingsOpportunityTypeDef,
         "currentPerformanceRiskRatings": CurrentPerformanceRiskRatingsTypeDef,
         "inferredWorkloadSavings": List[InferredWorkloadSavingTypeDef],
     },
     total=False,
 )
 
-GetRecommendationPreferencesResponseTypeDef = TypedDict(
-    "GetRecommendationPreferencesResponseTypeDef",
-    {
-        "nextToken": str,
-        "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AutoScalingGroupRecommendationTypeDef = TypedDict(
     "AutoScalingGroupRecommendationTypeDef",
     {
         "accountId": str,
         "autoScalingGroupArn": str,
         "autoScalingGroupName": str,
         "finding": FindingType,
@@ -1340,68 +1321,68 @@
 )
 
 DescribeRecommendationExportJobsResponseTypeDef = TypedDict(
     "DescribeRecommendationExportJobsResponseTypeDef",
     {
         "recommendationExportJobs": List[RecommendationExportJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationSummariesResponseTypeDef = TypedDict(
     "GetRecommendationSummariesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationSummaries": List[RecommendationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "GetAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "autoScalingGroupRecommendations": List[AutoScalingGroupRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetECSServiceRecommendationsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "ecsServiceRecommendations": List[ECSServiceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "GetEC2InstanceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "instanceRecommendations": List[InstanceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "lambdaFunctionRecommendations": List[LambdaFunctionRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "volumeRecommendations": List[VolumeRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer/type_defs.pyi` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -75,61 +75,61 @@
     "AccountEnrollmentStatusTypeDef",
     "AutoScalingGroupConfigurationTypeDef",
     "UtilizationMetricTypeDef",
     "MemorySizeConfigurationTypeDef",
     "CurrentPerformanceRiskRatingsTypeDef",
     "ScopeTypeDef",
     "JobFilterTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "EBSFilterTypeDef",
     "EBSUtilizationMetricTypeDef",
     "ECSServiceProjectedMetricTypeDef",
     "ECSServiceProjectedUtilizationMetricTypeDef",
     "ECSServiceRecommendationFilterTypeDef",
     "ECSServiceUtilizationMetricTypeDef",
     "TagTypeDef",
-    "ExternalMetricsPreferenceOutputTypeDef",
+    "ExternalMetricsPreferenceTypeDef",
     "EnrollmentFilterTypeDef",
     "EstimatedMonthlySavingsTypeDef",
     "FilterTypeDef",
     "RecommendationPreferencesTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "LambdaFunctionRecommendationFilterTypeDef",
     "ExternalMetricStatusTypeDef",
-    "ExternalMetricsPreferenceTypeDef",
     "GetRecommendationErrorTypeDef",
     "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
-    "GetEnrollmentStatusResponseTypeDef",
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
     "GetRecommendationSummariesRequestRequestTypeDef",
     "RecommendationSourceTypeDef",
     "LambdaFunctionMemoryProjectedMetricTypeDef",
     "LambdaFunctionUtilizationMetricTypeDef",
-    "PaginatorConfigTypeDef",
     "ProjectedMetricTypeDef",
     "ReasonCodeSummaryTypeDef",
-    "ScopeOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateEnrollmentStatusRequestRequestTypeDef",
-    "UpdateEnrollmentStatusResponseTypeDef",
     "VolumeConfigurationTypeDef",
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
     "ContainerConfigurationTypeDef",
     "ContainerRecommendationTypeDef",
     "DeleteRecommendationPreferencesRequestRequestTypeDef",
-    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     "GetRecommendationPreferencesRequestRequestTypeDef",
-    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
     "DescribeRecommendationExportJobsRequestRequestTypeDef",
+    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
+    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
+    "GetEnrollmentStatusResponseTypeDef",
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+    "UpdateEnrollmentStatusResponseTypeDef",
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     "ECSServiceRecommendedOptionProjectedMetricTypeDef",
     "GetECSServiceRecommendationsRequestRequestTypeDef",
     "EffectiveRecommendationPreferencesTypeDef",
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
+    "PutRecommendationPreferencesRequestRequestTypeDef",
+    "RecommendationPreferencesDetailTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     "InferredWorkloadSavingTypeDef",
     "SavingsOpportunityTypeDef",
     "GetAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "GetEC2InstanceRecommendationsRequestRequestTypeDef",
     "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
@@ -142,29 +142,27 @@
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     "ExportECSServiceRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
-    "PutRecommendationPreferencesRequestRequestTypeDef",
     "RecommendedOptionProjectedMetricTypeDef",
     "SummaryTypeDef",
-    "RecommendationPreferencesDetailTypeDef",
     "ServiceConfigurationTypeDef",
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
+    "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationOptionTypeDef",
     "ECSServiceRecommendationOptionTypeDef",
     "InstanceRecommendationOptionTypeDef",
     "LambdaFunctionMemoryRecommendationOptionTypeDef",
     "VolumeRecommendationOptionTypeDef",
     "RecommendationExportJobTypeDef",
     "GetEC2RecommendationProjectedMetricsResponseTypeDef",
     "RecommendationSummaryTypeDef",
-    "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationTypeDef",
     "ECSServiceRecommendationTypeDef",
     "InstanceRecommendationTypeDef",
     "LambdaFunctionRecommendationTypeDef",
     "VolumeRecommendationTypeDef",
     "DescribeRecommendationExportJobsResponseTypeDef",
     "GetRecommendationSummariesResponseTypeDef",
@@ -241,14 +239,35 @@
     {
         "name": JobFilterNameType,
         "values": Sequence[str],
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
 EBSFilterTypeDef = TypedDict(
     "EBSFilterTypeDef",
     {
         "name": Literal["Finding"],
         "values": Sequence[str],
     },
     total=False,
@@ -310,16 +329,16 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-ExternalMetricsPreferenceOutputTypeDef = TypedDict(
-    "ExternalMetricsPreferenceOutputTypeDef",
+ExternalMetricsPreferenceTypeDef = TypedDict(
+    "ExternalMetricsPreferenceTypeDef",
     {
         "source": ExternalMetricsSourceType,
     },
     total=False,
 )
 
 EnrollmentFilterTypeDef = TypedDict(
@@ -390,22 +409,14 @@
     {
         "statusCode": ExternalMetricStatusCodeType,
         "statusReason": str,
     },
     total=False,
 )
 
-ExternalMetricsPreferenceTypeDef = TypedDict(
-    "ExternalMetricsPreferenceTypeDef",
-    {
-        "source": ExternalMetricsSourceType,
-    },
-    total=False,
-)
-
 GetRecommendationErrorTypeDef = TypedDict(
     "GetRecommendationErrorTypeDef",
     {
         "identifier": str,
         "code": str,
         "message": str,
     },
@@ -426,35 +437,14 @@
 GetEffectiveRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetEnrollmentStatusResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "memberAccountsEnrolled": bool,
-        "lastUpdatedTimestamp": datetime,
-        "numberOfMemberAccountsOptedIn": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
-    {
-        "accountIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRecommendationSummariesRequestRequestTypeDef = TypedDict(
     "GetRecommendationSummariesRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -486,24 +476,14 @@
         "name": LambdaFunctionMetricNameType,
         "statistic": LambdaFunctionMetricStatisticType,
         "value": float,
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
 ProjectedMetricTypeDef = TypedDict(
     "ProjectedMetricTypeDef",
     {
         "name": MetricNameType,
         "timestamps": List[datetime],
         "values": List[float],
     },
@@ -515,34 +495,14 @@
     {
         "name": FindingReasonCodeType,
         "value": float,
     },
     total=False,
 )
 
-ScopeOutputTypeDef = TypedDict(
-    "ScopeOutputTypeDef",
-    {
-        "name": ScopeNameType,
-        "value": str,
-    },
-    total=False,
-)
-
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
 _RequiredUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnrollmentStatusRequestRequestTypeDef",
     {
         "status": StatusType,
     },
 )
 _OptionalUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
@@ -555,46 +515,28 @@
 
 class UpdateEnrollmentStatusRequestRequestTypeDef(
     _RequiredUpdateEnrollmentStatusRequestRequestTypeDef,
     _OptionalUpdateEnrollmentStatusRequestRequestTypeDef,
 ):
     pass
 
-UpdateEnrollmentStatusResponseTypeDef = TypedDict(
-    "UpdateEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VolumeConfigurationTypeDef = TypedDict(
     "VolumeConfigurationTypeDef",
     {
         "volumeType": str,
         "volumeSize": int,
         "volumeBaselineIOPS": int,
         "volumeBurstIOPS": int,
         "volumeBaselineThroughput": int,
         "volumeBurstThroughput": int,
         "rootVolume": bool,
     },
     total=False,
 )
 
-GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
-    {
-        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ContainerConfigurationTypeDef = TypedDict(
     "ContainerConfigurationTypeDef",
     {
         "containerName": str,
         "memorySizeConfiguration": MemorySizeConfigurationTypeDef,
         "cpu": int,
     },
@@ -628,35 +570,14 @@
 
 class DeleteRecommendationPreferencesRequestRequestTypeDef(
     _RequiredDeleteRecommendationPreferencesRequestRequestTypeDef,
     _OptionalDeleteRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-    },
-)
-_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
-    {
-        "scope": ScopeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
-    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
 _OptionalGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
@@ -671,35 +592,95 @@
 
 class GetRecommendationPreferencesRequestRequestTypeDef(
     _RequiredGetRecommendationPreferencesRequestRequestTypeDef,
     _OptionalGetRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
-DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
+DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestRequestTypeDef",
     {
         "jobIds": Sequence[str],
         "filters": Sequence[JobFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestRequestTypeDef",
+DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
     {
         "jobIds": Sequence[str],
         "filters": Sequence[JobFilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+    },
+)
+_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+    {
+        "scope": ScopeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
+    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+):
+    pass
+
+GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
+    {
+        "accountIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetEnrollmentStatusResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusResponseTypeDef",
+    {
+        "status": StatusType,
+        "statusReason": str,
+        "memberAccountsEnrolled": bool,
+        "lastUpdatedTimestamp": datetime,
+        "numberOfMemberAccountsOptedIn": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+    {
+        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEnrollmentStatusResponseTypeDef = TypedDict(
+    "UpdateEnrollmentStatusResponseTypeDef",
+    {
+        "status": StatusType,
+        "statusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetEBSVolumeRecommendationsRequestRequestTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     {
         "volumeArns": Sequence[str],
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[EBSFilterTypeDef],
@@ -732,33 +713,68 @@
 
 EffectiveRecommendationPreferencesTypeDef = TypedDict(
     "EffectiveRecommendationPreferencesTypeDef",
     {
         "cpuVendorArchitectures": List[CpuVendorArchitectureType],
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
         "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
+        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
     },
     total=False,
 )
 
 GetEffectiveRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     {
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+    },
+)
+_OptionalPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRecommendationPreferencesRequestRequestTypeDef",
+    {
+        "scope": ScopeTypeDef,
+        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
+        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
+        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+    },
+    total=False,
+)
+
+class PutRecommendationPreferencesRequestRequestTypeDef(
+    _RequiredPutRecommendationPreferencesRequestRequestTypeDef,
+    _OptionalPutRecommendationPreferencesRequestRequestTypeDef,
+):
+    pass
+
+RecommendationPreferencesDetailTypeDef = TypedDict(
+    "RecommendationPreferencesDetailTypeDef",
+    {
+        "scope": ScopeTypeDef,
+        "resourceType": ResourceTypeType,
+        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
+        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
+        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
+    },
+    total=False,
+)
+
 GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     {
         "filters": Sequence[EnrollmentFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetEnrollmentStatusesForOrganizationRequestRequestTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     {
@@ -936,15 +952,15 @@
     pass
 
 ExportAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "ExportAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportDestinationTypeDef = TypedDict(
     "ExportDestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
@@ -953,42 +969,42 @@
 )
 
 ExportEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportECSServiceRecommendationsResponseTypeDef = TypedDict(
     "ExportECSServiceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
         "s3DestinationConfig": S3DestinationConfigTypeDef,
@@ -1014,15 +1030,15 @@
 
 GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     {
         "functionArns": Sequence[str],
         "accountIds": Sequence[str],
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
@@ -1031,37 +1047,14 @@
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-    },
-)
-_OptionalPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRecommendationPreferencesRequestRequestTypeDef",
-    {
-        "scope": ScopeTypeDef,
-        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
-    },
-    total=False,
-)
-
-class PutRecommendationPreferencesRequestRequestTypeDef(
-    _RequiredPutRecommendationPreferencesRequestRequestTypeDef,
-    _OptionalPutRecommendationPreferencesRequestRequestTypeDef,
-):
-    pass
-
 RecommendedOptionProjectedMetricTypeDef = TypedDict(
     "RecommendedOptionProjectedMetricTypeDef",
     {
         "recommendedInstanceType": str,
         "rank": int,
         "projectedMetrics": List[ProjectedMetricTypeDef],
     },
@@ -1074,26 +1067,14 @@
         "name": FindingType,
         "value": float,
         "reasonCodeSummaries": List[ReasonCodeSummaryTypeDef],
     },
     total=False,
 )
 
-RecommendationPreferencesDetailTypeDef = TypedDict(
-    "RecommendationPreferencesDetailTypeDef",
-    {
-        "scope": ScopeOutputTypeDef,
-        "resourceType": ResourceTypeType,
-        "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
-        "inferredWorkloadTypes": InferredWorkloadTypesPreferenceType,
-        "externalMetricsPreference": ExternalMetricsPreferenceOutputTypeDef,
-    },
-    total=False,
-)
-
 ServiceConfigurationTypeDef = TypedDict(
     "ServiceConfigurationTypeDef",
     {
         "memory": int,
         "cpu": int,
         "containerConfigurations": List[ContainerConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationType,
@@ -1104,15 +1085,24 @@
 
 GetECSServiceRecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[
             ECSServiceRecommendedOptionProjectedMetricTypeDef
         ],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRecommendationPreferencesResponseTypeDef = TypedDict(
+    "GetRecommendationPreferencesResponseTypeDef",
+    {
+        "nextToken": str,
+        "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoScalingGroupRecommendationOptionTypeDef = TypedDict(
     "AutoScalingGroupRecommendationOptionTypeDef",
     {
         "configuration": AutoScalingGroupConfigurationTypeDef,
@@ -1187,15 +1177,15 @@
     total=False,
 )
 
 GetEC2RecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetEC2RecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[RecommendedOptionProjectedMetricTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "summaries": List[SummaryTypeDef],
@@ -1204,23 +1194,14 @@
         "savingsOpportunity": SavingsOpportunityTypeDef,
         "currentPerformanceRiskRatings": CurrentPerformanceRiskRatingsTypeDef,
         "inferredWorkloadSavings": List[InferredWorkloadSavingTypeDef],
     },
     total=False,
 )
 
-GetRecommendationPreferencesResponseTypeDef = TypedDict(
-    "GetRecommendationPreferencesResponseTypeDef",
-    {
-        "nextToken": str,
-        "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AutoScalingGroupRecommendationTypeDef = TypedDict(
     "AutoScalingGroupRecommendationTypeDef",
     {
         "accountId": str,
         "autoScalingGroupArn": str,
         "autoScalingGroupName": str,
         "finding": FindingType,
@@ -1317,68 +1298,68 @@
 )
 
 DescribeRecommendationExportJobsResponseTypeDef = TypedDict(
     "DescribeRecommendationExportJobsResponseTypeDef",
     {
         "recommendationExportJobs": List[RecommendationExportJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationSummariesResponseTypeDef = TypedDict(
     "GetRecommendationSummariesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationSummaries": List[RecommendationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "GetAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "autoScalingGroupRecommendations": List[AutoScalingGroupRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetECSServiceRecommendationsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "ecsServiceRecommendations": List[ECSServiceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "GetEC2InstanceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "instanceRecommendations": List[InstanceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "lambdaFunctionRecommendations": List[LambdaFunctionRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "volumeRecommendations": List[VolumeRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/PKG-INFO` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-compute-optimizer
-Version: 1.28.12
-Summary: Type annotations for boto3.ComputeOptimizer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ComputeOptimizer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-compute-optimizer)](https://pepy.tech/project/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,61 +399,61 @@
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
     CurrentPerformanceRiskRatingsTypeDef,
     ScopeTypeDef,
     JobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
     TagTypeDef,
-    ExternalMetricsPreferenceOutputTypeDef,
+    ExternalMetricsPreferenceTypeDef,
     EnrollmentFilterTypeDef,
     EstimatedMonthlySavingsTypeDef,
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
-    ExternalMetricsPreferenceTypeDef,
     GetRecommendationErrorTypeDef,
     GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
-    GetEnrollmentStatusResponseTypeDef,
-    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
-    PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
-    ScopeOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
-    UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
-    GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
     DeleteRecommendationPreferencesRequestRequestTypeDef,
-    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
     GetRecommendationPreferencesRequestRequestTypeDef,
-    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
     DescribeRecommendationExportJobsRequestRequestTypeDef,
+    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
+    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
+    GetEnrollmentStatusResponseTypeDef,
+    GetEnrollmentStatusesForOrganizationResponseTypeDef,
+    UpdateEnrollmentStatusResponseTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
+    PutRecommendationPreferencesRequestRequestTypeDef,
+    RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
     GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
@@ -466,29 +466,27 @@
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
-    PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
-    RecommendationPreferencesDetailTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
+    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
     InstanceRecommendationOptionTypeDef,
     LambdaFunctionMemoryRecommendationOptionTypeDef,
     VolumeRecommendationOptionTypeDef,
     RecommendationExportJobTypeDef,
     GetEC2RecommendationProjectedMetricsResponseTypeDef,
     RecommendationSummaryTypeDef,
-    GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationTypeDef,
     ECSServiceRecommendationTypeDef,
     InstanceRecommendationTypeDef,
     LambdaFunctionRecommendationTypeDef,
     VolumeRecommendationTypeDef,
     DescribeRecommendationExportJobsResponseTypeDef,
     GetRecommendationSummariesResponseTypeDef,
```

### Comparing `mypy-boto3-compute-optimizer-1.28.12/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt` & `mypy-boto3-compute-optimizer-1.28.15/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.28.12/setup.py` & `mypy-boto3-compute-optimizer-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-compute-optimizer",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_compute_optimizer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ComputeOptimizer 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ComputeOptimizer 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

