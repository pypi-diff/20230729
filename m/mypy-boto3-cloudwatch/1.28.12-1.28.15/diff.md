# Comparing `tmp/mypy-boto3-cloudwatch-1.28.12.tar.gz` & `tmp/mypy-boto3-cloudwatch-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudwatch-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudwatch-1.28.15.tar", last modified: Fri Jul 28 20:42:28 2023, max compression
```

## Comparing `mypy-boto3-cloudwatch-1.28.12.tar` & `mypy-boto3-cloudwatch-1.28.15.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.064556 mypy-boto3-cloudwatch-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-07-27 05:34:27.044556 mypy-boto3-cloudwatch-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.044556 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32773 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23159 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    45926 2023-07-27 05:18:52.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45877 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-27 05:18:51.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.044556 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:26.000000 mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.064556 mypy-boto3-cloudwatch-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:18:50.000000 mypy-boto3-cloudwatch-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.460823 mypy-boto3-cloudwatch-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:08.000000 mypy-boto3-cloudwatch-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-07-28 20:42:28.456823 mypy-boto3-cloudwatch-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-07-28 20:21:08.000000 mypy-boto3-cloudwatch-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.452823 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-28 20:21:08.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-28 20:21:08.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:21:08.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-07-28 20:21:09.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32773 2023-07-28 20:21:09.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-28 20:21:09.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-28 20:21:09.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-28 20:21:09.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-28 20:21:09.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:08.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23164 2023-07-28 20:21:09.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23119 2023-07-28 20:21:09.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    45319 2023-07-28 20:21:12.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45270 2023-07-28 20:21:10.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:08.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-28 20:21:09.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-28 20:21:09.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.456823 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-07-28 20:42:28.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 20:42:28.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:28.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:28.000000 mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:28.460823 mypy-boto3-cloudwatch-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:21:08.000000 mypy-boto3-cloudwatch-1.28.15/setup.py
```

### Comparing `mypy-boto3-cloudwatch-1.28.12/LICENSE` & `mypy-boto3-cloudwatch-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.12/PKG-INFO` & `mypy-boto3-cloudwatch-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudWatch 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudWatch 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -448,115 +448,112 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
     RangeOutputTypeDef,
     RangeTypeDef,
-    DimensionOutputTypeDef,
+    DimensionTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
-    DimensionTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
     DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
-    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAlarmHistoryInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
-    GetDashboardOutputTypeDef,
     GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
     MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
-    GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
-    ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
-    ManagedRuleStateTypeDef,
     TagTypeDef,
+    ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
     MetricStreamFilterTypeDef,
-    MetricStreamStatisticsMetricOutputTypeDef,
     MetricStreamStatisticsMetricTypeDef,
-    PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
-    PutMetricStreamOutputTypeDef,
-    ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    DescribeAlarmHistoryOutputTypeDef,
     AnomalyDetectorConfigurationOutputTypeDef,
     AnomalyDetectorConfigurationTypeDef,
-    MetricOutputTypeDef,
-    SingleMetricAnomalyDetectorOutputTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
-    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
     GetMetricStatisticsInputMetricGetStatisticsTypeDef,
     GetMetricStatisticsInputRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
+    SingleMetricAnomalyDetectorOutputTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
     DeleteInsightRulesOutputTypeDef,
+    DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableInsightRulesOutputTypeDef,
+    GetDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
+    GetMetricWidgetImageOutputTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
+    PutMetricStreamOutputTypeDef,
+    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
+    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
+    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
+    ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    ManagedRuleDescriptionTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
     MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
     MetricStatOutputTypeDef,
     MetricStatTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
-    ListManagedInsightRulesOutputTypeDef,
     PutManagedInsightRulesInputRequestTypeDef,
+    ListManagedInsightRulesOutputTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
     PutMetricStreamInputRequestTypeDef,
     MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     MetricAlarmTypeDef,
     MetricMathAnomalyDetectorOutputTypeDef,
```

### Comparing `mypy-boto3-cloudwatch-1.28.12/README.md` & `mypy-boto3-cloudwatch-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -416,115 +416,112 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
     RangeOutputTypeDef,
     RangeTypeDef,
-    DimensionOutputTypeDef,
+    DimensionTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
-    DimensionTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
     DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
-    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAlarmHistoryInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
-    GetDashboardOutputTypeDef,
     GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
     MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
-    GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
-    ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
-    ManagedRuleStateTypeDef,
     TagTypeDef,
+    ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
     MetricStreamFilterTypeDef,
-    MetricStreamStatisticsMetricOutputTypeDef,
     MetricStreamStatisticsMetricTypeDef,
-    PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
-    PutMetricStreamOutputTypeDef,
-    ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    DescribeAlarmHistoryOutputTypeDef,
     AnomalyDetectorConfigurationOutputTypeDef,
     AnomalyDetectorConfigurationTypeDef,
-    MetricOutputTypeDef,
-    SingleMetricAnomalyDetectorOutputTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
-    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
     GetMetricStatisticsInputMetricGetStatisticsTypeDef,
     GetMetricStatisticsInputRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
+    SingleMetricAnomalyDetectorOutputTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
     DeleteInsightRulesOutputTypeDef,
+    DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableInsightRulesOutputTypeDef,
+    GetDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
+    GetMetricWidgetImageOutputTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
+    PutMetricStreamOutputTypeDef,
+    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
+    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
+    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
+    ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    ManagedRuleDescriptionTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
     MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
     MetricStatOutputTypeDef,
     MetricStatTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
-    ListManagedInsightRulesOutputTypeDef,
     PutManagedInsightRulesInputRequestTypeDef,
+    ListManagedInsightRulesOutputTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
     PutMetricStreamInputRequestTypeDef,
     MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     MetricAlarmTypeDef,
     MetricMathAnomalyDetectorOutputTypeDef,
