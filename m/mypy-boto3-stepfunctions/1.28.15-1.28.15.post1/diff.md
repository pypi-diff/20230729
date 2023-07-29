# Comparing `tmp/mypy-boto3-stepfunctions-1.28.15.tar.gz` & `tmp/mypy-boto3-stepfunctions-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-stepfunctions-1.28.15.tar", last modified: Fri Jul 28 20:43:50 2023, max compression
+gzip compressed data, was "mypy-boto3-stepfunctions-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:18 2023, max compression
```

## Comparing `mypy-boto3-stepfunctions-1.28.15.tar` & `mypy-boto3-stepfunctions-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-stepfunctions-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18173 2023-07-28 20:43:50.521957 mypy-boto3-stepfunctions-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44183 2023-07-28 20:40:18.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44118 2023-07-28 20:40:17.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18173 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:50.521957 mypy-boto3-stepfunctions-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:18.989431 mypy-boto3-stepfunctions-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-07-29 10:04:18.981431 mypy-boto3-stepfunctions-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:18.977431 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28552 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28506 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44183 2023-07-29 10:00:30.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44118 2023-07-29 10:00:29.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:18.981431 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:04:18.000000 mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:18.989431 mypy-boto3-stepfunctions-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 10:00:24.000000 mypy-boto3-stepfunctions-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-stepfunctions-1.28.15/LICENSE` & `mypy-boto3-stepfunctions-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15/PKG-INFO` & `mypy-boto3-stepfunctions-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.28.15
-Summary: Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-stepfunctions-1.28.15/README.md` & `mypy-boto3-stepfunctions-1.28.15.post1/README.md`

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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__init__.py` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__init__.pyi` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__main__.py` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SFN 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.SFN 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
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

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/client.py` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_stepfunctions.client import SFNClient
 
     session = Session()
     client: SFNClient = session.client("stepfunctions")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ExecutionStatusType, StateMachineTypeType
 from .paginator import (
     GetExecutionHistoryPaginator,
     ListActivitiesPaginator,
@@ -41,14 +41,15 @@
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
@@ -151,15 +152,17 @@
     def create_state_machine(
         self,
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: Union[
+            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+        ] = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
@@ -507,15 +510,17 @@
 
     def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: Union[
+            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+        ] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
```

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/client.pyi` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_stepfunctions.client import SFNClient
 
     session = Session()
     client: SFNClient = session.client("stepfunctions")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ExecutionStatusType, StateMachineTypeType
 from .paginator import (
     GetExecutionHistoryPaginator,
     ListActivitiesPaginator,
@@ -41,14 +41,15 @@
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
@@ -143,15 +144,17 @@
     def create_state_machine(
         self,
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: Union[
+            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+        ] = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
@@ -467,15 +470,17 @@
         """
     def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: Union[
+            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+        ] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
```

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/literals.py` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/literals.pyi` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/paginator.py` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/paginator.pyi` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/type_defs.py` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/type_defs.pyi` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/PKG-INFO` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.28.15
-Summary: Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/SOURCES.txt` & `mypy-boto3-stepfunctions-1.28.15.post1/mypy_boto3_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.15/setup.py` & `mypy-boto3-stepfunctions-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-stepfunctions",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

