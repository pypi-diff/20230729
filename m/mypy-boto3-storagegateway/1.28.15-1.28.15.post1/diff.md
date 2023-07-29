# Comparing `tmp/mypy-boto3-storagegateway-1.28.15.tar.gz` & `tmp/mypy-boto3-storagegateway-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-storagegateway-1.28.15.tar", last modified: Fri Jul 28 20:43:50 2023, max compression
+gzip compressed data, was "mypy-boto3-storagegateway-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:19 2023, max compression
```

## Comparing `mypy-boto3-storagegateway-1.28.15.tar` & `mypy-boto3-storagegateway-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-storagegateway-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24137 2023-07-28 20:43:50.521957 mypy-boto3-storagegateway-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68220 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68112 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    77916 2023-07-28 20:40:22.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77837 2023-07-28 20:40:21.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24137 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:50.521957 mypy-boto3-storagegateway-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.085431 mypy-boto3-storagegateway-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-07-29 10:04:19.081431 mypy-boto3-storagegateway-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.077431 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68554 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68446 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-29 10:00:32.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-29 10:00:32.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    77993 2023-07-29 10:00:34.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77914 2023-07-29 10:00:33.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.081431 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:04:18.000000 mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:19.085431 mypy-boto3-storagegateway-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 10:00:31.000000 mypy-boto3-storagegateway-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-storagegateway-1.28.15/LICENSE` & `mypy-boto3-storagegateway-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15/PKG-INFO` & `mypy-boto3-storagegateway-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.28.15
-Summary: Type annotations for boto3.StorageGateway 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.StorageGateway 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-storagegateway-1.28.15/README.md` & `mypy-boto3-storagegateway-1.28.15.post1/README.md`

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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__init__.py` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__init__.pyi` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__main__.py` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.StorageGateway 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.StorageGateway 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway\nOther"
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

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/client.py` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_storagegateway.client import StorageGatewayClient
 
     session = Session()
     client: StorageGatewayClient = session.client("storagegateway")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CaseSensitivityType,
     GatewayCapacityType,
     ObjectACLType,
@@ -45,14 +45,15 @@
     AddTagsToResourceOutputTypeDef,
     AddUploadBufferOutputTypeDef,
     AddWorkingStorageOutputTypeDef,
     AssignTapePoolOutputTypeDef,
     AssociateFileSystemOutputTypeDef,
     AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     CacheAttributesTypeDef,
     CancelArchivalOutputTypeDef,
     CancelRetrievalOutputTypeDef,
     CreateCachediSCSIVolumeOutputTypeDef,
     CreateNFSFileShareOutputTypeDef,
     CreateSMBFileShareOutputTypeDef,
@@ -91,14 +92,15 @@
     DescribeTapesOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
+    EndpointNetworkConfigurationOutputTypeDef,
     EndpointNetworkConfigurationTypeDef,
     JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     ListFileSharesOutputTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListLocalDisksOutputTypeDef,
@@ -114,14 +116,15 @@
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayOutputTypeDef,
+    SMBLocalGroupsOutputTypeDef,
     SMBLocalGroupsTypeDef,
     StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayOutputTypeDef,
     TagTypeDef,
     UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitOutputTypeDef,
     UpdateBandwidthRateLimitScheduleOutputTypeDef,
@@ -255,15 +258,17 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...
+        EndpointNetworkConfiguration: Union[
+            EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
+        ] = ...
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#associate_file_system)
         """
@@ -1107,15 +1112,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit)
         """
 
     def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef]
+        BandwidthRateLimitIntervals: Sequence[
+            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
+        ]
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
@@ -1259,15 +1266,18 @@
         browse list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share_visibility)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_smb_file_share_visibility)
         """
 
     def update_smb_local_groups(
-        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsTypeDef
+        self,
+        *,
+        GatewayARN: str,
+        SMBLocalGroups: Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
     ) -> UpdateSMBLocalGroupsOutputTypeDef:
         """
         Updates the list of Active Directory users and groups that have special
         permissions for SMB file shares on the gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_local_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_smb_local_groups)
```

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/client.pyi` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_storagegateway.client import StorageGatewayClient
 
     session = Session()
     client: StorageGatewayClient = session.client("storagegateway")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CaseSensitivityType,
     GatewayCapacityType,
     ObjectACLType,
@@ -45,14 +45,15 @@
     AddTagsToResourceOutputTypeDef,
     AddUploadBufferOutputTypeDef,
     AddWorkingStorageOutputTypeDef,
     AssignTapePoolOutputTypeDef,
     AssociateFileSystemOutputTypeDef,
     AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     CacheAttributesTypeDef,
     CancelArchivalOutputTypeDef,
     CancelRetrievalOutputTypeDef,
     CreateCachediSCSIVolumeOutputTypeDef,
     CreateNFSFileShareOutputTypeDef,
     CreateSMBFileShareOutputTypeDef,
@@ -91,14 +92,15 @@
     DescribeTapesOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
+    EndpointNetworkConfigurationOutputTypeDef,
     EndpointNetworkConfigurationTypeDef,
     JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     ListFileSharesOutputTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListLocalDisksOutputTypeDef,
@@ -114,14 +116,15 @@
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayOutputTypeDef,
+    SMBLocalGroupsOutputTypeDef,
     SMBLocalGroupsTypeDef,
     StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayOutputTypeDef,
     TagTypeDef,
     UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitOutputTypeDef,
     UpdateBandwidthRateLimitScheduleOutputTypeDef,
@@ -244,15 +247,17 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...
+        EndpointNetworkConfiguration: Union[
+            EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
+        ] = ...
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#associate_file_system)
         """
@@ -1022,15 +1027,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit)
         """
     def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef]
+        BandwidthRateLimitIntervals: Sequence[
+            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
+        ]
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
@@ -1165,15 +1172,18 @@
         Controls whether the shares on an S3 File Gateway are visible in a net view or
         browse list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share_visibility)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_smb_file_share_visibility)
         """
     def update_smb_local_groups(
-        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsTypeDef
+        self,
+        *,
+        GatewayARN: str,
+        SMBLocalGroups: Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
     ) -> UpdateSMBLocalGroupsOutputTypeDef:
         """
         Updates the list of Active Directory users and groups that have special
         permissions for SMB file shares on the gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_local_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#update_smb_local_groups)
```

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/literals.py` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/literals.pyi` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/paginator.py` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/paginator.pyi` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/type_defs.py` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_storagegateway.type_defs import TagTypeDef
 
     data: TagTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ActiveDirectoryStatusType,
     AvailabilityMonitorTestStatusType,
     CaseSensitivityType,
     FileShareTypeType,
     GatewayCapacityType,
@@ -2462,15 +2462,17 @@
     },
 )
 
 UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+        "BandwidthRateLimitIntervals": Sequence[
+            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
+        ],
     },
 )
 
 CachediSCSIVolumeTypeDef = TypedDict(
     "CachediSCSIVolumeTypeDef",
     {
         "VolumeARN": str,
```

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/type_defs.pyi` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_storagegateway.type_defs import TagTypeDef
 
     data: TagTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ActiveDirectoryStatusType,
     AvailabilityMonitorTestStatusType,
     CaseSensitivityType,
     FileShareTypeType,
     GatewayCapacityType,
@@ -2395,15 +2395,17 @@
     },
 )
 
 UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+        "BandwidthRateLimitIntervals": Sequence[
+            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
+        ],
     },
 )
 
 CachediSCSIVolumeTypeDef = TypedDict(
     "CachediSCSIVolumeTypeDef",
     {
         "VolumeARN": str,
```

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/PKG-INFO` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.28.15
-Summary: Type annotations for boto3.StorageGateway 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.StorageGateway 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/SOURCES.txt` & `mypy-boto3-storagegateway-1.28.15.post1/mypy_boto3_storagegateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.15/setup.py` & `mypy-boto3-storagegateway-1.28.15.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-storagegateway",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_storagegateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.StorageGateway 1.28.15 service generated with"
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

