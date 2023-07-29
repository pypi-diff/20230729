# Comparing `tmp/mypy-boto3-iotevents-1.28.15.tar.gz` & `tmp/mypy-boto3-iotevents-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotevents-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
+gzip compressed data, was "mypy-boto3-iotevents-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:21 2023, max compression
```

## Comparing `mypy-boto3-iotevents-1.28.15.tar` & `mypy-boto3-iotevents-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.461257 mypy-boto3-iotevents-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16424 2023-07-28 20:42:59.453257 mypy-boto3-iotevents-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.445257 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-28 20:28:23.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-28 20:28:23.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42731 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42652 2023-07-28 20:28:23.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.453257 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16424 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.461257 mypy-boto3-iotevents-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.209187 mypy-boto3-iotevents-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-29 10:03:21.209187 mypy-boto3-iotevents-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.201187 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19455 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42731 2023-07-29 09:47:55.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42652 2023-07-29 09:47:55.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.209187 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:20.000000 mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:21.209187 mypy-boto3-iotevents-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:47:54.000000 mypy-boto3-iotevents-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-iotevents-1.28.15/LICENSE` & `mypy-boto3-iotevents-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.15/PKG-INFO` & `mypy-boto3-iotevents-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotevents-1.28.15/README.md` & `mypy-boto3-iotevents-1.28.15.post1/README.md`

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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/__main__.py` & `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTEvents 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.IoTEvents 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents\nOther"
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

### Comparing `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/client.py` & `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,44 +9,49 @@
     from boto3.session import Session
     from mypy_boto3_iotevents.client import IoTEventsClient
 
     session = Session()
     client: IoTEventsClient = session.client("iotevents")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EvaluationMethodType
 from .type_defs import (
     AlarmCapabilitiesTypeDef,
+    AlarmEventActionsOutputTypeDef,
     AlarmEventActionsTypeDef,
+    AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
     AlarmRuleTypeDef,
     CreateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     DescribeAlarmModelResponseTypeDef,
     DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelResponseTypeDef,
     DescribeInputResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    DetectorModelDefinitionOutputTypeDef,
     DetectorModelDefinitionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
+    InputDefinitionOutputTypeDef,
     InputDefinitionTypeDef,
     InputIdentifierTypeDef,
     ListAlarmModelsResponseTypeDef,
     ListAlarmModelVersionsResponseTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     ListInputRoutingsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    LoggingOptionsOutputTypeDef,
     LoggingOptionsTypeDef,
     StartDetectorModelAnalysisResponseTypeDef,
     TagTypeDef,
     UpdateAlarmModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     UpdateInputResponseTypeDef,
 )
@@ -114,30 +119,32 @@
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         key: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationTypeDef = ...,
-        alarmEventActions: AlarmEventActionsTypeDef = ...,
+        alarmNotification: Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef] = ...,
+        alarmEventActions: Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef] = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> CreateAlarmModelResponseTypeDef:
         """
         Creates an alarm model to monitor an AWS IoT Events input attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_alarm_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#create_alarm_model)
         """
 
     def create_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionTypeDef,
+        detectorModelDefinition: Union[
+            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
+        ],
         roleArn: str,
         detectorModelDescription: str = ...,
         key: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> CreateDetectorModelResponseTypeDef:
         """
@@ -147,15 +154,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#create_detector_model)
         """
 
     def create_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionTypeDef,
