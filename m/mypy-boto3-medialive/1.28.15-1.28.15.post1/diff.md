# Comparing `tmp/mypy-boto3-medialive-1.28.15.tar.gz` & `tmp/mypy-boto3-medialive-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medialive-1.28.15.tar", last modified: Fri Jul 28 20:43:15 2023, max compression
+gzip compressed data, was "mypy-boto3-medialive-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:38 2023, max compression
```

## Comparing `mypy-boto3-medialive-1.28.15.tar` & `mypy-boto3-medialive-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.285474 mypy-boto3-medialive-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    38868 2023-07-28 20:43:15.285474 mypy-boto3-medialive-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37373 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.277474 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52938 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52848 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39584 2023-07-28 20:31:26.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-07-28 20:31:26.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   172819 2023-07-28 20:31:33.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   172642 2023-07-28 20:31:28.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-28 20:31:25.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.285474 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38868 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:15.000000 mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:15.285474 mypy-boto3-medialive-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:31:24.000000 mypy-boto3-medialive-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:38.613275 mypy-boto3-medialive-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    38874 2023-07-29 10:03:38.609275 mypy-boto3-medialive-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37373 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:38.605275 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53424 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53334 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39584 2023-07-29 09:51:05.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   173017 2023-07-29 09:51:09.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172840 2023-07-29 09:51:07.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:01.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-29 09:51:04.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:38.609275 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38874 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:38.000000 mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:38.613275 mypy-boto3-medialive-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:51:00.000000 mypy-boto3-medialive-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-medialive-1.28.15/LICENSE` & `mypy-boto3-medialive-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15/PKG-INFO` & `mypy-boto3-medialive-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.28.15
-Summary: Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-medialive-1.28.15/README.md` & `mypy-boto3-medialive-1.28.15.post1/README.md`

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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__init__.py` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__init__.pyi` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/__main__.py` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaLive 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.MediaLive 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\nOther"
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

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/client.py` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_medialive.client import MediaLiveClient
 
     session = Session()
     client: MediaLiveClient = session.client("medialive")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ChannelClassType, InputTypeType, LogLevelType, RebootInputDeviceForceType
 from .paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
@@ -59,15 +59,17 @@
     DescribeMultiplexProgramResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     DescribeScheduleResponseTypeDef,
     DescribeThumbnailsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncoderSettingsOutputTypeDef,
     EncoderSettingsTypeDef,
+    InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputSpecificationTypeDef,
@@ -84,14 +86,15 @@
     ListReservationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceCreateSettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaConnectFlowRequestTypeDef,
     MultiplexProgramSettingsTypeDef,
     MultiplexSettingsTypeDef,
+    OutputDestinationOutputTypeDef,
     OutputDestinationTypeDef,
     PurchaseOfferingResponseTypeDef,
     RenewalSettingsTypeDef,
     StartChannelResponseTypeDef,
     StartMultiplexResponseTypeDef,
     StopChannelResponseTypeDef,
     StopMultiplexResponseTypeDef,
@@ -121,39 +124,35 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MediaLiveClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BadGatewayException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     GatewayTimeoutException: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     UnprocessableEntityException: Type[BotocoreClientError]
 
-
 class MediaLiveClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/)
     """
 
     meta: ClientMeta
@@ -162,116 +161,110 @@
     def exceptions(self) -> Exceptions:
         """
         MediaLiveClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#exceptions)
         """
-
     def accept_input_device_transfer(self, *, InputDeviceId: str) -> Dict[str, Any]:
         """
         Accept an incoming input device transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.accept_input_device_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#accept_input_device_transfer)
         """
-
     def batch_delete(
         self,
         *,
         ChannelIds: Sequence[str] = ...,
         InputIds: Sequence[str] = ...,
         InputSecurityGroupIds: Sequence[str] = ...,
         MultiplexIds: Sequence[str] = ...
     ) -> BatchDeleteResponseTypeDef:
         """
         Starts delete of resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#batch_delete)
         """
-
     def batch_start(
         self, *, ChannelIds: Sequence[str] = ..., MultiplexIds: Sequence[str] = ...
     ) -> BatchStartResponseTypeDef:
         """
         Starts existing resources See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/BatchStart).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_start)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#batch_start)
         """
-
     def batch_stop(
         self, *, ChannelIds: Sequence[str] = ..., MultiplexIds: Sequence[str] = ...
     ) -> BatchStopResponseTypeDef:
         """
         Stops running resources See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/BatchStop).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_stop)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#batch_stop)
         """
-
     def batch_update_schedule(
         self,
         *,
         ChannelId: str,
         Creates: BatchScheduleActionCreateRequestTypeDef = ...,
         Deletes: BatchScheduleActionDeleteRequestTypeDef = ...
     ) -> BatchUpdateScheduleResponseTypeDef:
         """
         Update a channel schedule See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/BatchUpdateSchedule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_update_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#batch_update_schedule)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#can_paginate)
         """
-
     def cancel_input_device_transfer(self, *, InputDeviceId: str) -> Dict[str, Any]:
         """
         Cancel an input device transfer that you have requested.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.cancel_input_device_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#cancel_input_device_transfer)
         """
-
     def claim_device(self, *, Id: str = ...) -> Dict[str, Any]:
         """
         Send a request to claim an AWS Elemental device that you have purchased from a
         third-party vendor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.claim_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#claim_device)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#close)
         """
-
     def create_channel(
         self,
         *,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
         ChannelClass: ChannelClassType = ...,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...,
-        EncoderSettings: EncoderSettingsTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
+        Destinations: Sequence[
+            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
+        ] = ...,
+        EncoderSettings: Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef] = ...,
+        InputAttachments: Sequence[
+            Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
+        ] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceCreateSettingsTypeDef = ...,
         Name: str = ...,
         RequestId: str = ...,
         Reserved: str = ...,
         RoleArn: str = ...,
@@ -281,15 +274,14 @@
         """
         Creates a new channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_channel)
         """
-
     def create_input(
         self,
         *,
         Destinations: Sequence[InputDestinationRequestTypeDef] = ...,
         InputDevices: Sequence[InputDeviceSettingsTypeDef] = ...,
         InputSecurityGroups: Sequence[str] = ...,
         MediaConnectFlows: Sequence[MediaConnectFlowRequestTypeDef] = ...,
@@ -304,29 +296,27 @@
         """
         Create an input See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_input)
         """
-
     def create_input_security_group(
         self,
         *,
         Tags: Mapping[str, str] = ...,
         WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...
     ) -> CreateInputSecurityGroupResponseTypeDef:
         """
         Creates a Input Security Group See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateInputSecurityGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_input_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_input_security_group)
         """
-
     def create_multiplex(
         self,
         *,
         AvailabilityZones: Sequence[str],
         MultiplexSettings: MultiplexSettingsTypeDef,
         Name: str,
         RequestId: str,
@@ -334,323 +324,291 @@
     ) -> CreateMultiplexResponseTypeDef:
         """
         Create a new multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_multiplex)
         """
-
     def create_multiplex_program(
         self,
         *,
         MultiplexId: str,
         MultiplexProgramSettings: MultiplexProgramSettingsTypeDef,
         ProgramName: str,
         RequestId: str
     ) -> CreateMultiplexProgramResponseTypeDef:
         """
         Create a new program in the multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_multiplex_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_multiplex_program)
         """
-
     def create_partner_input(
         self, *, InputId: str, RequestId: str = ..., Tags: Mapping[str, str] = ...
     ) -> CreatePartnerInputResponseTypeDef:
         """
         Create a partner input See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreatePartnerInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_partner_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_partner_input)
         """
-
     def create_tags(
         self, *, ResourceArn: str, Tags: Mapping[str, str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Create tags for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateTags).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_tags)
         """
-
     def delete_channel(self, *, ChannelId: str) -> DeleteChannelResponseTypeDef:
         """
         Starts deletion of channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_channel)
         """
-
     def delete_input(self, *, InputId: str) -> Dict[str, Any]:
         """
         Deletes the input end point See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_input)
         """
-
     def delete_input_security_group(self, *, InputSecurityGroupId: str) -> Dict[str, Any]:
         """
         Deletes an Input Security Group See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteInputSecurityGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_input_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_input_security_group)
         """
-
     def delete_multiplex(self, *, MultiplexId: str) -> DeleteMultiplexResponseTypeDef:
         """
         Delete a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_multiplex)
         """
-
     def delete_multiplex_program(
         self, *, MultiplexId: str, ProgramName: str
     ) -> DeleteMultiplexProgramResponseTypeDef:
         """
         Delete a program from a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_multiplex_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_multiplex_program)
         """
-
     def delete_reservation(self, *, ReservationId: str) -> DeleteReservationResponseTypeDef:
         """
         Delete an expired reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_reservation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_reservation)
         """
-
     def delete_schedule(self, *, ChannelId: str) -> Dict[str, Any]:
         """
         Delete all schedule actions on a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_schedule)
         """
-
     def delete_tags(
         self, *, ResourceArn: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes tags for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteTags).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_tags)
         """
-
     def describe_account_configuration(self) -> DescribeAccountConfigurationResponseTypeDef:
         """
         Get account configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeAccountConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_account_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_account_configuration)
         """
-
     def describe_channel(self, *, ChannelId: str) -> DescribeChannelResponseTypeDef:
         """
         Gets details about a channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_channel)
         """
-
     def describe_input(self, *, InputId: str) -> DescribeInputResponseTypeDef:
         """
         Produces details about an input See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_input)
         """
-
     def describe_input_device(self, *, InputDeviceId: str) -> DescribeInputDeviceResponseTypeDef:
         """
         Gets the details for the input device See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeInputDevice).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_input_device)
         """
-
     def describe_input_device_thumbnail(
         self, *, InputDeviceId: str, Accept: Literal["image/jpeg"]
     ) -> DescribeInputDeviceThumbnailResponseTypeDef:
         """
         Get the latest thumbnail data for the input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_input_device_thumbnail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_input_device_thumbnail)
         """
-
     def describe_input_security_group(
         self, *, InputSecurityGroupId: str
     ) -> DescribeInputSecurityGroupResponseTypeDef:
         """
         Produces a summary of an Input Security Group See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeInputSecurityGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_input_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_input_security_group)
         """
-
     def describe_multiplex(self, *, MultiplexId: str) -> DescribeMultiplexResponseTypeDef:
         """
         Gets details about a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_multiplex)
         """
-
     def describe_multiplex_program(
         self, *, MultiplexId: str, ProgramName: str
     ) -> DescribeMultiplexProgramResponseTypeDef:
         """
         Get the details for a program in a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_multiplex_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_multiplex_program)
         """
-
     def describe_offering(self, *, OfferingId: str) -> DescribeOfferingResponseTypeDef:
         """
         Get details for an offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_offering)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_offering)
         """
-
     def describe_reservation(self, *, ReservationId: str) -> DescribeReservationResponseTypeDef:
         """
         Get details for a reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_reservation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_reservation)
         """
-
     def describe_schedule(
         self, *, ChannelId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeScheduleResponseTypeDef:
         """
         Get a channel schedule See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeSchedule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_schedule)
         """
-
     def describe_thumbnails(
         self, *, ChannelId: str, PipelineId: str, ThumbnailType: str
     ) -> DescribeThumbnailsResponseTypeDef:
         """
         Describe the latest thumbnails data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_thumbnails)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_thumbnails)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#generate_presigned_url)
         """
-
     def list_channels(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelsResponseTypeDef:
         """
         Produces list of channels that have been created See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListChannels).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_channels)
         """
-
     def list_input_device_transfers(
         self, *, TransferType: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInputDeviceTransfersResponseTypeDef:
         """
         List input devices that are currently being transferred.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_input_device_transfers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_input_device_transfers)
         """
-
     def list_input_devices(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInputDevicesResponseTypeDef:
         """
         List input devices See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListInputDevices).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_input_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_input_devices)
         """
-
     def list_input_security_groups(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInputSecurityGroupsResponseTypeDef:
         """
         Produces a list of Input Security Groups for an account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListInputSecurityGroups).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_input_security_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_input_security_groups)
         """
-
     def list_inputs(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInputsResponseTypeDef:
         """
         Produces list of inputs that have been created See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListInputs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_inputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_inputs)
         """
-
     def list_multiplex_programs(
         self, *, MultiplexId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListMultiplexProgramsResponseTypeDef:
         """
         List the programs that currently exist for a specific multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_multiplex_programs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_multiplex_programs)
         """
-
     def list_multiplexes(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListMultiplexesResponseTypeDef:
         """
         Retrieve a list of the existing multiplexes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_multiplexes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_multiplexes)
         """
-
     def list_offerings(
         self,
         *,
         ChannelClass: str = ...,
         ChannelConfiguration: str = ...,
         Codec: str = ...,
         Duration: str = ...,
@@ -665,15 +623,14 @@
     ) -> ListOfferingsResponseTypeDef:
         """
         List offerings available for purchase.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_offerings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_offerings)
         """
-
     def list_reservations(
         self,
         *,
         ChannelClass: str = ...,
         Codec: str = ...,
         MaxResults: int = ...,
         MaximumBitrate: str = ...,
@@ -686,24 +643,22 @@
     ) -> ListReservationsResponseTypeDef:
         """
         List purchased reservations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_reservations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_reservations)
         """
-
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Produces list of tags that have been created for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListTagsForResource).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_tags_for_resource)
         """
-
     def purchase_offering(
         self,
         *,
         Count: int,
         OfferingId: str,
         Name: str = ...,
         RenewalSettings: RenewalSettingsTypeDef = ...,
@@ -713,136 +668,130 @@
     ) -> PurchaseOfferingResponseTypeDef:
         """
         Purchase an offering and create a reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.purchase_offering)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#purchase_offering)
         """
-
     def reboot_input_device(
         self, *, InputDeviceId: str, Force: RebootInputDeviceForceType = ...
     ) -> Dict[str, Any]:
         """
         Send a reboot command to the specified input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.reboot_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#reboot_input_device)
         """
-
     def reject_input_device_transfer(self, *, InputDeviceId: str) -> Dict[str, Any]:
         """
         Reject the transfer of the specified input device to your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.reject_input_device_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#reject_input_device_transfer)
         """
-
     def start_channel(self, *, ChannelId: str) -> StartChannelResponseTypeDef:
         """
         Starts an existing channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/StartChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_channel)
         """
-
     def start_input_device_maintenance_window(self, *, InputDeviceId: str) -> Dict[str, Any]:
         """
         Start a maintenance window for the specified input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_input_device_maintenance_window)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_input_device_maintenance_window)
         """
-
     def start_multiplex(self, *, MultiplexId: str) -> StartMultiplexResponseTypeDef:
         """
         Start (run) the multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_multiplex)
         """
-
     def stop_channel(self, *, ChannelId: str) -> StopChannelResponseTypeDef:
         """
         Stops a running channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/StopChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.stop_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#stop_channel)
         """
-
     def stop_multiplex(self, *, MultiplexId: str) -> StopMultiplexResponseTypeDef:
         """
         Stops a running multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.stop_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#stop_multiplex)
         """
-
     def transfer_input_device(
         self,
         *,
         InputDeviceId: str,
         TargetCustomerId: str = ...,
         TargetRegion: str = ...,
         TransferMessage: str = ...
     ) -> Dict[str, Any]:
         """
         Start an input device transfer to another AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.transfer_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#transfer_input_device)
         """
-
     def update_account_configuration(
         self, *, AccountConfiguration: AccountConfigurationTypeDef = ...
     ) -> UpdateAccountConfigurationResponseTypeDef:
         """
         Update account configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/UpdateAccountConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_account_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_account_configuration)
         """
-
     def update_channel(
         self,
         *,
         ChannelId: str,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...,
-        EncoderSettings: EncoderSettingsTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
+        Destinations: Sequence[
+            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
+        ] = ...,
+        EncoderSettings: Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef] = ...,
+        InputAttachments: Sequence[
+            Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
+        ] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceUpdateSettingsTypeDef = ...,
         Name: str = ...,
         RoleArn: str = ...
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel)
         """
-
     def update_channel_class(
         self,
         *,
         ChannelClass: ChannelClassType,
         ChannelId: str,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...
+        Destinations: Sequence[
+            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
+        ] = ...
     ) -> UpdateChannelClassResponseTypeDef:
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel_class)
         """
-
     def update_input(
         self,
         *,
         InputId: str,
         Destinations: Sequence[InputDestinationRequestTypeDef] = ...,
         InputDevices: Sequence[InputDeviceRequestTypeDef] = ...,
         InputSecurityGroups: Sequence[str] = ...,
@@ -853,235 +802,209 @@
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_input)
         """
-
     def update_input_device(
         self,
         *,
         InputDeviceId: str,
         HdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
         Name: str = ...,
         UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...
     ) -> UpdateInputDeviceResponseTypeDef:
         """
         Updates the parameters for the input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_input_device)
         """
-
     def update_input_security_group(
         self,
         *,
         InputSecurityGroupId: str,
         Tags: Mapping[str, str] = ...,
         WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...
     ) -> UpdateInputSecurityGroupResponseTypeDef:
         """
         Update an Input Security Group's Whilelists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_input_security_group)
         """
-
     def update_multiplex(
         self,
         *,
         MultiplexId: str,
         MultiplexSettings: MultiplexSettingsTypeDef = ...,
         Name: str = ...
     ) -> UpdateMultiplexResponseTypeDef:
         """
         Updates a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_multiplex)
         """
-
     def update_multiplex_program(
         self,
         *,
         MultiplexId: str,
         ProgramName: str,
         MultiplexProgramSettings: MultiplexProgramSettingsTypeDef = ...
     ) -> UpdateMultiplexProgramResponseTypeDef:
         """
         Update a program in a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_multiplex_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_multiplex_program)
         """
-
     def update_reservation(
         self, *, ReservationId: str, Name: str = ..., RenewalSettings: RenewalSettingsTypeDef = ...
     ) -> UpdateReservationResponseTypeDef:
         """
         Update reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_reservation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_reservation)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_schedule"]
     ) -> DescribeSchedulePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_channels"]) -> ListChannelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_input_device_transfers"]
     ) -> ListInputDeviceTransfersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_input_devices"]
     ) -> ListInputDevicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_input_security_groups"]
     ) -> ListInputSecurityGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_inputs"]) -> ListInputsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_multiplex_programs"]
     ) -> ListMultiplexProgramsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_multiplexes"]
     ) -> ListMultiplexesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_offerings"]) -> ListOfferingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_reservations"]
     ) -> ListReservationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["channel_created"]) -> ChannelCreatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["channel_deleted"]) -> ChannelDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["channel_running"]) -> ChannelRunningWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["channel_stopped"]) -> ChannelStoppedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["input_attached"]) -> InputAttachedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["input_deleted"]) -> InputDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["input_detached"]) -> InputDetachedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["multiplex_created"]) -> MultiplexCreatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["multiplex_deleted"]) -> MultiplexDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["multiplex_running"]) -> MultiplexRunningWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["multiplex_stopped"]) -> MultiplexStoppedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/client.pyi` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_medialive.client import MediaLiveClient
 
     session = Session()
     client: MediaLiveClient = session.client("medialive")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ChannelClassType, InputTypeType, LogLevelType, RebootInputDeviceForceType
 from .paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
