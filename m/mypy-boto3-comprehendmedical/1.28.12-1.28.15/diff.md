# Comparing `tmp/mypy-boto3-comprehendmedical-1.28.12.tar.gz` & `tmp/mypy-boto3-comprehendmedical-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-comprehendmedical-1.28.12.tar", last modified: Thu Jul 27 05:34:30 2023, max compression
+gzip compressed data, was "mypy-boto3-comprehendmedical-1.28.15.tar", last modified: Fri Jul 28 20:42:31 2023, max compression
```

## Comparing `mypy-boto3-comprehendmedical-1.28.12.tar` & `mypy-boto3-comprehendmedical-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.620545 mypy-boto3-comprehendmedical-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15900 2023-07-27 05:34:30.620545 mypy-boto3-comprehendmedical-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.620545 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-07-27 05:19:29.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25853 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.620545 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15900 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:30.620545 mypy-boto3-comprehendmedical-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.808871 mypy-boto3-comprehendmedical-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-07-28 20:42:31.808871 mypy-boto3-comprehendmedical-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.800871 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24890 2023-07-28 20:22:04.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-07-28 20:22:04.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.804871 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-07-28 20:42:31.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 20:42:31.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:31.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:31.000000 mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:31.808871 mypy-boto3-comprehendmedical-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-28 20:22:03.000000 mypy-boto3-comprehendmedical-1.28.15/setup.py
```

### Comparing `mypy-boto3-comprehendmedical-1.28.12/LICENSE` & `mypy-boto3-comprehendmedical-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.12/PKG-INFO` & `mypy-boto3-comprehendmedical-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehendmedical
-Version: 1.28.12
-Summary: Type annotations for boto3.ComprehendMedical 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ComprehendMedical 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehendmedical)](https://pepy.tech/project/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,65 +320,63 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
     ComprehendMedicalAsyncJobFilterTypeDef,
-    InputDataConfigOutputTypeDef,
-    OutputDataConfigOutputTypeDef,
+    InputDataConfigTypeDef,
+    OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
-    InputDataConfigTypeDef,
-    OutputDataConfigTypeDef,
-    ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
-    StartEntitiesDetectionV2JobResponseTypeDef,
-    StartICD10CMInferenceJobResponseTypeDef,
-    StartPHIDetectionJobResponseTypeDef,
-    StartRxNormInferenceJobResponseTypeDef,
-    StartSNOMEDCTInferenceJobResponseTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
-    StopEntitiesDetectionV2JobResponseTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
-    StopICD10CMInferenceJobResponseTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
-    StopPHIDetectionJobResponseTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
-    StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
-    StopSNOMEDCTInferenceJobResponseTypeDef,
     AttributeTypeDef,
     ListEntitiesDetectionV2JobsRequestRequestTypeDef,
     ListICD10CMInferenceJobsRequestRequestTypeDef,
     ListPHIDetectionJobsRequestRequestTypeDef,
     ListRxNormInferenceJobsRequestRequestTypeDef,
     ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
-    ICD10CMAttributeTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
+    StartEntitiesDetectionV2JobResponseTypeDef,
+    StartICD10CMInferenceJobResponseTypeDef,
+    StartPHIDetectionJobResponseTypeDef,
+    StartRxNormInferenceJobResponseTypeDef,
+    StartSNOMEDCTInferenceJobResponseTypeDef,
+    StopEntitiesDetectionV2JobResponseTypeDef,
+    StopICD10CMInferenceJobResponseTypeDef,
+    StopPHIDetectionJobResponseTypeDef,
+    StopRxNormInferenceJobResponseTypeDef,
+    StopSNOMEDCTInferenceJobResponseTypeDef,
+    ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
```

### Comparing `mypy-boto3-comprehendmedical-1.28.12/README.md` & `mypy-boto3-comprehendmedical-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehendmedical)](https://pepy.tech/project/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,65 +288,63 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
     ComprehendMedicalAsyncJobFilterTypeDef,
-    InputDataConfigOutputTypeDef,
-    OutputDataConfigOutputTypeDef,
+    InputDataConfigTypeDef,
+    OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
-    InputDataConfigTypeDef,
-    OutputDataConfigTypeDef,
-    ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
-    StartEntitiesDetectionV2JobResponseTypeDef,
-    StartICD10CMInferenceJobResponseTypeDef,
-    StartPHIDetectionJobResponseTypeDef,
-    StartRxNormInferenceJobResponseTypeDef,
-    StartSNOMEDCTInferenceJobResponseTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
-    StopEntitiesDetectionV2JobResponseTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
-    StopICD10CMInferenceJobResponseTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
-    StopPHIDetectionJobResponseTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
-    StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
-    StopSNOMEDCTInferenceJobResponseTypeDef,
     AttributeTypeDef,
     ListEntitiesDetectionV2JobsRequestRequestTypeDef,
     ListICD10CMInferenceJobsRequestRequestTypeDef,
     ListPHIDetectionJobsRequestRequestTypeDef,
     ListRxNormInferenceJobsRequestRequestTypeDef,
     ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
-    ICD10CMAttributeTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
+    StartEntitiesDetectionV2JobResponseTypeDef,
+    StartICD10CMInferenceJobResponseTypeDef,
+    StartPHIDetectionJobResponseTypeDef,
+    StartRxNormInferenceJobResponseTypeDef,
+    StartSNOMEDCTInferenceJobResponseTypeDef,
+    StopEntitiesDetectionV2JobResponseTypeDef,
+    StopICD10CMInferenceJobResponseTypeDef,
+    StopPHIDetectionJobResponseTypeDef,
+    StopRxNormInferenceJobResponseTypeDef,
+    StopSNOMEDCTInferenceJobResponseTypeDef,
+    ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
```

### Comparing `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/__main__.py` & `mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ComprehendMedical 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ComprehendMedical 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/client.py` & `mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/client.pyi` & `mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/literals.py` & `mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/literals.pyi` & `mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/type_defs.py` & `mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,70 +40,67 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TraitTypeDef",
     "CharactersTypeDef",
     "ComprehendMedicalAsyncJobFilterTypeDef",
-    "InputDataConfigOutputTypeDef",
-    "OutputDataConfigOutputTypeDef",
+    "InputDataConfigTypeDef",
+    "OutputDataConfigTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     "DescribePHIDetectionJobRequestRequestTypeDef",
     "DescribeRxNormInferenceJobRequestRequestTypeDef",
     "DescribeSNOMEDCTInferenceJobRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "DetectEntitiesV2RequestRequestTypeDef",
     "DetectPHIRequestRequestTypeDef",
     "ICD10CMTraitTypeDef",
     "ICD10CMConceptTypeDef",
     "InferICD10CMRequestRequestTypeDef",
     "InferRxNormRequestRequestTypeDef",
     "InferSNOMEDCTRequestRequestTypeDef",
     "SNOMEDCTDetailsTypeDef",
-    "InputDataConfigTypeDef",
-    "OutputDataConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RxNormTraitTypeDef",
     "RxNormConceptTypeDef",
     "SNOMEDCTConceptTypeDef",
     "SNOMEDCTTraitTypeDef",
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    "StartICD10CMInferenceJobResponseTypeDef",
-    "StartPHIDetectionJobResponseTypeDef",
-    "StartRxNormInferenceJobResponseTypeDef",
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
-    "StopEntitiesDetectionV2JobResponseTypeDef",
     "StopICD10CMInferenceJobRequestRequestTypeDef",
-    "StopICD10CMInferenceJobResponseTypeDef",
     "StopPHIDetectionJobRequestRequestTypeDef",
-    "StopPHIDetectionJobResponseTypeDef",
     "StopRxNormInferenceJobRequestRequestTypeDef",
-    "StopRxNormInferenceJobResponseTypeDef",
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
     "AttributeTypeDef",
     "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
     "ListICD10CMInferenceJobsRequestRequestTypeDef",
     "ListPHIDetectionJobsRequestRequestTypeDef",
     "ListRxNormInferenceJobsRequestRequestTypeDef",
     "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
-    "ICD10CMAttributeTypeDef",
     "StartEntitiesDetectionV2JobRequestRequestTypeDef",
     "StartICD10CMInferenceJobRequestRequestTypeDef",
     "StartPHIDetectionJobRequestRequestTypeDef",
     "StartRxNormInferenceJobRequestRequestTypeDef",
     "StartSNOMEDCTInferenceJobRequestRequestTypeDef",
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    "StartICD10CMInferenceJobResponseTypeDef",
+    "StartPHIDetectionJobResponseTypeDef",
+    "StartRxNormInferenceJobResponseTypeDef",
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
+    "StopEntitiesDetectionV2JobResponseTypeDef",
+    "StopICD10CMInferenceJobResponseTypeDef",
+    "StopPHIDetectionJobResponseTypeDef",
+    "StopRxNormInferenceJobResponseTypeDef",
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
+    "ICD10CMAttributeTypeDef",
     "RxNormAttributeTypeDef",
     "SNOMEDCTAttributeTypeDef",
     "EntityTypeDef",
     "UnmappedAttributeTypeDef",
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     "DescribeICD10CMInferenceJobResponseTypeDef",
     "DescribePHIDetectionJobResponseTypeDef",
@@ -149,63 +146,66 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredInputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredInputDataConfigOutputTypeDef",
+_RequiredInputDataConfigTypeDef = TypedDict(
+    "_RequiredInputDataConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalInputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalInputDataConfigOutputTypeDef",
+_OptionalInputDataConfigTypeDef = TypedDict(
+    "_OptionalInputDataConfigTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
-
-class InputDataConfigOutputTypeDef(
-    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
-):
+class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
-
-_RequiredOutputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredOutputDataConfigOutputTypeDef",
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalOutputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalOutputDataConfigOutputTypeDef",
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
-
-class OutputDataConfigOutputTypeDef(
-    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
-):
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
-
 DescribeEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 DescribeICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -297,63 +297,14 @@
         "Edition": str,
         "Language": str,
         "VersionDate": str,
     },
     total=False,
 )
 
-_RequiredInputDataConfigTypeDef = TypedDict(
-    "_RequiredInputDataConfigTypeDef",
-    {
-        "S3Bucket": str,
-    },
-)
-_OptionalInputDataConfigTypeDef = TypedDict(
-    "_OptionalInputDataConfigTypeDef",
-    {
-        "S3Key": str,
-    },
-    total=False,
-)
-
-
-class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
-    pass
-
-
-_RequiredOutputDataConfigTypeDef = TypedDict(
-    "_RequiredOutputDataConfigTypeDef",
-    {
-        "S3Bucket": str,
-    },
-)
-_OptionalOutputDataConfigTypeDef = TypedDict(
-    "_OptionalOutputDataConfigTypeDef",
-    {
-        "S3Key": str,
-    },
-    total=False,
-)
-
-
-class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
-    pass
-
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RxNormTraitTypeDef = TypedDict(
     "RxNormTraitTypeDef",
     {
         "Name": RxNormTraitNameType,
         "Score": float,
     },
     total=False,
@@ -384,129 +335,49 @@
     {
         "Name": SNOMEDCTTraitNameType,
         "Score": float,
     },
     total=False,
 )
 
-StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StartICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartPHIDetectionJobResponseTypeDef = TypedDict(
-    "StartPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StartRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "StopICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StopICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopPHIDetectionJobRequestRequestTypeDef = TypedDict(
     "StopPHIDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopPHIDetectionJobResponseTypeDef = TypedDict(
-    "StopPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopRxNormInferenceJobRequestRequestTypeDef = TypedDict(
     "StopRxNormInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StopRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopSNOMEDCTInferenceJobRequestRequestTypeDef = TypedDict(
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "Type": EntitySubTypeType,
         "Score": float,
         "RelationshipScore": float,
         "RelationshipType": RelationshipTypeType,
@@ -576,42 +447,25 @@
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "ExpirationTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": Literal["en"],
         "DataAccessRoleArn": str,
         "ManifestFilePath": str,
         "KMSKey": str,
         "ModelVersion": str,
     },
     total=False,
 )
 
-ICD10CMAttributeTypeDef = TypedDict(
-    "ICD10CMAttributeTypeDef",
-    {
-        "Type": ICD10CMAttributeTypeType,
-        "Score": float,
-        "RelationshipScore": float,
-        "Id": int,
-        "BeginOffset": int,
-        "EndOffset": int,
-        "Text": str,
-        "Traits": List[ICD10CMTraitTypeDef],
-        "Category": ICD10CMEntityTypeType,
-        "RelationshipType": ICD10CMRelationshipTypeType,
-    },
-    total=False,
-)
-
 _RequiredStartEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -623,22 +477,20 @@
         "JobName": str,
         "ClientRequestToken": str,
         "KMSKey": str,
     },
     total=False,
 )
 
