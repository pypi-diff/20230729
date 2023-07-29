# Comparing `tmp/mypy-boto3-iotanalytics-1.28.15.tar.gz` & `tmp/mypy-boto3-iotanalytics-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotanalytics-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
+gzip compressed data, was "mypy-boto3-iotanalytics-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:20 2023, max compression
```

## Comparing `mypy-boto3-iotanalytics-1.28.15.tar` & `mypy-boto3-iotanalytics-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.429256 mypy-boto3-iotanalytics-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19091 2023-07-28 20:42:59.429256 mypy-boto3-iotanalytics-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17584 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.429256 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26324 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26278 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51528 2023-07-28 20:28:19.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51447 2023-07-28 20:28:18.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:17.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.429256 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19091 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:59.000000 mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.429256 mypy-boto3-iotanalytics-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:28:16.000000 mypy-boto3-iotanalytics-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.025182 mypy-boto3-iotanalytics-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-07-29 10:03:20.025182 mypy-boto3-iotanalytics-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17584 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.017182 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27092 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27046 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51718 2023-07-29 09:47:52.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51637 2023-07-29 09:47:51.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.025182 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:19.000000 mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:20.025182 mypy-boto3-iotanalytics-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:47:48.000000 mypy-boto3-iotanalytics-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-iotanalytics-1.28.15/LICENSE` & `mypy-boto3-iotanalytics-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15/PKG-INFO` & `mypy-boto3-iotanalytics-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotanalytics
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotanalytics-1.28.15/README.md` & `mypy-boto3-iotanalytics-1.28.15.post1/README.md`

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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__init__.py` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__init__.pyi` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/__main__.py` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTAnalytics 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.IoTAnalytics 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics\nOther"
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

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/client.py` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,42 +26,48 @@
     ListDatasetsPaginator,
     ListDatastoresPaginator,
     ListPipelinesPaginator,
 )
 from .type_defs import (
     BatchPutMessageResponseTypeDef,
     ChannelMessagesTypeDef,
+    ChannelStorageOutputTypeDef,
     ChannelStorageTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     CreatePipelineResponseTypeDef,
+    DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetTriggerTypeDef,
+    DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     DescribePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     GetDatasetContentResponseTypeDef,
     LateDataRuleTypeDef,
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LoggingOptionsTypeDef,
     MessageTypeDef,
+    PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     RetentionPeriodTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     TagTypeDef,
     VersioningConfigurationTypeDef,
@@ -148,30 +154,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#close)
         """
 
     def create_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageTypeDef = ...,
+        channelStorage: Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Used to create a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_channel)
         """
 
     def create_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionTypeDef],
+        actions: Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
@@ -193,32 +199,36 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_dataset_content)
         """
 
     def create_datastore(
         self,
         *,
         datastoreName: str,
-        datastoreStorage: DatastoreStorageTypeDef = ...,
+        datastoreStorage: Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...,
-        datastorePartitions: DatastorePartitionsTypeDef = ...
+        fileFormatConfiguration: Union[
+            FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
+        ] = ...,
+        datastorePartitions: Union[
+            DatastorePartitionsTypeDef, DatastorePartitionsOutputTypeDef
+        ] = ...
     ) -> CreateDatastoreResponseTypeDef:
         """
         Creates a data store, which is a repository for messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_datastore)
         """
 
     def create_pipeline(
         self,
         *,
         pipelineName: str,
-        pipelineActivities: Sequence[PipelineActivityTypeDef],
+        pipelineActivities: Sequence[Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]],
         tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_pipeline)
@@ -407,15 +417,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.put_logging_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#put_logging_options)
         """
 
     def run_pipeline_activity(
         self,
         *,
-        pipelineActivity: PipelineActivityTypeDef,
+        pipelineActivity: Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef],
         payloads: Sequence[Union[str, bytes, IO[Any], StreamingBody]]
     ) -> RunPipelineActivityResponseTypeDef:
         """
         Simulates the results of running a pipeline activity on a message payload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.run_pipeline_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#run_pipeline_activity)
@@ -468,29 +478,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#untag_resource)
         """
 
     def update_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageTypeDef = ...,
+        channelStorage: Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_channel)
         """
 
     def update_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionTypeDef],
+        actions: Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
@@ -501,26 +511,31 @@
         """
 
     def update_datastore(
         self,
         *,
         datastoreName: str,
         retentionPeriod: RetentionPeriodTypeDef = ...,
-        datastoreStorage: DatastoreStorageTypeDef = ...,
-        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...
+        datastoreStorage: Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef] = ...,
+        fileFormatConfiguration: Union[
+            FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
+        ] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_datastore)
         """
 
     def update_pipeline(
-        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityTypeDef]
+        self,
+        *,
+        pipelineName: str,
+        pipelineActivities: Sequence[Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_pipeline)
         """
```

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/client.pyi` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,42 +26,48 @@
     ListDatasetsPaginator,
     ListDatastoresPaginator,
     ListPipelinesPaginator,
 )
 from .type_defs import (
     BatchPutMessageResponseTypeDef,
     ChannelMessagesTypeDef,
+    ChannelStorageOutputTypeDef,
     ChannelStorageTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     CreatePipelineResponseTypeDef,
+    DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetTriggerTypeDef,
+    DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     DescribePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     GetDatasetContentResponseTypeDef,
     LateDataRuleTypeDef,
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LoggingOptionsTypeDef,
     MessageTypeDef,
+    PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     RetentionPeriodTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     TagTypeDef,
     VersioningConfigurationTypeDef,
@@ -139,29 +145,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#close)
         """
     def create_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageTypeDef = ...,
+        channelStorage: Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Used to create a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_channel)
         """
     def create_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionTypeDef],
+        actions: Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
@@ -181,31 +187,35 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_dataset_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_dataset_content)
         """
     def create_datastore(
         self,
         *,
         datastoreName: str,
-        datastoreStorage: DatastoreStorageTypeDef = ...,
+        datastoreStorage: Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...,
-        datastorePartitions: DatastorePartitionsTypeDef = ...
+        fileFormatConfiguration: Union[
+            FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
+        ] = ...,
+        datastorePartitions: Union[
+            DatastorePartitionsTypeDef, DatastorePartitionsOutputTypeDef
+        ] = ...
     ) -> CreateDatastoreResponseTypeDef:
         """
         Creates a data store, which is a repository for messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_datastore)
         """
     def create_pipeline(
         self,
         *,
         pipelineName: str,
-        pipelineActivities: Sequence[PipelineActivityTypeDef],
+        pipelineActivities: Sequence[Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]],
         tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#create_pipeline)
@@ -374,15 +384,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.put_logging_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#put_logging_options)
         """
     def run_pipeline_activity(
         self,
         *,
-        pipelineActivity: PipelineActivityTypeDef,
+        pipelineActivity: Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef],
         payloads: Sequence[Union[str, bytes, IO[Any], StreamingBody]]
     ) -> RunPipelineActivityResponseTypeDef:
         """
         Simulates the results of running a pipeline activity on a message payload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.run_pipeline_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#run_pipeline_activity)
@@ -430,28 +440,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#untag_resource)
         """
     def update_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageTypeDef = ...,
+        channelStorage: Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_channel)
         """
     def update_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionTypeDef],
+        actions: Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
@@ -461,25 +471,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_dataset)
         """
     def update_datastore(
         self,
         *,
         datastoreName: str,
         retentionPeriod: RetentionPeriodTypeDef = ...,
-        datastoreStorage: DatastoreStorageTypeDef = ...,
-        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...
+        datastoreStorage: Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef] = ...,
+        fileFormatConfiguration: Union[
+            FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
+        ] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_datastore)
         """
     def update_pipeline(
-        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityTypeDef]
+        self,
+        *,
+        pipelineName: str,
+        pipelineActivities: Sequence[Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/client/#update_pipeline)
         """
```

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/literals.py` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/literals.pyi` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/paginator.py` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/paginator.pyi` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/type_defs.py` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1756,15 +1756,17 @@
     total=False,
 )
 
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityTypeDef],
+        "pipelineActivities": Sequence[
+            Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
+        ],
     },
 )
 _OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePipelineRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
@@ -1786,15 +1788,17 @@
     },
 )
 
 UpdatePipelineRequestRequestTypeDef = TypedDict(
     "UpdatePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityTypeDef],
+        "pipelineActivities": Sequence[
+            Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
+        ],
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
@@ -2004,15 +2008,15 @@
     total=False,
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionTypeDef],
+        "actions": Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
     },
 )
 _OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
@@ -2031,15 +2035,15 @@
     pass
 
 
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionTypeDef],
+        "actions": Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
     },
 )
 _OptionalUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
```

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics/type_defs.pyi` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1687,15 +1687,17 @@
     total=False,
 )
 
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityTypeDef],
+        "pipelineActivities": Sequence[
+            Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
+        ],
     },
 )
 _OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePipelineRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
@@ -1715,15 +1717,17 @@
     },
 )
 
 UpdatePipelineRequestRequestTypeDef = TypedDict(
     "UpdatePipelineRequestRequestTypeDef",
     {
         "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityTypeDef],
+        "pipelineActivities": Sequence[
+            Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
+        ],
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
@@ -1927,15 +1931,15 @@
     total=False,
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionTypeDef],
+        "actions": Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
     },
 )
 _OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
@@ -1952,15 +1956,15 @@
 ):
     pass
 
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionTypeDef],
+        "actions": Sequence[Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]],
     },
 )
 _OptionalUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
```

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/PKG-INFO` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotanalytics
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/
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
 [mypy-boto3-iotanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotanalytics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotanalytics-1.28.15/mypy_boto3_iotanalytics.egg-info/SOURCES.txt` & `mypy-boto3-iotanalytics-1.28.15.post1/mypy_boto3_iotanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotanalytics-1.28.15/setup.py` & `mypy-boto3-iotanalytics-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotanalytics",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_iotanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.IoTAnalytics 1.28.15 service generated with mypy-boto3-builder"
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