@@ -59,15 +59,17 @@
     DescribeMultiplexProgramResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     DescribeScheduleResponseTypeDef,
     DescribeThumbnailsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncoderSettingsOutputTypeDef,
     EncoderSettingsTypeDef,
+    InputAttachmentOutputTypeDef,
     InputAttachmentTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputSpecificationTypeDef,
@@ -84,14 +86,15 @@
     ListReservationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceCreateSettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaConnectFlowRequestTypeDef,
     MultiplexProgramSettingsTypeDef,
     MultiplexSettingsTypeDef,
+    OutputDestinationOutputTypeDef,
     OutputDestinationTypeDef,
     PurchaseOfferingResponseTypeDef,
     RenewalSettingsTypeDef,
     StartChannelResponseTypeDef,
     StartMultiplexResponseTypeDef,
     StopChannelResponseTypeDef,
     StopMultiplexResponseTypeDef,
@@ -121,35 +124,39 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("MediaLiveClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BadGatewayException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     GatewayTimeoutException: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     UnprocessableEntityException: Type[BotocoreClientError]
 
+
 class MediaLiveClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/)
     """
 
     meta: ClientMeta
@@ -158,106 +165,120 @@
     def exceptions(self) -> Exceptions:
         """
         MediaLiveClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#exceptions)
         """
+
     def accept_input_device_transfer(self, *, InputDeviceId: str) -> Dict[str, Any]:
         """
         Accept an incoming input device transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.accept_input_device_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#accept_input_device_transfer)
         """
+
     def batch_delete(
         self,
         *,
         ChannelIds: Sequence[str] = ...,
         InputIds: Sequence[str] = ...,
         InputSecurityGroupIds: Sequence[str] = ...,
         MultiplexIds: Sequence[str] = ...
     ) -> BatchDeleteResponseTypeDef:
         """
         Starts delete of resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#batch_delete)
         """
+
     def batch_start(
         self, *, ChannelIds: Sequence[str] = ..., MultiplexIds: Sequence[str] = ...
     ) -> BatchStartResponseTypeDef:
         """
         Starts existing resources See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/BatchStart).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_start)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#batch_start)
         """
+
     def batch_stop(
         self, *, ChannelIds: Sequence[str] = ..., MultiplexIds: Sequence[str] = ...
     ) -> BatchStopResponseTypeDef:
         """
         Stops running resources See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/BatchStop).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_stop)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#batch_stop)
         """
+
     def batch_update_schedule(
         self,
         *,
         ChannelId: str,
         Creates: BatchScheduleActionCreateRequestTypeDef = ...,
         Deletes: BatchScheduleActionDeleteRequestTypeDef = ...
     ) -> BatchUpdateScheduleResponseTypeDef:
         """
         Update a channel schedule See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/BatchUpdateSchedule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.batch_update_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#batch_update_schedule)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#can_paginate)
         """
+
     def cancel_input_device_transfer(self, *, InputDeviceId: str) -> Dict[str, Any]:
         """
         Cancel an input device transfer that you have requested.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.cancel_input_device_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#cancel_input_device_transfer)
         """
+
     def claim_device(self, *, Id: str = ...) -> Dict[str, Any]:
         """
         Send a request to claim an AWS Elemental device that you have purchased from a
         third-party vendor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.claim_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#claim_device)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#close)
         """
+
     def create_channel(
         self,
         *,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
         ChannelClass: ChannelClassType = ...,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...,
-        EncoderSettings: EncoderSettingsTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
+        Destinations: Sequence[
+            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
+        ] = ...,
+        EncoderSettings: Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef] = ...,
+        InputAttachments: Sequence[
+            Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
+        ] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceCreateSettingsTypeDef = ...,
         Name: str = ...,
         RequestId: str = ...,
         Reserved: str = ...,
         RoleArn: str = ...,
@@ -267,14 +288,15 @@
         """
         Creates a new channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_channel)
         """
+
     def create_input(
         self,
         *,
         Destinations: Sequence[InputDestinationRequestTypeDef] = ...,
         InputDevices: Sequence[InputDeviceSettingsTypeDef] = ...,
         InputSecurityGroups: Sequence[str] = ...,
         MediaConnectFlows: Sequence[MediaConnectFlowRequestTypeDef] = ...,
@@ -289,27 +311,29 @@
         """
         Create an input See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_input)
         """
+
     def create_input_security_group(
         self,
         *,
         Tags: Mapping[str, str] = ...,
         WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...
     ) -> CreateInputSecurityGroupResponseTypeDef:
         """
         Creates a Input Security Group See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateInputSecurityGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_input_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_input_security_group)
         """
+
     def create_multiplex(
         self,
         *,
         AvailabilityZones: Sequence[str],
         MultiplexSettings: MultiplexSettingsTypeDef,
         Name: str,
         RequestId: str,
@@ -317,291 +341,323 @@
     ) -> CreateMultiplexResponseTypeDef:
         """
         Create a new multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_multiplex)
         """
+
     def create_multiplex_program(
         self,
         *,
         MultiplexId: str,
         MultiplexProgramSettings: MultiplexProgramSettingsTypeDef,
         ProgramName: str,
         RequestId: str
     ) -> CreateMultiplexProgramResponseTypeDef:
         """
         Create a new program in the multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_multiplex_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_multiplex_program)
         """
+
     def create_partner_input(
         self, *, InputId: str, RequestId: str = ..., Tags: Mapping[str, str] = ...
     ) -> CreatePartnerInputResponseTypeDef:
         """
         Create a partner input See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreatePartnerInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_partner_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_partner_input)
         """
+
     def create_tags(
         self, *, ResourceArn: str, Tags: Mapping[str, str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Create tags for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateTags).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_tags)
         """
