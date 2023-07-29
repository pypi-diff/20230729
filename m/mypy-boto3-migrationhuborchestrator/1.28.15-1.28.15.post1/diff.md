# Comparing `tmp/mypy-boto3-migrationhuborchestrator-1.28.15.tar.gz` & `tmp/mypy-boto3-migrationhuborchestrator-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhuborchestrator-1.28.15.tar", last modified: Fri Jul 28 20:43:20 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhuborchestrator-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:44 2023, max compression
```

## Comparing `mypy-boto3-migrationhuborchestrator-1.28.15.tar` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.233542 mypy-boto3-migrationhuborchestrator-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-07-28 20:43:20.233542 mypy-boto3-migrationhuborchestrator-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.221542 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-28 20:32:04.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-28 20:32:04.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32109 2023-07-28 20:32:05.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-07-28 20:32:04.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.233542 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:20.233542 mypy-boto3-migrationhuborchestrator-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.161300 mypy-boto3-migrationhuborchestrator-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-07-29 10:03:44.149299 mypy-boto3-migrationhuborchestrator-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.145300 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25333 2023-07-29 09:51:44.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25291 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-29 09:51:44.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-29 09:51:44.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-07-29 09:51:44.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-07-29 09:51:44.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32532 2023-07-29 09:51:45.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32504 2023-07-29 09:51:45.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.149299 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-29 10:03:43.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:44.161300 mypy-boto3-migrationhuborchestrator-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-29 09:51:41.000000 mypy-boto3-migrationhuborchestrator-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/LICENSE` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/PKG-INFO` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhuborchestrator
-Version: 1.28.15
-Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,17 +358,17 @@
 ### Typed dictionaries
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
+    StepInputOutputTypeDef,
     StepInputTypeDef,
     ResponseMetadataTypeDef,
-    StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
@@ -398,26 +398,27 @@
     PlatformScriptKeyTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
+    WorkflowStepOutputUnionOutputTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
     UpdateMigrationWorkflowRequestRequestTypeDef,
+    CreateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowResponseTypeDef,
-    UpdateWorkflowStepResponseTypeDef,
-    CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
+    UpdateWorkflowStepResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
     ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
@@ -440,15 +441,15 @@
     GetTemplateStepResponseTypeDef,
     CreateWorkflowStepRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
 
 
-def get_structure() -> StepInputTypeDef:
+def get_structure() -> StepInputOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/README.md` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/README.md`

 * *Files 2% similar despite different names*

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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,17 +326,17 @@
 ### Typed dictionaries
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
+    StepInputOutputTypeDef,
     StepInputTypeDef,
     ResponseMetadataTypeDef,
-    StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
@@ -366,26 +366,27 @@
     PlatformScriptKeyTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
+    WorkflowStepOutputUnionOutputTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
     UpdateMigrationWorkflowRequestRequestTypeDef,
+    CreateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowResponseTypeDef,
-    UpdateWorkflowStepResponseTypeDef,
-    CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
+    UpdateWorkflowStepResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
     ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
@@ -408,15 +409,15 @@
     GetTemplateStepResponseTypeDef,
     CreateWorkflowStepRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
 
 
-def get_structure() -> StepInputTypeDef:
+def get_structure() -> StepInputOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__init__.py` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__init__.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__main__.py` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.MigrationHubOrchestrator 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator\nOther"
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/client.py` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migrationhuborchestrator.client import MigrationHubOrchestratorClient
 
     session = Session()
     client: MigrationHubOrchestratorClient = session.client("migrationhuborchestrator")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MigrationWorkflowStatusEnumType, StepActionTypeType, StepStatusType
 from .paginator import (
     ListPluginsPaginator,
     ListTemplatesPaginator,
@@ -45,14 +45,15 @@
     ListTagsForResourceResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
+    StepInputOutputTypeDef,
     StepInputTypeDef,
     StopMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepResponseTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
     WorkflowStepOutputTypeDef,
@@ -119,15 +120,15 @@
 
     def create_workflow(
         self,
         *,
         name: str,
         templateId: str,
         applicationConfigurationId: str,
-        inputParameters: Mapping[str, StepInputTypeDef],
+        inputParameters: Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
         description: str = ...,
         stepTargets: Sequence[str] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateMigrationWorkflowResponseTypeDef:
         """
         Create a workflow to orchestrate your migrations.
 
@@ -141,15 +142,15 @@
         name: str,
         stepGroupId: str,
         workflowId: str,
         stepActionType: StepActionTypeType,
         description: str = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
+        outputs: Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...
     ) -> CreateWorkflowStepResponseTypeDef:
         """
         Create a step in the migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step)
@@ -396,15 +397,15 @@
 
     def update_workflow(
         self,
         *,
         id: str,
         name: str = ...,
         description: str = ...,
-        inputParameters: Mapping[str, StepInputTypeDef] = ...,
+        inputParameters: Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]] = ...,
         stepTargets: Sequence[str] = ...
     ) -> UpdateMigrationWorkflowResponseTypeDef:
         """
         Update a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/client/#update_workflow)
@@ -417,15 +418,15 @@
         stepGroupId: str,
         workflowId: str,
         name: str = ...,
         description: str = ...,
         stepActionType: StepActionTypeType = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
+        outputs: Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...,
         status: StepStatusType = ...
     ) -> UpdateWorkflowStepResponseTypeDef:
         """
         Update a step in a migration workflow.
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/client.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migrationhuborchestrator.client import MigrationHubOrchestratorClient
 
     session = Session()
     client: MigrationHubOrchestratorClient = session.client("migrationhuborchestrator")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import MigrationWorkflowStatusEnumType, StepActionTypeType, StepStatusType
 from .paginator import (
     ListPluginsPaginator,
     ListTemplatesPaginator,
@@ -45,14 +45,15 @@
     ListTagsForResourceResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
+    StepInputOutputTypeDef,
     StepInputTypeDef,
     StopMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepResponseTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
     WorkflowStepOutputTypeDef,
@@ -112,15 +113,15 @@
         """
     def create_workflow(
         self,
         *,
         name: str,
         templateId: str,
         applicationConfigurationId: str,
-        inputParameters: Mapping[str, StepInputTypeDef],
+        inputParameters: Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
         description: str = ...,
         stepTargets: Sequence[str] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateMigrationWorkflowResponseTypeDef:
         """
         Create a workflow to orchestrate your migrations.
 
@@ -133,15 +134,15 @@
         name: str,
         stepGroupId: str,
         workflowId: str,
         stepActionType: StepActionTypeType,
         description: str = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
+        outputs: Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...
     ) -> CreateWorkflowStepResponseTypeDef:
         """
         Create a step in the migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step)
@@ -363,15 +364,15 @@
         """
     def update_workflow(
         self,
         *,
         id: str,
         name: str = ...,
         description: str = ...,
-        inputParameters: Mapping[str, StepInputTypeDef] = ...,
+        inputParameters: Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]] = ...,
         stepTargets: Sequence[str] = ...
     ) -> UpdateMigrationWorkflowResponseTypeDef:
         """
         Update a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/client/#update_workflow)
@@ -383,15 +384,15 @@
         stepGroupId: str,
         workflowId: str,
         name: str = ...,
         description: str = ...,
         stepActionType: StepActionTypeType = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
+        outputs: Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...,
         status: StepStatusType = ...
     ) -> UpdateWorkflowStepResponseTypeDef:
         """
         Update a step in a migration workflow.
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/literals.py` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/literals.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/paginator.py` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/paginator.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/type_defs.py` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for migrationhuborchestrator service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_migrationhuborchestrator.type_defs import StepInputTypeDef
+    from mypy_boto3_migrationhuborchestrator.type_defs import StepInputOutputTypeDef
 
-    data: StepInputTypeDef = {...}
+    data: StepInputOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     DataTypeType,
     MigrationWorkflowStatusEnumType,
     OwnerType,
     PluginHealthType,
     RunEnvironmentType,
@@ -34,17 +34,17 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "StepInputOutputTypeDef",
     "StepInputTypeDef",
     "ResponseMetadataTypeDef",
-    "StepInputOutputTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
     "GetMigrationWorkflowRequestRequestTypeDef",
     "GetMigrationWorkflowTemplateRequestRequestTypeDef",
@@ -74,26 +74,27 @@
     "PlatformScriptKeyTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
+    "WorkflowStepOutputUnionOutputTypeDef",
     "WorkflowStepOutputUnionTypeDef",
     "CreateMigrationWorkflowRequestRequestTypeDef",
     "UpdateMigrationWorkflowRequestRequestTypeDef",
+    "CreateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowResponseTypeDef",
-    "UpdateWorkflowStepResponseTypeDef",
-    "CreateMigrationWorkflowResponseTypeDef",
     "UpdateMigrationWorkflowResponseTypeDef",
+    "UpdateWorkflowStepResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
     "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
@@ -115,14 +116,25 @@
     "WorkflowStepOutputTypeDef",
     "GetTemplateStepResponseTypeDef",
     "CreateWorkflowStepRequestRequestTypeDef",
     "GetWorkflowStepResponseTypeDef",
     "UpdateWorkflowStepRequestRequestTypeDef",
 )
 
+StepInputOutputTypeDef = TypedDict(
+    "StepInputOutputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringsValue": List[str],
+        "mapOfStringValue": Dict[str, str],
+    },
+    total=False,
+)
+
 StepInputTypeDef = TypedDict(
     "StepInputTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
         "listOfStringsValue": Sequence[str],
         "mapOfStringValue": Mapping[str, str],
@@ -137,25 +149,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-StepInputOutputTypeDef = TypedDict(
-    "StepInputOutputTypeDef",
-    {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringsValue": List[str],
-        "mapOfStringValue": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredCreateWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "name": str,
     },
 )
@@ -599,14 +600,24 @@
 class UpdateWorkflowStepGroupRequestRequestTypeDef(
     _RequiredUpdateWorkflowStepGroupRequestRequestTypeDef,
     _OptionalUpdateWorkflowStepGroupRequestRequestTypeDef,
 ):
     pass
 
 
+WorkflowStepOutputUnionOutputTypeDef = TypedDict(
+    "WorkflowStepOutputUnionOutputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringValue": List[str],
+    },
+    total=False,
+)
+
 WorkflowStepOutputUnionTypeDef = TypedDict(
     "WorkflowStepOutputUnionTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
         "listOfStringValue": Sequence[str],
     },
@@ -615,15 +626,15 @@
 
 _RequiredCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMigrationWorkflowRequestRequestTypeDef",
     {
         "name": str,
         "templateId": str,
         "applicationConfigurationId": str,
-        "inputParameters": Mapping[str, StepInputTypeDef],
+        "inputParameters": Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
     },
 )
 _OptionalCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMigrationWorkflowRequestRequestTypeDef",
     {
         "description": str,
         "stepTargets": Sequence[str],
@@ -647,28 +658,46 @@
     },
 )
 _OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
-        "inputParameters": Mapping[str, StepInputTypeDef],
+        "inputParameters": Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
         "stepTargets": Sequence[str],
     },
     total=False,
 )
 
 
 class UpdateMigrationWorkflowRequestRequestTypeDef(
     _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
     _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
 
+CreateMigrationWorkflowResponseTypeDef = TypedDict(
+    "CreateMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "templateId": str,
+        "adsApplicationConfigurationId": str,
+        "workflowInputs": Dict[str, StepInputOutputTypeDef],
+        "stepTargets": List[str],
+        "status": MigrationWorkflowStatusEnumType,
+        "creationTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateWorkflowStepResponseTypeDef = TypedDict(
     "CreateWorkflowStepResponseTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "workflowId": str,
         "name": str,
@@ -725,58 +754,40 @@
         "status": MigrationWorkflowStatusEnumType,
         "statusMessage": str,
         "lastStopTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWorkflowStepResponseTypeDef = TypedDict(
-    "UpdateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMigrationWorkflowResponseTypeDef = TypedDict(
-    "CreateMigrationWorkflowResponseTypeDef",
+UpdateMigrationWorkflowResponseTypeDef = TypedDict(
+    "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
+        "lastModifiedTime": datetime,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateMigrationWorkflowResponseTypeDef = TypedDict(
-    "UpdateMigrationWorkflowResponseTypeDef",
+UpdateWorkflowStepResponseTypeDef = TypedDict(
+    "UpdateWorkflowStepResponseTypeDef",
     {
         "id": str,
-        "arn": str,
+        "stepGroupId": str,
+        "workflowId": str,
         "name": str,
-        "description": str,
-        "templateId": str,
-        "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputOutputTypeDef],
-        "stepTargets": List[str],
-        "status": MigrationWorkflowStatusEnumType,
-        "creationTime": datetime,
-        "lastModifiedTime": datetime,
-        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkflowStepGroupResponseTypeDef = TypedDict(
     "CreateWorkflowStepGroupResponseTypeDef",
     {
@@ -1092,15 +1103,15 @@
 
 WorkflowStepOutputTypeDef = TypedDict(
     "WorkflowStepOutputTypeDef",
     {
         "name": str,
         "dataType": DataTypeType,
         "required": bool,
-        "value": WorkflowStepOutputUnionTypeDef,
+        "value": WorkflowStepOutputUnionOutputTypeDef,
     },
     total=False,
 )
 
 GetTemplateStepResponseTypeDef = TypedDict(
     "GetTemplateStepResponseTypeDef",
     {
@@ -1130,15 +1141,15 @@
 )
 _OptionalCreateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWorkflowStepRequestRequestTypeDef",
     {
         "description": str,
         "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
         "stepTarget": Sequence[str],
-        "outputs": Sequence[WorkflowStepOutputTypeDef],
+        "outputs": Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]],
         "previous": Sequence[str],
         "next": Sequence[str],
     },
     total=False,
 )
 
 
@@ -1189,15 +1200,15 @@
     "_OptionalUpdateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
         "stepActionType": StepActionTypeType,
         "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
         "stepTarget": Sequence[str],
-        "outputs": Sequence[WorkflowStepOutputTypeDef],
+        "outputs": Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]],
         "previous": Sequence[str],
         "next": Sequence[str],
         "status": StepStatusType,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/type_defs.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for migrationhuborchestrator service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_migrationhuborchestrator.type_defs import StepInputTypeDef
+    from mypy_boto3_migrationhuborchestrator.type_defs import StepInputOutputTypeDef
 
-    data: StepInputTypeDef = {...}
+    data: StepInputOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     DataTypeType,
     MigrationWorkflowStatusEnumType,
     OwnerType,
     PluginHealthType,
     RunEnvironmentType,
@@ -33,17 +33,17 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "StepInputOutputTypeDef",
     "StepInputTypeDef",
     "ResponseMetadataTypeDef",
-    "StepInputOutputTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
     "GetMigrationWorkflowRequestRequestTypeDef",
     "GetMigrationWorkflowTemplateRequestRequestTypeDef",
@@ -73,26 +73,27 @@
     "PlatformScriptKeyTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
+    "WorkflowStepOutputUnionOutputTypeDef",
     "WorkflowStepOutputUnionTypeDef",
     "CreateMigrationWorkflowRequestRequestTypeDef",
     "UpdateMigrationWorkflowRequestRequestTypeDef",
+    "CreateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowResponseTypeDef",
-    "UpdateWorkflowStepResponseTypeDef",
-    "CreateMigrationWorkflowResponseTypeDef",
     "UpdateMigrationWorkflowResponseTypeDef",
+    "UpdateWorkflowStepResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
     "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
@@ -114,14 +115,25 @@
     "WorkflowStepOutputTypeDef",
     "GetTemplateStepResponseTypeDef",
     "CreateWorkflowStepRequestRequestTypeDef",
     "GetWorkflowStepResponseTypeDef",
     "UpdateWorkflowStepRequestRequestTypeDef",
 )
 
+StepInputOutputTypeDef = TypedDict(
+    "StepInputOutputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringsValue": List[str],
+        "mapOfStringValue": Dict[str, str],
+    },
+    total=False,
+)
+
 StepInputTypeDef = TypedDict(
     "StepInputTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
         "listOfStringsValue": Sequence[str],
         "mapOfStringValue": Mapping[str, str],
@@ -136,25 +148,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-StepInputOutputTypeDef = TypedDict(
-    "StepInputOutputTypeDef",
-    {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringsValue": List[str],
-        "mapOfStringValue": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredCreateWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "name": str,
     },
 )
@@ -586,14 +587,24 @@
 
 class UpdateWorkflowStepGroupRequestRequestTypeDef(
     _RequiredUpdateWorkflowStepGroupRequestRequestTypeDef,
     _OptionalUpdateWorkflowStepGroupRequestRequestTypeDef,
 ):
     pass
 
+WorkflowStepOutputUnionOutputTypeDef = TypedDict(
+    "WorkflowStepOutputUnionOutputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringValue": List[str],
+    },
+    total=False,
+)
+
 WorkflowStepOutputUnionTypeDef = TypedDict(
     "WorkflowStepOutputUnionTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
         "listOfStringValue": Sequence[str],
     },
@@ -602,15 +613,15 @@
 
 _RequiredCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMigrationWorkflowRequestRequestTypeDef",
     {
         "name": str,
         "templateId": str,
         "applicationConfigurationId": str,
-        "inputParameters": Mapping[str, StepInputTypeDef],
+        "inputParameters": Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
     },
 )
 _OptionalCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMigrationWorkflowRequestRequestTypeDef",
     {
         "description": str,
         "stepTargets": Sequence[str],
@@ -632,26 +643,44 @@
     },
 )
 _OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
-        "inputParameters": Mapping[str, StepInputTypeDef],
+        "inputParameters": Mapping[str, Union[StepInputTypeDef, StepInputOutputTypeDef]],
         "stepTargets": Sequence[str],
     },
     total=False,
 )
 
 class UpdateMigrationWorkflowRequestRequestTypeDef(
     _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
     _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
+CreateMigrationWorkflowResponseTypeDef = TypedDict(
+    "CreateMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "templateId": str,
+        "adsApplicationConfigurationId": str,
+        "workflowInputs": Dict[str, StepInputOutputTypeDef],
+        "stepTargets": List[str],
+        "status": MigrationWorkflowStatusEnumType,
+        "creationTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateWorkflowStepResponseTypeDef = TypedDict(
     "CreateWorkflowStepResponseTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "workflowId": str,
         "name": str,
@@ -708,58 +737,40 @@
         "status": MigrationWorkflowStatusEnumType,
         "statusMessage": str,
         "lastStopTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWorkflowStepResponseTypeDef = TypedDict(
-    "UpdateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMigrationWorkflowResponseTypeDef = TypedDict(
-    "CreateMigrationWorkflowResponseTypeDef",
+UpdateMigrationWorkflowResponseTypeDef = TypedDict(
+    "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
+        "lastModifiedTime": datetime,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateMigrationWorkflowResponseTypeDef = TypedDict(
-    "UpdateMigrationWorkflowResponseTypeDef",
+UpdateWorkflowStepResponseTypeDef = TypedDict(
+    "UpdateWorkflowStepResponseTypeDef",
     {
         "id": str,
-        "arn": str,
+        "stepGroupId": str,
+        "workflowId": str,
         "name": str,
-        "description": str,
-        "templateId": str,
-        "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputOutputTypeDef],
-        "stepTargets": List[str],
-        "status": MigrationWorkflowStatusEnumType,
-        "creationTime": datetime,
-        "lastModifiedTime": datetime,
-        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkflowStepGroupResponseTypeDef = TypedDict(
     "CreateWorkflowStepGroupResponseTypeDef",
     {
@@ -1067,15 +1078,15 @@
 
 WorkflowStepOutputTypeDef = TypedDict(
     "WorkflowStepOutputTypeDef",
     {
         "name": str,
         "dataType": DataTypeType,
         "required": bool,
-        "value": WorkflowStepOutputUnionTypeDef,
+        "value": WorkflowStepOutputUnionOutputTypeDef,
     },
     total=False,
 )
 
 GetTemplateStepResponseTypeDef = TypedDict(
     "GetTemplateStepResponseTypeDef",
     {
@@ -1105,15 +1116,15 @@
 )
 _OptionalCreateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWorkflowStepRequestRequestTypeDef",
     {
         "description": str,
         "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
         "stepTarget": Sequence[str],
-        "outputs": Sequence[WorkflowStepOutputTypeDef],
+        "outputs": Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]],
         "previous": Sequence[str],
         "next": Sequence[str],
     },
     total=False,
 )
 
 class CreateWorkflowStepRequestRequestTypeDef(
@@ -1162,15 +1173,15 @@
     "_OptionalUpdateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
         "stepActionType": StepActionTypeType,
         "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
         "stepTarget": Sequence[str],
-        "outputs": Sequence[WorkflowStepOutputTypeDef],
+        "outputs": Sequence[Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]],
         "previous": Sequence[str],
         "next": Sequence[str],
         "status": StepStatusType,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhuborchestrator
-Version: 1.28.15
-Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,17 +358,17 @@
 ### Typed dictionaries
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
+    StepInputOutputTypeDef,
     StepInputTypeDef,
     ResponseMetadataTypeDef,
-    StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
@@ -398,26 +398,27 @@
     PlatformScriptKeyTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
+    WorkflowStepOutputUnionOutputTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
     UpdateMigrationWorkflowRequestRequestTypeDef,
+    CreateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowResponseTypeDef,
-    UpdateWorkflowStepResponseTypeDef,
-    CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
+    UpdateWorkflowStepResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
     ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
@@ -440,15 +441,15 @@
     GetTemplateStepResponseTypeDef,
     CreateWorkflowStepRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
 
 
-def get_structure() -> StepInputTypeDef:
+def get_structure() -> StepInputOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.15/setup.py` & `mypy-boto3-migrationhuborchestrator-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhuborchestrator",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_migrationhuborchestrator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with"
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