```

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__init__.py` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__init__.pyi` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/__main__.py` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatch 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudWatch 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch\nOther"
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

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/client.py` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/client.pyi` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/literals.py` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/literals.pyi` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/paginator.py` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
         StartDate: Union[datetime, str] = ...,
         EndDate: Union[datetime, str] = ...,
         ScanBy: ScanByType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAlarmHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describealarmhistorypaginator)
         """
 
 
@@ -117,15 +117,15 @@
         AlarmNames: Sequence[str] = ...,
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAlarmsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describealarmspaginator)
         """
 
 
@@ -138,15 +138,15 @@
     def paginate(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAnomalyDetectorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAnomalyDetectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describeanomalydetectorspaginator)
         """
 
 
@@ -160,30 +160,30 @@
         self,
         *,
         MetricDataQueries: Sequence[MetricDataQueryTypeDef],
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetMetricDataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#getmetricdatapaginator)
         """
 
 
 class ListDashboardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listdashboardspaginator)
     """
 
     def paginate(
-        self, *, DashboardNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DashboardNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDashboardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listdashboardspaginator)
         """
 
 
@@ -198,13 +198,13 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
         OwningAccount: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMetricsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listmetricspaginator)
         """
```

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/paginator.pyi` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
         StartDate: Union[datetime, str] = ...,
         EndDate: Union[datetime, str] = ...,
         ScanBy: ScanByType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAlarmHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describealarmhistorypaginator)
         """
 
 class DescribeAlarmsPaginator(Paginator):
@@ -112,15 +112,15 @@
         AlarmNames: Sequence[str] = ...,
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAlarmsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describealarmspaginator)
         """
 
 class DescribeAnomalyDetectorsPaginator(Paginator):
@@ -132,15 +132,15 @@
     def paginate(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAnomalyDetectorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAnomalyDetectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describeanomalydetectorspaginator)
         """
 
 class GetMetricDataPaginator(Paginator):
@@ -153,29 +153,29 @@
         self,
         *,
         MetricDataQueries: Sequence[MetricDataQueryTypeDef],
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetMetricDataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#getmetricdatapaginator)
         """
 
 class ListDashboardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listdashboardspaginator)
     """
 
     def paginate(
-        self, *, DashboardNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DashboardNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDashboardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listdashboardspaginator)
         """
 
 class ListMetricsPaginator(Paginator):
@@ -189,13 +189,13 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
         OwningAccount: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMetricsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listmetricspaginator)
         """
```

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/service_resource.py` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     StandardUnitType,
     StateValueType,
     StatisticType,
 )
 from .type_defs import (
     DescribeAlarmHistoryOutputTypeDef,
     DimensionFilterTypeDef,
-    DimensionOutputTypeDef,
     DimensionTypeDef,
     GetMetricStatisticsOutputTypeDef,
     MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TagTypeDef,
 )
 
@@ -291,15 +290,15 @@
     state_reason: str
     state_reason_data: str
     state_updated_timestamp: datetime
     metric_name: str
     namespace: str
     statistic: StatisticType
     extended_statistic: str
-    dimensions: List[DimensionOutputTypeDef]
+    dimensions: List[DimensionTypeDef]
     period: int
     unit: StandardUnitType
     evaluation_periods: int
     datapoints_to_alarm: int
     threshold: float
     comparison_operator: ComparisonOperatorType
     treat_missing_data: str
@@ -396,15 +395,15 @@
 class Metric(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.Metric)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/service_resource/#metric)
     """
 
     metric_name: str
-    dimensions: List[DimensionOutputTypeDef]
+    dimensions: List[DimensionTypeDef]
     namespace: str
     name: str
     alarms: MetricAlarmsCollection
 
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
```

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/service_resource.pyi` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     StandardUnitType,
     StateValueType,
     StatisticType,
 )
 from .type_defs import (
     DescribeAlarmHistoryOutputTypeDef,
     DimensionFilterTypeDef,
-    DimensionOutputTypeDef,
     DimensionTypeDef,
     GetMetricStatisticsOutputTypeDef,
     MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TagTypeDef,
 )
 
@@ -265,15 +264,15 @@
     state_reason: str
     state_reason_data: str
     state_updated_timestamp: datetime
     metric_name: str
     namespace: str
     statistic: StatisticType
     extended_statistic: str
-    dimensions: List[DimensionOutputTypeDef]
+    dimensions: List[DimensionTypeDef]
     period: int
     unit: StandardUnitType
     evaluation_periods: int
     datapoints_to_alarm: int
     threshold: float
     comparison_operator: ComparisonOperatorType
     treat_missing_data: str
@@ -361,15 +360,15 @@
 class Metric(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.ServiceResource.Metric)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/service_resource/#metric)
     """
 
     metric_name: str
-    dimensions: List[DimensionOutputTypeDef]
+    dimensions: List[DimensionTypeDef]
     namespace: str
     name: str
     alarms: MetricAlarmsCollection
 
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
```

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/type_defs.py` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,115 +40,112 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AlarmHistoryItemTypeDef",
     "RangeOutputTypeDef",
     "RangeTypeDef",
-    "DimensionOutputTypeDef",
+    "DimensionTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
-    "DimensionTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
     "DeleteInsightRulesInputRequestTypeDef",
     "PartialFailureTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteMetricStreamInputRequestTypeDef",
     "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAlarmHistoryInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     "DescribeAlarmsInputRequestTypeDef",
     "DescribeInsightRulesInputRequestTypeDef",
     "InsightRuleTypeDef",
     "DimensionFilterTypeDef",
     "DisableAlarmActionsInputRequestTypeDef",
     "DisableInsightRulesInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableAlarmActionsInputRequestTypeDef",
     "EnableInsightRulesInputRequestTypeDef",
     "GetDashboardInputRequestTypeDef",
-    "GetDashboardOutputTypeDef",
     "GetInsightRuleReportInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
     "MetricStreamFilterOutputTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
-    "GetMetricWidgetImageOutputTypeDef",
     "InsightRuleContributorDatapointTypeDef",
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "ListDashboardsInputRequestTypeDef",
     "ListManagedInsightRulesInputRequestTypeDef",
     "ListMetricStreamsInputRequestTypeDef",
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagOutputTypeDef",
-    "ManagedRuleStateTypeDef",
     "TagTypeDef",
+    "ManagedRuleStateTypeDef",
     "StatisticSetTypeDef",
     "MetricStreamFilterTypeDef",
-    "MetricStreamStatisticsMetricOutputTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
-    "PaginatorConfigTypeDef",
     "PutDashboardInputRequestTypeDef",
-    "PutMetricStreamOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "DescribeAlarmHistoryOutputTypeDef",
     "AnomalyDetectorConfigurationOutputTypeDef",
     "AnomalyDetectorConfigurationTypeDef",
-    "MetricOutputTypeDef",
-    "SingleMetricAnomalyDetectorOutputTypeDef",
-    "ListDashboardsOutputTypeDef",
-    "PutDashboardOutputTypeDef",
-    "GetMetricStatisticsOutputTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
     "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
     "GetMetricStatisticsInputRequestTypeDef",
+    "MetricOutputTypeDef",
     "MetricTypeDef",
+    "SingleMetricAnomalyDetectorOutputTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
     "DeleteInsightRulesOutputTypeDef",
+    "DescribeAlarmHistoryOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableInsightRulesOutputTypeDef",
+    "GetDashboardOutputTypeDef",
+    "GetMetricStatisticsOutputTypeDef",
+    "GetMetricWidgetImageOutputTypeDef",
+    "ListDashboardsOutputTypeDef",
+    "PutDashboardOutputTypeDef",
     "PutManagedInsightRulesOutputTypeDef",
+    "PutMetricStreamOutputTypeDef",
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
     "ListMetricsInputListMetricsPaginateTypeDef",
     "ListMetricsInputRequestTypeDef",
     "MetricDataResultTypeDef",
     "InsightRuleContributorTypeDef",
     "ListMetricStreamsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "ManagedRuleDescriptionTypeDef",
     "ManagedRuleTypeDef",
     "PutCompositeAlarmInputRequestTypeDef",
     "PutInsightRuleInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "ManagedRuleDescriptionTypeDef",
     "MetricDatumTypeDef",
     "MetricStreamStatisticsConfigurationOutputTypeDef",
     "MetricStreamStatisticsConfigurationTypeDef",
     "ListMetricsOutputTypeDef",
     "MetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "GetMetricDataOutputTypeDef",
     "GetInsightRuleReportOutputTypeDef",
-    "ListManagedInsightRulesOutputTypeDef",
     "PutManagedInsightRulesInputRequestTypeDef",
+    "ListManagedInsightRulesOutputTypeDef",
     "PutMetricDataInputRequestTypeDef",
     "GetMetricStreamOutputTypeDef",
     "PutMetricStreamInputRequestTypeDef",
     "MetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
     "MetricAlarmTypeDef",
     "MetricMathAnomalyDetectorOutputTypeDef",
@@ -190,16 +187,16 @@
     "RangeTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
-DimensionOutputTypeDef = TypedDict(
-    "DimensionOutputTypeDef",
+DimensionTypeDef = TypedDict(
+    "DimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 CompositeAlarmTypeDef = TypedDict(
@@ -266,22 +263,14 @@
 DeleteAlarmsInputRequestTypeDef = TypedDict(
     "DeleteAlarmsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
-DimensionTypeDef = TypedDict(
-    "DimensionTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 DeleteDashboardsInputRequestTypeDef = TypedDict(
     "DeleteDashboardsInputRequestTypeDef",
     {
         "DashboardNames": Sequence[str],
     },
 )
 
@@ -299,14 +288,25 @@
         "ExceptionType": str,
         "FailureCode": str,
         "FailureDescription": str,
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
 DeleteMetricStreamInputRequestTypeDef = TypedDict(
     "DeleteMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -320,24 +320,20 @@
         "MaxRecords": int,
         "NextToken": str,
         "ScanBy": ScanByType,
     },
     total=False,
 )
 
-DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AlarmName": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "ScanBy": ScanByType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
     "DescribeAlarmHistoryInputRequestTypeDef",
     {
@@ -358,29 +354,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
-    {
-        "AlarmNames": Sequence[str],
-        "AlarmNamePrefix": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "ChildrenOfAlarmName": str,
-        "ParentsOfAlarmName": str,
-        "StateValue": StateValueType,
-        "ActionPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAlarmsInputRequestTypeDef = TypedDict(
     "DescribeAlarmsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
         "AlarmTypes": Sequence[AlarmTypeType],
         "ChildrenOfAlarmName": str,
@@ -453,21 +434,14 @@
 DisableInsightRulesInputRequestTypeDef = TypedDict(
     "DisableInsightRulesInputRequestTypeDef",
     {
         "RuleNames": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableAlarmActionsInputRequestTypeDef = TypedDict(
     "EnableAlarmActionsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
@@ -481,24 +455,14 @@
 GetDashboardInputRequestTypeDef = TypedDict(
     "GetDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
     },
 )
 
-GetDashboardOutputTypeDef = TypedDict(
-    "GetDashboardOutputTypeDef",
-    {
-        "DashboardArn": str,
-        "DashboardBody": str,
-        "DashboardName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
     "_RequiredGetInsightRuleReportInputRequestTypeDef",
     {
         "RuleName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Period": int,
@@ -600,39 +564,22 @@
 class GetMetricWidgetImageInputRequestTypeDef(
     _RequiredGetMetricWidgetImageInputRequestTypeDef,
     _OptionalGetMetricWidgetImageInputRequestTypeDef,
 ):
     pass
 
 
-GetMetricWidgetImageOutputTypeDef = TypedDict(
-    "GetMetricWidgetImageOutputTypeDef",
-    {
-        "MetricWidgetImage": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InsightRuleContributorDatapointTypeDef = TypedDict(
     "InsightRuleContributorDatapointTypeDef",
     {
         "Timestamp": datetime,
         "ApproximateValue": float,
     },
 )
 
-ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
-    {
-        "DashboardNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDashboardsInputRequestTypeDef = TypedDict(
     "ListDashboardsInputRequestTypeDef",
     {
         "DashboardNamePrefix": str,
         "NextToken": str,
     },
     total=False,
@@ -687,38 +634,30 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 ManagedRuleStateTypeDef = TypedDict(
     "ManagedRuleStateTypeDef",
     {
         "RuleName": str,
         "State": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 StatisticSetTypeDef = TypedDict(
     "StatisticSetTypeDef",
     {
         "SampleCount": float,
         "Sum": float,
         "Minimum": float,
         "Maximum": float,
@@ -730,67 +669,30 @@
     {
         "Namespace": str,
         "MetricNames": Sequence[str],
     },
     total=False,
 )
 
-MetricStreamStatisticsMetricOutputTypeDef = TypedDict(
-    "MetricStreamStatisticsMetricOutputTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-    },
-)
-
 MetricStreamStatisticsMetricTypeDef = TypedDict(
     "MetricStreamStatisticsMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
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
 PutDashboardInputRequestTypeDef = TypedDict(
     "PutDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
         "DashboardBody": str,
     },
 )
 
-PutMetricStreamOutputTypeDef = TypedDict(
-    "PutMetricStreamOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 _RequiredSetAlarmStateInputAlarmSetStateTypeDef = TypedDict(
     "_RequiredSetAlarmStateInputAlarmSetStateTypeDef",
     {
         "StateValue": StateValueType,
         "StateReason": str,
     },
 )
@@ -850,23 +752,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-DescribeAlarmHistoryOutputTypeDef = TypedDict(
-    "DescribeAlarmHistoryOutputTypeDef",
-    {
-        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AnomalyDetectorConfigurationOutputTypeDef = TypedDict(
     "AnomalyDetectorConfigurationOutputTypeDef",
     {
         "ExcludedTimeRanges": List[RangeOutputTypeDef],
         "MetricTimezone": str,
     },
     total=False,
@@ -877,61 +770,14 @@
     {
         "ExcludedTimeRanges": Sequence[RangeTypeDef],
         "MetricTimezone": str,
     },
     total=False,
 )
 
-MetricOutputTypeDef = TypedDict(
-    "MetricOutputTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionOutputTypeDef],
-    },
-    total=False,
-)
-
-SingleMetricAnomalyDetectorOutputTypeDef = TypedDict(
-    "SingleMetricAnomalyDetectorOutputTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionOutputTypeDef],
-        "Stat": str,
-    },
-    total=False,
-)
-
-ListDashboardsOutputTypeDef = TypedDict(
-    "ListDashboardsOutputTypeDef",
-    {
-        "DashboardEntries": List[DashboardEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutDashboardOutputTypeDef = TypedDict(
-    "PutDashboardOutputTypeDef",
-    {
-        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMetricStatisticsOutputTypeDef = TypedDict(
-    "GetMetricStatisticsOutputTypeDef",
-    {
-        "Label": str,
-        "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeAlarmsForMetricInputRequestTypeDef = TypedDict(
     "_RequiredDescribeAlarmsForMetricInputRequestTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
     },
 )
@@ -951,26 +797,14 @@
 class DescribeAlarmsForMetricInputRequestTypeDef(
     _RequiredDescribeAlarmsForMetricInputRequestTypeDef,
     _OptionalDescribeAlarmsForMetricInputRequestTypeDef,
 ):
     pass
 
 
-DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": Sequence[DimensionTypeDef],
-        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAnomalyDetectorsInputRequestTypeDef = TypedDict(
     "DescribeAnomalyDetectorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Namespace": str,
         "MetricName": str,
@@ -1031,24 +865,45 @@
 
 class GetMetricStatisticsInputRequestTypeDef(
     _RequiredGetMetricStatisticsInputRequestTypeDef, _OptionalGetMetricStatisticsInputRequestTypeDef
 ):
     pass
 
 
+MetricOutputTypeDef = TypedDict(
+    "MetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+    },
+    total=False,
+)
+
 MetricTypeDef = TypedDict(
     "MetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
     },
     total=False,
 )
 
+SingleMetricAnomalyDetectorOutputTypeDef = TypedDict(
+    "SingleMetricAnomalyDetectorOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+    },
+    total=False,
+)
+
 SingleMetricAnomalyDetectorTypeDef = TypedDict(
     "SingleMetricAnomalyDetectorTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
@@ -1056,40 +911,158 @@
     total=False,
 )
 
 DeleteInsightRulesOutputTypeDef = TypedDict(
     "DeleteInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmHistoryOutputTypeDef = TypedDict(
+    "DescribeAlarmHistoryOutputTypeDef",
+    {
+        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableInsightRulesOutputTypeDef = TypedDict(
     "DisableInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
 
 EnableInsightRulesOutputTypeDef = TypedDict(
     "EnableInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDashboardOutputTypeDef = TypedDict(
+    "GetDashboardOutputTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardBody": str,
+        "DashboardName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMetricStatisticsOutputTypeDef = TypedDict(
+    "GetMetricStatisticsOutputTypeDef",
+    {
+        "Label": str,
+        "Datapoints": List[DatapointTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMetricWidgetImageOutputTypeDef = TypedDict(
+    "GetMetricWidgetImageOutputTypeDef",
+    {
+        "MetricWidgetImage": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDashboardsOutputTypeDef = TypedDict(
+    "ListDashboardsOutputTypeDef",
+    {
+        "DashboardEntries": List[DashboardEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutDashboardOutputTypeDef = TypedDict(
+    "PutDashboardOutputTypeDef",
+    {
+        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutManagedInsightRulesOutputTypeDef = TypedDict(
     "PutManagedInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutMetricStreamOutputTypeDef = TypedDict(
+    "PutMetricStreamOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+    {
+        "AlarmName": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": Union[datetime, str],
+        "EndDate": Union[datetime, str],
+        "ScanBy": ScanByType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
+    {
+        "AlarmNames": Sequence[str],
+        "AlarmNamePrefix": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "ChildrenOfAlarmName": str,
+        "ParentsOfAlarmName": str,
+        "StateValue": StateValueType,
+        "ActionPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": Sequence[DimensionTypeDef],
+        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
+    {
+        "DashboardNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 DescribeAlarmsInputAlarmExistsWaitTypeDef = TypedDict(
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
@@ -1123,28 +1096,28 @@
 )
 
 DescribeInsightRulesOutputTypeDef = TypedDict(
     "DescribeInsightRulesOutputTypeDef",
     {
         "NextToken": str,
         "InsightRules": List[InsightRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMetricsInputListMetricsPaginateTypeDef = TypedDict(
     "ListMetricsInputListMetricsPaginateTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionFilterTypeDef],
         "RecentlyActive": Literal["PT3H"],
         "IncludeLinkedAccounts": bool,
         "OwningAccount": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMetricsInputRequestTypeDef = TypedDict(
     "ListMetricsInputRequestTypeDef",
     {
@@ -1182,34 +1155,24 @@
 )
 
 ListMetricStreamsOutputTypeDef = TypedDict(
     "ListMetricStreamsOutputTypeDef",
     {
         "NextToken": str,
         "Entries": List[MetricStreamEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ManagedRuleDescriptionTypeDef = TypedDict(
-    "ManagedRuleDescriptionTypeDef",
-    {
-        "TemplateName": str,
-        "ResourceARN": str,
-        "RuleState": ManagedRuleStateTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredManagedRuleTypeDef = TypedDict(
     "_RequiredManagedRuleTypeDef",
     {
         "TemplateName": str,
         "ResourceARN": str,
@@ -1285,14 +1248,24 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+ManagedRuleDescriptionTypeDef = TypedDict(
+    "ManagedRuleDescriptionTypeDef",
+    {
+        "TemplateName": str,
+        "ResourceARN": str,
+        "RuleState": ManagedRuleStateTypeDef,
+    },
+    total=False,
+)
+
 _RequiredMetricDatumTypeDef = TypedDict(
     "_RequiredMetricDatumTypeDef",
     {
         "MetricName": str,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
@@ -1314,15 +1287,15 @@
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
 
 MetricStreamStatisticsConfigurationOutputTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationOutputTypeDef",
     {
-        "IncludeMetrics": List[MetricStreamStatisticsMetricOutputTypeDef],
+        "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
         "AdditionalStatistics": List[str],
     },
 )
 
 MetricStreamStatisticsConfigurationTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationTypeDef",
     {
@@ -1333,15 +1306,15 @@
 
 ListMetricsOutputTypeDef = TypedDict(
     "ListMetricsOutputTypeDef",
     {
         "Metrics": List[MetricOutputTypeDef],
         "NextToken": str,
         "OwningAccounts": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMetricStatOutputTypeDef = TypedDict(
     "_RequiredMetricStatOutputTypeDef",
     {
         "Metric": MetricOutputTypeDef,
@@ -1385,44 +1358,44 @@
 
 GetMetricDataOutputTypeDef = TypedDict(
     "GetMetricDataOutputTypeDef",
     {
         "MetricDataResults": List[MetricDataResultTypeDef],
         "NextToken": str,
         "Messages": List[MessageDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightRuleReportOutputTypeDef = TypedDict(
     "GetInsightRuleReportOutputTypeDef",
     {
         "KeyLabels": List[str],
         "AggregationStatistic": str,
         "AggregateValue": float,
         "ApproximateUniqueCount": int,
         "Contributors": List[InsightRuleContributorTypeDef],
         "MetricDatapoints": List[InsightRuleMetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListManagedInsightRulesOutputTypeDef = TypedDict(
-    "ListManagedInsightRulesOutputTypeDef",
+PutManagedInsightRulesInputRequestTypeDef = TypedDict(
+    "PutManagedInsightRulesInputRequestTypeDef",
     {
-        "ManagedRules": List[ManagedRuleDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ManagedRules": Sequence[ManagedRuleTypeDef],
     },
 )
 
-PutManagedInsightRulesInputRequestTypeDef = TypedDict(
-    "PutManagedInsightRulesInputRequestTypeDef",
+ListManagedInsightRulesOutputTypeDef = TypedDict(
+    "ListManagedInsightRulesOutputTypeDef",
     {
-        "ManagedRules": Sequence[ManagedRuleTypeDef],
+        "ManagedRules": List[ManagedRuleDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMetricDataInputRequestTypeDef = TypedDict(
     "PutMetricDataInputRequestTypeDef",
     {
         "Namespace": str,
@@ -1441,15 +1414,15 @@
         "RoleArn": str,
         "State": str,
         "CreationDate": datetime,
         "LastUpdateDate": datetime,
         "OutputFormat": MetricStreamOutputFormatType,
         "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationOutputTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
     "_RequiredPutMetricStreamInputRequestTypeDef",
     {
         "Name": str,
@@ -1542,15 +1515,15 @@
         "StateReason": str,
         "StateReasonData": str,
         "StateUpdatedTimestamp": datetime,
         "MetricName": str,
         "Namespace": str,
         "Statistic": StatisticType,
         "ExtendedStatistic": str,
-        "Dimensions": List[DimensionOutputTypeDef],
+        "Dimensions": List[DimensionTypeDef],
         "Period": int,
         "Unit": StandardUnitType,
         "EvaluationPeriods": int,
         "DatapointsToAlarm": int,
         "Threshold": float,
         "ComparisonOperator": ComparisonOperatorType,
         "TreatMissingData": str,
@@ -1580,15 +1553,15 @@
     },
 )
 _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
     "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
     {
         "ScanBy": ScanByType,
         "LabelOptions": LabelOptionsTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetMetricDataInputGetMetricDataPaginateTypeDef(
     _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
@@ -1712,34 +1685,34 @@
     pass
 
 
 DescribeAlarmsForMetricOutputTypeDef = TypedDict(
     "DescribeAlarmsForMetricOutputTypeDef",
     {
         "MetricAlarms": List[MetricAlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAlarmsOutputTypeDef = TypedDict(
     "DescribeAlarmsOutputTypeDef",
     {
         "CompositeAlarms": List[CompositeAlarmTypeDef],
         "MetricAlarms": List[MetricAlarmTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AnomalyDetectorTypeDef = TypedDict(
     "AnomalyDetectorTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
-        "Dimensions": List[DimensionOutputTypeDef],
+        "Dimensions": List[DimensionTypeDef],
         "Stat": str,
         "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
         "StateValue": AnomalyDetectorStateValueType,
         "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
         "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
     },
     total=False,
@@ -1773,10 +1746,10 @@
 )
 
 DescribeAnomalyDetectorsOutputTypeDef = TypedDict(
     "DescribeAnomalyDetectorsOutputTypeDef",
     {
         "AnomalyDetectors": List[AnomalyDetectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/type_defs.pyi` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -39,115 +39,112 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlarmHistoryItemTypeDef",
     "RangeOutputTypeDef",
     "RangeTypeDef",