+        inputDefinition: Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef],
         inputDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateInputResponseTypeDef:
         """
         Creates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_input)
@@ -325,25 +332,29 @@
         Lists the tags (metadata) you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#list_tags_for_resource)
         """
 
     def put_logging_options(
-        self, *, loggingOptions: LoggingOptionsTypeDef
+        self, *, loggingOptions: Union[LoggingOptionsTypeDef, LoggingOptionsOutputTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets or updates the AWS IoT Events logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.put_logging_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#put_logging_options)
         """
 
     def start_detector_model_analysis(
-        self, *, detectorModelDefinition: DetectorModelDefinitionTypeDef
+        self,
+        *,
+        detectorModelDefinition: Union[
+            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
+        ]
     ) -> StartDetectorModelAnalysisResponseTypeDef:
         """
         Performs an analysis of your detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.start_detector_model_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#start_detector_model_analysis)
         """
@@ -368,30 +379,32 @@
         self,
         *,
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationTypeDef = ...,
-        alarmEventActions: AlarmEventActionsTypeDef = ...,
+        alarmNotification: Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef] = ...,
+        alarmEventActions: Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef] = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> UpdateAlarmModelResponseTypeDef:
         """
         Updates an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_alarm_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_alarm_model)
         """
 
     def update_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionTypeDef,
+        detectorModelDefinition: Union[
+            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
+        ],
         roleArn: str,
         detectorModelDescription: str = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> UpdateDetectorModelResponseTypeDef:
         """
         Updates a detector model.
 
@@ -399,15 +412,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_detector_model)
         """
 
     def update_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionTypeDef,
+        inputDefinition: Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef],
         inputDescription: str = ...
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_input)
```

### Comparing `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/client.pyi` & `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,44 +9,49 @@
     from boto3.session import Session
     from mypy_boto3_iotevents.client import IoTEventsClient
 
     session = Session()
     client: IoTEventsClient = session.client("iotevents")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EvaluationMethodType
 from .type_defs import (
     AlarmCapabilitiesTypeDef,
+    AlarmEventActionsOutputTypeDef,
     AlarmEventActionsTypeDef,
+    AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
     AlarmRuleTypeDef,
     CreateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     DescribeAlarmModelResponseTypeDef,
     DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelResponseTypeDef,
     DescribeInputResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    DetectorModelDefinitionOutputTypeDef,
     DetectorModelDefinitionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
+    InputDefinitionOutputTypeDef,
     InputDefinitionTypeDef,
     InputIdentifierTypeDef,
     ListAlarmModelsResponseTypeDef,
     ListAlarmModelVersionsResponseTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     ListInputRoutingsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    LoggingOptionsOutputTypeDef,
     LoggingOptionsTypeDef,
     StartDetectorModelAnalysisResponseTypeDef,
     TagTypeDef,
     UpdateAlarmModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     UpdateInputResponseTypeDef,
 )
@@ -108,29 +113,31 @@
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         key: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationTypeDef = ...,
-        alarmEventActions: AlarmEventActionsTypeDef = ...,
+        alarmNotification: Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef] = ...,
+        alarmEventActions: Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef] = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> CreateAlarmModelResponseTypeDef:
         """
         Creates an alarm model to monitor an AWS IoT Events input attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_alarm_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#create_alarm_model)
         """
     def create_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionTypeDef,
+        detectorModelDefinition: Union[
+            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
+        ],
         roleArn: str,
         detectorModelDescription: str = ...,
         key: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> CreateDetectorModelResponseTypeDef:
         """
@@ -139,15 +146,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_detector_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#create_detector_model)
         """
     def create_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionTypeDef,
+        inputDefinition: Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef],
         inputDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateInputResponseTypeDef:
         """
         Creates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_input)
@@ -299,24 +306,28 @@
         """
         Lists the tags (metadata) you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#list_tags_for_resource)
         """
     def put_logging_options(
-        self, *, loggingOptions: LoggingOptionsTypeDef
+        self, *, loggingOptions: Union[LoggingOptionsTypeDef, LoggingOptionsOutputTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets or updates the AWS IoT Events logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.put_logging_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#put_logging_options)
         """
     def start_detector_model_analysis(
-        self, *, detectorModelDefinition: DetectorModelDefinitionTypeDef
+        self,
+        *,
+        detectorModelDefinition: Union[
+            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
+        ]
     ) -> StartDetectorModelAnalysisResponseTypeDef:
         """
         Performs an analysis of your detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.start_detector_model_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#start_detector_model_analysis)
         """
@@ -338,44 +349,46 @@
         self,
         *,
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationTypeDef = ...,
-        alarmEventActions: AlarmEventActionsTypeDef = ...,
+        alarmNotification: Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef] = ...,
+        alarmEventActions: Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef] = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> UpdateAlarmModelResponseTypeDef:
         """
         Updates an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_alarm_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_alarm_model)
         """
     def update_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionTypeDef,
+        detectorModelDefinition: Union[
+            DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
+        ],
         roleArn: str,
         detectorModelDescription: str = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> UpdateDetectorModelResponseTypeDef:
         """
         Updates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_detector_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_detector_model)
         """
     def update_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionTypeDef,
+        inputDefinition: Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef],
         inputDescription: str = ...
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/client/#update_input)
```

### Comparing `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/literals.py` & `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/literals.pyi` & `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/type_defs.py` & `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/type_defs.pyi` & `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/PKG-INFO` & `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/SOURCES.txt` & `mypy-boto3-iotevents-1.28.15.post1/mypy_boto3_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.15/setup.py` & `mypy-boto3-iotevents-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotevents",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder"
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

