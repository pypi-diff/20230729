# Comparing `tmp/mypy-boto3-datapipeline-1.28.15.tar.gz` & `tmp/mypy-boto3-datapipeline-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datapipeline-1.28.15.tar", last modified: Fri Jul 28 20:42:37 2023, max compression
+gzip compressed data, was "mypy-boto3-datapipeline-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:55 2023, max compression
```

## Comparing `mypy-boto3-datapipeline-1.28.15.tar` & `mypy-boto3-datapipeline-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.572955 mypy-boto3-datapipeline-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-07-28 20:42:37.560954 mypy-boto3-datapipeline-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.552954 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-28 20:22:36.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-28 20:22:36.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-28 20:22:36.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-28 20:22:36.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-28 20:22:36.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-07-28 20:22:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18282 2023-07-28 20:22:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.560954 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:37.572955 mypy-boto3-datapipeline-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.265099 mypy-boto3-datapipeline-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-07-29 10:02:55.265099 mypy-boto3-datapipeline-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.265099 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-07-29 09:42:03.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-29 09:42:04.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-29 09:42:04.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-29 09:42:03.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-29 09:42:03.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18460 2023-07-29 09:42:04.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18428 2023-07-29 09:42:04.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.265099 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:02:55.000000 mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:55.265099 mypy-boto3-datapipeline-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:42:02.000000 mypy-boto3-datapipeline-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-datapipeline-1.28.15/LICENSE` & `mypy-boto3-datapipeline-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15/PKG-INFO` & `mypy-boto3-datapipeline-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datapipeline
-Version: 1.28.15
-Summary: Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datapipeline-1.28.15/README.md` & `mypy-boto3-datapipeline-1.28.15.post1/README.md`

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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__init__.py` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__init__.pyi` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__main__.py` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataPipeline 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.DataPipeline 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline\nOther"
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

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/client.py` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,18 @@
     DescribePipelinesOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluateExpressionOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     InstanceIdentityTypeDef,
     ListPipelinesOutputTypeDef,
+    ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
     ParameterValueTypeDef,
+    PipelineObjectOutputTypeDef,
     PipelineObjectTypeDef,
     PollForTaskOutputTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     QueryObjectsOutputTypeDef,
     QueryTypeDef,
     ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatOutputTypeDef,
@@ -233,16 +235,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#poll_for_task)
         """
 
     def put_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[PipelineObjectTypeDef],
-        parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
+        pipelineObjects: Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
+        parameterObjects: Sequence[
+            Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
+        ] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> PutPipelineDefinitionOutputTypeDef:
         """
         Adds tasks, schedules, and preconditions to the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.put_pipeline_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#put_pipeline_definition)
@@ -323,16 +327,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#set_task_status)
         """
 
     def validate_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[PipelineObjectTypeDef],
-        parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
+        pipelineObjects: Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
+        parameterObjects: Sequence[
+            Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
+        ] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> ValidatePipelineDefinitionOutputTypeDef:
         """
         Validates the specified pipeline definition to ensure that it is well formed and
         can be run without error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.validate_pipeline_definition)
```

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/client.pyi` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,18 @@
     DescribePipelinesOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluateExpressionOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     InstanceIdentityTypeDef,
     ListPipelinesOutputTypeDef,
+    ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
     ParameterValueTypeDef,
+    PipelineObjectOutputTypeDef,
     PipelineObjectTypeDef,
     PollForTaskOutputTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     QueryObjectsOutputTypeDef,
     QueryTypeDef,
     ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatOutputTypeDef,
@@ -214,16 +216,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.poll_for_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#poll_for_task)
         """
     def put_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[PipelineObjectTypeDef],
-        parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
+        pipelineObjects: Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
+        parameterObjects: Sequence[
+            Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
+        ] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> PutPipelineDefinitionOutputTypeDef:
         """
         Adds tasks, schedules, and preconditions to the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.put_pipeline_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#put_pipeline_definition)
@@ -297,16 +301,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.set_task_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/client/#set_task_status)
         """
     def validate_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[PipelineObjectTypeDef],
-        parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
+        pipelineObjects: Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
+        parameterObjects: Sequence[
+            Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
+        ] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> ValidatePipelineDefinitionOutputTypeDef:
         """
         Validates the specified pipeline definition to ensure that it is well formed and
         can be run without error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.validate_pipeline_definition)
```

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/literals.py` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/literals.pyi` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/paginator.py` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/paginator.pyi` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/type_defs.py` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -672,21 +672,21 @@
     },
 )
 
 _RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredPutPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
-        "pipelineObjects": Sequence[PipelineObjectTypeDef],
+        "pipelineObjects": Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
     },
 )
 _OptionalPutPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_OptionalPutPipelineDefinitionInputRequestTypeDef",
     {
-        "parameterObjects": Sequence[ParameterObjectTypeDef],
+        "parameterObjects": Sequence[Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]],
         "parameterValues": Sequence[ParameterValueTypeDef],
     },
     total=False,
 )
 
 
 class PutPipelineDefinitionInputRequestTypeDef(
@@ -696,21 +696,21 @@
     pass
 
 
 _RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
-        "pipelineObjects": Sequence[PipelineObjectTypeDef],
+        "pipelineObjects": Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
     },
 )
 _OptionalValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
     "_OptionalValidatePipelineDefinitionInputRequestTypeDef",
     {
-        "parameterObjects": Sequence[ParameterObjectTypeDef],
+        "parameterObjects": Sequence[Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]],
         "parameterValues": Sequence[ParameterValueTypeDef],
     },
     total=False,
 )
 
 
 class ValidatePipelineDefinitionInputRequestTypeDef(
```

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/type_defs.pyi` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -647,21 +647,21 @@
     },
 )
 
 _RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredPutPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
-        "pipelineObjects": Sequence[PipelineObjectTypeDef],
+        "pipelineObjects": Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
     },
 )
 _OptionalPutPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_OptionalPutPipelineDefinitionInputRequestTypeDef",
     {
-        "parameterObjects": Sequence[ParameterObjectTypeDef],
+        "parameterObjects": Sequence[Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]],
         "parameterValues": Sequence[ParameterValueTypeDef],
     },
     total=False,
 )
 
 class PutPipelineDefinitionInputRequestTypeDef(
     _RequiredPutPipelineDefinitionInputRequestTypeDef,
@@ -669,21 +669,21 @@
 ):
     pass
 
 _RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
-        "pipelineObjects": Sequence[PipelineObjectTypeDef],
+        "pipelineObjects": Sequence[Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]],
     },
 )
 _OptionalValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
     "_OptionalValidatePipelineDefinitionInputRequestTypeDef",
     {
-        "parameterObjects": Sequence[ParameterObjectTypeDef],
+        "parameterObjects": Sequence[Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]],
         "parameterValues": Sequence[ParameterValueTypeDef],
     },
     total=False,
 )
 
 class ValidatePipelineDefinitionInputRequestTypeDef(
     _RequiredValidatePipelineDefinitionInputRequestTypeDef,
```

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/PKG-INFO` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datapipeline
-Version: 1.28.15
-Summary: Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/SOURCES.txt` & `mypy-boto3-datapipeline-1.28.15.post1/mypy_boto3_datapipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.15/setup.py` & `mypy-boto3-datapipeline-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datapipeline",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_datapipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder"
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

