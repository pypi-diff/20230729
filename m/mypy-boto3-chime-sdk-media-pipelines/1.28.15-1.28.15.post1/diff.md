# Comparing `tmp/mypy-boto3-chime-sdk-media-pipelines-1.28.15.tar.gz` & `tmp/mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:38 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15.tar` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.408738 mypy-boto3-chime-sdk-media-pipelines-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-07-28 20:42:22.408738 mypy-boto3-chime-sdk-media-pipelines-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.388738 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-28 20:20:36.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48676 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48619 2023-07-28 20:20:36.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.408738 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.408738 mypy-boto3-chime-sdk-media-pipelines-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-28 20:20:35.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.237037 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-07-29 10:02:38.237037 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.237037 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18820 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-29 09:39:28.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49063 2023-07-29 09:39:30.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49006 2023-07-29 09:39:29.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.237037 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-07-29 10:02:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-29 10:02:38.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 10:02:37.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:38.237037 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-29 09:39:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/LICENSE` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.28.15
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/README.md` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/README.md`

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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/__main__.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
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

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/client.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,41 +10,47 @@
     from mypy_boto3_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient
 
     session = Session()
     client: ChimeSDKMediaPipelinesClient = session.client("chime-sdk-media-pipelines")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MediaPipelineStatusUpdateType
 from .type_defs import (
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     ConcatenationSinkTypeDef,
     ConcatenationSourceTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaPipelineResponseTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
+    RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     TagTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -114,15 +120,17 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,
+        ChimeSdkMeetingConfiguration: Union[
+            ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_capture_pipeline)
@@ -143,17 +151,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_concatenation_pipeline)
         """
 
     def create_media_insights_pipeline(
         self,
         *,
         MediaInsightsPipelineConfigurationArn: str,
-        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationTypeDef = ...,
+        KinesisVideoStreamSourceRuntimeConfiguration: Union[
+            KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+            KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
+        ] = ...,
         MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
-        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = ...,
+        KinesisVideoStreamRecordingSourceRuntimeConfiguration: Union[
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
+        ] = ...,
         S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineResponseTypeDef:
         """
         Creates a media insights pipeline.
 
