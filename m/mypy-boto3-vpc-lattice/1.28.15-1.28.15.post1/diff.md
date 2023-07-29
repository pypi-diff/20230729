# Comparing `tmp/mypy-boto3-vpc-lattice-1.28.15.tar.gz` & `tmp/mypy-boto3-vpc-lattice-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-vpc-lattice-1.28.15.tar", last modified: Fri Jul 28 20:43:55 2023, max compression
+gzip compressed data, was "mypy-boto3-vpc-lattice-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:23 2023, max compression
```

## Comparing `mypy-boto3-vpc-lattice-1.28.15.tar` & `mypy-boto3-vpc-lattice-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.298023 mypy-boto3-vpc-lattice-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-07-28 20:43:55.298023 mypy-boto3-vpc-lattice-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18820 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.290022 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38846 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49473 2023-07-28 20:41:03.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-07-28 20:41:02.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.298023 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:55.298023 mypy-boto3-vpc-lattice-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-28 20:41:00.000000 mypy-boto3-vpc-lattice-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.849449 mypy-boto3-vpc-lattice-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20328 2023-07-29 10:04:23.845449 mypy-boto3-vpc-lattice-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18820 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.837449 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39132 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39064 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-07-29 10:01:10.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-29 10:01:10.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49473 2023-07-29 10:01:11.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-07-29 10:01:10.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.845449 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20328 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:04:23.000000 mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:23.849449 mypy-boto3-vpc-lattice-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-29 10:01:09.000000 mypy-boto3-vpc-lattice-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15/LICENSE` & `mypy-boto3-vpc-lattice-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15/PKG-INFO` & `mypy-boto3-vpc-lattice-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.28.15
-Summary: Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15/README.md` & `mypy-boto3-vpc-lattice-1.28.15.post1/README.md`

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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__init__.py` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__init__.pyi` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__main__.py` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VPCLattice 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.VPCLattice 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice\nOther"
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

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/client.py` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_vpc_lattice.client import VPCLatticeClient
 
     session = Session()
     client: VPCLatticeClient = session.client("vpc-lattice")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AuthTypeType, ListenerProtocolType, TargetGroupTypeType
 from .paginator import (
     ListAccessLogSubscriptionsPaginator,
     ListListenersPaginator,
@@ -64,15 +64,17 @@
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PutAuthPolicyResponseTypeDef,
     RegisterTargetsResponseTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
+    RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
     RuleUpdateTypeDef,
     TargetGroupConfigTypeDef,
     TargetTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateListenerResponseTypeDef,
     UpdateRuleResponseTypeDef,
@@ -83,37 +85,33 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("VPCLatticeClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class VPCLatticeClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/)
     """
 
     meta: ClientMeta
@@ -122,41 +120,37 @@
     def exceptions(self) -> Exceptions:
         """
         VPCLatticeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#exceptions)
         """
-
     def batch_update_rule(
         self, *, listenerIdentifier: str, rules: Sequence[RuleUpdateTypeDef], serviceIdentifier: str
     ) -> BatchUpdateRuleResponseTypeDef:
         """
         Updates the listener rules in a batch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.batch_update_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#batch_update_rule)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#close)
         """
-
     def create_access_log_subscription(
         self,
         *,
         destinationArn: str,
         resourceIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
@@ -164,52 +158,49 @@
         """
         Enables access logs to be sent to Amazon CloudWatch, Amazon S3, and Amazon
         Kinesis Data Firehose.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_access_log_subscription)
         """
-
     def create_listener(
         self,
         *,
-        defaultAction: RuleActionTypeDef,
+        defaultAction: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateListenerResponseTypeDef:
         """
         Creates a listener for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_listener)
         """
-
     def create_rule(
         self,
         *,
-        action: RuleActionTypeDef,
+        action: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
         listenerIdentifier: str,
-        match: RuleMatchTypeDef,
+        match: Union[RuleMatchTypeDef, RuleMatchOutputTypeDef],
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a listener rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_rule)
         """
-
     def create_service(
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         certificateArn: str = ...,
         clientToken: str = ...,
@@ -218,45 +209,42 @@
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service)
         """
-
     def create_service_network(
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateServiceNetworkResponseTypeDef:
         """
         Creates a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network)
         """
-
     def create_service_network_service_association(
         self,
         *,
         serviceIdentifier: str,
         serviceNetworkIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateServiceNetworkServiceAssociationResponseTypeDef:
         """
         Associates a service with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_service_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network_service_association)
         """
-
     def create_service_network_vpc_association(
         self,
         *,
         serviceNetworkIdentifier: str,
         vpcIdentifier: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
@@ -264,15 +252,14 @@
     ) -> CreateServiceNetworkVpcAssociationResponseTypeDef:
         """
         Associates a VPC with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network_vpc_association)
         """
-
     def create_target_group(
         self,
         *,
         name: str,
         type: TargetGroupTypeType,
         clientToken: str = ...,
         config: TargetGroupConfigTypeDef = ...,
@@ -280,535 +267,486 @@
     ) -> CreateTargetGroupResponseTypeDef:
         """
         Creates a target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_target_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_target_group)
         """
-
     def delete_access_log_subscription(
         self, *, accessLogSubscriptionIdentifier: str
     ) -> Dict[str, Any]:
         """
         Deletes the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_access_log_subscription)
         """
-
     def delete_auth_policy(self, *, resourceIdentifier: str) -> Dict[str, Any]:
         """
         Deletes the specified auth policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_auth_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_auth_policy)
         """
-
     def delete_listener(self, *, listenerIdentifier: str, serviceIdentifier: str) -> Dict[str, Any]:
         """
         Deletes the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_listener)
         """
-
     def delete_resource_policy(self, *, resourceArn: str) -> Dict[str, Any]:
         """
         Deletes the specified resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_resource_policy)
         """
-
     def delete_rule(
         self, *, listenerIdentifier: str, ruleIdentifier: str, serviceIdentifier: str
     ) -> Dict[str, Any]:
         """
         Deletes a listener rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_rule)
         """
-
     def delete_service(self, *, serviceIdentifier: str) -> DeleteServiceResponseTypeDef:
         """
         Deletes a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_service)
         """
-
     def delete_service_network(self, *, serviceNetworkIdentifier: str) -> Dict[str, Any]:
         """
         Deletes a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_service_network)
         """
-
     def delete_service_network_service_association(
         self, *, serviceNetworkServiceAssociationIdentifier: str
     ) -> DeleteServiceNetworkServiceAssociationResponseTypeDef:
         """
         Deletes the association between a specified service and the specific service
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service_network_service_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_service_network_service_association)
         """
-
     def delete_service_network_vpc_association(
         self, *, serviceNetworkVpcAssociationIdentifier: str
     ) -> DeleteServiceNetworkVpcAssociationResponseTypeDef:
         """
         Disassociates the VPC from the service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service_network_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_service_network_vpc_association)
         """
-
     def delete_target_group(
         self, *, targetGroupIdentifier: str
     ) -> DeleteTargetGroupResponseTypeDef:
         """
         Deletes a target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_target_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_target_group)
         """
-
     def deregister_targets(
         self, *, targetGroupIdentifier: str, targets: Sequence[TargetTypeDef]
     ) -> DeregisterTargetsResponseTypeDef:
         """
         Deregisters the specified targets from the specified target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.deregister_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#deregister_targets)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#generate_presigned_url)
         """
-
     def get_access_log_subscription(
         self, *, accessLogSubscriptionIdentifier: str
     ) -> GetAccessLogSubscriptionResponseTypeDef:
         """
         Retrieves information about the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_access_log_subscription)
         """
-
     def get_auth_policy(self, *, resourceIdentifier: str) -> GetAuthPolicyResponseTypeDef:
         """
         Retrieves information about the auth policy for the specified service or service
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_auth_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_auth_policy)
         """
-
     def get_listener(
         self, *, listenerIdentifier: str, serviceIdentifier: str
     ) -> GetListenerResponseTypeDef:
         """
         Retrieves information about the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_listener)
         """
-
     def get_resource_policy(self, *, resourceArn: str) -> GetResourcePolicyResponseTypeDef:
         """
         Retrieves information about the resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_resource_policy)
         """
-
     def get_rule(
         self, *, listenerIdentifier: str, ruleIdentifier: str, serviceIdentifier: str
     ) -> GetRuleResponseTypeDef:
         """
         Retrieves information about listener rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_rule)
         """
-
     def get_service(self, *, serviceIdentifier: str) -> GetServiceResponseTypeDef:
         """
         Retrieves information about the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_service)
         """
-
     def get_service_network(
         self, *, serviceNetworkIdentifier: str
     ) -> GetServiceNetworkResponseTypeDef:
         """
         Retrieves information about the specified service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_service_network)
         """
-
     def get_service_network_service_association(
         self, *, serviceNetworkServiceAssociationIdentifier: str
     ) -> GetServiceNetworkServiceAssociationResponseTypeDef:
         """
         Retrieves information about the specified association between a service network
         and a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service_network_service_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_service_network_service_association)
         """
-
     def get_service_network_vpc_association(
         self, *, serviceNetworkVpcAssociationIdentifier: str
     ) -> GetServiceNetworkVpcAssociationResponseTypeDef:
         """
         Retrieves information about the association between a service network and a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service_network_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_service_network_vpc_association)
         """
-
     def get_target_group(self, *, targetGroupIdentifier: str) -> GetTargetGroupResponseTypeDef:
         """
         Retrieves information about the specified target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_target_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_target_group)
         """
-
     def list_access_log_subscriptions(
         self, *, resourceIdentifier: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAccessLogSubscriptionsResponseTypeDef:
         """
         Lists all access log subscriptions for the specified service network or service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_access_log_subscriptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_access_log_subscriptions)
         """
-
     def list_listeners(
         self, *, serviceIdentifier: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListListenersResponseTypeDef:
         """
         Lists the listeners for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_listeners)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_listeners)
         """
-
     def list_rules(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListRulesResponseTypeDef:
         """
         Lists the rules for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_rules)
         """
-
     def list_service_network_service_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...
     ) -> ListServiceNetworkServiceAssociationsResponseTypeDef:
         """
         Lists the associations between the service network and the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_service_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_service_network_service_associations)
         """
-
     def list_service_network_vpc_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...
     ) -> ListServiceNetworkVpcAssociationsResponseTypeDef:
         """
         Lists the service network and VPC associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_vpc_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_service_network_vpc_associations)
         """
-
     def list_service_networks(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListServiceNetworksResponseTypeDef:
         """
         Lists the service networks owned by the caller account or shared with the caller
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_networks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_service_networks)
         """
-
     def list_services(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListServicesResponseTypeDef:
         """
         Lists the services owned by the caller account or shared with the caller
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_services)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_tags_for_resource)
         """
-
     def list_target_groups(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...
     ) -> ListTargetGroupsResponseTypeDef:
         """
         Lists your target groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_target_groups)
         """
-
     def list_targets(
         self,
         *,
         targetGroupIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
         targets: Sequence[TargetTypeDef] = ...
     ) -> ListTargetsResponseTypeDef:
         """
         Lists the targets for the target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_targets)
         """
-
     def put_auth_policy(
         self, *, policy: str, resourceIdentifier: str
     ) -> PutAuthPolicyResponseTypeDef:
         """
         Creates or updates the auth policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.put_auth_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#put_auth_policy)
         """
-
     def put_resource_policy(self, *, policy: str, resourceArn: str) -> Dict[str, Any]:
         """
         Attaches a resource-based permission policy to a service or service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#put_resource_policy)
         """
-
     def register_targets(
         self, *, targetGroupIdentifier: str, targets: Sequence[TargetTypeDef]
     ) -> RegisterTargetsResponseTypeDef:
         """
         Registers the targets with the target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.register_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#register_targets)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the specified tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#untag_resource)
         """
-
     def update_access_log_subscription(
         self, *, accessLogSubscriptionIdentifier: str, destinationArn: str
     ) -> UpdateAccessLogSubscriptionResponseTypeDef:
         """
         Updates the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_access_log_subscription)
         """
-
     def update_listener(
-        self, *, defaultAction: RuleActionTypeDef, listenerIdentifier: str, serviceIdentifier: str
+        self,
+        *,
+        defaultAction: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
+        listenerIdentifier: str,
+        serviceIdentifier: str
     ) -> UpdateListenerResponseTypeDef:
         """
         Updates the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_listener)
         """
-
     def update_rule(
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
-        action: RuleActionTypeDef = ...,
-        match: RuleMatchTypeDef = ...,
+        action: Union[RuleActionTypeDef, RuleActionOutputTypeDef] = ...,
+        match: Union[RuleMatchTypeDef, RuleMatchOutputTypeDef] = ...,
         priority: int = ...
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_rule)
         """
-
     def update_service(
         self, *, serviceIdentifier: str, authType: AuthTypeType = ..., certificateArn: str = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Updates the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_service)
         """
-
     def update_service_network(
         self, *, authType: AuthTypeType, serviceNetworkIdentifier: str
     ) -> UpdateServiceNetworkResponseTypeDef:
         """
         Updates the specified service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_service_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_service_network)
         """
-
     def update_service_network_vpc_association(
         self, *, securityGroupIds: Sequence[str], serviceNetworkVpcAssociationIdentifier: str
     ) -> UpdateServiceNetworkVpcAssociationResponseTypeDef:
         """
         Updates the service network and VPC association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_service_network_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_service_network_vpc_association)
         """
-
     def update_target_group(
         self, *, healthCheck: HealthCheckConfigTypeDef, targetGroupIdentifier: str
     ) -> UpdateTargetGroupResponseTypeDef:
         """
         Updates the specified target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_target_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_target_group)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_access_log_subscriptions"]
     ) -> ListAccessLogSubscriptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_listeners"]) -> ListListenersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_rules"]) -> ListRulesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_network_service_associations"]
     ) -> ListServiceNetworkServiceAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_network_vpc_associations"]
     ) -> ListServiceNetworkVpcAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_networks"]
     ) -> ListServiceNetworksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_target_groups"]
     ) -> ListTargetGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_targets"]) -> ListTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/client.pyi` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_vpc_lattice.client import VPCLatticeClient
 
     session = Session()
     client: VPCLatticeClient = session.client("vpc-lattice")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AuthTypeType, ListenerProtocolType, TargetGroupTypeType
 from .paginator import (
     ListAccessLogSubscriptionsPaginator,
     ListListenersPaginator,
@@ -64,15 +64,17 @@
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PutAuthPolicyResponseTypeDef,
     RegisterTargetsResponseTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
+    RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
     RuleUpdateTypeDef,
     TargetGroupConfigTypeDef,
     TargetTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateListenerResponseTypeDef,
     UpdateRuleResponseTypeDef,
@@ -83,33 +85,37 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("VPCLatticeClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class VPCLatticeClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/)
     """
 
     meta: ClientMeta
@@ -118,37 +124,41 @@
     def exceptions(self) -> Exceptions:
         """
         VPCLatticeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#exceptions)
         """
+
     def batch_update_rule(
         self, *, listenerIdentifier: str, rules: Sequence[RuleUpdateTypeDef], serviceIdentifier: str
     ) -> BatchUpdateRuleResponseTypeDef:
         """
         Updates the listener rules in a batch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.batch_update_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#batch_update_rule)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#close)
         """
+
     def create_access_log_subscription(
         self,
         *,
         destinationArn: str,
         resourceIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
@@ -156,49 +166,52 @@
         """
         Enables access logs to be sent to Amazon CloudWatch, Amazon S3, and Amazon
         Kinesis Data Firehose.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_access_log_subscription)
         """
+
     def create_listener(
         self,
         *,
-        defaultAction: RuleActionTypeDef,
+        defaultAction: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateListenerResponseTypeDef:
         """
         Creates a listener for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_listener)
         """
+
     def create_rule(
         self,
         *,
-        action: RuleActionTypeDef,
+        action: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
         listenerIdentifier: str,
-        match: RuleMatchTypeDef,
+        match: Union[RuleMatchTypeDef, RuleMatchOutputTypeDef],
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a listener rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_rule)
         """
