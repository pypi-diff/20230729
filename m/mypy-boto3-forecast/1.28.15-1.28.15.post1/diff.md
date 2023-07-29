# Comparing `tmp/mypy-boto3-forecast-1.28.15.tar.gz` & `tmp/mypy-boto3-forecast-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-forecast-1.28.15.tar", last modified: Fri Jul 28 20:42:50 2023, max compression
+gzip compressed data, was "mypy-boto3-forecast-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:09 2023, max compression
```

## Comparing `mypy-boto3-forecast-1.28.15.tar` & `mypy-boto3-forecast-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.081128 mypy-boto3-forecast-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23727 2023-07-28 20:42:50.077128 mypy-boto3-forecast-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.073128 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51565 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51481 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-07-28 20:26:03.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71201 2023-07-28 20:26:06.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71135 2023-07-28 20:26:04.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.073128 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23727 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:50.081128 mypy-boto3-forecast-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:26:01.000000 mypy-boto3-forecast-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.669155 mypy-boto3-forecast-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23733 2023-07-29 10:03:09.669155 mypy-boto3-forecast-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.665155 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52340 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52256 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71276 2023-07-29 09:45:37.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71210 2023-07-29 09:45:36.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.669155 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23733 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:09.669155 mypy-boto3-forecast-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-forecast-1.28.15/LICENSE` & `mypy-boto3-forecast-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15/PKG-INFO` & `mypy-boto3-forecast-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-forecast
-Version: 1.28.15
-Summary: Type annotations for boto3.ForecastService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ForecastService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-forecast-1.28.15/README.md` & `mypy-boto3-forecast-1.28.15.post1/README.md`

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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__init__.py` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__init__.pyi` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__main__.py` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ForecastService 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.ForecastService 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService\nOther"
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

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/client.py` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_forecast.client import ForecastServiceClient
 
     session = Session()
     client: ForecastServiceClient = session.client("forecast")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoMLOverrideStrategyType,
     DatasetTypeType,
     DomainType,
@@ -52,14 +52,15 @@
     CreateForecastResponseTypeDef,
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
+    DataConfigOutputTypeDef,
     DataConfigTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
@@ -73,18 +74,21 @@
     DescribeWhatIfAnalysisResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     EvaluationParametersTypeDef,
     ExplainabilityConfigTypeDef,
+    FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
     FilterTypeDef,
     GetAccuracyMetricsResponseTypeDef,
+    HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListExplainabilitiesResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
@@ -94,19 +98,23 @@
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListPredictorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MonitorConfigTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
+    TimeSeriesReplacementsDataSourceOutputTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
+    TimeSeriesSelectorOutputTypeDef,
     TimeSeriesSelectorTypeDef,
+    TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -170,15 +178,15 @@
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int = ...,
         ForecastTypes: Sequence[str] = ...,
         ForecastDimensions: Sequence[str] = ...,
         ForecastFrequency: str = ...,
-        DataConfig: DataConfigTypeDef = ...,
+        DataConfig: Union[DataConfigTypeDef, DataConfigOutputTypeDef] = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         ReferencePredictorArn: str = ...,
         OptimizationMetric: OptimizationMetricType = ...,
         ExplainPredictor: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MonitorConfig: MonitorConfigTypeDef = ...,
         TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...
@@ -192,15 +200,15 @@
 
     def create_dataset(
         self,
         *,
         DatasetName: str,
         Domain: DomainType,
         DatasetType: DatasetTypeType,
-        Schema: SchemaTypeDef,
+        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef],
         DataFrequency: str = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an Amazon Forecast dataset.
 
@@ -247,15 +255,15 @@
     def create_explainability(
         self,
         *,
         ExplainabilityName: str,
         ResourceArn: str,
         ExplainabilityConfig: ExplainabilityConfigTypeDef,
         DataSource: DataSourceTypeDef = ...,
-        Schema: SchemaTypeDef = ...,
+        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...,
         EnableVisualization: bool = ...,
         StartDateTime: str = ...,
         EndDateTime: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateExplainabilityResponseTypeDef:
         """
         .
@@ -284,15 +292,15 @@
     def create_forecast(
         self,
         *,
         ForecastName: str,
         PredictorArn: str,
         ForecastTypes: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...
+        TimeSeriesSelector: Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef] = ...
     ) -> CreateForecastResponseTypeDef:
         """
         Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
         used to train the predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/client/#create_forecast)
@@ -326,24 +334,26 @@
         """
 
     def create_predictor(
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int,
-        InputDataConfig: InputDataConfigTypeDef,
-        FeaturizationConfig: FeaturizationConfigTypeDef,
+        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        FeaturizationConfig: Union[FeaturizationConfigTypeDef, FeaturizationConfigOutputTypeDef],
         AlgorithmArn: str = ...,
         ForecastTypes: Sequence[str] = ...,
         PerformAutoML: bool = ...,
         AutoMLOverrideStrategy: AutoMLOverrideStrategyType = ...,
         PerformHPO: bool = ...,
         TrainingParameters: Mapping[str, str] = ...,
         EvaluationParameters: EvaluationParametersTypeDef = ...,
-        HPOConfig: HyperParameterTuningJobConfigTypeDef = ...,
+        HPOConfig: Union[
+            HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
+        ] = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OptimizationMetric: OptimizationMetricType = ...
     ) -> CreatePredictorResponseTypeDef:
         """
         .
 
@@ -369,15 +379,15 @@
         """
 
     def create_what_if_analysis(
         self,
         *,
         WhatIfAnalysisName: str,
         ForecastArn: str,
-        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...,
+        TimeSeriesSelector: Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfAnalysisResponseTypeDef:
         """
         What-if analysis is a scenario modeling technique where you make a hypothetical
         change to a time series and compare the forecasts generated by these changes
         against the baseline, unchanged time series.
 
@@ -386,16 +396,20 @@
         """
 
     def create_what_if_forecast(
         self,
         *,
         WhatIfForecastName: str,
         WhatIfAnalysisArn: str,
-        TimeSeriesTransformations: Sequence[TimeSeriesTransformationTypeDef] = ...,
-        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceTypeDef = ...,
+        TimeSeriesTransformations: Sequence[
+            Union[TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef]
+        ] = ...,
+        TimeSeriesReplacementsDataSource: Union[
+            TimeSeriesReplacementsDataSourceTypeDef, TimeSeriesReplacementsDataSourceOutputTypeDef
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfForecastResponseTypeDef:
         """
         A what-if forecast is a forecast that is created from a modified version of the
         baseline forecast.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast)
```

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/client.pyi` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_forecast.client import ForecastServiceClient
 
     session = Session()
     client: ForecastServiceClient = session.client("forecast")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoMLOverrideStrategyType,
     DatasetTypeType,
     DomainType,
@@ -52,14 +52,15 @@
     CreateForecastResponseTypeDef,
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
+    DataConfigOutputTypeDef,
     DataConfigTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
@@ -73,18 +74,21 @@
     DescribeWhatIfAnalysisResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     EvaluationParametersTypeDef,
     ExplainabilityConfigTypeDef,
+    FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
     FilterTypeDef,
     GetAccuracyMetricsResponseTypeDef,
+    HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListExplainabilitiesResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
@@ -94,19 +98,23 @@
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListPredictorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MonitorConfigTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
+    TimeSeriesReplacementsDataSourceOutputTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
+    TimeSeriesSelectorOutputTypeDef,
     TimeSeriesSelectorTypeDef,
+    TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -163,15 +171,15 @@
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int = ...,
         ForecastTypes: Sequence[str] = ...,
         ForecastDimensions: Sequence[str] = ...,
         ForecastFrequency: str = ...,
-        DataConfig: DataConfigTypeDef = ...,
+        DataConfig: Union[DataConfigTypeDef, DataConfigOutputTypeDef] = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         ReferencePredictorArn: str = ...,
         OptimizationMetric: OptimizationMetricType = ...,
         ExplainPredictor: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MonitorConfig: MonitorConfigTypeDef = ...,
         TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...
@@ -184,15 +192,15 @@
         """
     def create_dataset(
         self,
         *,
         DatasetName: str,
         Domain: DomainType,
         DatasetType: DatasetTypeType,
-        Schema: SchemaTypeDef,
+        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef],
         DataFrequency: str = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an Amazon Forecast dataset.
 
@@ -236,15 +244,15 @@
     def create_explainability(
         self,
         *,
         ExplainabilityName: str,
         ResourceArn: str,
         ExplainabilityConfig: ExplainabilityConfigTypeDef,
         DataSource: DataSourceTypeDef = ...,
-        Schema: SchemaTypeDef = ...,
+        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...,
         EnableVisualization: bool = ...,
         StartDateTime: str = ...,
         EndDateTime: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateExplainabilityResponseTypeDef:
         """
         .
@@ -271,15 +279,15 @@
     def create_forecast(
         self,
         *,
         ForecastName: str,
         PredictorArn: str,
         ForecastTypes: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...
+        TimeSeriesSelector: Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef] = ...
     ) -> CreateForecastResponseTypeDef:
         """
         Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
         used to train the predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/client/#create_forecast)
@@ -310,24 +318,26 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/client/#create_monitor)
         """
     def create_predictor(
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int,
-        InputDataConfig: InputDataConfigTypeDef,
-        FeaturizationConfig: FeaturizationConfigTypeDef,
+        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
+        FeaturizationConfig: Union[FeaturizationConfigTypeDef, FeaturizationConfigOutputTypeDef],
         AlgorithmArn: str = ...,
         ForecastTypes: Sequence[str] = ...,
         PerformAutoML: bool = ...,
         AutoMLOverrideStrategy: AutoMLOverrideStrategyType = ...,
         PerformHPO: bool = ...,
         TrainingParameters: Mapping[str, str] = ...,
         EvaluationParameters: EvaluationParametersTypeDef = ...,
-        HPOConfig: HyperParameterTuningJobConfigTypeDef = ...,
+        HPOConfig: Union[
+            HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
+        ] = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OptimizationMetric: OptimizationMetricType = ...
     ) -> CreatePredictorResponseTypeDef:
         """
         .
 
@@ -351,15 +361,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/client/#create_predictor_backtest_export_job)
         """
     def create_what_if_analysis(
         self,
         *,
         WhatIfAnalysisName: str,
         ForecastArn: str,
-        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...,
+        TimeSeriesSelector: Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfAnalysisResponseTypeDef:
         """
         What-if analysis is a scenario modeling technique where you make a hypothetical
         change to a time series and compare the forecasts generated by these changes
         against the baseline, unchanged time series.
 
@@ -367,16 +377,20 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/client/#create_what_if_analysis)
         """
     def create_what_if_forecast(
         self,
         *,
         WhatIfForecastName: str,
         WhatIfAnalysisArn: str,
-        TimeSeriesTransformations: Sequence[TimeSeriesTransformationTypeDef] = ...,
-        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceTypeDef = ...,
+        TimeSeriesTransformations: Sequence[
+            Union[TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef]
+        ] = ...,
+        TimeSeriesReplacementsDataSource: Union[
+            TimeSeriesReplacementsDataSourceTypeDef, TimeSeriesReplacementsDataSourceOutputTypeDef
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfForecastResponseTypeDef:
         """
         A what-if forecast is a forecast that is created from a modified version of the
         baseline forecast.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast)
```

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/literals.py` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/literals.pyi` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/paginator.py` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/paginator.pyi` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/type_defs.py` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_forecast.type_defs import ActionTypeDef
 
     data: ActionTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AttributeTypeType,
     AutoMLOverrideStrategyType,
     ConditionType,
     DatasetTypeType,
     DayOfWeekType,
@@ -39,15 +39,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionTypeDef",
     "AdditionalDatasetOutputTypeDef",
     "AdditionalDatasetTypeDef",
     "AttributeConfigOutputTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
@@ -268,42 +267,38 @@
     "_OptionalAdditionalDatasetOutputTypeDef",
     {
         "Configuration": Dict[str, List[str]],
     },
     total=False,
 )
 
-
 class AdditionalDatasetOutputTypeDef(
     _RequiredAdditionalDatasetOutputTypeDef, _OptionalAdditionalDatasetOutputTypeDef
 ):
     pass
 
-
 _RequiredAdditionalDatasetTypeDef = TypedDict(
     "_RequiredAdditionalDatasetTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalAdditionalDatasetTypeDef = TypedDict(
     "_OptionalAdditionalDatasetTypeDef",
     {
         "Configuration": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class AdditionalDatasetTypeDef(
     _RequiredAdditionalDatasetTypeDef, _OptionalAdditionalDatasetTypeDef
 ):
     pass
 
-
 AttributeConfigOutputTypeDef = TypedDict(
     "AttributeConfigOutputTypeDef",
     {
         "AttributeName": str,
         "Transformations": Dict[str, str],
     },
 )
@@ -353,21 +348,19 @@
     "_OptionalContinuousParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
-
 class ContinuousParameterRangeTypeDef(
     _RequiredContinuousParameterRangeTypeDef, _OptionalContinuousParameterRangeTypeDef
 ):
     pass
 
-
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "RoleArn": str,
         "KMSKeyArn": str,
     },
 )
@@ -437,19 +430,17 @@
     "_OptionalS3ConfigTypeDef",
     {
         "KMSKeyArn": str,
     },
     total=False,
 )
 
-
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
-
 DatasetGroupSummaryTypeDef = TypedDict(
     "DatasetGroupSummaryTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetGroupName": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
@@ -734,42 +725,38 @@
     "_OptionalFeaturizationMethodOutputTypeDef",
     {
         "FeaturizationMethodParameters": Dict[str, str],
     },
     total=False,
 )
 
-
 class FeaturizationMethodOutputTypeDef(
     _RequiredFeaturizationMethodOutputTypeDef, _OptionalFeaturizationMethodOutputTypeDef
 ):
     pass
 
-
 _RequiredFeaturizationMethodTypeDef = TypedDict(
     "_RequiredFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodName": Literal["filling"],
     },
 )
 _OptionalFeaturizationMethodTypeDef = TypedDict(
     "_OptionalFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodParameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class FeaturizationMethodTypeDef(
     _RequiredFeaturizationMethodTypeDef, _OptionalFeaturizationMethodTypeDef
 ):
     pass
 
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Key": str,
         "Value": str,
         "Condition": FilterConditionStringType,
     },
@@ -818,21 +805,19 @@
     "_OptionalIntegerParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
-
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1012,19 +997,17 @@
     {
         "AttributeConfigs": List[AttributeConfigOutputTypeDef],
         "AdditionalDatasets": List[AdditionalDatasetOutputTypeDef],
     },
     total=False,
 )
 
-
 class DataConfigOutputTypeDef(_RequiredDataConfigOutputTypeDef, _OptionalDataConfigOutputTypeDef):
     pass
 
-
 _RequiredDataConfigTypeDef = TypedDict(
     "_RequiredDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalDataConfigTypeDef = TypedDict(
@@ -1032,19 +1015,17 @@
     {
         "AttributeConfigs": Sequence[AttributeConfigTypeDef],
         "AdditionalDatasets": Sequence[AdditionalDatasetTypeDef],
     },
     total=False,
 )
 
-
 class DataConfigTypeDef(_RequiredDataConfigTypeDef, _OptionalDataConfigTypeDef):
     pass
 
-
 PredictorBaselineTypeDef = TypedDict(
     "PredictorBaselineTypeDef",
     {
         "BaselineMetrics": List[BaselineMetricTypeDef],
     },
     total=False,
 )
@@ -1061,22 +1042,20 @@
     {
         "DatasetArns": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetGroupRequestRequestTypeDef(
     _RequiredCreateDatasetGroupRequestRequestTypeDef,
     _OptionalCreateDatasetGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMonitorRequestRequestTypeDef",
     {
         "MonitorName": str,
         "ResourceArn": str,
     },
 )
@@ -1084,21 +1063,19 @@
     "_OptionalCreateMonitorRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMonitorRequestRequestTypeDef(
     _RequiredCreateMonitorRequestRequestTypeDef, _OptionalCreateMonitorRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1317,40 +1294,36 @@
     "_OptionalFeaturizationOutputTypeDef",
     {
         "FeaturizationPipeline": List[FeaturizationMethodOutputTypeDef],
     },
     total=False,
 )
 
-
 class FeaturizationOutputTypeDef(
     _RequiredFeaturizationOutputTypeDef, _OptionalFeaturizationOutputTypeDef
 ):
     pass
 
-
 _RequiredFeaturizationTypeDef = TypedDict(
     "_RequiredFeaturizationTypeDef",
     {
         "AttributeName": str,
     },
 )
 _OptionalFeaturizationTypeDef = TypedDict(
     "_OptionalFeaturizationTypeDef",
     {
         "FeaturizationPipeline": Sequence[FeaturizationMethodTypeDef],
     },
     total=False,
 )
 
-
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
-
 ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetImportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
@@ -1409,22 +1382,20 @@
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class ListMonitorEvaluationsRequestRequestTypeDef(
     _RequiredListMonitorEvaluationsRequestRequestTypeDef,
     _OptionalListMonitorEvaluationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListMonitorsRequestRequestTypeDef = TypedDict(
     "ListMonitorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
@@ -1500,40 +1471,36 @@
     "_OptionalInputDataConfigOutputTypeDef",
     {
         "SupplementaryFeatures": List[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
-
 class InputDataConfigOutputTypeDef(
     _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
 ):
     pass
 
-
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalInputDataConfigTypeDef = TypedDict(
     "_OptionalInputDataConfigTypeDef",
     {
         "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
-
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
-
 ParameterRangesOutputTypeDef = TypedDict(
     "ParameterRangesOutputTypeDef",
     {
         "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
         "ContinuousParameterRanges": List[ContinuousParameterRangeTypeDef],
         "IntegerParameterRanges": List[IntegerParameterRangeTypeDef],
     },
@@ -1622,22 +1589,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
     _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
 ):
     pass
 
-
 ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
     "ListMonitorsRequestListMonitorsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1834,22 +1799,20 @@
         "Tags": Sequence[TagTypeDef],
         "MonitorConfig": MonitorConfigTypeDef,
         "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
     },
     total=False,
 )
 
-
 class CreateAutoPredictorRequestRequestTypeDef(
     _RequiredCreateAutoPredictorRequestRequestTypeDef,
     _OptionalCreateAutoPredictorRequestRequestTypeDef,
 ):
     pass
 
-
 BaselineTypeDef = TypedDict(
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
@@ -1876,22 +1839,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
-
 class CreateExplainabilityExportRequestRequestTypeDef(
     _RequiredCreateExplainabilityExportRequestRequestTypeDef,
     _OptionalCreateExplainabilityExportRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastExportJobRequestRequestTypeDef",
     {
         "ForecastExportJobName": str,
         "ForecastArn": str,
         "Destination": DataDestinationTypeDef,
     },
@@ -1901,22 +1862,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
-
 class CreateForecastExportJobRequestRequestTypeDef(
     _RequiredCreateForecastExportJobRequestRequestTypeDef,
     _OptionalCreateForecastExportJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
     {
         "PredictorBacktestExportJobName": str,
         "PredictorArn": str,
         "Destination": DataDestinationTypeDef,
     },
@@ -1926,22 +1885,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
-
 class CreatePredictorBacktestExportJobRequestRequestTypeDef(
     _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
     _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
     {
         "WhatIfForecastExportName": str,
         "WhatIfForecastArns": Sequence[str],
         "Destination": DataDestinationTypeDef,
     },
@@ -1951,22 +1908,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
-
 class CreateWhatIfForecastExportRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeExplainabilityExportResponseTypeDef = TypedDict(
     "DescribeExplainabilityExportResponseTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
         "ExplainabilityArn": str,
         "Destination": DataDestinationTypeDef,
@@ -2103,22 +2058,20 @@
         "Tags": Sequence[TagTypeDef],
         "Format": str,
         "ImportMode": ImportModeType,
     },
     total=False,
 )
 
-
 class CreateDatasetImportJobRequestRequestTypeDef(
     _RequiredCreateDatasetImportJobRequestRequestTypeDef,
     _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
-
 DatasetImportJobSummaryTypeDef = TypedDict(
     "DatasetImportJobSummaryTypeDef",
     {
         "DatasetImportJobArn": str,
         "DatasetImportJobName": str,
         "DataSource": DataSourceTypeDef,
         "Status": str,
@@ -2174,21 +2127,19 @@
     {
         "ForecastDimensions": List[str],
         "Featurizations": List[FeaturizationOutputTypeDef],
     },
     total=False,
 )
 
-
 class FeaturizationConfigOutputTypeDef(
     _RequiredFeaturizationConfigOutputTypeDef, _OptionalFeaturizationConfigOutputTypeDef
 ):
     pass
 
-
 _RequiredFeaturizationConfigTypeDef = TypedDict(
     "_RequiredFeaturizationConfigTypeDef",
     {
         "ForecastFrequency": str,
     },
 )
 _OptionalFeaturizationConfigTypeDef = TypedDict(
@@ -2196,21 +2147,19 @@
     {
         "ForecastDimensions": Sequence[str],
         "Featurizations": Sequence[FeaturizationTypeDef],
     },
     total=False,
 )
 
-
 class FeaturizationConfigTypeDef(
     _RequiredFeaturizationConfigTypeDef, _OptionalFeaturizationConfigTypeDef
 ):
     pass
 
-
 HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
     "HyperParameterTuningJobConfigOutputTypeDef",
     {
         "ParameterRanges": ParameterRangesOutputTypeDef,
     },
     total=False,
 )
@@ -2312,22 +2261,20 @@
     {
         "Format": str,
         "TimestampFormat": str,
     },
     total=False,
 )
 
-
 class TimeSeriesReplacementsDataSourceOutputTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceOutputTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceOutputTypeDef,
 ):
     pass
 
-
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "DatasetName": str,
         "Domain": DomainType,
         "DatasetType": DatasetTypeType,
         "Schema": SchemaTypeDef,
@@ -2339,21 +2286,19 @@
         "DataFrequency": str,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateExplainabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExplainabilityRequestRequestTypeDef",
     {
         "ExplainabilityName": str,
         "ResourceArn": str,
         "ExplainabilityConfig": ExplainabilityConfigTypeDef,
     },
@@ -2367,22 +2312,20 @@
         "StartDateTime": str,
         "EndDateTime": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateExplainabilityRequestRequestTypeDef(
     _RequiredCreateExplainabilityRequestRequestTypeDef,
     _OptionalCreateExplainabilityRequestRequestTypeDef,
 ):
     pass
 
-
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Schema": SchemaTypeDef,
         "Format": str,
     },
@@ -2401,22 +2344,20 @@
     {
         "Format": str,
         "TimestampFormat": str,
     },
     total=False,
 )
 
-
 class TimeSeriesReplacementsDataSourceTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceTypeDef,
 ):
     pass
 
-
 DescribeMonitorResponseTypeDef = TypedDict(
     "DescribeMonitorResponseTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "ResourceArn": str,
         "Status": str,
@@ -2499,21 +2440,19 @@
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "OptimizationMetric": OptimizationMetricType,
     },
     total=False,
 )
 
-
 class CreatePredictorRequestRequestTypeDef(
     _RequiredCreatePredictorRequestRequestTypeDef, _OptionalCreatePredictorRequestRequestTypeDef
 ):
     pass
 
-
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "AlgorithmArn": str,
         "TestWindows": List[WindowSummaryTypeDef],
     },
     total=False,
@@ -2590,29 +2529,29 @@
         "WhatIfForecastName": str,
         "WhatIfAnalysisArn": str,
     },
 )
 _OptionalCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWhatIfForecastRequestRequestTypeDef",
     {
-        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationTypeDef],
+        "TimeSeriesTransformations": Sequence[
+            Union[TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef]
+        ],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateWhatIfForecastRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastRequestRequestTypeDef,
 ):
     pass
 
-
 GetAccuracyMetricsResponseTypeDef = TypedDict(
     "GetAccuracyMetricsResponseTypeDef",
     {
         "PredictorEvaluationResults": List[EvaluationResultTypeDef],
         "IsAutoPredictor": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "OptimizationMetric": OptimizationMetricType,
@@ -2667,21 +2606,19 @@
         "ForecastTypes": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
     },
     total=False,
 )
 
-
 class CreateForecastRequestRequestTypeDef(
     _RequiredCreateForecastRequestRequestTypeDef, _OptionalCreateForecastRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateWhatIfAnalysisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfAnalysisRequestRequestTypeDef",
     {
         "WhatIfAnalysisName": str,
         "ForecastArn": str,
     },
 )
@@ -2690,13 +2627,12 @@
     {
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateWhatIfAnalysisRequestRequestTypeDef(
     _RequiredCreateWhatIfAnalysisRequestRequestTypeDef,
     _OptionalCreateWhatIfAnalysisRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/type_defs.pyi` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_forecast.type_defs import ActionTypeDef
 
     data: ActionTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AttributeTypeType,
     AutoMLOverrideStrategyType,
     ConditionType,
     DatasetTypeType,
     DayOfWeekType,