@@ -162,31 +176,43 @@
         """
 
     def create_media_insights_pipeline_configuration(
         self,
         *,
         MediaInsightsPipelineConfigurationName: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,
+        Elements: Sequence[
+            Union[
+                MediaInsightsPipelineConfigurationElementTypeDef,
+                MediaInsightsPipelineConfigurationElementOutputTypeDef,
+            ]
+        ],
+        RealTimeAlertConfiguration: Union[
+            RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         A structure that contains the static configurations for a media insights
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_insights_pipeline_configuration)
         """
 
     def create_media_live_connector_pipeline(
         self,
         *,
-        Sources: Sequence[LiveConnectorSourceConfigurationTypeDef],
+        Sources: Sequence[
+            Union[
+                LiveConnectorSourceConfigurationTypeDef,
+                LiveConnectorSourceConfigurationOutputTypeDef,
+            ]
+        ],
         Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaLiveConnectorPipelineResponseTypeDef:
         """
         Creates a media live connector pipeline in an Amazon Chime SDK meeting.
 
@@ -319,16 +345,23 @@
         """
 
     def update_media_insights_pipeline_configuration(
         self,
         *,
         Identifier: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...
+        Elements: Sequence[
+            Union[
+                MediaInsightsPipelineConfigurationElementTypeDef,
+                MediaInsightsPipelineConfigurationElementOutputTypeDef,
+            ]
+        ],
+        RealTimeAlertConfiguration: Union[
+            RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
+        ] = ...
     ) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Updates the media insights pipeline's configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_configuration)
         """
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/client.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,41 +10,47 @@
     from mypy_boto3_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient
 
     session = Session()
     client: ChimeSDKMediaPipelinesClient = session.client("chime-sdk-media-pipelines")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MediaPipelineStatusUpdateType
 from .type_defs import (
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     ConcatenationSinkTypeDef,
     ConcatenationSourceTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaPipelineResponseTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
     KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
+    LiveConnectorSourceConfigurationOutputTypeDef,
     LiveConnectorSourceConfigurationTypeDef,
+    MediaInsightsPipelineConfigurationElementOutputTypeDef,
     MediaInsightsPipelineConfigurationElementTypeDef,
+    RealTimeAlertConfigurationOutputTypeDef,
     RealTimeAlertConfigurationTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     TagTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -107,15 +113,17 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,
+        ChimeSdkMeetingConfiguration: Union[
+            ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_capture_pipeline)
@@ -134,17 +142,23 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_concatenation_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_concatenation_pipeline)
         """
     def create_media_insights_pipeline(
         self,
         *,
         MediaInsightsPipelineConfigurationArn: str,
-        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationTypeDef = ...,
+        KinesisVideoStreamSourceRuntimeConfiguration: Union[
+            KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
+            KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
+        ] = ...,
         MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
-        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = ...,
+        KinesisVideoStreamRecordingSourceRuntimeConfiguration: Union[
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
+        ] = ...,
         S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineResponseTypeDef:
         """
         Creates a media insights pipeline.
 
@@ -152,30 +166,42 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_insights_pipeline)
         """
     def create_media_insights_pipeline_configuration(
         self,
         *,
         MediaInsightsPipelineConfigurationName: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,
+        Elements: Sequence[
+            Union[
+                MediaInsightsPipelineConfigurationElementTypeDef,
+                MediaInsightsPipelineConfigurationElementOutputTypeDef,
+            ]
+        ],
+        RealTimeAlertConfiguration: Union[
+            RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         A structure that contains the static configurations for a media insights
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#create_media_insights_pipeline_configuration)
         """
     def create_media_live_connector_pipeline(
         self,
         *,
-        Sources: Sequence[LiveConnectorSourceConfigurationTypeDef],
+        Sources: Sequence[
+            Union[
+                LiveConnectorSourceConfigurationTypeDef,
+                LiveConnectorSourceConfigurationOutputTypeDef,
+            ]
+        ],
         Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaLiveConnectorPipelineResponseTypeDef:
         """
         Creates a media live connector pipeline in an Amazon Chime SDK meeting.
 
@@ -294,16 +320,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#untag_resource)
         """
     def update_media_insights_pipeline_configuration(
         self,
         *,
         Identifier: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...
+        Elements: Sequence[
+            Union[
+                MediaInsightsPipelineConfigurationElementTypeDef,
+                MediaInsightsPipelineConfigurationElementOutputTypeDef,
+            ]
+        ],
+        RealTimeAlertConfiguration: Union[
+            RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
+        ] = ...
     ) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Updates the media insights pipeline's configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_configuration)
         """
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/literals.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/literals.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/type_defs.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveSpeakerOnlyConfigurationTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
@@ -193,21 +192,19 @@
     {
         "ContentRedactionOutput": ContentRedactionOutputType,
         "OutputEncryptionKMSKeyId": str,
     },
     total=False,
 )
 
-
 class PostCallAnalyticsSettingsTypeDef(
     _RequiredPostCallAnalyticsSettingsTypeDef, _OptionalPostCallAnalyticsSettingsTypeDef
 ):
     pass
 
-
 AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
     "AmazonTranscribeProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
@@ -294,63 +291,57 @@
     "_OptionalContentArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["ContentOnly"],
     },
     total=False,
 )
 
-
 class ContentArtifactsConfigurationTypeDef(
     _RequiredContentArtifactsConfigurationTypeDef, _OptionalContentArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredVideoArtifactsConfigurationTypeDef",
     {
         "State": ArtifactsStateType,
     },
 )
 _OptionalVideoArtifactsConfigurationTypeDef = TypedDict(
     "_OptionalVideoArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["VideoOnly"],
     },
     total=False,
 )
 
-
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
     "_OptionalChannelDefinitionTypeDef",
     {
         "ParticipantRole": ParticipantRoleType,
     },
     total=False,
 )
 
-
 class ChannelDefinitionTypeDef(
     _RequiredChannelDefinitionTypeDef, _OptionalChannelDefinitionTypeDef
 ):
     pass
 
-
 S3BucketSinkConfigurationTypeDef = TypedDict(
     "S3BucketSinkConfigurationTypeDef",
     {
         "Destination": str,
     },
 )
 
@@ -498,21 +489,19 @@
     "_OptionalKeywordMatchConfigurationOutputTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
-
 class KeywordMatchConfigurationOutputTypeDef(
     _RequiredKeywordMatchConfigurationOutputTypeDef, _OptionalKeywordMatchConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -520,21 +509,19 @@
     "_OptionalKeywordMatchConfigurationTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
-
 class KeywordMatchConfigurationTypeDef(
     _RequiredKeywordMatchConfigurationTypeDef, _OptionalKeywordMatchConfigurationTypeDef
 ):
     pass
 
-
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
@@ -628,21 +615,19 @@
     {
         "AudioChannels": AudioChannelsOptionType,
         "AudioSampleRate": str,
     },
     total=False,
 )
 
