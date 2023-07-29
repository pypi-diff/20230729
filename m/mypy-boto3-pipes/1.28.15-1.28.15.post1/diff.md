# Comparing `tmp/mypy-boto3-pipes-1.28.15.tar.gz` & `tmp/mypy-boto3-pipes-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pipes-1.28.15.tar", last modified: Fri Jul 28 20:43:29 2023, max compression
+gzip compressed data, was "mypy-boto3-pipes-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:54 2023, max compression
```

## Comparing `mypy-boto3-pipes-1.28.15.tar` & `mypy-boto3-pipes-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:29.193665 mypy-boto3-pipes-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-07-28 20:43:29.189665 mypy-boto3-pipes-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:29.173665 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42541 2023-07-28 20:33:32.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42499 2023-07-28 20:33:32.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:29.189665 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:29.193665 mypy-boto3-pipes-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.677343 mypy-boto3-pipes-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-29 10:03:54.677343 mypy-boto3-pipes-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.661343 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42541 2023-07-29 09:53:27.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42499 2023-07-29 09:53:27.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.677343 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:54.677343 mypy-boto3-pipes-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-pipes-1.28.15/LICENSE` & `mypy-boto3-pipes-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15/PKG-INFO` & `mypy-boto3-pipes-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.28.15
-Summary: Type annotations for boto3.EventBridgePipes 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EventBridgePipes 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pipes-1.28.15/README.md` & `mypy-boto3-pipes-1.28.15.post1/README.md`

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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__init__.py` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__init__.pyi` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__main__.py` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgePipes 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.EventBridgePipes 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes\nOther"
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

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/client.py` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,31 @@
     from mypy_boto3_pipes.client import EventBridgePipesClient
 
     session = Session()
     client: EventBridgePipesClient = session.client("pipes")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PipeStateType, RequestedPipeStateType
 from .paginator import ListPipesPaginator
 from .type_defs import (
     CreatePipeResponseTypeDef,
     DeletePipeResponseTypeDef,
     DescribePipeResponseTypeDef,
     ListPipesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
+    PipeSourceParametersOutputTypeDef,
     PipeSourceParametersTypeDef,
+    PipeTargetParametersOutputTypeDef,
     PipeTargetParametersTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
     UpdatePipeSourceParametersTypeDef,
 )
 
@@ -101,18 +104,24 @@
         Name: str,
         RoleArn: str,
         Source: str,
         Target: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
-        SourceParameters: PipeSourceParametersTypeDef = ...,
+        EnrichmentParameters: Union[
+            PipeEnrichmentParametersTypeDef, PipeEnrichmentParametersOutputTypeDef
+        ] = ...,
+        SourceParameters: Union[
+            PipeSourceParametersTypeDef, PipeSourceParametersOutputTypeDef
+        ] = ...,
         Tags: Mapping[str, str] = ...,
-        TargetParameters: PipeTargetParametersTypeDef = ...
+        TargetParameters: Union[
+            PipeTargetParametersTypeDef, PipeTargetParametersOutputTypeDef
+        ] = ...
     ) -> CreatePipeResponseTypeDef:
         """
         Create a pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.create_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#create_pipe)
         """
@@ -209,18 +218,22 @@
         self,
         *,
         Name: str,
         RoleArn: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
+        EnrichmentParameters: Union[
+            PipeEnrichmentParametersTypeDef, PipeEnrichmentParametersOutputTypeDef
+        ] = ...,
         SourceParameters: UpdatePipeSourceParametersTypeDef = ...,
         Target: str = ...,
-        TargetParameters: PipeTargetParametersTypeDef = ...
+        TargetParameters: Union[
+            PipeTargetParametersTypeDef, PipeTargetParametersOutputTypeDef
+        ] = ...
     ) -> UpdatePipeResponseTypeDef:
         """
         Update an existing pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.update_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#update_pipe)
         """
```

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/client.pyi` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,31 @@
     from mypy_boto3_pipes.client import EventBridgePipesClient
 
     session = Session()
     client: EventBridgePipesClient = session.client("pipes")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PipeStateType, RequestedPipeStateType
 from .paginator import ListPipesPaginator
 from .type_defs import (
     CreatePipeResponseTypeDef,
     DeletePipeResponseTypeDef,
     DescribePipeResponseTypeDef,
     ListPipesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
+    PipeSourceParametersOutputTypeDef,
     PipeSourceParametersTypeDef,
+    PipeTargetParametersOutputTypeDef,
     PipeTargetParametersTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
     UpdatePipeSourceParametersTypeDef,
 )
 
@@ -94,18 +97,24 @@
         Name: str,
         RoleArn: str,
         Source: str,
         Target: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
-        SourceParameters: PipeSourceParametersTypeDef = ...,
+        EnrichmentParameters: Union[
+            PipeEnrichmentParametersTypeDef, PipeEnrichmentParametersOutputTypeDef
+        ] = ...,
+        SourceParameters: Union[
+            PipeSourceParametersTypeDef, PipeSourceParametersOutputTypeDef
+        ] = ...,
         Tags: Mapping[str, str] = ...,
-        TargetParameters: PipeTargetParametersTypeDef = ...
+        TargetParameters: Union[
+            PipeTargetParametersTypeDef, PipeTargetParametersOutputTypeDef
+        ] = ...
     ) -> CreatePipeResponseTypeDef:
         """
         Create a pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.create_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#create_pipe)
         """
@@ -192,18 +201,22 @@
         self,
         *,
         Name: str,
         RoleArn: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
+        EnrichmentParameters: Union[
+            PipeEnrichmentParametersTypeDef, PipeEnrichmentParametersOutputTypeDef
+        ] = ...,
         SourceParameters: UpdatePipeSourceParametersTypeDef = ...,
         Target: str = ...,
-        TargetParameters: PipeTargetParametersTypeDef = ...
+        TargetParameters: Union[
+            PipeTargetParametersTypeDef, PipeTargetParametersOutputTypeDef
+        ] = ...
     ) -> UpdatePipeResponseTypeDef:
         """
         Update an existing pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.update_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#update_pipe)
         """
```

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/literals.py` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/literals.pyi` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/paginator.py` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/paginator.pyi` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/type_defs.py` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/type_defs.pyi` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/PKG-INFO` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.28.15
-Summary: Type annotations for boto3.EventBridgePipes 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EventBridgePipes 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/SOURCES.txt` & `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15/setup.py` & `mypy-boto3-pipes-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pipes",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_pipes"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.EventBridgePipes 1.28.15 service generated with"
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

