# Comparing `tmp/mypy-boto3-application-autoscaling-1.28.15.tar.gz` & `tmp/mypy-boto3-application-autoscaling-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-application-autoscaling-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
+gzip compressed data, was "mypy-boto3-application-autoscaling-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:31 2023, max compression
```

## Comparing `mypy-boto3-application-autoscaling-1.28.15.tar` & `mypy-boto3-application-autoscaling-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.216654 mypy-boto3-application-autoscaling-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16405 2023-07-28 20:42:16.216654 mypy-boto3-application-autoscaling-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.212654 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26057 2023-07-28 20:19:25.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26008 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.216654 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16405 2023-07-28 20:42:15.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 20:42:16.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:15.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 20:42:15.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.216654 mypy-boto3-application-autoscaling-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.025007 mypy-boto3-application-autoscaling-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-07-29 10:02:31.021007 mypy-boto3-application-autoscaling-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.021007 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26057 2023-07-29 09:38:15.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26008 2023-07-29 09:38:15.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.021007 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 10:02:30.000000 mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:31.025007 mypy-boto3-application-autoscaling-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-29 09:38:14.000000 mypy-boto3-application-autoscaling-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15/LICENSE` & `mypy-boto3-application-autoscaling-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15/PKG-INFO` & `mypy-boto3-application-autoscaling-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.28.15
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15/README.md` & `mypy-boto3-application-autoscaling-1.28.15.post1/README.md`

 * *Files 1% similar despite different names*

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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__init__.py` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__init__.pyi` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__main__.py` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.ApplicationAutoScaling 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling\nOther"
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

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/client.py` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,49 +31,47 @@
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalableTargetActionTypeDef,
+    StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     SuspendedStateTypeDef,
+    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
     TargetTrackingScalingPolicyConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ApplicationAutoScalingClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConcurrentUpdateException: Type[BotocoreClientError]
     FailedResourceAccessException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ObjectNotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class ApplicationAutoScalingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/)
     """
 
     meta: ClientMeta
@@ -82,31 +80,28 @@
     def exceptions(self) -> Exceptions:
         """
         ApplicationAutoScalingClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#close)
         """
-
     def delete_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
@@ -114,15 +109,14 @@
         """
         Deletes the specified scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#delete_scaling_policy)
         """
-
     def delete_scheduled_action(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
@@ -130,30 +124,28 @@
         """
         Deletes the specified scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#delete_scheduled_action)
         """
-
     def deregister_scalable_target(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
     ) -> Dict[str, Any]:
         """
         Deregisters an Application Auto Scaling scalable target when you have finished
         using it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.deregister_scalable_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#deregister_scalable_target)
         """
-
     def describe_scalable_targets(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
@@ -161,15 +153,14 @@
     ) -> DescribeScalableTargetsResponseTypeDef:
         """
         Gets information about the scalable targets in the specified namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scalable_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scalable_targets)
         """
-
     def describe_scaling_activities(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
@@ -179,15 +170,14 @@
         """
         Provides descriptive information about the scaling activities in the specified
         namespace from the previous six weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_activities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scaling_activities)
         """
-
     def describe_scaling_policies(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
@@ -197,15 +187,14 @@
         """
         Describes the Application Auto Scaling scaling policies for the specified
         service namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scaling_policies)
         """
-
     def describe_scheduled_actions(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
@@ -215,56 +204,57 @@
         """
         Describes the Application Auto Scaling scheduled actions for the specified
         service namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scheduled_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scheduled_actions)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#generate_presigned_url)
         """
-
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns all the tags on the specified Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#list_tags_for_resource)
         """
-
     def put_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         PolicyType: PolicyTypeType = ...,
-        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationTypeDef = ...,
-        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...
+        StepScalingPolicyConfiguration: Union[
+            StepScalingPolicyConfigurationTypeDef, StepScalingPolicyConfigurationOutputTypeDef
+        ] = ...,
+        TargetTrackingScalingPolicyConfiguration: Union[
+            TargetTrackingScalingPolicyConfigurationTypeDef,
+            TargetTrackingScalingPolicyConfigurationOutputTypeDef,
+        ] = ...
     ) -> PutScalingPolicyResponseTypeDef:
         """
         Creates or updates a scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#put_scaling_policy)
         """
-
     def put_scheduled_action(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
@@ -277,15 +267,14 @@
         """
         Creates or updates a scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#put_scheduled_action)
         """
-
     def register_scalable_target(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         MinCapacity: int = ...,
@@ -297,58 +286,52 @@
         """
         Registers or updates a scalable target, which is the resource that you want to
         scale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.register_scalable_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#register_scalable_target)
         """
-
     def tag_resource(self, *, ResourceARN: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds or edits tags on an Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes tags from an Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#untag_resource)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scalable_targets"]
     ) -> DescribeScalableTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scaling_activities"]
     ) -> DescribeScalingActivitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scaling_policies"]
     ) -> DescribeScalingPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scheduled_actions"]
     ) -> DescribeScheduledActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/client.pyi` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,45 +31,51 @@
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalableTargetActionTypeDef,
+    StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     SuspendedStateTypeDef,
+    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
     TargetTrackingScalingPolicyConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ApplicationAutoScalingClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConcurrentUpdateException: Type[BotocoreClientError]
     FailedResourceAccessException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ObjectNotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class ApplicationAutoScalingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/)
     """
 
     meta: ClientMeta
@@ -78,28 +84,31 @@
     def exceptions(self) -> Exceptions:
         """
         ApplicationAutoScalingClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#close)
         """
+
     def delete_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
@@ -107,14 +116,15 @@
         """
         Deletes the specified scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#delete_scaling_policy)
         """
+
     def delete_scheduled_action(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
@@ -122,28 +132,30 @@
         """
         Deletes the specified scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.delete_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#delete_scheduled_action)
         """
+
     def deregister_scalable_target(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType
     ) -> Dict[str, Any]:
         """
         Deregisters an Application Auto Scaling scalable target when you have finished
         using it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.deregister_scalable_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#deregister_scalable_target)
         """
+
     def describe_scalable_targets(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
@@ -151,14 +163,15 @@
     ) -> DescribeScalableTargetsResponseTypeDef:
         """
         Gets information about the scalable targets in the specified namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scalable_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scalable_targets)
         """
+
     def describe_scaling_activities(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         MaxResults: int = ...,
@@ -168,14 +181,15 @@
         """
         Provides descriptive information about the scaling activities in the specified
         namespace from the previous six weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_activities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scaling_activities)
         """
+
     def describe_scaling_policies(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
@@ -185,14 +199,15 @@
         """
         Describes the Application Auto Scaling scaling policies for the specified
         service namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scaling_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scaling_policies)
         """
+
     def describe_scheduled_actions(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
@@ -202,52 +217,61 @@
         """
         Describes the Application Auto Scaling scheduled actions for the specified
         service namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.describe_scheduled_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#describe_scheduled_actions)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#generate_presigned_url)
         """
+
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns all the tags on the specified Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#list_tags_for_resource)
         """