-
 class LiveConnectorRTMPConfigurationTypeDef(
     _RequiredLiveConnectorRTMPConfigurationTypeDef, _OptionalLiveConnectorRTMPConfigurationTypeDef
 ):
     pass
 
-
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
@@ -737,22 +722,20 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": List[str],
     },
     total=False,
 )
 
-
 class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -770,22 +753,20 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": Sequence[str],
     },
     total=False,
 )
 
-
 class AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
 ):
     pass
 
-
 ArtifactsConcatenationConfigurationTypeDef = TypedDict(
     "ArtifactsConcatenationConfigurationTypeDef",
     {
         "Audio": AudioConcatenationConfigurationTypeDef,
         "Video": VideoConcatenationConfigurationTypeDef,
         "Content": ContentConcatenationConfigurationTypeDef,
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
@@ -805,42 +786,38 @@
     "_OptionalStreamChannelDefinitionOutputTypeDef",
     {
         "ChannelDefinitions": List[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
-
 class StreamChannelDefinitionOutputTypeDef(
     _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
 ):
     pass
 
-
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
     "_OptionalStreamChannelDefinitionTypeDef",
     {
         "ChannelDefinitions": Sequence[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
-
 class StreamChannelDefinitionTypeDef(
     _RequiredStreamChannelDefinitionTypeDef, _OptionalStreamChannelDefinitionTypeDef
 ):
     pass
 
-
 ConcatenationSinkTypeDef = TypedDict(
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
@@ -899,21 +876,19 @@
         "VerticalLayoutConfiguration": VerticalLayoutConfigurationTypeDef,
         "VideoAttribute": VideoAttributeTypeDef,
         "CanvasOrientation": CanvasOrientationType,
     },
     total=False,
 )
 
-
 class GridViewConfigurationTypeDef(
     _RequiredGridViewConfigurationTypeDef, _OptionalGridViewConfigurationTypeDef
 ):
     pass
 
-
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -959,21 +934,19 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class RealTimeAlertRuleOutputTypeDef(
     _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
 ):
     pass
 
-
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -982,21 +955,19 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
-
 SourceConfigurationOutputTypeDef = TypedDict(
     "SourceConfigurationOutputTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
     },
     total=False,
 )
@@ -1028,22 +999,20 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class MediaInsightsPipelineConfigurationElementOutputTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
 ):
     pass
 
-
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -1059,22 +1028,20 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class MediaInsightsPipelineConfigurationElementTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementTypeDef,
 ):
     pass
 
-
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
@@ -1089,21 +1056,19 @@
     "_OptionalStreamConfigurationOutputTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
-
 class StreamConfigurationOutputTypeDef(
     _RequiredStreamConfigurationOutputTypeDef, _OptionalStreamConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
 )
@@ -1111,21 +1076,19 @@
     "_OptionalStreamConfigurationTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
-
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
-
 KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     {
         "Streams": List[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorOutputTypeDef,
     },
 )
@@ -1149,22 +1112,20 @@
     {
         "Layout": Literal["GridView"],
         "Resolution": ResolutionOptionType,
     },
     total=False,
 )
 
-
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
-
 RealTimeAlertConfigurationOutputTypeDef = TypedDict(
     "RealTimeAlertConfigurationOutputTypeDef",
     {
         "Disabled": bool,
         "Rules": List[RealTimeAlertRuleOutputTypeDef],
     },
     total=False,
@@ -1217,21 +1178,19 @@
     "_OptionalArtifactsConfigurationTypeDef",
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1240,22 +1199,20 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1264,22 +1221,20 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
-
 MediaInsightsPipelineConfigurationTypeDef = TypedDict(
     "MediaInsightsPipelineConfigurationTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "MediaInsightsPipelineConfigurationArn": str,
         "ResourceAccessRoleArn": str,
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
@@ -1292,59 +1247,65 @@
 )
 
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        "Elements": Sequence[
+            Union[
+                MediaInsightsPipelineConfigurationElementTypeDef,
+                MediaInsightsPipelineConfigurationElementOutputTypeDef,
+            ]
+        ],
     },
 )
 _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        "Elements": Sequence[
+            Union[
+                MediaInsightsPipelineConfigurationElementTypeDef,
+                MediaInsightsPipelineConfigurationElementOutputTypeDef,
+            ]
+        ],
     },
 )
 _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 ConcatenationSourceTypeDef = TypedDict(
     "ConcatenationSourceTypeDef",
     {
         "Type": Literal["MediaCapturePipeline"],
         "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
 )
@@ -1388,22 +1349,20 @@
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateMediaInsightsPipelineRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
 ):
     pass
 
-
 ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
