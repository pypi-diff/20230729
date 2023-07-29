# Comparing `tmp/mypy-boto3-autoscaling-plans-1.28.15.tar.gz` & `tmp/mypy-boto3-autoscaling-plans-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-plans-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-plans-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-plans-1.28.15.tar` & `mypy-boto3-autoscaling-plans-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.376697 mypy-boto3-autoscaling-plans-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-07-28 20:42:19.364697 mypy-boto3-autoscaling-plans-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.364697 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-07-28 20:20:01.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-07-28 20:20:01.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.364697 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.376697 mypy-boto3-autoscaling-plans-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 20:19:59.000000 mypy-boto3-autoscaling-plans-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.605022 mypy-boto3-autoscaling-plans-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-29 10:02:34.601022 mypy-boto3-autoscaling-plans-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.593021 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-29 09:38:53.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-07-29 09:38:52.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-07-29 09:38:53.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-07-29 09:38:53.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.601022 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:02:34.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.605022 mypy-boto3-autoscaling-plans-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 09:38:51.000000 mypy-boto3-autoscaling-plans-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/LICENSE` & `mypy-boto3-autoscaling-plans-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/PKG-INFO` & `mypy-boto3-autoscaling-plans-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling-plans
-Version: 1.28.15
-Summary: Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/README.md` & `mypy-boto3-autoscaling-plans-1.28.15.post1/README.md`

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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__init__.py` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__init__.pyi` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__main__.py` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScalingPlans 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.AutoScalingPlans 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans\nOther"
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

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/client.py` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ForecastDataTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import DescribeScalingPlanResourcesPaginator, DescribeScalingPlansPaginator
 from .type_defs import (
+    ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
     CreateScalingPlanResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
+    ScalingInstructionOutputTypeDef,
     ScalingInstructionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -90,16 +92,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#close)
         """
 
     def create_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
-        ApplicationSource: ApplicationSourceTypeDef,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef]
+        ApplicationSource: Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef],
+        ScalingInstructions: Sequence[
+            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
+        ]
     ) -> CreateScalingPlanResponseTypeDef:
         """
         Creates a scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#create_scaling_plan)
         """
@@ -130,15 +134,17 @@
         """
 
     def describe_scaling_plans(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
+        ApplicationSources: Sequence[
+            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
+        ] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeScalingPlansResponseTypeDef:
         """
         Describes one or more of your scaling plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)
@@ -179,16 +185,18 @@
         """
 
     def update_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        ApplicationSource: ApplicationSourceTypeDef = ...,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...
+        ApplicationSource: Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef] = ...,
+        ScalingInstructions: Sequence[
+            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#update_scaling_plan)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/client.pyi` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ForecastDataTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import DescribeScalingPlanResourcesPaginator, DescribeScalingPlansPaginator
 from .type_defs import (
+    ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
     CreateScalingPlanResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
+    ScalingInstructionOutputTypeDef,
     ScalingInstructionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -83,16 +85,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#close)
         """
     def create_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
-        ApplicationSource: ApplicationSourceTypeDef,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef]
+        ApplicationSource: Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef],
+        ScalingInstructions: Sequence[
+            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
+        ]
     ) -> CreateScalingPlanResponseTypeDef:
         """
         Creates a scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#create_scaling_plan)
         """
@@ -120,15 +124,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#describe_scaling_plan_resources)
         """
     def describe_scaling_plans(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
+        ApplicationSources: Sequence[
+            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
+        ] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeScalingPlansResponseTypeDef:
         """
         Describes one or more of your scaling plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)
@@ -166,16 +172,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#get_scaling_plan_resource_forecast_data)
         """
     def update_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        ApplicationSource: ApplicationSourceTypeDef = ...,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...
+        ApplicationSource: Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef] = ...,
+        ScalingInstructions: Sequence[
+            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/client/#update_scaling_plan)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/literals.py` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/literals.pyi` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/paginator.py` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,20 @@
     session = Session()
     client: AutoScalingPlansClient = session.client("autoscaling-plans")
 
     describe_scaling_plan_resources_paginator: DescribeScalingPlanResourcesPaginator = client.get_paginator("describe_scaling_plan_resources")
     describe_scaling_plans_paginator: DescribeScalingPlansPaginator = client.get_paginator("describe_scaling_plans")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
+    ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeScalingPlanResourcesPaginator", "DescribeScalingPlansPaginator")
@@ -71,14 +72,16 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
+        ApplicationSources: Sequence[
+            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
+        ] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/paginator.pyi` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,20 @@
     session = Session()
     client: AutoScalingPlansClient = session.client("autoscaling-plans")
 
     describe_scaling_plan_resources_paginator: DescribeScalingPlanResourcesPaginator = client.get_paginator("describe_scaling_plan_resources")
     describe_scaling_plans_paginator: DescribeScalingPlansPaginator = client.get_paginator("describe_scaling_plans")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
+    ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeScalingPlanResourcesPaginator", "DescribeScalingPlansPaginator")
@@ -67,14 +68,16 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
+        ApplicationSources: Sequence[
+            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
+        ] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/type_defs.py` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,26 +379,30 @@
 
 
 DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     {
         "ScalingPlanNames": Sequence[str],
         "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
+        "ApplicationSources": Sequence[
+            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
+        ],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeScalingPlansRequestRequestTypeDef = TypedDict(
     "DescribeScalingPlansRequestRequestTypeDef",
     {
         "ScalingPlanNames": Sequence[str],
         "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
+        "ApplicationSources": Sequence[
+            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
+        ],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
 _RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
@@ -593,30 +597,34 @@
 
 
 CreateScalingPlanRequestRequestTypeDef = TypedDict(
     "CreateScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+        "ScalingInstructions": Sequence[
+            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
+        ],
     },
 )
 
 _RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
 _OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateScalingPlanRequestRequestTypeDef",
     {
         "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+        "ScalingInstructions": Sequence[
+            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateScalingPlanRequestRequestTypeDef(
     _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/type_defs.pyi` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -362,26 +362,30 @@
     pass
 
 DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     {
         "ScalingPlanNames": Sequence[str],
         "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
+        "ApplicationSources": Sequence[
+            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
+        ],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeScalingPlansRequestRequestTypeDef = TypedDict(
     "DescribeScalingPlansRequestRequestTypeDef",
     {
         "ScalingPlanNames": Sequence[str],
         "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
+        "ApplicationSources": Sequence[
+            Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
+        ],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
 _RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
@@ -562,30 +566,34 @@
     pass
 
 CreateScalingPlanRequestRequestTypeDef = TypedDict(
     "CreateScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+        "ScalingInstructions": Sequence[
+            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
+        ],
     },
 )
 
 _RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
 _OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateScalingPlanRequestRequestTypeDef",
     {
         "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+        "ScalingInstructions": Sequence[
+            Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateScalingPlanRequestRequestTypeDef(
     _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling-plans
-Version: 1.28.15
-Summary: Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-plans-1.28.15.post1/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.15/setup.py` & `mypy-boto3-autoscaling-plans-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling-plans",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_autoscaling_plans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with"
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

