# Comparing `tmp/mypy-boto3-panorama-1.28.15.tar.gz` & `tmp/mypy-boto3-panorama-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-panorama-1.28.15.tar", last modified: Fri Jul 28 20:43:26 2023, max compression
+gzip compressed data, was "mypy-boto3-panorama-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:50 2023, max compression
```

## Comparing `mypy-boto3-panorama-1.28.15.tar` & `mypy-boto3-panorama-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:26.165623 mypy-boto3-panorama-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16578 2023-07-28 20:43:26.153623 mypy-boto3-panorama-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:26.145623 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23775 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-28 20:33:10.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-28 20:33:10.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38744 2023-07-28 20:33:11.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38701 2023-07-28 20:33:10.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:26.153623 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16578 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:26.165623 mypy-boto3-panorama-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:50.865328 mypy-boto3-panorama-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-07-29 10:03:50.861328 mypy-boto3-panorama-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:50.853328 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-07-29 09:52:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23918 2023-07-29 09:52:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-29 09:52:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-29 09:52:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38825 2023-07-29 09:52:51.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38782 2023-07-29 09:52:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:50.861328 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:50.000000 mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:50.865328 mypy-boto3-panorama-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:52:49.000000 mypy-boto3-panorama-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-panorama-1.28.15/LICENSE` & `mypy-boto3-panorama-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.15/PKG-INFO` & `mypy-boto3-panorama-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-panorama
-Version: 1.28.15
-Summary: Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,27 +326,27 @@
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
     ResponseMetadataTypeDef,
     JobTypeDef,
+    JobResourceTagsOutputTypeDef,
     JobResourceTagsTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
-    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
     StaticIpConnectionInfoOutputTypeDef,
@@ -393,19 +393,19 @@
     DescribeDeviceJobResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
     EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
```

### Comparing `mypy-boto3-panorama-1.28.15/README.md` & `mypy-boto3-panorama-1.28.15.post1/README.md`

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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,27 +294,27 @@
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
     ResponseMetadataTypeDef,
     JobTypeDef,
+    JobResourceTagsOutputTypeDef,
     JobResourceTagsTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
-    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
     StaticIpConnectionInfoOutputTypeDef,
@@ -361,19 +361,19 @@
     DescribeDeviceJobResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
     EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
```

### Comparing `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/__main__.py` & `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Panorama 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Panorama 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama\nOther"
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

### Comparing `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/client.py` & `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_panorama.client import PanoramaClient
 
     session = Session()
     client: PanoramaClient = session.client("panorama")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeviceAggregatedStatusType,
     JobTypeType,
     ListDevicesSortByType,
@@ -40,27 +40,29 @@
     DescribeDeviceResponseTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DescribeNodeResponseTypeDef,
     DescribePackageImportJobResponseTypeDef,
     DescribePackageResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     DeviceJobConfigTypeDef,
+    JobResourceTagsOutputTypeDef,
     JobResourceTagsTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesJobsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
+    NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
     NodeSignalTypeDef,
     PackageImportJobInputConfigTypeDef,
     PackageImportJobOutputConfigTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
@@ -163,15 +165,15 @@
         self,
         *,
         NodeName: str,
         OutputPackageName: str,
         OutputPackageVersion: str,
         TemplateParameters: Mapping[str, str],
         TemplateType: Literal["RTSP_CAMERA_STREAM"],
-        JobTags: Sequence[JobResourceTagsTypeDef] = ...,
+        JobTags: Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]] = ...,
         NodeDescription: str = ...
     ) -> CreateNodeFromTemplateJobResponseTypeDef:
         """
         Creates a camera stream node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#create_node_from_template_job)
@@ -190,15 +192,15 @@
     def create_package_import_job(
         self,
         *,
         ClientToken: str,
         InputConfig: PackageImportJobInputConfigTypeDef,
         JobType: PackageImportJobTypeType,
         OutputConfig: PackageImportJobOutputConfigTypeDef,
-        JobTags: Sequence[JobResourceTagsTypeDef] = ...
+        JobTags: Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]] = ...
     ) -> CreatePackageImportJobResponseTypeDef:
         """
         Imports a node package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#create_package_import_job)
         """
@@ -453,15 +455,15 @@
         """
 
     def provision_device(
         self,
         *,
         Name: str,
         Description: str = ...,
-        NetworkingConfiguration: NetworkPayloadTypeDef = ...,
+        NetworkingConfiguration: Union[NetworkPayloadTypeDef, NetworkPayloadOutputTypeDef] = ...,
         Tags: Mapping[str, str] = ...
     ) -> ProvisionDeviceResponseTypeDef:
         """
         Creates a device and returns a configuration archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#provision_device)
```

### Comparing `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/client.pyi` & `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_panorama.client import PanoramaClient
 
     session = Session()
     client: PanoramaClient = session.client("panorama")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeviceAggregatedStatusType,
     JobTypeType,
     ListDevicesSortByType,
@@ -40,27 +40,29 @@
     DescribeDeviceResponseTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DescribeNodeResponseTypeDef,
     DescribePackageImportJobResponseTypeDef,
     DescribePackageResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     DeviceJobConfigTypeDef,
+    JobResourceTagsOutputTypeDef,
     JobResourceTagsTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesJobsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
+    NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
     NodeSignalTypeDef,
     PackageImportJobInputConfigTypeDef,
     PackageImportJobOutputConfigTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
@@ -154,15 +156,15 @@
         self,
         *,
         NodeName: str,
         OutputPackageName: str,
         OutputPackageVersion: str,
         TemplateParameters: Mapping[str, str],
         TemplateType: Literal["RTSP_CAMERA_STREAM"],
-        JobTags: Sequence[JobResourceTagsTypeDef] = ...,
+        JobTags: Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]] = ...,
         NodeDescription: str = ...
     ) -> CreateNodeFromTemplateJobResponseTypeDef:
         """
         Creates a camera stream node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#create_node_from_template_job)
