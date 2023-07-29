# Comparing `tmp/mypy-boto3-frauddetector-1.28.15.tar.gz` & `tmp/mypy-boto3-frauddetector-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-frauddetector-1.28.15.tar", last modified: Fri Jul 28 20:42:50 2023, max compression
+gzip compressed data, was "mypy-boto3-frauddetector-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:10 2023, max compression
```

## Comparing `mypy-boto3-frauddetector-1.28.15.tar` & `mypy-boto3-frauddetector-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.209129 mypy-boto3-frauddetector-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-07-28 20:42:50.209129 mypy-boto3-frauddetector-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.197129 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46336 2023-07-28 20:26:08.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46256 2023-07-28 20:26:08.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-28 20:26:08.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-28 20:26:08.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60744 2023-07-28 20:26:11.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60673 2023-07-28 20:26:09.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.209129 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-07-28 20:42:49.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-28 20:42:50.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:49.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:50.209129 mypy-boto3-frauddetector-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:10.113157 mypy-boto3-frauddetector-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-07-29 10:03:10.113157 mypy-boto3-frauddetector-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:10.105157 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46531 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46451 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-29 09:45:41.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60744 2023-07-29 09:45:43.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60673 2023-07-29 09:45:42.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:10.113157 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:09.000000 mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:10.113157 mypy-boto3-frauddetector-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-29 09:45:39.000000 mypy-boto3-frauddetector-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-frauddetector-1.28.15/LICENSE` & `mypy-boto3-frauddetector-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.15/PKG-INFO` & `mypy-boto3-frauddetector-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.28.15
-Summary: Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-frauddetector-1.28.15/README.md` & `mypy-boto3-frauddetector-1.28.15.post1/README.md`

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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/__main__.py` & `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FraudDetector 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.FraudDetector 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector\nOther"
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

### Comparing `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/client.py` & `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_frauddetector.client import FraudDetectorClient
 
     session = Session()
     client: FraudDetectorClient = session.client("frauddetector")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
@@ -64,19 +64,21 @@
     GetRulesResultTypeDef,
     GetVariablesResultTypeDef,
     IngestedEventsDetailTypeDef,
     ListEventPredictionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     ModelEndpointDataBlobTypeDef,
     ModelInputConfigurationTypeDef,
+    ModelOutputConfigurationOutputTypeDef,
     ModelOutputConfigurationTypeDef,
     ModelVersionTypeDef,
     PredictionTimeRangeTypeDef,
     RuleTypeDef,
     TagTypeDef,
+    TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     UpdateModelVersionResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     VariableEntryTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -262,15 +264,15 @@
 
     def create_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         trainingDataSource: TrainingDataSourceEnumType,
-        trainingDataSchema: TrainingDataSchemaTypeDef,
+        trainingDataSchema: Union[TrainingDataSchemaTypeDef, TrainingDataSchemaOutputTypeDef],
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
         ingestedEventsDetail: IngestedEventsDetailTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelVersionResultTypeDef:
         """
         Creates a version of the model using the specified model type and model id.
 
@@ -792,15 +794,17 @@
     def put_external_model(
         self,
         *,
         modelEndpoint: str,
         modelSource: Literal["SAGEMAKER"],
         invokeModelEndpointRoleArn: str,
         inputConfiguration: ModelInputConfigurationTypeDef,
-        outputConfiguration: ModelOutputConfigurationTypeDef,
+        outputConfiguration: Union[
+            ModelOutputConfigurationTypeDef, ModelOutputConfigurationOutputTypeDef
+        ],
         modelEndpointStatus: ModelEndpointStatusType,
         tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon SageMaker model endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_external_model)
```

### Comparing `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/client.pyi` & `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_frauddetector.client import FraudDetectorClient
 
     session = Session()
     client: FraudDetectorClient = session.client("frauddetector")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
@@ -64,19 +64,21 @@
     GetRulesResultTypeDef,
     GetVariablesResultTypeDef,
     IngestedEventsDetailTypeDef,
     ListEventPredictionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     ModelEndpointDataBlobTypeDef,
     ModelInputConfigurationTypeDef,
+    ModelOutputConfigurationOutputTypeDef,
     ModelOutputConfigurationTypeDef,
     ModelVersionTypeDef,
     PredictionTimeRangeTypeDef,
     RuleTypeDef,
     TagTypeDef,
+    TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     UpdateModelVersionResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     VariableEntryTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -246,15 +248,15 @@
         """
     def create_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         trainingDataSource: TrainingDataSourceEnumType,
-        trainingDataSchema: TrainingDataSchemaTypeDef,
+        trainingDataSchema: Union[TrainingDataSchemaTypeDef, TrainingDataSchemaOutputTypeDef],
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
         ingestedEventsDetail: IngestedEventsDetailTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelVersionResultTypeDef:
         """
         Creates a version of the model using the specified model type and model id.
 
@@ -729,15 +731,17 @@
     def put_external_model(
         self,
         *,
         modelEndpoint: str,
         modelSource: Literal["SAGEMAKER"],
         invokeModelEndpointRoleArn: str,
         inputConfiguration: ModelInputConfigurationTypeDef,
-        outputConfiguration: ModelOutputConfigurationTypeDef,
+        outputConfiguration: Union[
+            ModelOutputConfigurationTypeDef, ModelOutputConfigurationOutputTypeDef
+        ],
         modelEndpointStatus: ModelEndpointStatusType,
         tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon SageMaker model endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_external_model)
```

### Comparing `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/literals.py` & `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/literals.pyi` & `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/type_defs.py` & `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/type_defs.pyi` & `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/PKG-INFO` & `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.28.15
-Summary: Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/SOURCES.txt` & `mypy-boto3-frauddetector-1.28.15.post1/mypy_boto3_frauddetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.15/setup.py` & `mypy-boto3-frauddetector-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-frauddetector",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_frauddetector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