+
     def delete_channel(self, *, ChannelId: str) -> DeleteChannelResponseTypeDef:
         """
         Starts deletion of channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_channel)
         """
+
     def delete_input(self, *, InputId: str) -> Dict[str, Any]:
         """
         Deletes the input end point See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_input)
         """
+
     def delete_input_security_group(self, *, InputSecurityGroupId: str) -> Dict[str, Any]:
         """
         Deletes an Input Security Group See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteInputSecurityGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_input_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_input_security_group)
         """
+
     def delete_multiplex(self, *, MultiplexId: str) -> DeleteMultiplexResponseTypeDef:
         """
         Delete a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_multiplex)
         """
+
     def delete_multiplex_program(
         self, *, MultiplexId: str, ProgramName: str
     ) -> DeleteMultiplexProgramResponseTypeDef:
         """
         Delete a program from a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_multiplex_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_multiplex_program)
         """
+
     def delete_reservation(self, *, ReservationId: str) -> DeleteReservationResponseTypeDef:
         """
         Delete an expired reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_reservation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_reservation)
         """
+
     def delete_schedule(self, *, ChannelId: str) -> Dict[str, Any]:
         """
         Delete all schedule actions on a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_schedule)
         """
+
     def delete_tags(
         self, *, ResourceArn: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes tags for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteTags).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_tags)
         """
+
     def describe_account_configuration(self) -> DescribeAccountConfigurationResponseTypeDef:
         """
         Get account configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeAccountConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_account_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_account_configuration)
         """
+
     def describe_channel(self, *, ChannelId: str) -> DescribeChannelResponseTypeDef:
         """
         Gets details about a channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_channel)
         """
+
     def describe_input(self, *, InputId: str) -> DescribeInputResponseTypeDef:
         """
         Produces details about an input See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_input)
         """
+
     def describe_input_device(self, *, InputDeviceId: str) -> DescribeInputDeviceResponseTypeDef:
         """
         Gets the details for the input device See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeInputDevice).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_input_device)
         """
+
     def describe_input_device_thumbnail(
         self, *, InputDeviceId: str, Accept: Literal["image/jpeg"]
     ) -> DescribeInputDeviceThumbnailResponseTypeDef:
         """
         Get the latest thumbnail data for the input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_input_device_thumbnail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_input_device_thumbnail)
         """
+
     def describe_input_security_group(
         self, *, InputSecurityGroupId: str
     ) -> DescribeInputSecurityGroupResponseTypeDef:
         """
         Produces a summary of an Input Security Group See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeInputSecurityGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_input_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_input_security_group)
         """
+
     def describe_multiplex(self, *, MultiplexId: str) -> DescribeMultiplexResponseTypeDef:
         """
         Gets details about a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_multiplex)
         """
+
     def describe_multiplex_program(
         self, *, MultiplexId: str, ProgramName: str
     ) -> DescribeMultiplexProgramResponseTypeDef:
         """
         Get the details for a program in a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_multiplex_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_multiplex_program)
         """
+
     def describe_offering(self, *, OfferingId: str) -> DescribeOfferingResponseTypeDef:
         """
         Get details for an offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_offering)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_offering)
         """
+
     def describe_reservation(self, *, ReservationId: str) -> DescribeReservationResponseTypeDef:
         """
         Get details for a reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_reservation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_reservation)
         """
+
     def describe_schedule(
         self, *, ChannelId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeScheduleResponseTypeDef:
         """
         Get a channel schedule See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeSchedule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_schedule)
         """
+
     def describe_thumbnails(
         self, *, ChannelId: str, PipelineId: str, ThumbnailType: str
     ) -> DescribeThumbnailsResponseTypeDef:
         """
         Describe the latest thumbnails data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_thumbnails)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#describe_thumbnails)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#generate_presigned_url)
         """
+
     def list_channels(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelsResponseTypeDef:
         """
         Produces list of channels that have been created See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListChannels).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_channels)
         """
+
     def list_input_device_transfers(
         self, *, TransferType: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInputDeviceTransfersResponseTypeDef:
         """
         List input devices that are currently being transferred.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_input_device_transfers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_input_device_transfers)
         """
+
     def list_input_devices(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInputDevicesResponseTypeDef:
         """
         List input devices See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListInputDevices).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_input_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_input_devices)
         """
+
     def list_input_security_groups(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInputSecurityGroupsResponseTypeDef:
         """
         Produces a list of Input Security Groups for an account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListInputSecurityGroups).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_input_security_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_input_security_groups)
         """
+
     def list_inputs(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInputsResponseTypeDef:
         """
         Produces list of inputs that have been created See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListInputs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_inputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_inputs)
         """
+
     def list_multiplex_programs(
         self, *, MultiplexId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListMultiplexProgramsResponseTypeDef:
         """
         List the programs that currently exist for a specific multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_multiplex_programs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_multiplex_programs)
         """
+
     def list_multiplexes(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListMultiplexesResponseTypeDef:
         """
         Retrieve a list of the existing multiplexes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_multiplexes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_multiplexes)
         """
+
     def list_offerings(
         self,
         *,
         ChannelClass: str = ...,
         ChannelConfiguration: str = ...,
         Codec: str = ...,
         Duration: str = ...,
@@ -616,14 +672,15 @@
     ) -> ListOfferingsResponseTypeDef:
         """
         List offerings available for purchase.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_offerings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_offerings)
         """
+
     def list_reservations(
         self,
         *,
         ChannelClass: str = ...,
         Codec: str = ...,
         MaxResults: int = ...,
         MaximumBitrate: str = ...,
@@ -636,22 +693,24 @@
     ) -> ListReservationsResponseTypeDef:
         """
         List purchased reservations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_reservations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_reservations)
         """
+
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Produces list of tags that have been created for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListTagsForResource).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_tags_for_resource)
         """
