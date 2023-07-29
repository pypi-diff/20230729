# Comparing `tmp/mypy-boto3-kinesisvideo-1.28.15.tar.gz` & `tmp/mypy-boto3-kinesisvideo-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisvideo-1.28.15.tar", last modified: Fri Jul 28 20:43:06 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisvideo-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:29 2023, max compression
```

## Comparing `mypy-boto3-kinesisvideo-1.28.15.tar` & `mypy-boto3-kinesisvideo-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:06.025347 mypy-boto3-kinesisvideo-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-07-28 20:43:06.021347 mypy-boto3-kinesisvideo-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15701 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:06.013347 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-07-28 20:29:24.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-07-28 20:29:24.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29470 2023-07-28 20:29:24.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-07-28 20:29:24.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:06.021347 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:05.000000 mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:06.025347 mypy-boto3-kinesisvideo-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:29:23.000000 mypy-boto3-kinesisvideo-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:29.917229 mypy-boto3-kinesisvideo-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-29 10:03:29.917229 mypy-boto3-kinesisvideo-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15701 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:29.913229 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25063 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29470 2023-07-29 09:49:00.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-07-29 09:49:00.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:29.917229 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:29.000000 mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:29.917229 mypy-boto3-kinesisvideo-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:48:59.000000 mypy-boto3-kinesisvideo-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15/LICENSE` & `mypy-boto3-kinesisvideo-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15/PKG-INFO` & `mypy-boto3-kinesisvideo-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.28.15
-Summary: Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15/README.md` & `mypy-boto3-kinesisvideo-1.28.15.post1/README.md`

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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__init__.py` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__init__.pyi` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/__main__.py` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideo 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.KinesisVideo 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
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

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/client.py` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_kinesisvideo.client import KinesisVideoClient
 
     session = Session()
     client: KinesisVideoClient = session.client("kinesisvideo")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import APINameType, ChannelTypeType, UpdateDataRetentionOperationType
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
     ListEdgeAgentConfigurationsPaginator,
@@ -35,14 +35,15 @@
     DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
+    ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
@@ -422,15 +423,17 @@
         """
 
     def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
+        ImageGenerationConfiguration: Union[
+            ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_image_generation_configuration)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/client.pyi` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_kinesisvideo.client import KinesisVideoClient
 
     session = Session()
     client: KinesisVideoClient = session.client("kinesisvideo")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import APINameType, ChannelTypeType, UpdateDataRetentionOperationType
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
     ListEdgeAgentConfigurationsPaginator,
@@ -35,14 +35,15 @@
     DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
+    ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
@@ -389,15 +390,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_data_retention)
         """
     def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
+        ImageGenerationConfiguration: Union[
+            ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_image_generation_configuration)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/literals.py` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/literals.pyi` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/paginator.py` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/paginator.pyi` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/type_defs.py` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo/type_defs.pyi` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/PKG-INFO` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.28.15
-Summary: Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
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
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kinesisvideo-1.28.15/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt` & `mypy-boto3-kinesisvideo-1.28.15.post1/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.15/setup.py` & `mypy-boto3-kinesisvideo-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisvideo",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.KinesisVideo 1.28.15 service generated with mypy-boto3-builder"
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