-    "DimensionOutputTypeDef",
+    "DimensionTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
-    "DimensionTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
     "DeleteInsightRulesInputRequestTypeDef",
     "PartialFailureTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteMetricStreamInputRequestTypeDef",
     "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAlarmHistoryInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     "DescribeAlarmsInputRequestTypeDef",
     "DescribeInsightRulesInputRequestTypeDef",
     "InsightRuleTypeDef",
     "DimensionFilterTypeDef",
     "DisableAlarmActionsInputRequestTypeDef",
     "DisableInsightRulesInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableAlarmActionsInputRequestTypeDef",
     "EnableInsightRulesInputRequestTypeDef",
     "GetDashboardInputRequestTypeDef",
-    "GetDashboardOutputTypeDef",
     "GetInsightRuleReportInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
     "MetricStreamFilterOutputTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
-    "GetMetricWidgetImageOutputTypeDef",
     "InsightRuleContributorDatapointTypeDef",
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "ListDashboardsInputRequestTypeDef",
     "ListManagedInsightRulesInputRequestTypeDef",
     "ListMetricStreamsInputRequestTypeDef",
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagOutputTypeDef",
-    "ManagedRuleStateTypeDef",
     "TagTypeDef",
+    "ManagedRuleStateTypeDef",
     "StatisticSetTypeDef",
     "MetricStreamFilterTypeDef",
-    "MetricStreamStatisticsMetricOutputTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
-    "PaginatorConfigTypeDef",
     "PutDashboardInputRequestTypeDef",
-    "PutMetricStreamOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "DescribeAlarmHistoryOutputTypeDef",
     "AnomalyDetectorConfigurationOutputTypeDef",
     "AnomalyDetectorConfigurationTypeDef",
-    "MetricOutputTypeDef",
-    "SingleMetricAnomalyDetectorOutputTypeDef",
-    "ListDashboardsOutputTypeDef",
-    "PutDashboardOutputTypeDef",
-    "GetMetricStatisticsOutputTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
     "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
     "GetMetricStatisticsInputRequestTypeDef",
+    "MetricOutputTypeDef",
     "MetricTypeDef",
+    "SingleMetricAnomalyDetectorOutputTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
     "DeleteInsightRulesOutputTypeDef",
+    "DescribeAlarmHistoryOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableInsightRulesOutputTypeDef",
+    "GetDashboardOutputTypeDef",
+    "GetMetricStatisticsOutputTypeDef",
+    "GetMetricWidgetImageOutputTypeDef",
+    "ListDashboardsOutputTypeDef",
+    "PutDashboardOutputTypeDef",
     "PutManagedInsightRulesOutputTypeDef",
