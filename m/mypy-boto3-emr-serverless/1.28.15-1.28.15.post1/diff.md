# Comparing `tmp/mypy-boto3-emr-serverless-1.28.15.tar.gz` & `tmp/mypy-boto3-emr-serverless-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-serverless-1.28.15.tar", last modified: Fri Jul 28 20:42:47 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-serverless-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:06 2023, max compression
```

## Comparing `mypy-boto3-emr-serverless-1.28.15.tar` & `mypy-boto3-emr-serverless-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.081086 mypy-boto3-emr-serverless-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-28 20:42:47.081086 mypy-boto3-emr-serverless-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.077087 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23608 2023-07-28 20:25:33.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23567 2023-07-28 20:25:32.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.081086 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:46.000000 mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:47.081086 mypy-boto3-emr-serverless-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:25:31.000000 mypy-boto3-emr-serverless-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.157143 mypy-boto3-emr-serverless-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-07-29 10:03:06.149143 mypy-boto3-emr-serverless-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.141143 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14559 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23608 2023-07-29 09:45:04.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23567 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.149143 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:06.157143 mypy-boto3-emr-serverless-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 09:45:02.000000 mypy-boto3-emr-serverless-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-emr-serverless-1.28.15/LICENSE` & `mypy-boto3-emr-serverless-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15/PKG-INFO` & `mypy-boto3-emr-serverless-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.28.15
-Summary: Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
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
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-serverless-1.28.15/README.md` & `mypy-boto3-emr-serverless-1.28.15.post1/README.md`

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
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__init__.py` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__init__.pyi` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/__main__.py` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRServerless 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.EMRServerless 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
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

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/client.py` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,29 @@
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 from .paginator import ListApplicationsPaginator, ListJobRunsPaginator
 from .type_defs import (
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunResponseTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     GetJobRunResponseTypeDef,
     ImageConfigurationInputTypeDef,
     InitialCapacityConfigTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaximumAllowedResourcesTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     StartJobRunResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -118,15 +121,17 @@
         clientToken: str,
         name: str = ...,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
@@ -232,16 +237,18 @@
 
     def start_job_run(
         self,
         *,
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
-        jobDriver: JobDriverTypeDef = ...,
-        configurationOverrides: ConfigurationOverridesTypeDef = ...,
+        jobDriver: Union[JobDriverTypeDef, JobDriverOutputTypeDef] = ...,
+        configurationOverrides: Union[
+            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+        ] = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
         name: str = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
@@ -278,15 +285,17 @@
         *,
         applicationId: str,
         clientToken: str,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         releaseLabel: str = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
```

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/client.pyi` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,29 @@
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 from .paginator import ListApplicationsPaginator, ListJobRunsPaginator
 from .type_defs import (
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunResponseTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     GetJobRunResponseTypeDef,
     ImageConfigurationInputTypeDef,
     InitialCapacityConfigTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaximumAllowedResourcesTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     StartJobRunResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -110,15 +113,17 @@
         clientToken: str,
         name: str = ...,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
@@ -214,16 +219,18 @@
         """
     def start_job_run(
         self,
         *,
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
-        jobDriver: JobDriverTypeDef = ...,
-        configurationOverrides: ConfigurationOverridesTypeDef = ...,
+        jobDriver: Union[JobDriverTypeDef, JobDriverOutputTypeDef] = ...,
+        configurationOverrides: Union[
+            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+        ] = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
         name: str = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
@@ -256,15 +263,17 @@
         *,
         applicationId: str,
         clientToken: str,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: Union[
+            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+        ] = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         releaseLabel: str = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
```

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/literals.py` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/literals.pyi` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/paginator.py` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/paginator.pyi` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/type_defs.py` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless/type_defs.pyi` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/PKG-INFO` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.28.15
-Summary: Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
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
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-serverless-1.28.15/mypy_boto3_emr_serverless.egg-info/SOURCES.txt` & `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15/setup.py` & `mypy-boto3-emr-serverless-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-serverless",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder"
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

