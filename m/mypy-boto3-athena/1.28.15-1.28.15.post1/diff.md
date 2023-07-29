# Comparing `tmp/mypy-boto3-athena-1.28.15.tar.gz` & `tmp/mypy-boto3-athena-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-athena-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
+gzip compressed data, was "mypy-boto3-athena-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
```

## Comparing `mypy-boto3-athena-1.28.15.tar` & `mypy-boto3-athena-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.228695 mypy-boto3-athena-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20977 2023-07-28 20:42:19.228695 mypy-boto3-athena-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19494 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.220695 mypy-boto3-athena-1.28.15/mypy_boto3_athena/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46117 2023-07-28 20:19:47.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46035 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-28 20:19:47.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-07-28 20:19:47.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-28 20:19:47.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-28 20:19:47.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63549 2023-07-28 20:19:49.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63458 2023-07-28 20:19:48.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.228695 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20977 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.228695 mypy-boto3-athena-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.381021 mypy-boto3-athena-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-07-29 10:02:34.377021 mypy-boto3-athena-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19494 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.373021 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46302 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46220 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-29 09:38:39.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-07-29 09:38:39.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63618 2023-07-29 09:38:42.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63527 2023-07-29 09:38:41.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.377021 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.381021 mypy-boto3-athena-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-athena-1.28.15/LICENSE` & `mypy-boto3-athena-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15/PKG-INFO` & `mypy-boto3-athena-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.28.15
-Summary: Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-athena-1.28.15/README.md` & `mypy-boto3-athena-1.28.15.post1/README.md`

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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/__init__.py` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/__init__.pyi` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/__main__.py` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Athena 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Athena 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
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

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/client.py` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_athena.client import AthenaClient
 
     session = Session()
     client: AthenaClient = session.client("athena")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CalculationExecutionStateType,
     DataCatalogTypeType,
     ExecutorStateType,
@@ -35,18 +35,20 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
+    CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
+    EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
@@ -724,15 +726,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_work_groups)
         """
 
     def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[CapacityAssignmentTypeDef]
+        CapacityAssignments: Sequence[
+            Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
+        ]
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#put_capacity_assignment_configuration)
@@ -772,15 +776,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_query_execution)
         """
 
     def start_session(
         self,
         *,
         WorkGroup: str,
-        EngineConfiguration: EngineConfigurationTypeDef,
+        EngineConfiguration: Union[EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef],
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
         ClientRequestToken: str = ...
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
```

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/client.pyi` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_athena.client import AthenaClient
 
     session = Session()
     client: AthenaClient = session.client("athena")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CalculationExecutionStateType,
     DataCatalogTypeType,
     ExecutorStateType,
@@ -35,18 +35,20 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
+    CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
+    EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
@@ -664,15 +666,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_work_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_work_groups)
         """
     def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[CapacityAssignmentTypeDef]
+        CapacityAssignments: Sequence[
+            Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
+        ]
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#put_capacity_assignment_configuration)
@@ -709,15 +713,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_query_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_query_execution)
         """
     def start_session(
         self,
         *,
         WorkGroup: str,
-        EngineConfiguration: EngineConfigurationTypeDef,
+        EngineConfiguration: Union[EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef],
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
         ClientRequestToken: str = ...
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
```

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/literals.py` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/literals.pyi` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/paginator.py` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/paginator.pyi` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/type_defs.py` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_athena.type_defs import AclConfigurationTypeDef
 
     data: AclConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CalculationExecutionStateType,
     CapacityAllocationStatusType,
     CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
@@ -1773,15 +1773,17 @@
     total=False,
 )
 
 PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
     "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     {
         "CapacityReservationName": str,
-        "CapacityAssignments": Sequence[CapacityAssignmentTypeDef],
+        "CapacityAssignments": Sequence[
+            Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
+        ],
     },
 )
 
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
```

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena/type_defs.pyi` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_athena.type_defs import AclConfigurationTypeDef
 
     data: AclConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CalculationExecutionStateType,
     CapacityAllocationStatusType,
     CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
@@ -1708,15 +1708,17 @@
     total=False,
 )
 
 PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
     "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     {
         "CapacityReservationName": str,
-        "CapacityAssignments": Sequence[CapacityAssignmentTypeDef],
+        "CapacityAssignments": Sequence[
+            Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
+        ],
     },
 )
 
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
```

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/PKG-INFO` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.28.15
-Summary: Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/SOURCES.txt` & `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15/setup.py` & `mypy-boto3-athena-1.28.15.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-athena",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