@@ -39,14 +39,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActionTypeDef",
     "AdditionalDatasetOutputTypeDef",
     "AdditionalDatasetTypeDef",
     "AttributeConfigOutputTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
@@ -267,38 +268,42 @@
     "_OptionalAdditionalDatasetOutputTypeDef",
     {
         "Configuration": Dict[str, List[str]],
     },
     total=False,
 )
 
+
 class AdditionalDatasetOutputTypeDef(
     _RequiredAdditionalDatasetOutputTypeDef, _OptionalAdditionalDatasetOutputTypeDef
 ):
     pass
 
+
 _RequiredAdditionalDatasetTypeDef = TypedDict(
     "_RequiredAdditionalDatasetTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalAdditionalDatasetTypeDef = TypedDict(
     "_OptionalAdditionalDatasetTypeDef",
     {
         "Configuration": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class AdditionalDatasetTypeDef(
     _RequiredAdditionalDatasetTypeDef, _OptionalAdditionalDatasetTypeDef
 ):
     pass
 
+
 AttributeConfigOutputTypeDef = TypedDict(
     "AttributeConfigOutputTypeDef",
     {
         "AttributeName": str,
         "Transformations": Dict[str, str],
     },
 )
@@ -348,19 +353,21 @@
     "_OptionalContinuousParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
+
 class ContinuousParameterRangeTypeDef(
     _RequiredContinuousParameterRangeTypeDef, _OptionalContinuousParameterRangeTypeDef
 ):
     pass
 
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "RoleArn": str,
         "KMSKeyArn": str,
     },
 )
