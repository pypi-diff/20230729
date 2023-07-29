# Comparing `tmp/mypy-boto3-lookoutmetrics-1.28.15.tar.gz` & `tmp/mypy-boto3-lookoutmetrics-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutmetrics-1.28.15.tar", last modified: Fri Jul 28 20:43:11 2023, max compression
+gzip compressed data, was "mypy-boto3-lookoutmetrics-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:34 2023, max compression
```

## Comparing `mypy-boto3-lookoutmetrics-1.28.15.tar` & `mypy-boto3-lookoutmetrics-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.773426 mypy-boto3-lookoutmetrics-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-07-28 20:43:11.769426 mypy-boto3-lookoutmetrics-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.765426 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39698 2023-07-28 20:30:36.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39665 2023-07-28 20:30:35.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.765426 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:11.773426 mypy-boto3-lookoutmetrics-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.025253 mypy-boto3-lookoutmetrics-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16902 2023-07-29 10:03:34.017253 mypy-boto3-lookoutmetrics-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.009253 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22906 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-07-29 09:50:13.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-07-29 09:50:14.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-07-29 09:50:13.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.017253 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16902 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:34.025253 mypy-boto3-lookoutmetrics-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/LICENSE` & `mypy-boto3-lookoutmetrics-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/PKG-INFO` & `mypy-boto3-lookoutmetrics-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutmetrics
-Version: 1.28.15
-Summary: Type annotations for boto3.LookoutMetrics 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LookoutMetrics 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/README.md` & `mypy-boto3-lookoutmetrics-1.28.15.post1/README.md`

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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/__main__.py` & `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutMetrics 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.LookoutMetrics 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics\nOther"
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

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/client.py` & `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,22 @@
     from boto3.session import Session
     from mypy_boto3_lookoutmetrics.client import LookoutMetricsClient
 
     session = Session()
     client: LookoutMetricsClient = session.client("lookoutmetrics")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FrequencyType, RelationshipTypeType
 from .type_defs import (
     ActionTypeDef,
+    AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AutoDetectionMetricSourceTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
@@ -40,15 +41,17 @@
     ListAlertsResponseTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MetricSetDimensionFilterOutputTypeDef,
     MetricSetDimensionFilterTypeDef,
+    MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     MetricTypeDef,
     SampleDataS3SourceConfigTypeDef,
     TimestampColumnTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
@@ -130,15 +133,15 @@
         *,
         AlertName: str,
         AnomalyDetectorArn: str,
         Action: ActionTypeDef,
         AlertSensitivityThreshold: int = ...,
         AlertDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef] = ...
     ) -> CreateAlertResponseTypeDef:
         """
         Creates an alert for an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_alert)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#create_alert)
         """
@@ -161,23 +164,25 @@
 
     def create_metric_set(
         self,
         *,
         AnomalyDetectorArn: str,
         MetricSetName: str,
         MetricList: Sequence[MetricTypeDef],
-        MetricSource: MetricSourceTypeDef,
+        MetricSource: Union[MetricSourceTypeDef, MetricSourceOutputTypeDef],
         MetricSetDescription: str = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         Timezone: str = ...,
         Tags: Mapping[str, str] = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        DimensionFilterList: Sequence[
+            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
+        ] = ...
     ) -> CreateMetricSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_metric_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#create_metric_set)
         """
@@ -441,15 +446,15 @@
     def update_alert(
         self,
         *,
         AlertArn: str,
         AlertDescription: str = ...,
         AlertSensitivityThreshold: int = ...,
         Action: ActionTypeDef = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef] = ...
     ) -> UpdateAlertResponseTypeDef:
         """
         Make changes to an existing alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_alert)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#update_alert)
         """
@@ -475,16 +480,18 @@
         MetricSetArn: str,
         MetricSetDescription: str = ...,
         MetricList: Sequence[MetricTypeDef] = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
-        MetricSource: MetricSourceTypeDef = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        MetricSource: Union[MetricSourceTypeDef, MetricSourceOutputTypeDef] = ...,
+        DimensionFilterList: Sequence[
+            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
+        ] = ...
     ) -> UpdateMetricSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_metric_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#update_metric_set)
         """
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/client.pyi` & `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,22 @@
     from boto3.session import Session
     from mypy_boto3_lookoutmetrics.client import LookoutMetricsClient
 
     session = Session()
     client: LookoutMetricsClient = session.client("lookoutmetrics")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FrequencyType, RelationshipTypeType
 from .type_defs import (
     ActionTypeDef,
+    AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AutoDetectionMetricSourceTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
@@ -40,15 +41,17 @@
     ListAlertsResponseTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MetricSetDimensionFilterOutputTypeDef,
     MetricSetDimensionFilterTypeDef,
+    MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     MetricTypeDef,
     SampleDataS3SourceConfigTypeDef,
     TimestampColumnTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
@@ -122,15 +125,15 @@
         *,
         AlertName: str,
         AnomalyDetectorArn: str,
         Action: ActionTypeDef,
         AlertSensitivityThreshold: int = ...,
         AlertDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef] = ...
     ) -> CreateAlertResponseTypeDef:
         """
         Creates an alert for an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_alert)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#create_alert)
         """
@@ -151,23 +154,25 @@
         """
     def create_metric_set(
         self,
         *,
         AnomalyDetectorArn: str,
         MetricSetName: str,
         MetricList: Sequence[MetricTypeDef],
-        MetricSource: MetricSourceTypeDef,
+        MetricSource: Union[MetricSourceTypeDef, MetricSourceOutputTypeDef],
         MetricSetDescription: str = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         Timezone: str = ...,
         Tags: Mapping[str, str] = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        DimensionFilterList: Sequence[
+            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
+        ] = ...
     ) -> CreateMetricSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_metric_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#create_metric_set)
         """
@@ -407,15 +412,15 @@
     def update_alert(
         self,
         *,
         AlertArn: str,
         AlertDescription: str = ...,
         AlertSensitivityThreshold: int = ...,
         Action: ActionTypeDef = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef] = ...
     ) -> UpdateAlertResponseTypeDef:
         """
         Make changes to an existing alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_alert)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#update_alert)
         """
@@ -439,16 +444,18 @@
         MetricSetArn: str,
         MetricSetDescription: str = ...,
         MetricList: Sequence[MetricTypeDef] = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
-        MetricSource: MetricSourceTypeDef = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        MetricSource: Union[MetricSourceTypeDef, MetricSourceOutputTypeDef] = ...,
+        DimensionFilterList: Sequence[
+            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
+        ] = ...
     ) -> UpdateMetricSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_metric_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#update_metric_set)
         """
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/literals.py` & `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/literals.pyi` & `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/type_defs.py` & `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
 
     data: LambdaConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregationFunctionType,
     AlertStatusType,
     AlertTypeType,
     AnomalyDetectionTaskStatusType,
     AnomalyDetectorFailureTypeType,
@@ -1477,15 +1477,17 @@
         "MetricSetDescription": str,
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "Tags": Mapping[str, str],
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
+        "DimensionFilterList": Sequence[
+            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
@@ -1505,15 +1507,17 @@
         "MetricSetDescription": str,
         "MetricList": Sequence[MetricTypeDef],
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
+        "DimensionFilterList": Sequence[
+            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/type_defs.pyi` & `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
 
     data: LambdaConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregationFunctionType,
     AlertStatusType,
     AlertTypeType,
     AnomalyDetectionTaskStatusType,
     AnomalyDetectorFailureTypeType,
@@ -1448,15 +1448,17 @@
         "MetricSetDescription": str,
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "Tags": Mapping[str, str],
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
+        "DimensionFilterList": Sequence[
+            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
@@ -1474,15 +1476,17 @@
         "MetricSetDescription": str,
         "MetricList": Sequence[MetricTypeDef],
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
+        "DimensionFilterList": Sequence[
+            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO` & `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutmetrics
-Version: 1.28.15
-Summary: Type annotations for boto3.LookoutMetrics 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LookoutMetrics 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt` & `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.15/setup.py` & `mypy-boto3-lookoutmetrics-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutmetrics",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_lookoutmetrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.LookoutMetrics 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