-
 class StartEntitiesDetectionV2JobRequestRequestTypeDef(
     _RequiredStartEntitiesDetectionV2JobRequestRequestTypeDef,
     _OptionalStartEntitiesDetectionV2JobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartICD10CMInferenceJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -650,22 +502,20 @@
         "JobName": str,
         "ClientRequestToken": str,
         "KMSKey": str,
     },
     total=False,
 )
 
-
 class StartICD10CMInferenceJobRequestRequestTypeDef(
     _RequiredStartICD10CMInferenceJobRequestRequestTypeDef,
     _OptionalStartICD10CMInferenceJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartPHIDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartPHIDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -677,22 +527,20 @@
         "JobName": str,
         "ClientRequestToken": str,
         "KMSKey": str,
     },
     total=False,
 )
 
-
 class StartPHIDetectionJobRequestRequestTypeDef(
     _RequiredStartPHIDetectionJobRequestRequestTypeDef,
     _OptionalStartPHIDetectionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartRxNormInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartRxNormInferenceJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -704,22 +552,20 @@
         "JobName": str,
         "ClientRequestToken": str,
         "KMSKey": str,
     },
     total=False,
 )
 
-
 class StartRxNormInferenceJobRequestRequestTypeDef(
     _RequiredStartRxNormInferenceJobRequestRequestTypeDef,
     _OptionalStartRxNormInferenceJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -731,21 +577,116 @@
         "JobName": str,
         "ClientRequestToken": str,
         "KMSKey": str,
     },
     total=False,
 )
 