@@ -430,17 +437,19 @@
     "_OptionalS3ConfigTypeDef",
     {
         "KMSKeyArn": str,
     },
     total=False,
 )
 
+
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
+
 DatasetGroupSummaryTypeDef = TypedDict(
     "DatasetGroupSummaryTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetGroupName": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
@@ -725,38 +734,42 @@
     "_OptionalFeaturizationMethodOutputTypeDef",
     {
         "FeaturizationMethodParameters": Dict[str, str],
     },
     total=False,
 )
 
+
 class FeaturizationMethodOutputTypeDef(
     _RequiredFeaturizationMethodOutputTypeDef, _OptionalFeaturizationMethodOutputTypeDef
 ):
     pass
 
+
 _RequiredFeaturizationMethodTypeDef = TypedDict(
     "_RequiredFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodName": Literal["filling"],
     },
 )
 _OptionalFeaturizationMethodTypeDef = TypedDict(
     "_OptionalFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodParameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class FeaturizationMethodTypeDef(
     _RequiredFeaturizationMethodTypeDef, _OptionalFeaturizationMethodTypeDef
 ):
     pass
 
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Key": str,
         "Value": str,
         "Condition": FilterConditionStringType,
     },
@@ -805,19 +818,21 @@
     "_OptionalIntegerParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
