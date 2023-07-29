# Comparing `tmp/mypy-boto3-batch-1.28.15.tar.gz` & `tmp/mypy-boto3-batch-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-batch-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
+gzip compressed data, was "mypy-boto3-batch-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:37 2023, max compression
```

## Comparing `mypy-boto3-batch-1.28.15.tar` & `mypy-boto3-batch-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.232736 mypy-boto3-batch-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-07-28 20:42:22.224736 mypy-boto3-batch-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.212736 mypy-boto3-batch-1.28.15/mypy_boto3_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20489 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51341 2023-07-28 20:20:12.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51272 2023-07-28 20:20:11.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.224736 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-07-28 20:42:21.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:42:22.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:21.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:21.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:21.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:42:21.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.232736 mypy-boto3-batch-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.201032 mypy-boto3-batch-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-07-29 10:02:37.197032 mypy-boto3-batch-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.181032 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21074 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51341 2023-07-29 09:39:04.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51272 2023-07-29 09:39:03.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.197032 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:37.201032 mypy-boto3-batch-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-batch-1.28.15/LICENSE` & `mypy-boto3-batch-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15/PKG-INFO` & `mypy-boto3-batch-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.28.15
-Summary: Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-batch-1.28.15/README.md` & `mypy-boto3-batch-1.28.15.post1/README.md`

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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/__init__.py` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/__init__.pyi` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/__main__.py` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Batch 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Batch 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\nOther"
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

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/client.py` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_batch.client import BatchClient
 
     session = Session()
     client: BatchClient = session.client("batch")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CEStateType,
     CETypeType,
     JobDefinitionTypeType,
@@ -32,69 +32,71 @@
     DescribeJobQueuesPaginator,
     ListJobsPaginator,
     ListSchedulingPoliciesPaginator,
 )
 from .type_defs import (
     ArrayPropertiesTypeDef,
     ComputeEnvironmentOrderTypeDef,
+    ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
+    ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobQueuesResponseTypeDef,
     DescribeJobsResponseTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     EksConfigurationTypeDef,
+    EksPropertiesOutputTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesTypeDef,
+    FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobDependencyTypeDef,
     JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     ListJobsResponseTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NodeOverridesTypeDef,
+    NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     RegisterJobDefinitionResponseTypeDef,
+    RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
     SubmitJobResponseTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     UpdatePolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BatchClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ClientException: Type[BotocoreClientError]
     ServerException: Type[BotocoreClientError]
 
-
 class BatchClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/)
     """
 
     meta: ClientMeta
@@ -103,58 +105,53 @@
     def exceptions(self) -> Exceptions:
         """
         BatchClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#can_paginate)
         """
-
     def cancel_job(self, *, jobId: str, reason: str) -> Dict[str, Any]:
         """
         Cancels a job in an Batch job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.cancel_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#cancel_job)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#close)
         """
-
     def create_compute_environment(
         self,
         *,
         computeEnvironmentName: str,
         type: CETypeType,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
-        computeResources: ComputeResourceTypeDef = ...,
+        computeResources: Union[ComputeResourceTypeDef, ComputeResourceOutputTypeDef] = ...,
         serviceRole: str = ...,
         tags: Mapping[str, str] = ...,
         eksConfiguration: EksConfigurationTypeDef = ...
     ) -> CreateComputeEnvironmentResponseTypeDef:
         """
         Creates an Batch compute environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_compute_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#create_compute_environment)
         """
-
     def create_job_queue(
         self,
         *,
         jobQueueName: str,
         priority: int,
         computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef],
         state: JQStateType = ...,
@@ -163,75 +160,68 @@
     ) -> CreateJobQueueResponseTypeDef:
         """
         Creates an Batch job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_job_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#create_job_queue)
         """
-
     def create_scheduling_policy(
         self,
         *,
         name: str,
-        fairsharePolicy: FairsharePolicyTypeDef = ...,
+        fairsharePolicy: Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSchedulingPolicyResponseTypeDef:
         """
         Creates an Batch scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#create_scheduling_policy)
         """
-
     def delete_compute_environment(self, *, computeEnvironment: str) -> Dict[str, Any]:
         """
         Deletes an Batch compute environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.delete_compute_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#delete_compute_environment)
         """
-
     def delete_job_queue(self, *, jobQueue: str) -> Dict[str, Any]:
         """
         Deletes the specified job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.delete_job_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#delete_job_queue)
         """
-
     def delete_scheduling_policy(self, *, arn: str) -> Dict[str, Any]:
         """
         Deletes the specified scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.delete_scheduling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#delete_scheduling_policy)
         """
-
     def deregister_job_definition(self, *, jobDefinition: str) -> Dict[str, Any]:
         """
         Deregisters an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.deregister_job_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#deregister_job_definition)
         """
-
     def describe_compute_environments(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeComputeEnvironmentsResponseTypeDef:
         """
         Describes one or more of your compute environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_compute_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#describe_compute_environments)
         """
-
     def describe_job_definitions(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         maxResults: int = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
@@ -239,57 +229,52 @@
     ) -> DescribeJobDefinitionsResponseTypeDef:
         """
         Describes a list of job definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_job_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#describe_job_definitions)
         """
-
     def describe_job_queues(
         self, *, jobQueues: Sequence[str] = ..., maxResults: int = ..., nextToken: str = ...
     ) -> DescribeJobQueuesResponseTypeDef:
         """
         Describes one or more of your job queues.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_job_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#describe_job_queues)
         """
-
     def describe_jobs(self, *, jobs: Sequence[str]) -> DescribeJobsResponseTypeDef:
         """
         Describes a list of Batch jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#describe_jobs)
         """
-
     def describe_scheduling_policies(
         self, *, arns: Sequence[str]
     ) -> DescribeSchedulingPoliciesResponseTypeDef:
         """
         Describes one or more of your scheduling policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_scheduling_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#describe_scheduling_policies)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#generate_presigned_url)
         """
-
     def list_jobs(
         self,
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
@@ -299,106 +284,100 @@
     ) -> ListJobsResponseTypeDef:
         """
         Returns a list of Batch jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#list_jobs)
         """
-
     def list_scheduling_policies(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListSchedulingPoliciesResponseTypeDef:
         """
         Returns a list of Batch scheduling policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_scheduling_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#list_scheduling_policies)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for an Batch resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#list_tags_for_resource)
         """
-
     def register_job_definition(
         self,
         *,
         jobDefinitionName: str,
         type: JobDefinitionTypeType,
         parameters: Mapping[str, str] = ...,
         schedulingPriority: int = ...,
-        containerProperties: ContainerPropertiesTypeDef = ...,
-        nodeProperties: NodePropertiesTypeDef = ...,
-        retryStrategy: RetryStrategyTypeDef = ...,
+        containerProperties: Union[
+            ContainerPropertiesTypeDef, ContainerPropertiesOutputTypeDef
+        ] = ...,
+        nodeProperties: Union[NodePropertiesTypeDef, NodePropertiesOutputTypeDef] = ...,
+        retryStrategy: Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef] = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         platformCapabilities: Sequence[PlatformCapabilityType] = ...,
-        eksProperties: EksPropertiesTypeDef = ...
+        eksProperties: Union[EksPropertiesTypeDef, EksPropertiesOutputTypeDef] = ...
     ) -> RegisterJobDefinitionResponseTypeDef:
         """
         Registers an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#register_job_definition)
         """
-
     def submit_job(
         self,
         *,
         jobName: str,
         jobQueue: str,
         jobDefinition: str,
         shareIdentifier: str = ...,
         schedulingPriorityOverride: int = ...,
         arrayProperties: ArrayPropertiesTypeDef = ...,
         dependsOn: Sequence[JobDependencyTypeDef] = ...,
         parameters: Mapping[str, str] = ...,
         containerOverrides: ContainerOverridesTypeDef = ...,
         nodeOverrides: NodeOverridesTypeDef = ...,
-        retryStrategy: RetryStrategyTypeDef = ...,
+        retryStrategy: Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef] = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...
     ) -> SubmitJobResponseTypeDef:
         """
         Submits an Batch job from a job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.submit_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#submit_job)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Associates the specified tags to a resource with the specified `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#tag_resource)
         """
-
     def terminate_job(self, *, jobId: str, reason: str) -> Dict[str, Any]:
         """
         Terminates a job in a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.terminate_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#terminate_job)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes specified tags from an Batch resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#untag_resource)
         """
-
     def update_compute_environment(
         self,
         *,
         computeEnvironment: str,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
         computeResources: ComputeResourceUpdateTypeDef = ...,
@@ -407,15 +386,14 @@
     ) -> UpdateComputeEnvironmentResponseTypeDef:
         """
         Updates an Batch compute environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_compute_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#update_compute_environment)
         """
-
     def update_job_queue(
         self,
         *,
         jobQueue: str,
         state: JQStateType = ...,
         schedulingPolicyArn: str = ...,
         priority: int = ...,
@@ -423,59 +401,56 @@
     ) -> UpdateJobQueueResponseTypeDef:
         """
         Updates a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#update_job_queue)
         """
-
     def update_scheduling_policy(
-        self, *, arn: str, fairsharePolicy: FairsharePolicyTypeDef = ...
+        self,
+        *,
+        arn: str,
+        fairsharePolicy: Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates a scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_scheduling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#update_scheduling_policy)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_compute_environments"]
     ) -> DescribeComputeEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_job_definitions"]
     ) -> DescribeJobDefinitionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_job_queues"]
     ) -> DescribeJobQueuesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_jobs"]) -> ListJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_scheduling_policies"]
     ) -> ListSchedulingPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#get_paginator)
```

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/client.pyi` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_batch.client import BatchClient
 
     session = Session()
     client: BatchClient = session.client("batch")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CEStateType,
     CETypeType,
     JobDefinitionTypeType,
@@ -32,65 +32,75 @@
     DescribeJobQueuesPaginator,
     ListJobsPaginator,
     ListSchedulingPoliciesPaginator,
 )
 from .type_defs import (
     ArrayPropertiesTypeDef,
     ComputeEnvironmentOrderTypeDef,
+    ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
+    ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobQueuesResponseTypeDef,
     DescribeJobsResponseTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     EksConfigurationTypeDef,
+    EksPropertiesOutputTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesTypeDef,
+    FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobDependencyTypeDef,
     JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     ListJobsResponseTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NodeOverridesTypeDef,
+    NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     RegisterJobDefinitionResponseTypeDef,
+    RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
     SubmitJobResponseTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     UpdatePolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("BatchClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ClientException: Type[BotocoreClientError]
     ServerException: Type[BotocoreClientError]
 
+
 class BatchClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/)
     """
 
     meta: ClientMeta
