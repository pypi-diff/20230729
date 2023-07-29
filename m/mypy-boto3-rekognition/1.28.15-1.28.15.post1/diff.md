# Comparing `tmp/mypy-boto3-rekognition-1.28.15.tar.gz` & `tmp/mypy-boto3-rekognition-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rekognition-1.28.15.tar", last modified: Fri Jul 28 20:43:33 2023, max compression
+gzip compressed data, was "mypy-boto3-rekognition-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:59 2023, max compression
```

## Comparing `mypy-boto3-rekognition-1.28.15.tar` & `mypy-boto3-rekognition-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.773728 mypy-boto3-rekognition-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26556 2023-07-28 20:43:33.769728 mypy-boto3-rekognition-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.761727 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57491 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57401 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98431 2023-07-28 20:36:51.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98310 2023-07-28 20:36:49.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-28 20:36:48.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.769728 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26556 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:33.000000 mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:33.773728 mypy-boto3-rekognition-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:36:47.000000 mypy-boto3-rekognition-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.141358 mypy-boto3-rekognition-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26562 2023-07-29 10:03:59.141358 mypy-boto3-rekognition-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.125358 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57868 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57778 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-29 09:56:53.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98551 2023-07-29 09:56:55.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98430 2023-07-29 09:56:54.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-29 09:56:52.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.141358 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26562 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:03:58.000000 mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:59.141358 mypy-boto3-rekognition-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:56:51.000000 mypy-boto3-rekognition-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-rekognition-1.28.15/LICENSE` & `mypy-boto3-rekognition-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15/PKG-INFO` & `mypy-boto3-rekognition-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.28.15
-Summary: Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-rekognition-1.28.15/README.md` & `mypy-boto3-rekognition-1.28.15.post1/README.md`

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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__init__.py` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__init__.pyi` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/__main__.py` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Rekognition 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Rekognition 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
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

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/client.py` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_rekognition.client import RekognitionClient
 
     session = Session()
     client: RekognitionClient = session.client("rekognition")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AttributeType,
     CelebrityRecognitionSortByType,
     ContentModerationAggregateByType,
@@ -100,14 +100,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
+    RegionOfInterestOutputTypeDef,
     RegionOfInterestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
@@ -125,16 +126,19 @@
     StreamProcessingStartSelectorTypeDef,
     StreamProcessingStopSelectorTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorInputTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     StreamProcessorOutputTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
+    StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
+    TestingDataOutputTypeDef,
     TestingDataTypeDef,
+    TrainingDataOutputTypeDef,
     TrainingDataTypeDef,
     VideoTypeDef,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -311,16 +315,16 @@
 
     def create_project_version(
         self,
         *,
         ProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
-        TrainingData: TrainingDataTypeDef = ...,
-        TestingData: TestingDataTypeDef = ...,
+        TrainingData: Union[TrainingDataTypeDef, TrainingDataOutputTypeDef] = ...,
+        TestingData: Union[TestingDataTypeDef, TestingDataOutputTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of a model and begins training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
@@ -329,20 +333,22 @@
 
     def create_stream_processor(
         self,
         *,
         Input: StreamProcessorInputTypeDef,
         Output: StreamProcessorOutputTypeDef,
         Name: str,
-        Settings: StreamProcessorSettingsTypeDef,
+        Settings: Union[StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef],
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
-        RegionsOfInterest: Sequence[RegionOfInterestTypeDef] = ...,
+        RegionsOfInterest: Sequence[
+            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
+        ] = ...,
         DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
@@ -1132,15 +1138,17 @@
         """
 
     def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
-        RegionsOfInterestForUpdate: Sequence[RegionOfInterestTypeDef] = ...,
+        RegionsOfInterestForUpdate: Sequence[
+            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
+        ] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
         ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
```

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/client.pyi` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_rekognition.client import RekognitionClient
 
     session = Session()
     client: RekognitionClient = session.client("rekognition")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AttributeType,
     CelebrityRecognitionSortByType,
     ContentModerationAggregateByType,
@@ -100,14 +100,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
+    RegionOfInterestOutputTypeDef,
     RegionOfInterestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
@@ -125,16 +126,19 @@
     StreamProcessingStartSelectorTypeDef,
     StreamProcessingStopSelectorTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorInputTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     StreamProcessorOutputTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
+    StreamProcessorSettingsOutputTypeDef,
     StreamProcessorSettingsTypeDef,
+    TestingDataOutputTypeDef,
     TestingDataTypeDef,
+    TrainingDataOutputTypeDef,
     TrainingDataTypeDef,
     VideoTypeDef,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -297,16 +301,16 @@
         """
     def create_project_version(
         self,
         *,
         ProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
-        TrainingData: TrainingDataTypeDef = ...,
-        TestingData: TestingDataTypeDef = ...,
+        TrainingData: Union[TrainingDataTypeDef, TrainingDataOutputTypeDef] = ...,
+        TestingData: Union[TestingDataTypeDef, TestingDataOutputTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of a model and begins training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
@@ -314,20 +318,22 @@
         """
     def create_stream_processor(
         self,
         *,
         Input: StreamProcessorInputTypeDef,
         Output: StreamProcessorOutputTypeDef,
         Name: str,
-        Settings: StreamProcessorSettingsTypeDef,
+        Settings: Union[StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef],
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
-        RegionsOfInterest: Sequence[RegionOfInterestTypeDef] = ...,
+        RegionsOfInterest: Sequence[
+            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
+        ] = ...,
         DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
@@ -1053,15 +1059,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#update_dataset_entries)
         """
     def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
-        RegionsOfInterestForUpdate: Sequence[RegionOfInterestTypeDef] = ...,
+        RegionsOfInterestForUpdate: Sequence[
+            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
+        ] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
         ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
```

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/literals.py` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/literals.pyi` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/paginator.py` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/paginator.pyi` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/type_defs.py` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3336,15 +3336,17 @@
         "Name": str,
     },
 )
 _OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
     {
         "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
+        "RegionsOfInterestForUpdate": Sequence[
+            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
+        ],
         "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
         "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
     },
     total=False,
 )
 
 
@@ -3424,15 +3426,17 @@
 )
 _OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
     "_OptionalCreateStreamProcessorRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
         "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
-        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+        "RegionsOfInterest": Sequence[
+            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
+        ],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
     },
     total=False,
 )
 
 
 class CreateStreamProcessorRequestRequestTypeDef(
```

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/type_defs.pyi` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -3233,15 +3233,17 @@
         "Name": str,
     },
 )
 _OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
     {
         "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
+        "RegionsOfInterestForUpdate": Sequence[
+            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
+        ],
         "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
         "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
     },
     total=False,
 )
 
 class UpdateStreamProcessorRequestRequestTypeDef(
@@ -3315,15 +3317,17 @@
 )
 _OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
     "_OptionalCreateStreamProcessorRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
         "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
-        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+        "RegionsOfInterest": Sequence[
+            Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
+        ],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
     },
     total=False,
 )
 
 class CreateStreamProcessorRequestRequestTypeDef(
     _RequiredCreateStreamProcessorRequestRequestTypeDef,
```

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/waiter.py` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition/waiter.pyi` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/PKG-INFO` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rekognition
-Version: 1.28.15
-Summary: Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/
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
 [mypy-boto3-rekognition docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-rekognition-1.28.15/mypy_boto3_rekognition.egg-info/SOURCES.txt` & `mypy-boto3-rekognition-1.28.15.post1/mypy_boto3_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.15/setup.py` & `mypy-boto3-rekognition-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rekognition",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Rekognition 1.28.15 service generated with mypy-boto3-builder"
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

