# Comparing `tmp/mypy-boto3-entityresolution-1.28.15.tar.gz` & `tmp/mypy-boto3-entityresolution-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-entityresolution-1.28.15.tar", last modified: Fri Jul 28 20:42:46 2023, max compression
+gzip compressed data, was "mypy-boto3-entityresolution-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:06 2023, max compression
```

## Comparing `mypy-boto3-entityresolution-1.28.15.tar` & `mypy-boto3-entityresolution-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.953085 mypy-boto3-entityresolution-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-07-28 20:42:46.949085 mypy-boto3-entityresolution-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.941084 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-07-28 20:25:35.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-07-28 20:25:34.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.949085 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-07-28 20:42:46.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:42:46.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:42:46.000000 mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:46.953085 mypy-boto3-entityresolution-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:25:33.000000 mypy-boto3-entityresolution-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.165143 mypy-boto3-entityresolution-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-07-29 10:03:06.165143 mypy-boto3-entityresolution-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.157143 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17808 2023-07-29 09:45:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17786 2023-07-29 09:45:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.165143 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:06.165143 mypy-boto3-entityresolution-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-entityresolution-1.28.15/LICENSE` & `mypy-boto3-entityresolution-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15/PKG-INFO` & `mypy-boto3-entityresolution-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-entityresolution
-Version: 1.28.15
-Summary: Type annotations for boto3.EntityResolution 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EntityResolution 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/
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
 [mypy-boto3-entityresolution docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-entityresolution-1.28.15/README.md` & `mypy-boto3-entityresolution-1.28.15.post1/README.md`

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
 [mypy-boto3-entityresolution docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/__init__.py` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/__init__.pyi` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/__main__.py` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EntityResolution 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.EntityResolution 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution\nOther"
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

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/client.py` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_entityresolution.client import EntityResolutionClient
 
     session = Session()
     client: EntityResolutionClient = session.client("entityresolution")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListSchemaMappingsPaginator,
@@ -34,15 +34,17 @@
     GetSchemaMappingOutputTypeDef,
     IncrementalRunConfigTypeDef,
     InputSourceTypeDef,
     ListMatchingJobsOutputTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    OutputSourceOutputTypeDef,
     OutputSourceTypeDef,
+    ResolutionTechniquesOutputTypeDef,
     ResolutionTechniquesTypeDef,
     SchemaInputAttributeTypeDef,
     StartMatchingJobOutputTypeDef,
     UpdateMatchingWorkflowOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -106,16 +108,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#close)
         """
 
     def create_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
-        outputSourceConfig: Sequence[OutputSourceTypeDef],
-        resolutionTechniques: ResolutionTechniquesTypeDef,
+        outputSourceConfig: Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
+        resolutionTechniques: Union[ResolutionTechniquesTypeDef, ResolutionTechniquesOutputTypeDef],
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateMatchingWorkflowOutputTypeDef:
         """
@@ -273,16 +275,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#untag_resource)
         """
 
     def update_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
-        outputSourceConfig: Sequence[OutputSourceTypeDef],
-        resolutionTechniques: ResolutionTechniquesTypeDef,
+        outputSourceConfig: Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
+        resolutionTechniques: Union[ResolutionTechniquesTypeDef, ResolutionTechniquesOutputTypeDef],
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...
     ) -> UpdateMatchingWorkflowOutputTypeDef:
         """
         Updates an existing `MatchingWorkflow`.
```

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/client.pyi` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_entityresolution.client import EntityResolutionClient
 
     session = Session()
     client: EntityResolutionClient = session.client("entityresolution")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListSchemaMappingsPaginator,
@@ -34,15 +34,17 @@
     GetSchemaMappingOutputTypeDef,
     IncrementalRunConfigTypeDef,
     InputSourceTypeDef,
     ListMatchingJobsOutputTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    OutputSourceOutputTypeDef,
     OutputSourceTypeDef,
+    ResolutionTechniquesOutputTypeDef,
     ResolutionTechniquesTypeDef,
     SchemaInputAttributeTypeDef,
     StartMatchingJobOutputTypeDef,
     UpdateMatchingWorkflowOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -99,16 +101,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#close)
         """
     def create_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
-        outputSourceConfig: Sequence[OutputSourceTypeDef],
-        resolutionTechniques: ResolutionTechniquesTypeDef,
+        outputSourceConfig: Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
+        resolutionTechniques: Union[ResolutionTechniquesTypeDef, ResolutionTechniquesOutputTypeDef],
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateMatchingWorkflowOutputTypeDef:
         """
@@ -250,16 +252,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#untag_resource)
         """
     def update_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
-        outputSourceConfig: Sequence[OutputSourceTypeDef],
-        resolutionTechniques: ResolutionTechniquesTypeDef,
+        outputSourceConfig: Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
+        resolutionTechniques: Union[ResolutionTechniquesTypeDef, ResolutionTechniquesOutputTypeDef],
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...
     ) -> UpdateMatchingWorkflowOutputTypeDef:
         """
         Updates an existing `MatchingWorkflow`.
```

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/literals.py` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/literals.pyi` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/paginator.py` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/paginator.pyi` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/type_defs.py` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_entityresolution.type_defs import IncrementalRunConfigTypeDef
 
     data: IncrementalRunConfigTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AttributeMatchingModelType,
     JobStatusType,
     ResolutionTypeType,
     SchemaAttributeTypeType,
 )
@@ -659,15 +659,15 @@
     },
 )
 
 _RequiredCreateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_RequiredCreateMatchingWorkflowInputRequestTypeDef",
     {
         "inputSourceConfig": Sequence[InputSourceTypeDef],
-        "outputSourceConfig": Sequence[OutputSourceTypeDef],
+        "outputSourceConfig": Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
         "resolutionTechniques": ResolutionTechniquesTypeDef,
         "roleArn": str,
         "workflowName": str,
     },
 )
 _OptionalCreateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_OptionalCreateMatchingWorkflowInputRequestTypeDef",
@@ -687,15 +687,15 @@
     pass
 
 
 _RequiredUpdateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMatchingWorkflowInputRequestTypeDef",
     {
         "inputSourceConfig": Sequence[InputSourceTypeDef],
-        "outputSourceConfig": Sequence[OutputSourceTypeDef],
+        "outputSourceConfig": Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
         "resolutionTechniques": ResolutionTechniquesTypeDef,
         "roleArn": str,
         "workflowName": str,
     },
 )
 _OptionalUpdateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_OptionalUpdateMatchingWorkflowInputRequestTypeDef",
```

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution/type_defs.pyi` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_entityresolution.type_defs import IncrementalRunConfigTypeDef
 
     data: IncrementalRunConfigTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AttributeMatchingModelType,
     JobStatusType,
     ResolutionTypeType,
     SchemaAttributeTypeType,
 )
@@ -640,15 +640,15 @@
     },
 )
 
 _RequiredCreateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_RequiredCreateMatchingWorkflowInputRequestTypeDef",
     {
         "inputSourceConfig": Sequence[InputSourceTypeDef],
-        "outputSourceConfig": Sequence[OutputSourceTypeDef],
+        "outputSourceConfig": Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
         "resolutionTechniques": ResolutionTechniquesTypeDef,
         "roleArn": str,
         "workflowName": str,
     },
 )
 _OptionalCreateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_OptionalCreateMatchingWorkflowInputRequestTypeDef",
@@ -666,15 +666,15 @@
 ):
     pass
 
 _RequiredUpdateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMatchingWorkflowInputRequestTypeDef",
     {
         "inputSourceConfig": Sequence[InputSourceTypeDef],
-        "outputSourceConfig": Sequence[OutputSourceTypeDef],
+        "outputSourceConfig": Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
         "resolutionTechniques": ResolutionTechniquesTypeDef,
         "roleArn": str,
         "workflowName": str,
     },
 )
 _OptionalUpdateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_OptionalUpdateMatchingWorkflowInputRequestTypeDef",
```

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution.egg-info/PKG-INFO` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-entityresolution
-Version: 1.28.15
-Summary: Type annotations for boto3.EntityResolution 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EntityResolution 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/
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
 [mypy-boto3-entityresolution docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-entityresolution-1.28.15/mypy_boto3_entityresolution.egg-info/SOURCES.txt` & `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15/setup.py` & `mypy-boto3-entityresolution-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-entityresolution",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_entityresolution"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.EntityResolution 1.28.15 service generated with"
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