@@ -99,53 +109,58 @@
     def exceptions(self) -> Exceptions:
         """
         BatchClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#can_paginate)
         """
+
     def cancel_job(self, *, jobId: str, reason: str) -> Dict[str, Any]:
         """
         Cancels a job in an Batch job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.cancel_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#cancel_job)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#close)
         """
+
     def create_compute_environment(
         self,
         *,
         computeEnvironmentName: str,
         type: CETypeType,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
-        computeResources: ComputeResourceTypeDef = ...,
+        computeResources: Union[ComputeResourceTypeDef, ComputeResourceOutputTypeDef] = ...,
         serviceRole: str = ...,
         tags: Mapping[str, str] = ...,
         eksConfiguration: EksConfigurationTypeDef = ...
     ) -> CreateComputeEnvironmentResponseTypeDef:
         """
         Creates an Batch compute environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_compute_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#create_compute_environment)
         """
+
     def create_job_queue(
         self,
         *,
         jobQueueName: str,
         priority: int,
         computeEnvironmentOrder: Sequence[ComputeEnvironmentOrderTypeDef],
         state: JQStateType = ...,
@@ -154,68 +169,75 @@
     ) -> CreateJobQueueResponseTypeDef:
         """
         Creates an Batch job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_job_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#create_job_queue)
         """