+
     def purchase_offering(
         self,
         *,
         Count: int,
         OfferingId: str,
         Name: str = ...,
         RenewalSettings: RenewalSettingsTypeDef = ...,
@@ -661,124 +720,142 @@
     ) -> PurchaseOfferingResponseTypeDef:
         """
         Purchase an offering and create a reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.purchase_offering)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#purchase_offering)
         """
+
     def reboot_input_device(
         self, *, InputDeviceId: str, Force: RebootInputDeviceForceType = ...
     ) -> Dict[str, Any]:
         """
         Send a reboot command to the specified input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.reboot_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#reboot_input_device)
         """
+
     def reject_input_device_transfer(self, *, InputDeviceId: str) -> Dict[str, Any]:
         """
         Reject the transfer of the specified input device to your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.reject_input_device_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#reject_input_device_transfer)
         """
+
     def start_channel(self, *, ChannelId: str) -> StartChannelResponseTypeDef:
         """
         Starts an existing channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/StartChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_channel)
         """
+
     def start_input_device_maintenance_window(self, *, InputDeviceId: str) -> Dict[str, Any]:
         """
         Start a maintenance window for the specified input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_input_device_maintenance_window)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_input_device_maintenance_window)
         """
+
     def start_multiplex(self, *, MultiplexId: str) -> StartMultiplexResponseTypeDef:
         """
         Start (run) the multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_multiplex)
         """
