# Comparing `tmp/mypy-boto3-emr-containers-1.28.15.tar.gz` & `tmp/mypy-boto3-emr-containers-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-containers-1.28.15.tar", last modified: Fri Jul 28 20:42:46 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-containers-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:05 2023, max compression
```

## Comparing `mypy-boto3-emr-containers-1.28.15.tar` & `mypy-boto3-emr-containers-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.689081 mypy-boto3-emr-containers-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-07-28 20:42:46.681081 mypy-boto3-emr-containers-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.673081 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28645 2023-07-28 20:25:31.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-07-28 20:25:31.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.681081 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:46.000000 mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:46.689081 mypy-boto3-emr-containers-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:25:30.000000 mypy-boto3-emr-containers-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.913142 mypy-boto3-emr-containers-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16598 2023-07-29 10:03:05.913142 mypy-boto3-emr-containers-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.913142 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18682 2023-07-29 09:45:01.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18651 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-29 09:45:01.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-29 09:45:01.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-29 09:45:01.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-29 09:45:01.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28645 2023-07-29 09:45:02.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-07-29 09:45:02.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.913142 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16598 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:05.913142 mypy-boto3-emr-containers-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-emr-containers-1.28.15/LICENSE` & `mypy-boto3-emr-containers-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15/PKG-INFO` & `mypy-boto3-emr-containers-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.28.15
-Summary: Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-containers-1.28.15/README.md` & `mypy-boto3-emr-containers-1.28.15.post1/README.md`

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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__init__.py` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__init__.pyi` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/__main__.py` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRContainers 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.EMRContainers 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\nOther"
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

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/client.py` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,31 @@
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
     ListVirtualClustersPaginator,
 )
 from .type_defs import (
     CancelJobRunResponseTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     ContainerProviderTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeJobTemplateResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
+    JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     RetryPolicyConfigurationTypeDef,
@@ -119,15 +122,15 @@
         """
 
     def create_job_template(
         self,
         *,
         name: str,
         clientToken: str,
-        jobTemplateData: JobTemplateDataTypeDef,
+        jobTemplateData: Union[JobTemplateDataTypeDef, JobTemplateDataOutputTypeDef],
         tags: Mapping[str, str] = ...,
         kmsKeyArn: str = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_job_template)
@@ -140,15 +143,17 @@
         name: str,
         virtualClusterId: str,
         type: str,
         releaseLabel: str,
         executionRoleArn: str,
         clientToken: str,
         certificateArn: str = ...,
-        configurationOverrides: ConfigurationOverridesTypeDef = ...,
+        configurationOverrides: Union[
+            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+        ] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateManagedEndpointResponseTypeDef:
         """
         Creates a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#create_managed_endpoint)
@@ -342,16 +347,18 @@
         self,
         *,
         virtualClusterId: str,
         clientToken: str,
         name: str = ...,
         executionRoleArn: str = ...,
         releaseLabel: str = ...,
-        jobDriver: JobDriverTypeDef = ...,
-        configurationOverrides: ConfigurationOverridesTypeDef = ...,
+        jobDriver: Union[JobDriverTypeDef, JobDriverOutputTypeDef] = ...,
+        configurationOverrides: Union[
+            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+        ] = ...,
         tags: Mapping[str, str] = ...,
         jobTemplateId: str = ...,
         jobTemplateParameters: Mapping[str, str] = ...,
         retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
```

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/client.pyi` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,31 @@
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
     ListVirtualClustersPaginator,
 )
 from .type_defs import (
     CancelJobRunResponseTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     ContainerProviderTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeJobTemplateResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
+    JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     RetryPolicyConfigurationTypeDef,
@@ -111,15 +114,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#close)
         """
     def create_job_template(
         self,
         *,
         name: str,
         clientToken: str,
-        jobTemplateData: JobTemplateDataTypeDef,
+        jobTemplateData: Union[JobTemplateDataTypeDef, JobTemplateDataOutputTypeDef],
         tags: Mapping[str, str] = ...,
         kmsKeyArn: str = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_job_template)
@@ -131,15 +134,17 @@
         name: str,
         virtualClusterId: str,
         type: str,
         releaseLabel: str,
         executionRoleArn: str,
         clientToken: str,
         certificateArn: str = ...,
-        configurationOverrides: ConfigurationOverridesTypeDef = ...,
+        configurationOverrides: Union[
+            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+        ] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateManagedEndpointResponseTypeDef:
         """
         Creates a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#create_managed_endpoint)
@@ -317,16 +322,18 @@
         self,
         *,
         virtualClusterId: str,
         clientToken: str,
         name: str = ...,
         executionRoleArn: str = ...,
         releaseLabel: str = ...,
-        jobDriver: JobDriverTypeDef = ...,
-        configurationOverrides: ConfigurationOverridesTypeDef = ...,
+        jobDriver: Union[JobDriverTypeDef, JobDriverOutputTypeDef] = ...,
+        configurationOverrides: Union[
+            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+        ] = ...,
         tags: Mapping[str, str] = ...,
         jobTemplateId: str = ...,
         jobTemplateParameters: Mapping[str, str] = ...,
         retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
```

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/literals.py` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/literals.pyi` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/paginator.py` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/paginator.pyi` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/type_defs.py` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers/type_defs.pyi` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/PKG-INFO` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.28.15
-Summary: Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-containers-1.28.15/mypy_boto3_emr_containers.egg-info/SOURCES.txt` & `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15/setup.py` & `mypy-boto3-emr-containers-1.28.15.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-containers",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder"
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

