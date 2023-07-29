# Comparing `tmp/mypy-boto3-sqs-1.28.15.tar.gz` & `tmp/mypy-boto3-sqs-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sqs-1.28.15.tar", last modified: Fri Jul 28 20:43:47 2023, max compression
+gzip compressed data, was "mypy-boto3-sqs-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:15 2023, max compression
```

## Comparing `mypy-boto3-sqs-1.28.15.tar` & `mypy-boto3-sqs-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:47.873921 mypy-boto3-sqs-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-07-28 20:43:47.873921 mypy-boto3-sqs-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:47.865921 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18084 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18052 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19031 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    18992 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-07-28 20:39:48.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-07-28 20:39:48.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:47.873921 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-07-28 20:43:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-28 20:43:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:47.000000 mypy-boto3-sqs-1.28.15/mypy_boto3_sqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:47.873921 mypy-boto3-sqs-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:39:46.000000 mypy-boto3-sqs-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.945419 mypy-boto3-sqs-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-07-29 10:04:15.945419 mypy-boto3-sqs-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.945419 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18164 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19031 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18992 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25272 2023-07-29 09:59:59.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25233 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.945419 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:15.945419 mypy-boto3-sqs-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-sqs-1.28.15/LICENSE` & `mypy-boto3-sqs-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15/PKG-INFO` & `mypy-boto3-sqs-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.28.15
-Summary: Type annotations for boto3.SQS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SQS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
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
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sqs-1.28.15/README.md` & `mypy-boto3-sqs-1.28.15.post1/README.md`

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
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/__init__.py` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/__init__.pyi` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/__main__.py` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SQS 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.SQS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\nOther"
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

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/client.py` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_sqs.client import SQSClient
 
     session = Session()
     client: SQSClient = session.client("sqs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import QueueAttributeFilterType, QueueAttributeNameType
 from .paginator import ListDeadLetterSourceQueuesPaginator, ListQueuesPaginator
 from .type_defs import (
     CancelMessageMoveTaskResultTypeDef,
@@ -30,14 +30,15 @@
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksResultTypeDef,
     ListQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
+    MessageAttributeValueOutputTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
     StartMessageMoveTaskResultTypeDef,
@@ -306,15 +307,17 @@
 
     def send_message(
         self,
         *,
         QueueUrl: str,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
+        MessageAttributes: Mapping[
+            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
+        ] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> SendMessageResultTypeDef:
         """
```

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/client.pyi` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_sqs.client import SQSClient
 
     session = Session()
     client: SQSClient = session.client("sqs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import QueueAttributeFilterType, QueueAttributeNameType
 from .paginator import ListDeadLetterSourceQueuesPaginator, ListQueuesPaginator
 from .type_defs import (
     CancelMessageMoveTaskResultTypeDef,
@@ -30,14 +30,15 @@
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksResultTypeDef,
     ListQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
+    MessageAttributeValueOutputTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
     StartMessageMoveTaskResultTypeDef,
@@ -281,15 +282,17 @@
         """
     def send_message(
         self,
         *,
         QueueUrl: str,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
+        MessageAttributes: Mapping[
+            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
+        ] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> SendMessageResultTypeDef:
         """
```

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/literals.py` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/literals.pyi` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/paginator.py` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/paginator.pyi` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/service_resource.py` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/service_resource.pyi` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/type_defs.py` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -895,15 +895,17 @@
         "MessageBody": str,
     },
 )
 _OptionalSendMessageRequestRequestTypeDef = TypedDict(
     "_OptionalSendMessageRequestRequestTypeDef",
     {
         "DelaySeconds": int,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Mapping[
+            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
+        ],
         "MessageSystemAttributes": Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
```

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs/type_defs.pyi` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -858,15 +858,17 @@
         "MessageBody": str,
     },
 )
 _OptionalSendMessageRequestRequestTypeDef = TypedDict(
     "_OptionalSendMessageRequestRequestTypeDef",
     {
         "DelaySeconds": int,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Mapping[
+            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
+        ],
         "MessageSystemAttributes": Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
```

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs.egg-info/PKG-INFO` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.28.15
-Summary: Type annotations for boto3.SQS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SQS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
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
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sqs-1.28.15/mypy_boto3_sqs.egg-info/SOURCES.txt` & `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15/setup.py` & `mypy-boto3-sqs-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sqs",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_sqs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SQS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.SQS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