+
     def put_scaling_policy(
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         PolicyType: PolicyTypeType = ...,
-        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationTypeDef = ...,
-        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...
+        StepScalingPolicyConfiguration: Union[
+            StepScalingPolicyConfigurationTypeDef, StepScalingPolicyConfigurationOutputTypeDef
+        ] = ...,
+        TargetTrackingScalingPolicyConfiguration: Union[
+            TargetTrackingScalingPolicyConfigurationTypeDef,
+            TargetTrackingScalingPolicyConfigurationOutputTypeDef,
+        ] = ...
     ) -> PutScalingPolicyResponseTypeDef:
         """
         Creates or updates a scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#put_scaling_policy)
         """
+
     def put_scheduled_action(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
@@ -260,14 +284,15 @@
         """
         Creates or updates a scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#put_scheduled_action)
         """
+
     def register_scalable_target(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         MinCapacity: int = ...,
@@ -279,52 +304,58 @@
         """
         Registers or updates a scalable target, which is the resource that you want to
         scale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.register_scalable_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#register_scalable_target)
         """
+
     def tag_resource(self, *, ResourceARN: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds or edits tags on an Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes tags from an Application Auto Scaling scalable target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#untag_resource)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scalable_targets"]
     ) -> DescribeScalableTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scaling_activities"]
     ) -> DescribeScalingActivitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scaling_policies"]
     ) -> DescribeScalingPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scheduled_actions"]
     ) -> DescribeScheduledActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/client/#get_paginator)
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/literals.py` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/literals.pyi` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/paginator.py` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/paginator.pyi` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/type_defs.py` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/type_defs.pyi` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.28.15
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-application-autoscaling-1.28.15.post1/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.15/setup.py` & `mypy-boto3-application-autoscaling-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-application-autoscaling",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_application_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with"
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