+    "PutMetricStreamOutputTypeDef",
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
     "ListMetricsInputListMetricsPaginateTypeDef",
     "ListMetricsInputRequestTypeDef",
     "MetricDataResultTypeDef",
     "InsightRuleContributorTypeDef",
     "ListMetricStreamsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "ManagedRuleDescriptionTypeDef",
     "ManagedRuleTypeDef",
     "PutCompositeAlarmInputRequestTypeDef",
     "PutInsightRuleInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "ManagedRuleDescriptionTypeDef",
     "MetricDatumTypeDef",
     "MetricStreamStatisticsConfigurationOutputTypeDef",
     "MetricStreamStatisticsConfigurationTypeDef",
     "ListMetricsOutputTypeDef",
     "MetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "GetMetricDataOutputTypeDef",
     "GetInsightRuleReportOutputTypeDef",
-    "ListManagedInsightRulesOutputTypeDef",
     "PutManagedInsightRulesInputRequestTypeDef",
+    "ListManagedInsightRulesOutputTypeDef",
     "PutMetricDataInputRequestTypeDef",
     "GetMetricStreamOutputTypeDef",
     "PutMetricStreamInputRequestTypeDef",
     "MetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
     "MetricAlarmTypeDef",
     "MetricMathAnomalyDetectorOutputTypeDef",