-
 class StartSNOMEDCTInferenceJobRequestRequestTypeDef(
     _RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef,
     _OptionalStartSNOMEDCTInferenceJobRequestRequestTypeDef,
 ):
     pass
 
+StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StartICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartPHIDetectionJobResponseTypeDef = TypedDict(
+    "StartPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StartRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StopICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopPHIDetectionJobResponseTypeDef = TypedDict(
+    "StopPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StopRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ICD10CMAttributeTypeDef = TypedDict(
+    "ICD10CMAttributeTypeDef",
+    {
+        "Type": ICD10CMAttributeTypeType,
+        "Score": float,
+        "RelationshipScore": float,
+        "Id": int,
+        "BeginOffset": int,
+        "EndOffset": int,
+        "Text": str,
+        "Traits": List[ICD10CMTraitTypeDef],
+        "Category": ICD10CMEntityTypeType,
+        "RelationshipType": ICD10CMRelationshipTypeType,
+    },
+    total=False,
+)
 
 RxNormAttributeTypeDef = TypedDict(
     "RxNormAttributeTypeDef",
     {
         "Type": RxNormAttributeTypeType,
         "Score": float,
         "RelationshipScore": float,
@@ -801,92 +742,92 @@
     total=False,
 )
 
 DescribeEntitiesDetectionV2JobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeICD10CMInferenceJobResponseTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePHIDetectionJobResponseTypeDef = TypedDict(
     "DescribePHIDetectionJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRxNormInferenceJobResponseTypeDef = TypedDict(
     "DescribeRxNormInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
     "DescribeSNOMEDCTInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesDetectionV2JobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionV2JobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListICD10CMInferenceJobsResponseTypeDef = TypedDict(
     "ListICD10CMInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPHIDetectionJobsResponseTypeDef = TypedDict(
     "ListPHIDetectionJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRxNormInferenceJobsResponseTypeDef = TypedDict(
     "ListRxNormInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSNOMEDCTInferenceJobsResponseTypeDef = TypedDict(
     "ListSNOMEDCTInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ICD10CMEntityTypeDef = TypedDict(
     "ICD10CMEntityTypeDef",
     {
         "Id": int,
@@ -939,64 +880,64 @@
 
 DetectPHIResponseTypeDef = TypedDict(
     "DetectPHIResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectEntitiesResponseTypeDef = TypedDict(
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectEntitiesV2ResponseTypeDef = TypedDict(
     "DetectEntitiesV2ResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferICD10CMResponseTypeDef = TypedDict(
     "InferICD10CMResponseTypeDef",
     {
         "Entities": List[ICD10CMEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferRxNormResponseTypeDef = TypedDict(
     "InferRxNormResponseTypeDef",
     {
         "Entities": List[RxNormEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferSNOMEDCTResponseTypeDef = TypedDict(
     "InferSNOMEDCTResponseTypeDef",
     {
         "Entities": List[SNOMEDCTEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
         "SNOMEDCTDetails": SNOMEDCTDetailsTypeDef,
         "Characters": CharactersTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/type_defs.pyi` & `mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,69 +40,68 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TraitTypeDef",
     "CharactersTypeDef",
     "ComprehendMedicalAsyncJobFilterTypeDef",
-    "InputDataConfigOutputTypeDef",
-    "OutputDataConfigOutputTypeDef",
+    "InputDataConfigTypeDef",
+    "OutputDataConfigTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     "DescribePHIDetectionJobRequestRequestTypeDef",
     "DescribeRxNormInferenceJobRequestRequestTypeDef",
     "DescribeSNOMEDCTInferenceJobRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "DetectEntitiesV2RequestRequestTypeDef",
     "DetectPHIRequestRequestTypeDef",
     "ICD10CMTraitTypeDef",
     "ICD10CMConceptTypeDef",
     "InferICD10CMRequestRequestTypeDef",
     "InferRxNormRequestRequestTypeDef",
     "InferSNOMEDCTRequestRequestTypeDef",
     "SNOMEDCTDetailsTypeDef",
-    "InputDataConfigTypeDef",
-    "OutputDataConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RxNormTraitTypeDef",
     "RxNormConceptTypeDef",
     "SNOMEDCTConceptTypeDef",
     "SNOMEDCTTraitTypeDef",
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    "StartICD10CMInferenceJobResponseTypeDef",
-    "StartPHIDetectionJobResponseTypeDef",
-    "StartRxNormInferenceJobResponseTypeDef",
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
-    "StopEntitiesDetectionV2JobResponseTypeDef",
     "StopICD10CMInferenceJobRequestRequestTypeDef",
-    "StopICD10CMInferenceJobResponseTypeDef",
     "StopPHIDetectionJobRequestRequestTypeDef",
-    "StopPHIDetectionJobResponseTypeDef",
     "StopRxNormInferenceJobRequestRequestTypeDef",
-    "StopRxNormInferenceJobResponseTypeDef",
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
     "AttributeTypeDef",
     "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
     "ListICD10CMInferenceJobsRequestRequestTypeDef",
     "ListPHIDetectionJobsRequestRequestTypeDef",
     "ListRxNormInferenceJobsRequestRequestTypeDef",
     "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
-    "ICD10CMAttributeTypeDef",
     "StartEntitiesDetectionV2JobRequestRequestTypeDef",
     "StartICD10CMInferenceJobRequestRequestTypeDef",
     "StartPHIDetectionJobRequestRequestTypeDef",
     "StartRxNormInferenceJobRequestRequestTypeDef",
     "StartSNOMEDCTInferenceJobRequestRequestTypeDef",
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    "StartICD10CMInferenceJobResponseTypeDef",
+    "StartPHIDetectionJobResponseTypeDef",
+    "StartRxNormInferenceJobResponseTypeDef",
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
+    "StopEntitiesDetectionV2JobResponseTypeDef",
+    "StopICD10CMInferenceJobResponseTypeDef",
+    "StopPHIDetectionJobResponseTypeDef",
+    "StopRxNormInferenceJobResponseTypeDef",
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
+    "ICD10CMAttributeTypeDef",
     "RxNormAttributeTypeDef",
     "SNOMEDCTAttributeTypeDef",
     "EntityTypeDef",
     "UnmappedAttributeTypeDef",
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     "DescribeICD10CMInferenceJobResponseTypeDef",
     "DescribePHIDetectionJobResponseTypeDef",
@@ -148,59 +147,70 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredInputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredInputDataConfigOutputTypeDef",
+_RequiredInputDataConfigTypeDef = TypedDict(
+    "_RequiredInputDataConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalInputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalInputDataConfigOutputTypeDef",
+_OptionalInputDataConfigTypeDef = TypedDict(
+    "_OptionalInputDataConfigTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
-class InputDataConfigOutputTypeDef(
-    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
-):
+
+class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
-_RequiredOutputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredOutputDataConfigOutputTypeDef",
+
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalOutputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalOutputDataConfigOutputTypeDef",
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
-class OutputDataConfigOutputTypeDef(
-    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
-):
+
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
+
 DescribeEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 DescribeICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -292,59 +302,14 @@
         "Edition": str,
         "Language": str,
         "VersionDate": str,
     },
     total=False,
 )
 
-_RequiredInputDataConfigTypeDef = TypedDict(
-    "_RequiredInputDataConfigTypeDef",
-    {
-        "S3Bucket": str,
-    },
-)
-_OptionalInputDataConfigTypeDef = TypedDict(
-    "_OptionalInputDataConfigTypeDef",
-    {
-        "S3Key": str,
-    },
-    total=False,
-)
-
-class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
-    pass
-
-_RequiredOutputDataConfigTypeDef = TypedDict(
-    "_RequiredOutputDataConfigTypeDef",
-    {
-        "S3Bucket": str,
-    },
-)
-_OptionalOutputDataConfigTypeDef = TypedDict(
-    "_OptionalOutputDataConfigTypeDef",
-    {
-        "S3Key": str,
-    },
-    total=False,
-)
-
-class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
-    pass
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RxNormTraitTypeDef = TypedDict(
     "RxNormTraitTypeDef",
     {
         "Name": RxNormTraitNameType,
         "Score": float,
     },
     total=False,
@@ -375,129 +340,49 @@
     {
         "Name": SNOMEDCTTraitNameType,
         "Score": float,
     },
     total=False,
 )
 
-StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StartICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartPHIDetectionJobResponseTypeDef = TypedDict(
-    "StartPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StartRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "StopICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StopICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopPHIDetectionJobRequestRequestTypeDef = TypedDict(
     "StopPHIDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopPHIDetectionJobResponseTypeDef = TypedDict(
-    "StopPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopRxNormInferenceJobRequestRequestTypeDef = TypedDict(
     "StopRxNormInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StopRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopSNOMEDCTInferenceJobRequestRequestTypeDef = TypedDict(
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "Type": EntitySubTypeType,
         "Score": float,
         "RelationshipScore": float,
         "RelationshipType": RelationshipTypeType,
@@ -567,42 +452,25 @@
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "ExpirationTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "LanguageCode": Literal["en"],
         "DataAccessRoleArn": str,
         "ManifestFilePath": str,
         "KMSKey": str,
         "ModelVersion": str,
     },
     total=False,
 )
 
-ICD10CMAttributeTypeDef = TypedDict(
-    "ICD10CMAttributeTypeDef",
-    {
-        "Type": ICD10CMAttributeTypeType,
-        "Score": float,
-        "RelationshipScore": float,
-        "Id": int,
-        "BeginOffset": int,
-        "EndOffset": int,
-        "Text": str,
-        "Traits": List[ICD10CMTraitTypeDef],
-        "Category": ICD10CMEntityTypeType,
-        "RelationshipType": ICD10CMRelationshipTypeType,
-    },
-    total=False,
-)
-
 _RequiredStartEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -614,20 +482,22 @@
         "JobName": str,
         "ClientRequestToken": str,
         "KMSKey": str,
     },
     total=False,
 )
 
+
 class StartEntitiesDetectionV2JobRequestRequestTypeDef(
     _RequiredStartEntitiesDetectionV2JobRequestRequestTypeDef,
     _OptionalStartEntitiesDetectionV2JobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartICD10CMInferenceJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -639,20 +509,22 @@
         "JobName": str,
         "ClientRequestToken": str,
         "KMSKey": str,
     },
     total=False,
 )
 
+
 class StartICD10CMInferenceJobRequestRequestTypeDef(
     _RequiredStartICD10CMInferenceJobRequestRequestTypeDef,
     _OptionalStartICD10CMInferenceJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartPHIDetectionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartPHIDetectionJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -664,20 +536,22 @@
         "JobName": str,
         "ClientRequestToken": str,
         "KMSKey": str,
     },
     total=False,
 )
 
+
 class StartPHIDetectionJobRequestRequestTypeDef(
     _RequiredStartPHIDetectionJobRequestRequestTypeDef,
     _OptionalStartPHIDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartRxNormInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartRxNormInferenceJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -689,20 +563,22 @@
         "JobName": str,
         "ClientRequestToken": str,
         "KMSKey": str,
     },
     total=False,
 )
 
+
 class StartRxNormInferenceJobRequestRequestTypeDef(
     _RequiredStartRxNormInferenceJobRequestRequestTypeDef,
     _OptionalStartRxNormInferenceJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -714,20 +590,119 @@
         "JobName": str,
         "ClientRequestToken": str,
         "KMSKey": str,
     },
     total=False,
 )
 
+
 class StartSNOMEDCTInferenceJobRequestRequestTypeDef(
     _RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef,
     _OptionalStartSNOMEDCTInferenceJobRequestRequestTypeDef,
 ):
     pass
 
+
+StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StartICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartPHIDetectionJobResponseTypeDef = TypedDict(
+    "StartPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StartRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StopICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopPHIDetectionJobResponseTypeDef = TypedDict(
+    "StopPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StopRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ICD10CMAttributeTypeDef = TypedDict(
+    "ICD10CMAttributeTypeDef",
+    {
+        "Type": ICD10CMAttributeTypeType,
+        "Score": float,
+        "RelationshipScore": float,
+        "Id": int,
+        "BeginOffset": int,
+        "EndOffset": int,
+        "Text": str,
+        "Traits": List[ICD10CMTraitTypeDef],
+        "Category": ICD10CMEntityTypeType,
+        "RelationshipType": ICD10CMRelationshipTypeType,
+    },
+    total=False,
+)
+
 RxNormAttributeTypeDef = TypedDict(
     "RxNormAttributeTypeDef",
     {
         "Type": RxNormAttributeTypeType,
         "Score": float,
         "RelationshipScore": float,
         "Id": int,
@@ -782,92 +757,92 @@
     total=False,
 )
 
 DescribeEntitiesDetectionV2JobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeICD10CMInferenceJobResponseTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePHIDetectionJobResponseTypeDef = TypedDict(
     "DescribePHIDetectionJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRxNormInferenceJobResponseTypeDef = TypedDict(
     "DescribeRxNormInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
     "DescribeSNOMEDCTInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesDetectionV2JobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionV2JobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListICD10CMInferenceJobsResponseTypeDef = TypedDict(
     "ListICD10CMInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPHIDetectionJobsResponseTypeDef = TypedDict(
     "ListPHIDetectionJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRxNormInferenceJobsResponseTypeDef = TypedDict(
     "ListRxNormInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSNOMEDCTInferenceJobsResponseTypeDef = TypedDict(
     "ListSNOMEDCTInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ICD10CMEntityTypeDef = TypedDict(
     "ICD10CMEntityTypeDef",
     {
         "Id": int,
@@ -920,64 +895,64 @@
 
 DetectPHIResponseTypeDef = TypedDict(
     "DetectPHIResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectEntitiesResponseTypeDef = TypedDict(
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectEntitiesV2ResponseTypeDef = TypedDict(
     "DetectEntitiesV2ResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferICD10CMResponseTypeDef = TypedDict(
     "InferICD10CMResponseTypeDef",
     {
         "Entities": List[ICD10CMEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferRxNormResponseTypeDef = TypedDict(
     "InferRxNormResponseTypeDef",
     {
         "Entities": List[RxNormEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferSNOMEDCTResponseTypeDef = TypedDict(
     "InferSNOMEDCTResponseTypeDef",
     {
         "Entities": List[SNOMEDCTEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
         "SNOMEDCTDetails": SNOMEDCTDetailsTypeDef,
         "Characters": CharactersTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/PKG-INFO` & `mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehendmedical
-Version: 1.28.12
-Summary: Type annotations for boto3.ComprehendMedical 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ComprehendMedical 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehendmedical)](https://pepy.tech/project/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,65 +320,63 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
     ComprehendMedicalAsyncJobFilterTypeDef,
-    InputDataConfigOutputTypeDef,
-    OutputDataConfigOutputTypeDef,
+    InputDataConfigTypeDef,
+    OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
-    InputDataConfigTypeDef,
-    OutputDataConfigTypeDef,
-    ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
-    StartEntitiesDetectionV2JobResponseTypeDef,
-    StartICD10CMInferenceJobResponseTypeDef,
-    StartPHIDetectionJobResponseTypeDef,
-    StartRxNormInferenceJobResponseTypeDef,
-    StartSNOMEDCTInferenceJobResponseTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
-    StopEntitiesDetectionV2JobResponseTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
-    StopICD10CMInferenceJobResponseTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
-    StopPHIDetectionJobResponseTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
-    StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
-    StopSNOMEDCTInferenceJobResponseTypeDef,
     AttributeTypeDef,
     ListEntitiesDetectionV2JobsRequestRequestTypeDef,
     ListICD10CMInferenceJobsRequestRequestTypeDef,
     ListPHIDetectionJobsRequestRequestTypeDef,
     ListRxNormInferenceJobsRequestRequestTypeDef,
     ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
-    ICD10CMAttributeTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
+    StartEntitiesDetectionV2JobResponseTypeDef,
+    StartICD10CMInferenceJobResponseTypeDef,
+    StartPHIDetectionJobResponseTypeDef,
+    StartRxNormInferenceJobResponseTypeDef,
+    StartSNOMEDCTInferenceJobResponseTypeDef,
+    StopEntitiesDetectionV2JobResponseTypeDef,
+    StopICD10CMInferenceJobResponseTypeDef,
+    StopPHIDetectionJobResponseTypeDef,
+    StopRxNormInferenceJobResponseTypeDef,
+    StopSNOMEDCTInferenceJobResponseTypeDef,
+    ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
```

### Comparing `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt` & `mypy-boto3-comprehendmedical-1.28.15/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.12/setup.py` & `mypy-boto3-comprehendmedical-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-comprehendmedical",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_comprehendmedical"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ComprehendMedical 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ComprehendMedical 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

