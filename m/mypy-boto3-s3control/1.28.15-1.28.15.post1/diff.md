# Comparing `tmp/mypy-boto3-s3control-1.28.15.tar.gz` & `tmp/mypy-boto3-s3control-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3control-1.28.15.tar", last modified: Fri Jul 28 20:43:38 2023, max compression
+gzip compressed data, was "mypy-boto3-s3control-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:04 2023, max compression
```

## Comparing `mypy-boto3-s3control-1.28.15.tar` & `mypy-boto3-s3control-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:38.185788 mypy-boto3-s3control-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-07-28 20:43:38.185788 mypy-boto3-s3control-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22529 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:38.185788 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43055 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42983 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85262 2023-07-28 20:37:46.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85163 2023-07-28 20:37:45.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:38.185788 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-07-28 20:43:37.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:38.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:37.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:37.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:37.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:37.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:38.185788 mypy-boto3-s3control-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.869378 mypy-boto3-s3control-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-07-29 10:04:04.869378 mypy-boto3-s3control-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22529 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.861378 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43922 2023-07-29 09:57:50.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43850 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-29 09:57:50.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-29 09:57:50.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 09:57:50.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-29 09:57:50.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85262 2023-07-29 09:57:52.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85163 2023-07-29 09:57:51.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.869378 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:04.869378 mypy-boto3-s3control-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-s3control-1.28.15/LICENSE` & `mypy-boto3-s3control-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15/PKG-INFO` & `mypy-boto3-s3control-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.28.15
-Summary: Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-s3control-1.28.15/README.md` & `mypy-boto3-s3control-1.28.15.post1/README.md`

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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__init__.py` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__init__.pyi` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__main__.py` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3Control 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.S3Control 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\nOther"
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

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/client.py` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,27 @@
     from mypy_boto3_s3control.client import S3ControlClient
 
     session = Session()
     client: S3ControlClient = session.client("s3control")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BucketCannedACLType, JobStatusType, RequestedJobStatusType
 from .paginator import ListAccessPointsForObjectLambdaPaginator
 from .type_defs import (
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketConfigurationTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
+    CreateMultiRegionAccessPointInputOutputTypeDef,
     CreateMultiRegionAccessPointInputTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     DeleteMultiRegionAccessPointResultTypeDef,
     DescribeJobResultTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -50,32 +51,38 @@
     GetMultiRegionAccessPointPolicyResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
+    JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
+    JobManifestOutputTypeDef,
     JobManifestTypeDef,
+    JobOperationOutputTypeDef,
     JobOperationTypeDef,
     JobReportTypeDef,
     LifecycleConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     ListAccessPointsResultTypeDef,
     ListJobsResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MultiRegionAccessPointRouteTypeDef,
+    ObjectLambdaConfigurationOutputTypeDef,
     ObjectLambdaConfigurationTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     PutMultiRegionAccessPointPolicyResultTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     S3TagTypeDef,
+    StorageLensConfigurationOutputTypeDef,
     StorageLensConfigurationTypeDef,
     StorageLensTagTypeDef,
     TaggingTypeDef,
     UpdateJobPriorityResultTypeDef,
     UpdateJobStatusResultTypeDef,
     VersioningConfigurationTypeDef,
     VpcConfigurationTypeDef,
@@ -161,15 +168,21 @@
         Creates an access point and associates it with the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_access_point)
         """
 
     def create_access_point_for_object_lambda(
-        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationTypeDef
+        self,
+        *,
+        AccountId: str,
+        Name: str,
+        Configuration: Union[
+            ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
+        ]
     ) -> CreateAccessPointForObjectLambdaResultTypeDef:
         """
         Creates an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_access_point_for_object_lambda)
         """
@@ -195,35 +208,43 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_bucket)
         """
 
     def create_job(
         self,
         *,
         AccountId: str,
-        Operation: JobOperationTypeDef,
+        Operation: Union[JobOperationTypeDef, JobOperationOutputTypeDef],
         Report: JobReportTypeDef,
         ClientRequestToken: str,
         Priority: int,
         RoleArn: str,
         ConfirmationRequired: bool = ...,
-        Manifest: JobManifestTypeDef = ...,
+        Manifest: Union[JobManifestTypeDef, JobManifestOutputTypeDef] = ...,
         Description: str = ...,
         Tags: Sequence[S3TagTypeDef] = ...,
-        ManifestGenerator: JobManifestGeneratorTypeDef = ...
+        ManifestGenerator: Union[
+            JobManifestGeneratorTypeDef, JobManifestGeneratorOutputTypeDef
+        ] = ...
     ) -> CreateJobResultTypeDef:
         """
         You can use S3 Batch Operations to perform large-scale batch actions on Amazon
         S3 objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_job)
         """
 
     def create_multi_region_access_point(
-        self, *, AccountId: str, ClientToken: str, Details: CreateMultiRegionAccessPointInputTypeDef
+        self,
+        *,
+        AccountId: str,
+        ClientToken: str,
+        Details: Union[
+            CreateMultiRegionAccessPointInputTypeDef, CreateMultiRegionAccessPointInputOutputTypeDef
+        ]
     ) -> CreateMultiRegionAccessPointResultTypeDef:
         """
         Creates a Multi-Region Access Point and associates it with the specified
         buckets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_multi_region_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_multi_region_access_point)
@@ -664,15 +685,21 @@
         Gets a list of Amazon S3 Storage Lens configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_storage_lens_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#list_storage_lens_configurations)
         """
 
     def put_access_point_configuration_for_object_lambda(
-        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationTypeDef
+        self,
+        *,
+        AccountId: str,
+        Name: str,
+        Configuration: Union[
+            ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
+        ]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Replaces configuration for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_configuration_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_access_point_configuration_for_object_lambda)
         """
@@ -722,15 +749,17 @@
         """
 
     def put_bucket_replication(
         self,
         *,
         AccountId: str,
         Bucket: str,
-        ReplicationConfiguration: ReplicationConfigurationTypeDef
+        ReplicationConfiguration: Union[
+            ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+        ]
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_bucket_replication)
         """
@@ -800,15 +829,17 @@
         """
 
     def put_storage_lens_configuration(
         self,
         *,
         ConfigId: str,
         AccountId: str,
-        StorageLensConfiguration: StorageLensConfigurationTypeDef,
+        StorageLensConfiguration: Union[
+            StorageLensConfigurationTypeDef, StorageLensConfigurationOutputTypeDef
+        ],
         Tags: Sequence[StorageLensTagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Puts an Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_storage_lens_configuration)
```

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/client.pyi` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,27 @@
     from mypy_boto3_s3control.client import S3ControlClient
 
     session = Session()
     client: S3ControlClient = session.client("s3control")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BucketCannedACLType, JobStatusType, RequestedJobStatusType
 from .paginator import ListAccessPointsForObjectLambdaPaginator
 from .type_defs import (
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketConfigurationTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
+    CreateMultiRegionAccessPointInputOutputTypeDef,
     CreateMultiRegionAccessPointInputTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     DeleteMultiRegionAccessPointResultTypeDef,
     DescribeJobResultTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -50,32 +51,38 @@
     GetMultiRegionAccessPointPolicyResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
+    JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
+    JobManifestOutputTypeDef,
     JobManifestTypeDef,
+    JobOperationOutputTypeDef,
     JobOperationTypeDef,
     JobReportTypeDef,
     LifecycleConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     ListAccessPointsResultTypeDef,
     ListJobsResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MultiRegionAccessPointRouteTypeDef,
+    ObjectLambdaConfigurationOutputTypeDef,
     ObjectLambdaConfigurationTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     PutMultiRegionAccessPointPolicyResultTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     S3TagTypeDef,
+    StorageLensConfigurationOutputTypeDef,
     StorageLensConfigurationTypeDef,
     StorageLensTagTypeDef,
     TaggingTypeDef,
     UpdateJobPriorityResultTypeDef,
     UpdateJobStatusResultTypeDef,
     VersioningConfigurationTypeDef,
     VpcConfigurationTypeDef,
@@ -153,15 +160,21 @@
         """
         Creates an access point and associates it with the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_access_point)
         """
     def create_access_point_for_object_lambda(
-        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationTypeDef
+        self,
+        *,
+        AccountId: str,
+        Name: str,
+        Configuration: Union[
+            ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
+        ]
     ) -> CreateAccessPointForObjectLambdaResultTypeDef:
         """
         Creates an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_access_point_for_object_lambda)
         """
@@ -185,34 +198,42 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_bucket)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_bucket)
         """
     def create_job(
         self,
         *,
         AccountId: str,
-        Operation: JobOperationTypeDef,
+        Operation: Union[JobOperationTypeDef, JobOperationOutputTypeDef],
         Report: JobReportTypeDef,
         ClientRequestToken: str,
         Priority: int,
         RoleArn: str,
         ConfirmationRequired: bool = ...,
-        Manifest: JobManifestTypeDef = ...,
+        Manifest: Union[JobManifestTypeDef, JobManifestOutputTypeDef] = ...,
         Description: str = ...,
         Tags: Sequence[S3TagTypeDef] = ...,
-        ManifestGenerator: JobManifestGeneratorTypeDef = ...
+        ManifestGenerator: Union[
+            JobManifestGeneratorTypeDef, JobManifestGeneratorOutputTypeDef
+        ] = ...
     ) -> CreateJobResultTypeDef:
         """
         You can use S3 Batch Operations to perform large-scale batch actions on Amazon
         S3 objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_job)
         """
     def create_multi_region_access_point(
-        self, *, AccountId: str, ClientToken: str, Details: CreateMultiRegionAccessPointInputTypeDef
+        self,
+        *,
+        AccountId: str,
+        ClientToken: str,
+        Details: Union[
+            CreateMultiRegionAccessPointInputTypeDef, CreateMultiRegionAccessPointInputOutputTypeDef
+        ]
     ) -> CreateMultiRegionAccessPointResultTypeDef:
         """
         Creates a Multi-Region Access Point and associates it with the specified
         buckets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_multi_region_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_multi_region_access_point)
@@ -608,15 +629,21 @@
         """
         Gets a list of Amazon S3 Storage Lens configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_storage_lens_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#list_storage_lens_configurations)
         """
     def put_access_point_configuration_for_object_lambda(
-        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationTypeDef
+        self,
+        *,
+        AccountId: str,
+        Name: str,
+        Configuration: Union[
+            ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
+        ]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Replaces configuration for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_configuration_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_access_point_configuration_for_object_lambda)
         """
@@ -661,15 +688,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_bucket_policy)
         """
     def put_bucket_replication(
         self,
         *,
         AccountId: str,
         Bucket: str,
-        ReplicationConfiguration: ReplicationConfigurationTypeDef
+        ReplicationConfiguration: Union[
+            ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+        ]
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_bucket_replication)
         """
@@ -733,15 +762,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_public_access_block)
         """
     def put_storage_lens_configuration(
         self,
         *,
         ConfigId: str,
         AccountId: str,
-        StorageLensConfiguration: StorageLensConfigurationTypeDef,
+        StorageLensConfiguration: Union[
+            StorageLensConfigurationTypeDef, StorageLensConfigurationOutputTypeDef
+        ],
         Tags: Sequence[StorageLensTagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Puts an Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_storage_lens_configuration)
```

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/literals.py` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/literals.pyi` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/paginator.py` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/paginator.pyi` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/type_defs.py` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/type_defs.pyi` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/PKG-INFO` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.28.15
-Summary: Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/SOURCES.txt` & `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15/setup.py` & `mypy-boto3-s3control-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3control",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_s3control"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder"
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