+
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -997,17 +1012,19 @@
     {
         "AttributeConfigs": List[AttributeConfigOutputTypeDef],
         "AdditionalDatasets": List[AdditionalDatasetOutputTypeDef],
     },
     total=False,
 )
 
+
 class DataConfigOutputTypeDef(_RequiredDataConfigOutputTypeDef, _OptionalDataConfigOutputTypeDef):
     pass
 
+
 _RequiredDataConfigTypeDef = TypedDict(
     "_RequiredDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalDataConfigTypeDef = TypedDict(
@@ -1015,17 +1032,19 @@
     {
         "AttributeConfigs": Sequence[AttributeConfigTypeDef],
         "AdditionalDatasets": Sequence[AdditionalDatasetTypeDef],
     },
     total=False,
 )
 
+
 class DataConfigTypeDef(_RequiredDataConfigTypeDef, _OptionalDataConfigTypeDef):
     pass
 
+
 PredictorBaselineTypeDef = TypedDict(
     "PredictorBaselineTypeDef",
     {
         "BaselineMetrics": List[BaselineMetricTypeDef],
     },
     total=False,
 )
@@ -1042,20 +1061,22 @@
     {
         "DatasetArns": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetGroupRequestRequestTypeDef(
     _RequiredCreateDatasetGroupRequestRequestTypeDef,
     _OptionalCreateDatasetGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMonitorRequestRequestTypeDef",
     {
         "MonitorName": str,
         "ResourceArn": str,
     },
 )
@@ -1063,19 +1084,21 @@
     "_OptionalCreateMonitorRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMonitorRequestRequestTypeDef(
     _RequiredCreateMonitorRequestRequestTypeDef, _OptionalCreateMonitorRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1294,36 +1317,40 @@
     "_OptionalFeaturizationOutputTypeDef",
     {
         "FeaturizationPipeline": List[FeaturizationMethodOutputTypeDef],
     },
     total=False,
 )
 