+
     def stop_channel(self, *, ChannelId: str) -> StopChannelResponseTypeDef:
         """
         Stops a running channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/StopChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.stop_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#stop_channel)
         """
+
     def stop_multiplex(self, *, MultiplexId: str) -> StopMultiplexResponseTypeDef:
         """
         Stops a running multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.stop_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#stop_multiplex)
         """
+
     def transfer_input_device(
         self,
         *,
         InputDeviceId: str,
         TargetCustomerId: str = ...,
         TargetRegion: str = ...,
         TransferMessage: str = ...
     ) -> Dict[str, Any]:
         """
         Start an input device transfer to another AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.transfer_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#transfer_input_device)
         """
+
     def update_account_configuration(
         self, *, AccountConfiguration: AccountConfigurationTypeDef = ...
     ) -> UpdateAccountConfigurationResponseTypeDef:
         """
         Update account configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/UpdateAccountConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_account_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_account_configuration)
         """
+
     def update_channel(
         self,
         *,
         ChannelId: str,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...,
-        EncoderSettings: EncoderSettingsTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
+        Destinations: Sequence[
+            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
+        ] = ...,
+        EncoderSettings: Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef] = ...,
+        InputAttachments: Sequence[
+            Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
+        ] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceUpdateSettingsTypeDef = ...,
         Name: str = ...,
         RoleArn: str = ...
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel)
         """
+
     def update_channel_class(
         self,
         *,
         ChannelClass: ChannelClassType,
         ChannelId: str,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...
+        Destinations: Sequence[
+            Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
+        ] = ...
     ) -> UpdateChannelClassResponseTypeDef:
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel_class)
         """