@@ -1474,22 +1433,20 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaConcatenationPipelineRequestRequestTypeDef(
     _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef,
     _OptionalCreateMediaConcatenationPipelineRequestRequestTypeDef,
 ):
     pass
 
-
 MediaConcatenationPipelineTypeDef = TypedDict(
     "MediaConcatenationPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Sources": List[ConcatenationSourceTypeDef],
         "Sinks": List[ConcatenationSinkTypeDef],
@@ -1540,22 +1497,20 @@
         "ClientRequestToken": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
-
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
         "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
@@ -1565,35 +1520,38 @@
     },
     total=False,
 )
 
 _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
-        "Sources": Sequence[LiveConnectorSourceConfigurationTypeDef],
+        "Sources": Sequence[
+            Union[
+                LiveConnectorSourceConfigurationTypeDef,
+                LiveConnectorSourceConfigurationOutputTypeDef,
+            ]
+        ],
         "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
     },
 )
 _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
     _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
 ):
     pass
 
-
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveSpeakerOnlyConfigurationTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
@@ -192,19 +193,21 @@
     {
         "ContentRedactionOutput": ContentRedactionOutputType,
         "OutputEncryptionKMSKeyId": str,
     },
     total=False,
 )
 
+
 class PostCallAnalyticsSettingsTypeDef(
     _RequiredPostCallAnalyticsSettingsTypeDef, _OptionalPostCallAnalyticsSettingsTypeDef
 ):
     pass
 
+
 AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
     "AmazonTranscribeProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
@@ -291,57 +294,63 @@
     "_OptionalContentArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["ContentOnly"],
     },
     total=False,
 )
 
+
 class ContentArtifactsConfigurationTypeDef(
     _RequiredContentArtifactsConfigurationTypeDef, _OptionalContentArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredVideoArtifactsConfigurationTypeDef",
     {
         "State": ArtifactsStateType,
     },
 )
 _OptionalVideoArtifactsConfigurationTypeDef = TypedDict(
     "_OptionalVideoArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["VideoOnly"],
     },
     total=False,
 )
 
+
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
     "_OptionalChannelDefinitionTypeDef",
     {
         "ParticipantRole": ParticipantRoleType,
     },
     total=False,
 )
 
+
 class ChannelDefinitionTypeDef(
     _RequiredChannelDefinitionTypeDef, _OptionalChannelDefinitionTypeDef
 ):
     pass
 
+
 S3BucketSinkConfigurationTypeDef = TypedDict(
     "S3BucketSinkConfigurationTypeDef",
     {
         "Destination": str,
     },
 )
 
@@ -489,19 +498,21 @@
     "_OptionalKeywordMatchConfigurationOutputTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
+
 class KeywordMatchConfigurationOutputTypeDef(
     _RequiredKeywordMatchConfigurationOutputTypeDef, _OptionalKeywordMatchConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -509,19 +520,21 @@
     "_OptionalKeywordMatchConfigurationTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
+
 class KeywordMatchConfigurationTypeDef(
     _RequiredKeywordMatchConfigurationTypeDef, _OptionalKeywordMatchConfigurationTypeDef
 ):
     pass
 
+
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
@@ -615,19 +628,21 @@
     {
         "AudioChannels": AudioChannelsOptionType,
         "AudioSampleRate": str,
     },
     total=False,
 )
 
+
 class LiveConnectorRTMPConfigurationTypeDef(
     _RequiredLiveConnectorRTMPConfigurationTypeDef, _OptionalLiveConnectorRTMPConfigurationTypeDef
 ):
     pass
 
+
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
@@ -722,20 +737,22 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": List[str],
     },
     total=False,
 )
 
+
 class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -753,20 +770,22 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": Sequence[str],
     },
     total=False,
 )
 
+
 class AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
 ):
     pass
 