+
 class FeaturizationOutputTypeDef(
     _RequiredFeaturizationOutputTypeDef, _OptionalFeaturizationOutputTypeDef
 ):
     pass
 
+
 _RequiredFeaturizationTypeDef = TypedDict(
     "_RequiredFeaturizationTypeDef",
     {
         "AttributeName": str,
     },
 )
 _OptionalFeaturizationTypeDef = TypedDict(
     "_OptionalFeaturizationTypeDef",
     {
         "FeaturizationPipeline": Sequence[FeaturizationMethodTypeDef],
     },
     total=False,
 )
 
+
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
+
 ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetImportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
@@ -1382,20 +1409,22 @@
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class ListMonitorEvaluationsRequestRequestTypeDef(
     _RequiredListMonitorEvaluationsRequestRequestTypeDef,
     _OptionalListMonitorEvaluationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListMonitorsRequestRequestTypeDef = TypedDict(
     "ListMonitorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
@@ -1471,36 +1500,40 @@
     "_OptionalInputDataConfigOutputTypeDef",
     {
         "SupplementaryFeatures": List[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
+
 class InputDataConfigOutputTypeDef(
     _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
 ):
     pass
 
+
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalInputDataConfigTypeDef = TypedDict(
     "_OptionalInputDataConfigTypeDef",
     {
         "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
+
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
+
 ParameterRangesOutputTypeDef = TypedDict(
     "ParameterRangesOutputTypeDef",
     {
         "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
         "ContinuousParameterRanges": List[ContinuousParameterRangeTypeDef],
         "IntegerParameterRanges": List[IntegerParameterRangeTypeDef],
     },
@@ -1589,20 +1622,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
     _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
 ):
     pass
 
+
 ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
     "ListMonitorsRequestListMonitorsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1799,20 +1834,22 @@
         "Tags": Sequence[TagTypeDef],
         "MonitorConfig": MonitorConfigTypeDef,
         "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
     },
     total=False,
 )
 
+
 class CreateAutoPredictorRequestRequestTypeDef(
     _RequiredCreateAutoPredictorRequestRequestTypeDef,
     _OptionalCreateAutoPredictorRequestRequestTypeDef,
 ):
     pass
 
+
 BaselineTypeDef = TypedDict(
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
@@ -1839,20 +1876,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
+
 class CreateExplainabilityExportRequestRequestTypeDef(
     _RequiredCreateExplainabilityExportRequestRequestTypeDef,
     _OptionalCreateExplainabilityExportRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastExportJobRequestRequestTypeDef",
     {
         "ForecastExportJobName": str,
         "ForecastArn": str,
         "Destination": DataDestinationTypeDef,
     },
@@ -1862,20 +1901,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
+
 class CreateForecastExportJobRequestRequestTypeDef(
     _RequiredCreateForecastExportJobRequestRequestTypeDef,
     _OptionalCreateForecastExportJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
     {
         "PredictorBacktestExportJobName": str,
         "PredictorArn": str,
         "Destination": DataDestinationTypeDef,
     },
@@ -1885,20 +1926,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
+
 class CreatePredictorBacktestExportJobRequestRequestTypeDef(
     _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
     _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
     {
         "WhatIfForecastExportName": str,
         "WhatIfForecastArns": Sequence[str],
         "Destination": DataDestinationTypeDef,
     },
@@ -1908,20 +1951,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
+
 class CreateWhatIfForecastExportRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeExplainabilityExportResponseTypeDef = TypedDict(
     "DescribeExplainabilityExportResponseTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
         "ExplainabilityArn": str,
         "Destination": DataDestinationTypeDef,
@@ -2058,20 +2103,22 @@
         "Tags": Sequence[TagTypeDef],
         "Format": str,
         "ImportMode": ImportModeType,
     },
     total=False,
 )
 
+
 class CreateDatasetImportJobRequestRequestTypeDef(
     _RequiredCreateDatasetImportJobRequestRequestTypeDef,
     _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
+
 DatasetImportJobSummaryTypeDef = TypedDict(
     "DatasetImportJobSummaryTypeDef",
     {
         "DatasetImportJobArn": str,
         "DatasetImportJobName": str,
         "DataSource": DataSourceTypeDef,
         "Status": str,
@@ -2127,19 +2174,21 @@
     {
         "ForecastDimensions": List[str],
         "Featurizations": List[FeaturizationOutputTypeDef],
     },
     total=False,
 )
 
+
 class FeaturizationConfigOutputTypeDef(
     _RequiredFeaturizationConfigOutputTypeDef, _OptionalFeaturizationConfigOutputTypeDef
 ):
     pass
 
+
 _RequiredFeaturizationConfigTypeDef = TypedDict(
     "_RequiredFeaturizationConfigTypeDef",
     {
         "ForecastFrequency": str,
     },
 )
 _OptionalFeaturizationConfigTypeDef = TypedDict(
@@ -2147,19 +2196,21 @@
     {
         "ForecastDimensions": Sequence[str],
         "Featurizations": Sequence[FeaturizationTypeDef],
     },
     total=False,
 )
 
+
 class FeaturizationConfigTypeDef(
     _RequiredFeaturizationConfigTypeDef, _OptionalFeaturizationConfigTypeDef
 ):
     pass
 
+
 HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
     "HyperParameterTuningJobConfigOutputTypeDef",
     {
         "ParameterRanges": ParameterRangesOutputTypeDef,
     },
     total=False,
 )
@@ -2261,20 +2312,22 @@
     {
         "Format": str,
         "TimestampFormat": str,
     },
     total=False,
 )
 
+
 class TimeSeriesReplacementsDataSourceOutputTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceOutputTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceOutputTypeDef,
 ):
     pass
 
+
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "DatasetName": str,
         "Domain": DomainType,
         "DatasetType": DatasetTypeType,
         "Schema": SchemaTypeDef,
@@ -2286,19 +2339,21 @@
         "DataFrequency": str,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateExplainabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExplainabilityRequestRequestTypeDef",
     {
         "ExplainabilityName": str,
         "ResourceArn": str,
         "ExplainabilityConfig": ExplainabilityConfigTypeDef,
     },
@@ -2312,20 +2367,22 @@
         "StartDateTime": str,
         "EndDateTime": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateExplainabilityRequestRequestTypeDef(
     _RequiredCreateExplainabilityRequestRequestTypeDef,
     _OptionalCreateExplainabilityRequestRequestTypeDef,
 ):
     pass
 
+
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Schema": SchemaTypeDef,
         "Format": str,
     },
@@ -2344,20 +2401,22 @@
     {
         "Format": str,
         "TimestampFormat": str,
     },
     total=False,
 )
 
+
 class TimeSeriesReplacementsDataSourceTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceTypeDef,
 ):
     pass
 
+
 DescribeMonitorResponseTypeDef = TypedDict(
     "DescribeMonitorResponseTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "ResourceArn": str,
         "Status": str,
@@ -2440,19 +2499,21 @@
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "OptimizationMetric": OptimizationMetricType,
     },
     total=False,
 )
 
+
 class CreatePredictorRequestRequestTypeDef(
     _RequiredCreatePredictorRequestRequestTypeDef, _OptionalCreatePredictorRequestRequestTypeDef
 ):
     pass
 
+
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "AlgorithmArn": str,
         "TestWindows": List[WindowSummaryTypeDef],
     },
     total=False,
@@ -2529,27 +2590,31 @@
         "WhatIfForecastName": str,
         "WhatIfAnalysisArn": str,
     },
 )
 _OptionalCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWhatIfForecastRequestRequestTypeDef",
     {
-        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationTypeDef],
+        "TimeSeriesTransformations": Sequence[
+            Union[TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef]
+        ],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateWhatIfForecastRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastRequestRequestTypeDef,
 ):
     pass
 