+
     def update_input(
         self,
         *,
         InputId: str,
         Destinations: Sequence[InputDestinationRequestTypeDef] = ...,
         InputDevices: Sequence[InputDeviceRequestTypeDef] = ...,
         InputSecurityGroups: Sequence[str] = ...,
@@ -789,209 +866,235 @@
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_input)
         """
+
     def update_input_device(
         self,
         *,
         InputDeviceId: str,
         HdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
         Name: str = ...,
         UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...
     ) -> UpdateInputDeviceResponseTypeDef:
         """
         Updates the parameters for the input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_input_device)
         """
+
     def update_input_security_group(
         self,
         *,
         InputSecurityGroupId: str,
         Tags: Mapping[str, str] = ...,
         WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...
     ) -> UpdateInputSecurityGroupResponseTypeDef:
         """
         Update an Input Security Group's Whilelists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_security_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_input_security_group)
         """
+
     def update_multiplex(
         self,
         *,
         MultiplexId: str,
         MultiplexSettings: MultiplexSettingsTypeDef = ...,
         Name: str = ...
     ) -> UpdateMultiplexResponseTypeDef:
         """
         Updates a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_multiplex)
         """
+
     def update_multiplex_program(
         self,
         *,
         MultiplexId: str,
         ProgramName: str,
         MultiplexProgramSettings: MultiplexProgramSettingsTypeDef = ...
     ) -> UpdateMultiplexProgramResponseTypeDef:
         """
         Update a program in a multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_multiplex_program)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_multiplex_program)
         """
+
     def update_reservation(
         self, *, ReservationId: str, Name: str = ..., RenewalSettings: RenewalSettingsTypeDef = ...
     ) -> UpdateReservationResponseTypeDef:
         """
         Update reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_reservation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_reservation)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_schedule"]
     ) -> DescribeSchedulePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_channels"]) -> ListChannelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_input_device_transfers"]
     ) -> ListInputDeviceTransfersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_input_devices"]
     ) -> ListInputDevicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_input_security_groups"]
     ) -> ListInputSecurityGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_inputs"]) -> ListInputsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_multiplex_programs"]
     ) -> ListMultiplexProgramsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_multiplexes"]
     ) -> ListMultiplexesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_offerings"]) -> ListOfferingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_reservations"]
     ) -> ListReservationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["channel_created"]) -> ChannelCreatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["channel_deleted"]) -> ChannelDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["channel_running"]) -> ChannelRunningWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["channel_stopped"]) -> ChannelStoppedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["input_attached"]) -> InputAttachedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["input_deleted"]) -> InputDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["input_detached"]) -> InputDetachedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["multiplex_created"]) -> MultiplexCreatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["multiplex_deleted"]) -> MultiplexDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["multiplex_running"]) -> MultiplexRunningWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["multiplex_stopped"]) -> MultiplexStoppedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/literals.py` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/literals.pyi` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/paginator.py` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/paginator.pyi` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/type_defs.py` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_medialive.type_defs import AacSettingsTypeDef
 
     data: AacSettingsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AacCodingModeType,
     AacInputTypeType,
     AacProfileType,
@@ -4916,15 +4916,15 @@
         "ChannelClass": ChannelClassType,
         "ChannelId": str,
     },
 )
 _OptionalUpdateChannelClassRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelClassRequestRequestTypeDef",
     {
-        "Destinations": Sequence[OutputDestinationTypeDef],
+        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
     },
     total=False,
 )
 
 
 class UpdateChannelClassRequestRequestTypeDef(
     _RequiredUpdateChannelClassRequestRequestTypeDef,
@@ -6088,17 +6088,17 @@
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": Sequence[OutputDestinationTypeDef],
+        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
         "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[InputAttachmentTypeDef],
+        "InputAttachments": Sequence[Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceCreateSettingsTypeDef,
         "Name": str,
         "RequestId": str,
         "Reserved": str,
         "RoleArn": str,
@@ -6114,17 +6114,17 @@
         "ChannelId": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
-        "Destinations": Sequence[OutputDestinationTypeDef],
+        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
         "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[InputAttachmentTypeDef],
+        "InputAttachments": Sequence[Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceUpdateSettingsTypeDef,
         "Name": str,
         "RoleArn": str,
     },
     total=False,
```

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/type_defs.pyi` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_medialive.type_defs import AacSettingsTypeDef
 
     data: AacSettingsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AacCodingModeType,
     AacInputTypeType,
     AacProfileType,
@@ -4791,15 +4791,15 @@
         "ChannelClass": ChannelClassType,
         "ChannelId": str,
     },
 )
 _OptionalUpdateChannelClassRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelClassRequestRequestTypeDef",
     {
-        "Destinations": Sequence[OutputDestinationTypeDef],
+        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
     },
     total=False,
 )
 
 class UpdateChannelClassRequestRequestTypeDef(
     _RequiredUpdateChannelClassRequestRequestTypeDef,
     _OptionalUpdateChannelClassRequestRequestTypeDef,
@@ -5915,17 +5915,17 @@
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": Sequence[OutputDestinationTypeDef],
+        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
         "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[InputAttachmentTypeDef],
+        "InputAttachments": Sequence[Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceCreateSettingsTypeDef,
         "Name": str,
         "RequestId": str,
         "Reserved": str,
         "RoleArn": str,
@@ -5941,17 +5941,17 @@
         "ChannelId": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
-        "Destinations": Sequence[OutputDestinationTypeDef],
+        "Destinations": Sequence[Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]],
         "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[InputAttachmentTypeDef],
+        "InputAttachments": Sequence[Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceUpdateSettingsTypeDef,
         "Name": str,
         "RoleArn": str,
     },
     total=False,
```

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/waiter.py` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive/waiter.pyi` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/PKG-INFO` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.28.15
-Summary: Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-medialive-1.28.15/mypy_boto3_medialive.egg-info/SOURCES.txt` & `mypy-boto3-medialive-1.28.15.post1/mypy_boto3_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.15/setup.py` & `mypy-boto3-medialive-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medialive",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.MediaLive 1.28.15 service generated with mypy-boto3-builder"
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