+
     def create_service(
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         certificateArn: str = ...,
         clientToken: str = ...,
@@ -207,42 +220,45 @@
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service)
         """
+
     def create_service_network(
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateServiceNetworkResponseTypeDef:
         """
         Creates a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network)
         """
+
     def create_service_network_service_association(
         self,
         *,
         serviceIdentifier: str,
         serviceNetworkIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateServiceNetworkServiceAssociationResponseTypeDef:
         """
         Associates a service with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_service_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network_service_association)
         """
+
     def create_service_network_vpc_association(
         self,
         *,
         serviceNetworkIdentifier: str,
         vpcIdentifier: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
@@ -250,14 +266,15 @@
     ) -> CreateServiceNetworkVpcAssociationResponseTypeDef:
         """
         Associates a VPC with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network_vpc_association)
         """
+
     def create_target_group(
         self,
         *,
         name: str,
         type: TargetGroupTypeType,
         clientToken: str = ...,
         config: TargetGroupConfigTypeDef = ...,
@@ -265,482 +282,539 @@
     ) -> CreateTargetGroupResponseTypeDef:
         """
         Creates a target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_target_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_target_group)
         """
+
     def delete_access_log_subscription(
         self, *, accessLogSubscriptionIdentifier: str
     ) -> Dict[str, Any]:
         """
         Deletes the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_access_log_subscription)
         """
+
     def delete_auth_policy(self, *, resourceIdentifier: str) -> Dict[str, Any]:
         """
         Deletes the specified auth policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_auth_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_auth_policy)
         """
+
     def delete_listener(self, *, listenerIdentifier: str, serviceIdentifier: str) -> Dict[str, Any]:
         """
         Deletes the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_listener)
         """
+
     def delete_resource_policy(self, *, resourceArn: str) -> Dict[str, Any]:
         """
         Deletes the specified resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_resource_policy)
         """
+
     def delete_rule(
         self, *, listenerIdentifier: str, ruleIdentifier: str, serviceIdentifier: str
     ) -> Dict[str, Any]:
         """
         Deletes a listener rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_rule)
         """
+
     def delete_service(self, *, serviceIdentifier: str) -> DeleteServiceResponseTypeDef:
         """
         Deletes a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_service)
         """
+
     def delete_service_network(self, *, serviceNetworkIdentifier: str) -> Dict[str, Any]:
         """
         Deletes a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_service_network)
         """
+
     def delete_service_network_service_association(
         self, *, serviceNetworkServiceAssociationIdentifier: str
     ) -> DeleteServiceNetworkServiceAssociationResponseTypeDef:
         """
         Deletes the association between a specified service and the specific service
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service_network_service_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_service_network_service_association)
         """
+
     def delete_service_network_vpc_association(
         self, *, serviceNetworkVpcAssociationIdentifier: str
     ) -> DeleteServiceNetworkVpcAssociationResponseTypeDef:
         """
         Disassociates the VPC from the service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service_network_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_service_network_vpc_association)
         """
+
     def delete_target_group(
         self, *, targetGroupIdentifier: str
     ) -> DeleteTargetGroupResponseTypeDef:
         """
         Deletes a target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_target_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#delete_target_group)
         """
+
     def deregister_targets(
         self, *, targetGroupIdentifier: str, targets: Sequence[TargetTypeDef]
     ) -> DeregisterTargetsResponseTypeDef:
         """
         Deregisters the specified targets from the specified target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.deregister_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#deregister_targets)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#generate_presigned_url)
         """
+
     def get_access_log_subscription(
         self, *, accessLogSubscriptionIdentifier: str
     ) -> GetAccessLogSubscriptionResponseTypeDef:
         """
         Retrieves information about the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_access_log_subscription)
         """
+
     def get_auth_policy(self, *, resourceIdentifier: str) -> GetAuthPolicyResponseTypeDef:
         """
         Retrieves information about the auth policy for the specified service or service
         network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_auth_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_auth_policy)
         """
+
     def get_listener(
         self, *, listenerIdentifier: str, serviceIdentifier: str
     ) -> GetListenerResponseTypeDef:
         """
         Retrieves information about the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_listener)
         """
+
     def get_resource_policy(self, *, resourceArn: str) -> GetResourcePolicyResponseTypeDef:
         """
         Retrieves information about the resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_resource_policy)
         """
+
     def get_rule(
         self, *, listenerIdentifier: str, ruleIdentifier: str, serviceIdentifier: str
     ) -> GetRuleResponseTypeDef:
         """
         Retrieves information about listener rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_rule)
         """
+
     def get_service(self, *, serviceIdentifier: str) -> GetServiceResponseTypeDef:
         """
         Retrieves information about the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_service)
         """
+
     def get_service_network(
         self, *, serviceNetworkIdentifier: str
     ) -> GetServiceNetworkResponseTypeDef:
         """
         Retrieves information about the specified service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_service_network)
         """
+
     def get_service_network_service_association(
         self, *, serviceNetworkServiceAssociationIdentifier: str
     ) -> GetServiceNetworkServiceAssociationResponseTypeDef:
         """
         Retrieves information about the specified association between a service network
         and a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service_network_service_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_service_network_service_association)
         """
+
     def get_service_network_vpc_association(
         self, *, serviceNetworkVpcAssociationIdentifier: str
     ) -> GetServiceNetworkVpcAssociationResponseTypeDef:
         """
         Retrieves information about the association between a service network and a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service_network_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_service_network_vpc_association)
         """
+
     def get_target_group(self, *, targetGroupIdentifier: str) -> GetTargetGroupResponseTypeDef:
         """
         Retrieves information about the specified target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_target_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_target_group)
         """
+
     def list_access_log_subscriptions(
         self, *, resourceIdentifier: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAccessLogSubscriptionsResponseTypeDef:
         """
         Lists all access log subscriptions for the specified service network or service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_access_log_subscriptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_access_log_subscriptions)
         """
+
     def list_listeners(
         self, *, serviceIdentifier: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListListenersResponseTypeDef:
         """
         Lists the listeners for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_listeners)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_listeners)
         """
+
     def list_rules(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListRulesResponseTypeDef:
         """
         Lists the rules for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_rules)
         """
+
     def list_service_network_service_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...
     ) -> ListServiceNetworkServiceAssociationsResponseTypeDef:
         """
         Lists the associations between the service network and the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_service_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_service_network_service_associations)
         """
+
     def list_service_network_vpc_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...
     ) -> ListServiceNetworkVpcAssociationsResponseTypeDef:
         """
         Lists the service network and VPC associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_vpc_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_service_network_vpc_associations)
         """
+
     def list_service_networks(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListServiceNetworksResponseTypeDef:
         """
         Lists the service networks owned by the caller account or shared with the caller
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_networks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_service_networks)
         """
+
     def list_services(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListServicesResponseTypeDef:
         """
         Lists the services owned by the caller account or shared with the caller
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_services)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_tags_for_resource)
         """
+
     def list_target_groups(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...
     ) -> ListTargetGroupsResponseTypeDef:
         """
         Lists your target groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_target_groups)
         """
+
     def list_targets(
         self,
         *,
         targetGroupIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
         targets: Sequence[TargetTypeDef] = ...
     ) -> ListTargetsResponseTypeDef:
         """
         Lists the targets for the target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_targets)
         """
+
     def put_auth_policy(
         self, *, policy: str, resourceIdentifier: str
     ) -> PutAuthPolicyResponseTypeDef:
         """
         Creates or updates the auth policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.put_auth_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#put_auth_policy)
         """
+
     def put_resource_policy(self, *, policy: str, resourceArn: str) -> Dict[str, Any]:
         """
         Attaches a resource-based permission policy to a service or service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#put_resource_policy)
         """
+
     def register_targets(
         self, *, targetGroupIdentifier: str, targets: Sequence[TargetTypeDef]
     ) -> RegisterTargetsResponseTypeDef:
         """
         Registers the targets with the target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.register_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#register_targets)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the specified tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#untag_resource)
         """
+
     def update_access_log_subscription(
         self, *, accessLogSubscriptionIdentifier: str, destinationArn: str
     ) -> UpdateAccessLogSubscriptionResponseTypeDef:
         """
         Updates the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_access_log_subscription)
         """
+
     def update_listener(
-        self, *, defaultAction: RuleActionTypeDef, listenerIdentifier: str, serviceIdentifier: str
+        self,
+        *,
+        defaultAction: Union[RuleActionTypeDef, RuleActionOutputTypeDef],
+        listenerIdentifier: str,
+        serviceIdentifier: str
     ) -> UpdateListenerResponseTypeDef:
         """
         Updates the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_listener)
         """
+
     def update_rule(
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
-        action: RuleActionTypeDef = ...,
-        match: RuleMatchTypeDef = ...,
+        action: Union[RuleActionTypeDef, RuleActionOutputTypeDef] = ...,
+        match: Union[RuleMatchTypeDef, RuleMatchOutputTypeDef] = ...,
         priority: int = ...
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_rule)
         """