+
     def create_scheduling_policy(
         self,
         *,
         name: str,
-        fairsharePolicy: FairsharePolicyTypeDef = ...,
+        fairsharePolicy: Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSchedulingPolicyResponseTypeDef:
         """
         Creates an Batch scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#create_scheduling_policy)
         """
+
     def delete_compute_environment(self, *, computeEnvironment: str) -> Dict[str, Any]:
         """
         Deletes an Batch compute environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.delete_compute_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#delete_compute_environment)
         """
+
     def delete_job_queue(self, *, jobQueue: str) -> Dict[str, Any]:
         """
         Deletes the specified job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.delete_job_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#delete_job_queue)
         """
+
     def delete_scheduling_policy(self, *, arn: str) -> Dict[str, Any]:
         """
         Deletes the specified scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.delete_scheduling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#delete_scheduling_policy)
         """
+
     def deregister_job_definition(self, *, jobDefinition: str) -> Dict[str, Any]:
         """
         Deregisters an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.deregister_job_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#deregister_job_definition)
         """
+
     def describe_compute_environments(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeComputeEnvironmentsResponseTypeDef:
         """
         Describes one or more of your compute environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_compute_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#describe_compute_environments)
         """
+
     def describe_job_definitions(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         maxResults: int = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
@@ -223,52 +245,57 @@
     ) -> DescribeJobDefinitionsResponseTypeDef:
         """
         Describes a list of job definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_job_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#describe_job_definitions)
         """
+
     def describe_job_queues(
         self, *, jobQueues: Sequence[str] = ..., maxResults: int = ..., nextToken: str = ...
     ) -> DescribeJobQueuesResponseTypeDef:
         """
         Describes one or more of your job queues.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_job_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#describe_job_queues)
         """
+
     def describe_jobs(self, *, jobs: Sequence[str]) -> DescribeJobsResponseTypeDef:
         """
         Describes a list of Batch jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#describe_jobs)
         """
+
     def describe_scheduling_policies(
         self, *, arns: Sequence[str]
     ) -> DescribeSchedulingPoliciesResponseTypeDef:
         """
         Describes one or more of your scheduling policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_scheduling_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#describe_scheduling_policies)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#generate_presigned_url)
         """
+
     def list_jobs(
         self,
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
@@ -278,98 +305,108 @@
     ) -> ListJobsResponseTypeDef:
         """
         Returns a list of Batch jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#list_jobs)
         """
+
     def list_scheduling_policies(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListSchedulingPoliciesResponseTypeDef:
         """
         Returns a list of Batch scheduling policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_scheduling_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#list_scheduling_policies)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for an Batch resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#list_tags_for_resource)
         """
+
     def register_job_definition(
         self,
         *,
         jobDefinitionName: str,
         type: JobDefinitionTypeType,
         parameters: Mapping[str, str] = ...,
         schedulingPriority: int = ...,
-        containerProperties: ContainerPropertiesTypeDef = ...,
-        nodeProperties: NodePropertiesTypeDef = ...,
-        retryStrategy: RetryStrategyTypeDef = ...,
+        containerProperties: Union[
+            ContainerPropertiesTypeDef, ContainerPropertiesOutputTypeDef
+        ] = ...,
+        nodeProperties: Union[NodePropertiesTypeDef, NodePropertiesOutputTypeDef] = ...,
+        retryStrategy: Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef] = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         platformCapabilities: Sequence[PlatformCapabilityType] = ...,
-        eksProperties: EksPropertiesTypeDef = ...
+        eksProperties: Union[EksPropertiesTypeDef, EksPropertiesOutputTypeDef] = ...
     ) -> RegisterJobDefinitionResponseTypeDef:
         """
         Registers an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#register_job_definition)
         """
+
     def submit_job(
         self,
         *,
         jobName: str,
         jobQueue: str,
         jobDefinition: str,
         shareIdentifier: str = ...,
         schedulingPriorityOverride: int = ...,
         arrayProperties: ArrayPropertiesTypeDef = ...,
         dependsOn: Sequence[JobDependencyTypeDef] = ...,
         parameters: Mapping[str, str] = ...,
         containerOverrides: ContainerOverridesTypeDef = ...,
         nodeOverrides: NodeOverridesTypeDef = ...,
-        retryStrategy: RetryStrategyTypeDef = ...,
+        retryStrategy: Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef] = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...
     ) -> SubmitJobResponseTypeDef:
         """
         Submits an Batch job from a job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.submit_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#submit_job)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Associates the specified tags to a resource with the specified `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#tag_resource)
         """
+
     def terminate_job(self, *, jobId: str, reason: str) -> Dict[str, Any]:
         """
         Terminates a job in a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.terminate_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#terminate_job)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes specified tags from an Batch resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#untag_resource)
         """
+
     def update_compute_environment(
         self,
         *,
         computeEnvironment: str,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
         computeResources: ComputeResourceUpdateTypeDef = ...,
@@ -378,14 +415,15 @@
     ) -> UpdateComputeEnvironmentResponseTypeDef:
         """
         Updates an Batch compute environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_compute_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#update_compute_environment)
         """
+
     def update_job_queue(
         self,
         *,
         jobQueue: str,
         state: JQStateType = ...,
         schedulingPolicyArn: str = ...,
         priority: int = ...,
@@ -393,53 +431,62 @@
     ) -> UpdateJobQueueResponseTypeDef:
         """
         Updates a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#update_job_queue)
         """
+
     def update_scheduling_policy(
-        self, *, arn: str, fairsharePolicy: FairsharePolicyTypeDef = ...
+        self,
+        *,
+        arn: str,
+        fairsharePolicy: Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates a scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_scheduling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#update_scheduling_policy)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_compute_environments"]
     ) -> DescribeComputeEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_job_definitions"]
     ) -> DescribeJobDefinitionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_job_queues"]
     ) -> DescribeJobQueuesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_jobs"]) -> ListJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_scheduling_policies"]
     ) -> ListSchedulingPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#get_paginator)
```

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/literals.py` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/literals.pyi` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/paginator.py` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/paginator.pyi` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/type_defs.py` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch/type_defs.pyi` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/PKG-INFO` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.28.15
-Summary: Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/SOURCES.txt` & `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15/setup.py` & `mypy-boto3-batch-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-batch",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