+
 ArtifactsConcatenationConfigurationTypeDef = TypedDict(
     "ArtifactsConcatenationConfigurationTypeDef",
     {
         "Audio": AudioConcatenationConfigurationTypeDef,
         "Video": VideoConcatenationConfigurationTypeDef,
         "Content": ContentConcatenationConfigurationTypeDef,
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
@@ -786,38 +805,42 @@
     "_OptionalStreamChannelDefinitionOutputTypeDef",
     {
         "ChannelDefinitions": List[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
+
 class StreamChannelDefinitionOutputTypeDef(
     _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
 ):
     pass
 
+
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
     "_OptionalStreamChannelDefinitionTypeDef",
     {
         "ChannelDefinitions": Sequence[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
+
 class StreamChannelDefinitionTypeDef(
     _RequiredStreamChannelDefinitionTypeDef, _OptionalStreamChannelDefinitionTypeDef
 ):
     pass
 
+
 ConcatenationSinkTypeDef = TypedDict(
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
@@ -876,19 +899,21 @@
         "VerticalLayoutConfiguration": VerticalLayoutConfigurationTypeDef,
         "VideoAttribute": VideoAttributeTypeDef,
         "CanvasOrientation": CanvasOrientationType,
     },
     total=False,
 )
 
+
 class GridViewConfigurationTypeDef(
     _RequiredGridViewConfigurationTypeDef, _OptionalGridViewConfigurationTypeDef
 ):
     pass
 
+
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -934,19 +959,21 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class RealTimeAlertRuleOutputTypeDef(
     _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
 ):
     pass
 
+
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -955,19 +982,21 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
+
 SourceConfigurationOutputTypeDef = TypedDict(
     "SourceConfigurationOutputTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
     },
     total=False,
 )
@@ -999,20 +1028,22 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class MediaInsightsPipelineConfigurationElementOutputTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
 ):
     pass
 
+
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -1028,20 +1059,22 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class MediaInsightsPipelineConfigurationElementTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementTypeDef,
 ):
     pass
 
+
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
@@ -1056,19 +1089,21 @@
     "_OptionalStreamConfigurationOutputTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
+
 class StreamConfigurationOutputTypeDef(
     _RequiredStreamConfigurationOutputTypeDef, _OptionalStreamConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
 )
@@ -1076,19 +1111,21 @@
     "_OptionalStreamConfigurationTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
+
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
+
 KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     {
         "Streams": List[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorOutputTypeDef,
     },
 )
@@ -1112,20 +1149,22 @@
     {
         "Layout": Literal["GridView"],
         "Resolution": ResolutionOptionType,
     },
     total=False,
 )
 
+
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
+
 RealTimeAlertConfigurationOutputTypeDef = TypedDict(
     "RealTimeAlertConfigurationOutputTypeDef",
     {
         "Disabled": bool,
         "Rules": List[RealTimeAlertRuleOutputTypeDef],
     },
     total=False,
@@ -1178,19 +1217,21 @@
     "_OptionalArtifactsConfigurationTypeDef",
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1199,20 +1240,22 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1221,20 +1264,22 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
+
 MediaInsightsPipelineConfigurationTypeDef = TypedDict(
     "MediaInsightsPipelineConfigurationTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "MediaInsightsPipelineConfigurationArn": str,
         "ResourceAccessRoleArn": str,
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
@@ -1247,55 +1292,69 @@
 )
 
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        "Elements": Sequence[
+            Union[
+                MediaInsightsPipelineConfigurationElementTypeDef,
+                MediaInsightsPipelineConfigurationElementOutputTypeDef,
+            ]
+        ],
     },
 )
 _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        "Elements": Sequence[
+            Union[
+                MediaInsightsPipelineConfigurationElementTypeDef,
+                MediaInsightsPipelineConfigurationElementOutputTypeDef,
+            ]
+        ],
     },
 )
 _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 ConcatenationSourceTypeDef = TypedDict(
     "ConcatenationSourceTypeDef",
     {
         "Type": Literal["MediaCapturePipeline"],
         "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
 )
@@ -1339,20 +1398,22 @@
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateMediaInsightsPipelineRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
 ):
     pass
 
+
 ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
@@ -1423,20 +1484,22 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaConcatenationPipelineRequestRequestTypeDef(
     _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef,
     _OptionalCreateMediaConcatenationPipelineRequestRequestTypeDef,
 ):
     pass
 
+
 MediaConcatenationPipelineTypeDef = TypedDict(
     "MediaConcatenationPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Sources": List[ConcatenationSourceTypeDef],
         "Sinks": List[ConcatenationSinkTypeDef],
@@ -1487,20 +1550,22 @@
         "ClientRequestToken": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
+
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
         "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
@@ -1510,33 +1575,40 @@
     },
     total=False,
 )
 
 _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
-        "Sources": Sequence[LiveConnectorSourceConfigurationTypeDef],
+        "Sources": Sequence[
+            Union[
+                LiveConnectorSourceConfigurationTypeDef,
+                LiveConnectorSourceConfigurationOutputTypeDef,
+            ]
+        ],
         "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
     },
 )
 _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
     _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
 ):
     pass
 
+
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.28.15
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.28.15/setup.py` & `mypy-boto3-chime-sdk-media-pipelines-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-media-pipelines",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ChimeSDKMediaPipelines 1.28.15 service generated with"
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