@@ -179,15 +181,15 @@
     def create_package_import_job(
         self,
         *,
         ClientToken: str,
         InputConfig: PackageImportJobInputConfigTypeDef,
         JobType: PackageImportJobTypeType,
         OutputConfig: PackageImportJobOutputConfigTypeDef,
-        JobTags: Sequence[JobResourceTagsTypeDef] = ...
+        JobTags: Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]] = ...
     ) -> CreatePackageImportJobResponseTypeDef:
         """
         Imports a node package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#create_package_import_job)
         """
@@ -418,15 +420,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#list_tags_for_resource)
         """
     def provision_device(
         self,
         *,
         Name: str,
         Description: str = ...,
-        NetworkingConfiguration: NetworkPayloadTypeDef = ...,
+        NetworkingConfiguration: Union[NetworkPayloadTypeDef, NetworkPayloadOutputTypeDef] = ...,
         Tags: Mapping[str, str] = ...
     ) -> ProvisionDeviceResponseTypeDef:
         """
         Creates a device and returns a configuration archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/client/#provision_device)
```

### Comparing `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/literals.py` & `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/literals.pyi` & `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/type_defs.py` & `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_panorama.type_defs import AlternateSoftwareMetadataTypeDef
 
     data: AlternateSoftwareMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApplicationInstanceHealthStatusType,
     ApplicationInstanceStatusType,
     ConnectionTypeType,
     DesiredStateType,
     DeviceAggregatedStatusType,
@@ -55,27 +55,27 @@
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
     "ResponseMetadataTypeDef",
     "JobTypeDef",
+    "JobResourceTagsOutputTypeDef",
     "JobResourceTagsTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
-    "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
     "StaticIpConnectionInfoOutputTypeDef",
@@ -122,19 +122,19 @@
     "DescribeDeviceJobResponseTypeDef",
     "DescribePackageVersionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ProvisionDeviceResponseTypeDef",
     "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
+    "DescribeNodeFromTemplateJobResponseTypeDef",
     "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
     "DeviceTypeDef",
-    "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
     "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     "ListNodeFromTemplateJobsResponseTypeDef",
@@ -210,14 +210,22 @@
     {
         "DeviceId": str,
         "JobId": str,
     },
     total=False,
 )
 
+JobResourceTagsOutputTypeDef = TypedDict(
+    "JobResourceTagsOutputTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Dict[str, str],
+    },
+)
+
 JobResourceTagsTypeDef = TypedDict(
     "JobResourceTagsTypeDef",
     {
         "ResourceType": Literal["PACKAGE"],
         "Tags": Mapping[str, str],
     },
 )
@@ -348,22 +356,14 @@
 DescribeNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-JobResourceTagsOutputTypeDef = TypedDict(
-    "JobResourceTagsOutputTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Dict[str, str],
-    },
-)
-
 _RequiredDescribeNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeRequestRequestTypeDef",
     {
         "NodeId": str,
     },
 )
 _OptionalDescribeNodeRequestRequestTypeDef = TypedDict(
@@ -1070,28 +1070,47 @@
     "CreateJobForDevicesResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "DescribeNodeFromTemplateJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "LastUpdatedTime": datetime,
+        "NodeDescription": str,
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "Status": NodeFromTemplateJobStatusType,
+        "StatusMessage": str,
+        "TemplateParameters": Dict[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
     {
         "NodeName": str,
         "OutputPackageName": str,
         "OutputPackageVersion": str,
         "TemplateParameters": Mapping[str, str],
         "TemplateType": Literal["RTSP_CAMERA_STREAM"],
     },
 )
 _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
     {
-        "JobTags": Sequence[JobResourceTagsTypeDef],
+        "JobTags": Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]],
         "NodeDescription": str,
     },
     total=False,
 )
 
 
 class CreateNodeFromTemplateJobRequestRequestTypeDef(
@@ -1142,33 +1161,14 @@
         "ProvisioningStatus": DeviceStatusType,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
     },
     total=False,
 )
 
-DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "DescribeNodeFromTemplateJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsOutputTypeDef],
-        "LastUpdatedTime": datetime,
-        "NodeDescription": str,
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "Status": NodeFromTemplateJobStatusType,
-        "StatusMessage": str,
-        "TemplateParameters": Dict[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeviceJobConfigTypeDef = TypedDict(
     "DeviceJobConfigTypeDef",
     {
         "OTAJobConfig": OTAJobConfigTypeDef,
     },
     total=False,
 )
@@ -1476,15 +1476,15 @@
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
     },
 )
 _OptionalCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePackageImportJobRequestRequestTypeDef",
     {
-        "JobTags": Sequence[JobResourceTagsTypeDef],
+        "JobTags": Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]],
     },
     total=False,
 )
 
 
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/type_defs.pyi` & `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_panorama.type_defs import AlternateSoftwareMetadataTypeDef
 
     data: AlternateSoftwareMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApplicationInstanceHealthStatusType,
     ApplicationInstanceStatusType,
     ConnectionTypeType,
     DesiredStateType,
     DeviceAggregatedStatusType,
@@ -54,27 +54,27 @@
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
     "ResponseMetadataTypeDef",
     "JobTypeDef",
+    "JobResourceTagsOutputTypeDef",
     "JobResourceTagsTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
-    "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
     "StaticIpConnectionInfoOutputTypeDef",
@@ -121,19 +121,19 @@
     "DescribeDeviceJobResponseTypeDef",
     "DescribePackageVersionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ProvisionDeviceResponseTypeDef",
     "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
+    "DescribeNodeFromTemplateJobResponseTypeDef",
     "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
     "DeviceTypeDef",
-    "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
     "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     "ListNodeFromTemplateJobsResponseTypeDef",
@@ -209,14 +209,22 @@
     {
         "DeviceId": str,
         "JobId": str,
     },
     total=False,
 )
 
+JobResourceTagsOutputTypeDef = TypedDict(
+    "JobResourceTagsOutputTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Dict[str, str],
+    },
+)
+
 JobResourceTagsTypeDef = TypedDict(
     "JobResourceTagsTypeDef",
     {
         "ResourceType": Literal["PACKAGE"],
         "Tags": Mapping[str, str],
     },
 )
@@ -341,22 +349,14 @@
 DescribeNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-JobResourceTagsOutputTypeDef = TypedDict(
-    "JobResourceTagsOutputTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Dict[str, str],
-    },
-)
-
 _RequiredDescribeNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeRequestRequestTypeDef",
     {
         "NodeId": str,
     },
 )
 _OptionalDescribeNodeRequestRequestTypeDef = TypedDict(
@@ -1039,28 +1039,47 @@
     "CreateJobForDevicesResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "DescribeNodeFromTemplateJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "LastUpdatedTime": datetime,
+        "NodeDescription": str,
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "Status": NodeFromTemplateJobStatusType,
+        "StatusMessage": str,
+        "TemplateParameters": Dict[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
     {
         "NodeName": str,
         "OutputPackageName": str,
         "OutputPackageVersion": str,
         "TemplateParameters": Mapping[str, str],
         "TemplateType": Literal["RTSP_CAMERA_STREAM"],
     },
 )
 _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
     {
-        "JobTags": Sequence[JobResourceTagsTypeDef],
+        "JobTags": Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]],
         "NodeDescription": str,
     },
     total=False,
 )
 
 class CreateNodeFromTemplateJobRequestRequestTypeDef(
     _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
@@ -1109,33 +1128,14 @@
         "ProvisioningStatus": DeviceStatusType,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
     },
     total=False,
 )
 
-DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "DescribeNodeFromTemplateJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsOutputTypeDef],
-        "LastUpdatedTime": datetime,
-        "NodeDescription": str,
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "Status": NodeFromTemplateJobStatusType,
-        "StatusMessage": str,
-        "TemplateParameters": Dict[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeviceJobConfigTypeDef = TypedDict(
     "DeviceJobConfigTypeDef",
     {
         "OTAJobConfig": OTAJobConfigTypeDef,
     },
     total=False,
 )
@@ -1435,15 +1435,15 @@
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
     },
 )
 _OptionalCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePackageImportJobRequestRequestTypeDef",
     {
-        "JobTags": Sequence[JobResourceTagsTypeDef],
+        "JobTags": Sequence[Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]],
     },
     total=False,
 )
 
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
     _OptionalCreatePackageImportJobRequestRequestTypeDef,
```

### Comparing `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/PKG-INFO` & `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-panorama
-Version: 1.28.15
-Summary: Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,27 +326,27 @@
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
     ResponseMetadataTypeDef,
     JobTypeDef,
+    JobResourceTagsOutputTypeDef,
     JobResourceTagsTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
-    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
     StaticIpConnectionInfoOutputTypeDef,
@@ -393,19 +393,19 @@
     DescribeDeviceJobResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
     EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
```

### Comparing `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/SOURCES.txt` & `mypy-boto3-panorama-1.28.15.post1/mypy_boto3_panorama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.15/setup.py` & `mypy-boto3-panorama-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-panorama",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_panorama"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder"
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