+
 GetAccuracyMetricsResponseTypeDef = TypedDict(
     "GetAccuracyMetricsResponseTypeDef",
     {
         "PredictorEvaluationResults": List[EvaluationResultTypeDef],
         "IsAutoPredictor": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "OptimizationMetric": OptimizationMetricType,
@@ -2604,19 +2669,21 @@
         "ForecastTypes": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
     },
     total=False,
 )
 
+
 class CreateForecastRequestRequestTypeDef(
     _RequiredCreateForecastRequestRequestTypeDef, _OptionalCreateForecastRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateWhatIfAnalysisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfAnalysisRequestRequestTypeDef",
     {
         "WhatIfAnalysisName": str,
         "ForecastArn": str,
     },
 )
@@ -2625,12 +2692,13 @@
     {
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateWhatIfAnalysisRequestRequestTypeDef(
     _RequiredCreateWhatIfAnalysisRequestRequestTypeDef,
     _OptionalCreateWhatIfAnalysisRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/PKG-INFO` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-forecast
-Version: 1.28.15
-Summary: Type annotations for boto3.ForecastService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ForecastService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/SOURCES.txt` & `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15/setup.py` & `mypy-boto3-forecast-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-forecast",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_forecast"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ForecastService 1.28.15 service generated with"
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