@@ -189,16 +186,16 @@
     "RangeTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
-DimensionOutputTypeDef = TypedDict(
-    "DimensionOutputTypeDef",
+DimensionTypeDef = TypedDict(
+    "DimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
 CompositeAlarmTypeDef = TypedDict(
@@ -265,22 +262,14 @@
 DeleteAlarmsInputRequestTypeDef = TypedDict(
     "DeleteAlarmsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
-DimensionTypeDef = TypedDict(
-    "DimensionTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 DeleteDashboardsInputRequestTypeDef = TypedDict(
     "DeleteDashboardsInputRequestTypeDef",
     {
         "DashboardNames": Sequence[str],
     },
 )
 
@@ -298,14 +287,25 @@
         "ExceptionType": str,
         "FailureCode": str,
         "FailureDescription": str,
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
 DeleteMetricStreamInputRequestTypeDef = TypedDict(
     "DeleteMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -319,24 +319,20 @@
         "MaxRecords": int,
         "NextToken": str,
         "ScanBy": ScanByType,
     },
     total=False,
 )
 
-DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AlarmName": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "ScanBy": ScanByType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
     "DescribeAlarmHistoryInputRequestTypeDef",
     {
@@ -357,29 +353,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
-    {
-        "AlarmNames": Sequence[str],
-        "AlarmNamePrefix": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "ChildrenOfAlarmName": str,
-        "ParentsOfAlarmName": str,
-        "StateValue": StateValueType,
-        "ActionPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAlarmsInputRequestTypeDef = TypedDict(
     "DescribeAlarmsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
         "AlarmTypes": Sequence[AlarmTypeType],
         "ChildrenOfAlarmName": str,
@@ -448,21 +429,14 @@
 DisableInsightRulesInputRequestTypeDef = TypedDict(
     "DisableInsightRulesInputRequestTypeDef",
     {
         "RuleNames": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableAlarmActionsInputRequestTypeDef = TypedDict(
     "EnableAlarmActionsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
@@ -476,24 +450,14 @@
 GetDashboardInputRequestTypeDef = TypedDict(
     "GetDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
     },
 )
 
-GetDashboardOutputTypeDef = TypedDict(
-    "GetDashboardOutputTypeDef",
-    {
-        "DashboardArn": str,
-        "DashboardBody": str,
-        "DashboardName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
     "_RequiredGetInsightRuleReportInputRequestTypeDef",
     {
         "RuleName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Period": int,
@@ -589,39 +553,22 @@
 
 class GetMetricWidgetImageInputRequestTypeDef(
     _RequiredGetMetricWidgetImageInputRequestTypeDef,
     _OptionalGetMetricWidgetImageInputRequestTypeDef,
 ):
     pass
 
-GetMetricWidgetImageOutputTypeDef = TypedDict(
-    "GetMetricWidgetImageOutputTypeDef",
-    {
-        "MetricWidgetImage": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InsightRuleContributorDatapointTypeDef = TypedDict(
     "InsightRuleContributorDatapointTypeDef",
     {
         "Timestamp": datetime,
         "ApproximateValue": float,
     },
 )
 
-ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
-    {
-        "DashboardNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDashboardsInputRequestTypeDef = TypedDict(
     "ListDashboardsInputRequestTypeDef",
     {
         "DashboardNamePrefix": str,
         "NextToken": str,
     },
     total=False,
@@ -674,38 +621,30 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 ManagedRuleStateTypeDef = TypedDict(
     "ManagedRuleStateTypeDef",
     {
         "RuleName": str,
         "State": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 StatisticSetTypeDef = TypedDict(
     "StatisticSetTypeDef",
     {
         "SampleCount": float,
         "Sum": float,
         "Minimum": float,
         "Maximum": float,
@@ -717,67 +656,30 @@
     {
         "Namespace": str,
         "MetricNames": Sequence[str],
     },
     total=False,
 )
 
-MetricStreamStatisticsMetricOutputTypeDef = TypedDict(
-    "MetricStreamStatisticsMetricOutputTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-    },
-)
-
 MetricStreamStatisticsMetricTypeDef = TypedDict(
     "MetricStreamStatisticsMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
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
 PutDashboardInputRequestTypeDef = TypedDict(
     "PutDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
         "DashboardBody": str,
     },
 )
 
-PutMetricStreamOutputTypeDef = TypedDict(
-    "PutMetricStreamOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 _RequiredSetAlarmStateInputAlarmSetStateTypeDef = TypedDict(
     "_RequiredSetAlarmStateInputAlarmSetStateTypeDef",
     {
         "StateValue": StateValueType,
         "StateReason": str,
     },
 )
@@ -833,23 +735,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-DescribeAlarmHistoryOutputTypeDef = TypedDict(
-    "DescribeAlarmHistoryOutputTypeDef",
-    {
-        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AnomalyDetectorConfigurationOutputTypeDef = TypedDict(
     "AnomalyDetectorConfigurationOutputTypeDef",
     {
         "ExcludedTimeRanges": List[RangeOutputTypeDef],
         "MetricTimezone": str,
     },
     total=False,
@@ -860,61 +753,14 @@
     {
         "ExcludedTimeRanges": Sequence[RangeTypeDef],
         "MetricTimezone": str,
     },
     total=False,
 )
 
-MetricOutputTypeDef = TypedDict(
-    "MetricOutputTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionOutputTypeDef],
-    },
-    total=False,
-)
-
-SingleMetricAnomalyDetectorOutputTypeDef = TypedDict(
-    "SingleMetricAnomalyDetectorOutputTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionOutputTypeDef],
-        "Stat": str,
-    },
-    total=False,
-)
-
-ListDashboardsOutputTypeDef = TypedDict(
-    "ListDashboardsOutputTypeDef",
-    {
-        "DashboardEntries": List[DashboardEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutDashboardOutputTypeDef = TypedDict(
-    "PutDashboardOutputTypeDef",
-    {
-        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMetricStatisticsOutputTypeDef = TypedDict(
-    "GetMetricStatisticsOutputTypeDef",
-    {
-        "Label": str,
-        "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeAlarmsForMetricInputRequestTypeDef = TypedDict(
     "_RequiredDescribeAlarmsForMetricInputRequestTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
     },
 )
@@ -932,26 +778,14 @@
 
 class DescribeAlarmsForMetricInputRequestTypeDef(
     _RequiredDescribeAlarmsForMetricInputRequestTypeDef,
     _OptionalDescribeAlarmsForMetricInputRequestTypeDef,
 ):
     pass
 
-DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": Sequence[DimensionTypeDef],
-        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAnomalyDetectorsInputRequestTypeDef = TypedDict(
     "DescribeAnomalyDetectorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Namespace": str,
         "MetricName": str,
@@ -1008,24 +842,45 @@
 )
 
 class GetMetricStatisticsInputRequestTypeDef(
     _RequiredGetMetricStatisticsInputRequestTypeDef, _OptionalGetMetricStatisticsInputRequestTypeDef
 ):
     pass
 
+MetricOutputTypeDef = TypedDict(
+    "MetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+    },
+    total=False,
+)
+
 MetricTypeDef = TypedDict(
     "MetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
     },
     total=False,
 )
 
+SingleMetricAnomalyDetectorOutputTypeDef = TypedDict(
+    "SingleMetricAnomalyDetectorOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+    },
+    total=False,
+)
+
 SingleMetricAnomalyDetectorTypeDef = TypedDict(
     "SingleMetricAnomalyDetectorTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
@@ -1033,40 +888,158 @@
     total=False,
 )
 
 DeleteInsightRulesOutputTypeDef = TypedDict(
     "DeleteInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmHistoryOutputTypeDef = TypedDict(
+    "DescribeAlarmHistoryOutputTypeDef",
+    {
+        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableInsightRulesOutputTypeDef = TypedDict(
     "DisableInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
 
 EnableInsightRulesOutputTypeDef = TypedDict(
     "EnableInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDashboardOutputTypeDef = TypedDict(
+    "GetDashboardOutputTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardBody": str,
+        "DashboardName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMetricStatisticsOutputTypeDef = TypedDict(
+    "GetMetricStatisticsOutputTypeDef",
+    {
+        "Label": str,
+        "Datapoints": List[DatapointTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMetricWidgetImageOutputTypeDef = TypedDict(
+    "GetMetricWidgetImageOutputTypeDef",
+    {
+        "MetricWidgetImage": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDashboardsOutputTypeDef = TypedDict(
+    "ListDashboardsOutputTypeDef",
+    {
+        "DashboardEntries": List[DashboardEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutDashboardOutputTypeDef = TypedDict(
+    "PutDashboardOutputTypeDef",
+    {
+        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutManagedInsightRulesOutputTypeDef = TypedDict(
     "PutManagedInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutMetricStreamOutputTypeDef = TypedDict(
+    "PutMetricStreamOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+    {
+        "AlarmName": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": Union[datetime, str],
+        "EndDate": Union[datetime, str],
+        "ScanBy": ScanByType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
+    {
+        "AlarmNames": Sequence[str],
+        "AlarmNamePrefix": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "ChildrenOfAlarmName": str,
+        "ParentsOfAlarmName": str,
+        "StateValue": StateValueType,
+        "ActionPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": Sequence[DimensionTypeDef],
+        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
+    {
+        "DashboardNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 DescribeAlarmsInputAlarmExistsWaitTypeDef = TypedDict(
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
@@ -1100,28 +1073,28 @@
 )
 
 DescribeInsightRulesOutputTypeDef = TypedDict(
     "DescribeInsightRulesOutputTypeDef",
     {
         "NextToken": str,
         "InsightRules": List[InsightRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMetricsInputListMetricsPaginateTypeDef = TypedDict(
     "ListMetricsInputListMetricsPaginateTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionFilterTypeDef],
         "RecentlyActive": Literal["PT3H"],
         "IncludeLinkedAccounts": bool,
         "OwningAccount": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMetricsInputRequestTypeDef = TypedDict(
     "ListMetricsInputRequestTypeDef",
     {
@@ -1159,34 +1132,24 @@
 )
 
 ListMetricStreamsOutputTypeDef = TypedDict(
     "ListMetricStreamsOutputTypeDef",
     {
         "NextToken": str,
         "Entries": List[MetricStreamEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ManagedRuleDescriptionTypeDef = TypedDict(
-    "ManagedRuleDescriptionTypeDef",
-    {
-        "TemplateName": str,
-        "ResourceARN": str,
-        "RuleState": ManagedRuleStateTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredManagedRuleTypeDef = TypedDict(
     "_RequiredManagedRuleTypeDef",
     {
         "TemplateName": str,
         "ResourceARN": str,
@@ -1256,14 +1219,24 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+ManagedRuleDescriptionTypeDef = TypedDict(
+    "ManagedRuleDescriptionTypeDef",
+    {
+        "TemplateName": str,
+        "ResourceARN": str,
+        "RuleState": ManagedRuleStateTypeDef,
+    },
+    total=False,
+)
+
 _RequiredMetricDatumTypeDef = TypedDict(
     "_RequiredMetricDatumTypeDef",
     {
         "MetricName": str,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
@@ -1283,15 +1256,15 @@
 
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
 MetricStreamStatisticsConfigurationOutputTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationOutputTypeDef",
     {
-        "IncludeMetrics": List[MetricStreamStatisticsMetricOutputTypeDef],
+        "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
         "AdditionalStatistics": List[str],
     },
 )
 
 MetricStreamStatisticsConfigurationTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationTypeDef",
     {
@@ -1302,15 +1275,15 @@
 
 ListMetricsOutputTypeDef = TypedDict(
     "ListMetricsOutputTypeDef",
     {
         "Metrics": List[MetricOutputTypeDef],
         "NextToken": str,
         "OwningAccounts": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMetricStatOutputTypeDef = TypedDict(
     "_RequiredMetricStatOutputTypeDef",
     {
         "Metric": MetricOutputTypeDef,
@@ -1350,44 +1323,44 @@
 
 GetMetricDataOutputTypeDef = TypedDict(
     "GetMetricDataOutputTypeDef",
     {
         "MetricDataResults": List[MetricDataResultTypeDef],
         "NextToken": str,
         "Messages": List[MessageDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightRuleReportOutputTypeDef = TypedDict(
     "GetInsightRuleReportOutputTypeDef",
     {
         "KeyLabels": List[str],
         "AggregationStatistic": str,
         "AggregateValue": float,
         "ApproximateUniqueCount": int,
         "Contributors": List[InsightRuleContributorTypeDef],
         "MetricDatapoints": List[InsightRuleMetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListManagedInsightRulesOutputTypeDef = TypedDict(
-    "ListManagedInsightRulesOutputTypeDef",
+PutManagedInsightRulesInputRequestTypeDef = TypedDict(
+    "PutManagedInsightRulesInputRequestTypeDef",
     {
-        "ManagedRules": List[ManagedRuleDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ManagedRules": Sequence[ManagedRuleTypeDef],
     },
 )
 
-PutManagedInsightRulesInputRequestTypeDef = TypedDict(
-    "PutManagedInsightRulesInputRequestTypeDef",
+ListManagedInsightRulesOutputTypeDef = TypedDict(
+    "ListManagedInsightRulesOutputTypeDef",
     {
-        "ManagedRules": Sequence[ManagedRuleTypeDef],
+        "ManagedRules": List[ManagedRuleDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMetricDataInputRequestTypeDef = TypedDict(
     "PutMetricDataInputRequestTypeDef",
     {
         "Namespace": str,
@@ -1406,15 +1379,15 @@
         "RoleArn": str,
         "State": str,
         "CreationDate": datetime,
         "LastUpdateDate": datetime,
         "OutputFormat": MetricStreamOutputFormatType,
         "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationOutputTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
     "_RequiredPutMetricStreamInputRequestTypeDef",
     {
         "Name": str,
@@ -1501,15 +1474,15 @@
         "StateReason": str,
         "StateReasonData": str,
         "StateUpdatedTimestamp": datetime,
         "MetricName": str,
         "Namespace": str,
         "Statistic": StatisticType,
         "ExtendedStatistic": str,
-        "Dimensions": List[DimensionOutputTypeDef],
+        "Dimensions": List[DimensionTypeDef],
         "Period": int,
         "Unit": StandardUnitType,
         "EvaluationPeriods": int,
         "DatapointsToAlarm": int,
         "Threshold": float,
         "ComparisonOperator": ComparisonOperatorType,
         "TreatMissingData": str,
@@ -1539,15 +1512,15 @@
     },
 )
 _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
     "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
     {
         "ScanBy": ScanByType,
         "LabelOptions": LabelOptionsTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class GetMetricDataInputGetMetricDataPaginateTypeDef(
     _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
     _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
@@ -1663,34 +1636,34 @@
 ):
     pass
 
 DescribeAlarmsForMetricOutputTypeDef = TypedDict(
     "DescribeAlarmsForMetricOutputTypeDef",
     {
         "MetricAlarms": List[MetricAlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAlarmsOutputTypeDef = TypedDict(
     "DescribeAlarmsOutputTypeDef",
     {
         "CompositeAlarms": List[CompositeAlarmTypeDef],
         "MetricAlarms": List[MetricAlarmTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AnomalyDetectorTypeDef = TypedDict(
     "AnomalyDetectorTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
-        "Dimensions": List[DimensionOutputTypeDef],
+        "Dimensions": List[DimensionTypeDef],
         "Stat": str,
         "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
         "StateValue": AnomalyDetectorStateValueType,
         "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
         "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
     },
     total=False,
@@ -1724,10 +1697,10 @@
 )
 
 DescribeAnomalyDetectorsOutputTypeDef = TypedDict(
     "DescribeAnomalyDetectorsOutputTypeDef",
     {
         "AnomalyDetectors": List[AnomalyDetectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/waiter.py` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch/waiter.pyi` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/PKG-INFO` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudWatch 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudWatch 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -448,115 +448,112 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
     RangeOutputTypeDef,
     RangeTypeDef,
-    DimensionOutputTypeDef,
+    DimensionTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
-    DimensionTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
     DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
-    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAlarmHistoryInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
-    GetDashboardOutputTypeDef,
     GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
     MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
-    GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
-    ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
-    ManagedRuleStateTypeDef,
     TagTypeDef,
+    ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
     MetricStreamFilterTypeDef,
-    MetricStreamStatisticsMetricOutputTypeDef,
     MetricStreamStatisticsMetricTypeDef,
-    PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
-    PutMetricStreamOutputTypeDef,
-    ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    DescribeAlarmHistoryOutputTypeDef,
     AnomalyDetectorConfigurationOutputTypeDef,
     AnomalyDetectorConfigurationTypeDef,
-    MetricOutputTypeDef,
-    SingleMetricAnomalyDetectorOutputTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
-    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
     GetMetricStatisticsInputMetricGetStatisticsTypeDef,
     GetMetricStatisticsInputRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
+    SingleMetricAnomalyDetectorOutputTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
     DeleteInsightRulesOutputTypeDef,
+    DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableInsightRulesOutputTypeDef,
+    GetDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
+    GetMetricWidgetImageOutputTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
+    PutMetricStreamOutputTypeDef,
+    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
+    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
+    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
+    ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    ManagedRuleDescriptionTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
     MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
     MetricStatOutputTypeDef,
     MetricStatTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
-    ListManagedInsightRulesOutputTypeDef,
     PutManagedInsightRulesInputRequestTypeDef,
+    ListManagedInsightRulesOutputTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
     PutMetricStreamInputRequestTypeDef,
     MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     MetricAlarmTypeDef,
     MetricMathAnomalyDetectorOutputTypeDef,
```

### Comparing `mypy-boto3-cloudwatch-1.28.12/mypy_boto3_cloudwatch.egg-info/SOURCES.txt` & `mypy-boto3-cloudwatch-1.28.15/mypy_boto3_cloudwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.12/setup.py` & `mypy-boto3-cloudwatch-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudwatch",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cloudwatch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatch 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CloudWatch 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

