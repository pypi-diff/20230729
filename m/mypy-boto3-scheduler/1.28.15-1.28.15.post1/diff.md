# Comparing `tmp/mypy-boto3-scheduler-1.28.15.tar.gz` & `tmp/mypy-boto3-scheduler-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-scheduler-1.28.15.tar", last modified: Fri Jul 28 20:43:41 2023, max compression
+gzip compressed data, was "mypy-boto3-scheduler-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:08 2023, max compression
```

## Comparing `mypy-boto3-scheduler-1.28.15.tar` & `mypy-boto3-scheduler-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:41.353831 mypy-boto3-scheduler-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-07-28 20:43:41.349831 mypy-boto3-scheduler-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:41.345831 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18384 2023-07-28 20:38:35.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:41.349831 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-07-28 20:43:41.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:41.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:41.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:41.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:41.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:41.000000 mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:41.353831 mypy-boto3-scheduler-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-28 20:38:34.000000 mypy-boto3-scheduler-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:08.437389 mypy-boto3-scheduler-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-07-29 10:04:08.437389 mypy-boto3-scheduler-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:08.437389 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-29 09:58:43.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-29 09:58:43.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18384 2023-07-29 09:58:43.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-07-29 09:58:43.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:08.437389 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:04:08.000000 mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:08.437389 mypy-boto3-scheduler-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-29 09:58:42.000000 mypy-boto3-scheduler-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-scheduler-1.28.15/LICENSE` & `mypy-boto3-scheduler-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15/PKG-INFO` & `mypy-boto3-scheduler-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-scheduler
-Version: 1.28.15
-Summary: Type annotations for boto3.EventBridgeScheduler 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EventBridgeScheduler 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-scheduler-1.28.15/README.md` & `mypy-boto3-scheduler-1.28.15.post1/README.md`

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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/__init__.py` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/__init__.pyi` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/__main__.py` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgeScheduler 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.EventBridgeScheduler 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler\nOther"
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

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/client.py` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,45 +27,42 @@
     FlexibleTimeWindowTypeDef,
     GetScheduleGroupOutputTypeDef,
     GetScheduleOutputTypeDef,
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
     UpdateScheduleOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EventBridgeSchedulerClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class EventBridgeSchedulerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/)
     """
 
     meta: ClientMeta
@@ -74,38 +71,35 @@
     def exceptions(self) -> Exceptions:
         """
         EventBridgeSchedulerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#close)
         """
-
     def create_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: TargetTypeDef,
+        Target: Union[TargetTypeDef, TargetOutputTypeDef],
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: Union[datetime, str] = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
@@ -113,83 +107,75 @@
     ) -> CreateScheduleOutputTypeDef:
         """
         Creates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.create_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#create_schedule)
         """
-
     def create_schedule_group(
         self, *, Name: str, ClientToken: str = ..., Tags: Sequence[TagTypeDef] = ...
     ) -> CreateScheduleGroupOutputTypeDef:
         """
         Creates the specified schedule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.create_schedule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#create_schedule_group)
         """
-
     def delete_schedule(
         self, *, Name: str, ClientToken: str = ..., GroupName: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.delete_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#delete_schedule)
         """
-
     def delete_schedule_group(self, *, Name: str, ClientToken: str = ...) -> Dict[str, Any]:
         """
         Deletes the specified schedule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.delete_schedule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#delete_schedule_group)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#generate_presigned_url)
         """
-
     def get_schedule(self, *, Name: str, GroupName: str = ...) -> GetScheduleOutputTypeDef:
         """
         Retrieves the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.get_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#get_schedule)
         """
-
     def get_schedule_group(self, *, Name: str) -> GetScheduleGroupOutputTypeDef:
         """
         Retrieves the specified schedule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.get_schedule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#get_schedule_group)
         """
-
     def list_schedule_groups(
         self, *, MaxResults: int = ..., NamePrefix: str = ..., NextToken: str = ...
     ) -> ListScheduleGroupsOutputTypeDef:
         """
         Returns a paginated list of your schedule groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.list_schedule_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#list_schedule_groups)
         """
-
     def list_schedules(
         self,
         *,
         GroupName: str = ...,
         MaxResults: int = ...,
         NamePrefix: str = ...,
         NextToken: str = ...,
@@ -197,48 +183,44 @@
     ) -> ListSchedulesOutputTypeDef:
         """
         Returns a paginated list of your EventBridge Scheduler schedules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.list_schedules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#list_schedules)
         """
-
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceOutputTypeDef:
         """
         Lists the tags associated with the Scheduler resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#list_tags_for_resource)
         """
-
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Assigns one or more tags (key-value pairs) to the specified EventBridge
         Scheduler resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from the specified EventBridge Scheduler schedule
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#untag_resource)
         """
-
     def update_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: TargetTypeDef,
+        Target: Union[TargetTypeDef, TargetOutputTypeDef],
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: Union[datetime, str] = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
@@ -246,23 +228,21 @@
     ) -> UpdateScheduleOutputTypeDef:
         """
         Updates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.update_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#update_schedule)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_schedule_groups"]
     ) -> ListScheduleGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_schedules"]) -> ListSchedulesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/client.pyi` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,41 +27,46 @@
     FlexibleTimeWindowTypeDef,
     GetScheduleGroupOutputTypeDef,
     GetScheduleOutputTypeDef,
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
     UpdateScheduleOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("EventBridgeSchedulerClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class EventBridgeSchedulerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/)
     """
 
     meta: ClientMeta
@@ -70,35 +75,38 @@
     def exceptions(self) -> Exceptions:
         """
         EventBridgeSchedulerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#close)
         """
+
     def create_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: TargetTypeDef,
+        Target: Union[TargetTypeDef, TargetOutputTypeDef],
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: Union[datetime, str] = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
@@ -106,75 +114,83 @@
     ) -> CreateScheduleOutputTypeDef:
         """
         Creates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.create_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#create_schedule)
         """
+
     def create_schedule_group(
         self, *, Name: str, ClientToken: str = ..., Tags: Sequence[TagTypeDef] = ...
     ) -> CreateScheduleGroupOutputTypeDef:
         """
         Creates the specified schedule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.create_schedule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#create_schedule_group)
         """
+
     def delete_schedule(
         self, *, Name: str, ClientToken: str = ..., GroupName: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.delete_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#delete_schedule)
         """
+
     def delete_schedule_group(self, *, Name: str, ClientToken: str = ...) -> Dict[str, Any]:
         """
         Deletes the specified schedule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.delete_schedule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#delete_schedule_group)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#generate_presigned_url)
         """
+
     def get_schedule(self, *, Name: str, GroupName: str = ...) -> GetScheduleOutputTypeDef:
         """
         Retrieves the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.get_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#get_schedule)
         """
+
     def get_schedule_group(self, *, Name: str) -> GetScheduleGroupOutputTypeDef:
         """
         Retrieves the specified schedule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.get_schedule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#get_schedule_group)
         """
+
     def list_schedule_groups(
         self, *, MaxResults: int = ..., NamePrefix: str = ..., NextToken: str = ...
     ) -> ListScheduleGroupsOutputTypeDef:
         """
         Returns a paginated list of your schedule groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.list_schedule_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#list_schedule_groups)
         """
+
     def list_schedules(
         self,
         *,
         GroupName: str = ...,
         MaxResults: int = ...,
         NamePrefix: str = ...,
         NextToken: str = ...,
@@ -182,44 +198,48 @@
     ) -> ListSchedulesOutputTypeDef:
         """
         Returns a paginated list of your EventBridge Scheduler schedules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.list_schedules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#list_schedules)
         """
+
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceOutputTypeDef:
         """
         Lists the tags associated with the Scheduler resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#list_tags_for_resource)
         """
+
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Assigns one or more tags (key-value pairs) to the specified EventBridge
         Scheduler resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from the specified EventBridge Scheduler schedule
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#untag_resource)
         """
+
     def update_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: TargetTypeDef,
+        Target: Union[TargetTypeDef, TargetOutputTypeDef],
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: Union[datetime, str] = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: Union[datetime, str] = ...,
@@ -227,21 +247,23 @@
     ) -> UpdateScheduleOutputTypeDef:
         """
         Updates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.update_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#update_schedule)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_schedule_groups"]
     ) -> ListScheduleGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_schedules"]) -> ListSchedulesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/literals.py` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/literals.pyi` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/paginator.py` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/paginator.pyi` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/type_defs.py` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler/type_defs.pyi` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler.egg-info/PKG-INFO` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-scheduler
-Version: 1.28.15
-Summary: Type annotations for boto3.EventBridgeScheduler 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EventBridgeScheduler 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-scheduler-1.28.15/mypy_boto3_scheduler.egg-info/SOURCES.txt` & `mypy-boto3-scheduler-1.28.15.post1/mypy_boto3_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.15/setup.py` & `mypy-boto3-scheduler-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-scheduler",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_scheduler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.EventBridgeScheduler 1.28.15 service generated with"
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