+
     def update_service(
         self, *, serviceIdentifier: str, authType: AuthTypeType = ..., certificateArn: str = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Updates the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_service)
         """
+
     def update_service_network(
         self, *, authType: AuthTypeType, serviceNetworkIdentifier: str
     ) -> UpdateServiceNetworkResponseTypeDef:
         """
         Updates the specified service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_service_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_service_network)
         """
+
     def update_service_network_vpc_association(
         self, *, securityGroupIds: Sequence[str], serviceNetworkVpcAssociationIdentifier: str
     ) -> UpdateServiceNetworkVpcAssociationResponseTypeDef:
         """
         Updates the service network and VPC association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_service_network_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_service_network_vpc_association)
         """
+
     def update_target_group(
         self, *, healthCheck: HealthCheckConfigTypeDef, targetGroupIdentifier: str
     ) -> UpdateTargetGroupResponseTypeDef:
         """
         Updates the specified target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_target_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_target_group)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_access_log_subscriptions"]
     ) -> ListAccessLogSubscriptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_listeners"]) -> ListListenersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_rules"]) -> ListRulesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_network_service_associations"]
     ) -> ListServiceNetworkServiceAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_network_vpc_associations"]
     ) -> ListServiceNetworkVpcAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_service_networks"]
     ) -> ListServiceNetworksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_target_groups"]
     ) -> ListTargetGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_targets"]) -> ListTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/literals.py` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/literals.pyi` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/paginator.py` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/paginator.pyi` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/type_defs.py` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/type_defs.pyi` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/PKG-INFO` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.28.15
-Summary: Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt` & `mypy-boto3-vpc-lattice-1.28.15.post1/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.15/setup.py` & `mypy-boto3-vpc-lattice-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-vpc-lattice",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_vpc_lattice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder"
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

