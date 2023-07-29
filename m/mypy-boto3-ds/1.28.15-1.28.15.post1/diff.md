# Comparing `tmp/mypy-boto3-ds-1.28.15.tar.gz` & `tmp/mypy-boto3-ds-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ds-1.28.15.tar", last modified: Fri Jul 28 20:42:40 2023, max compression
+gzip compressed data, was "mypy-boto3-ds-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:59 2023, max compression
```

## Comparing `mypy-boto3-ds-1.28.15.tar` & `mypy-boto3-ds-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.700998 mypy-boto3-ds-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-07-28 20:42:40.692998 mypy-boto3-ds-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.680998 mypy-boto3-ds-1.28.15/mypy_boto3_ds/
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51628 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51540 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-07-28 20:23:23.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-28 20:23:23.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58274 2023-07-28 20:23:25.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58201 2023-07-28 20:23:24.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.692998 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 20:42:40.000000 mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:40.700998 mypy-boto3-ds-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-28 20:23:22.000000 mypy-boto3-ds-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.153114 mypy-boto3-ds-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-07-29 10:02:59.149114 mypy-boto3-ds-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.141114 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51985 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51897 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-07-29 09:42:51.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-29 09:42:51.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-07-29 09:42:51.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58274 2023-07-29 09:42:54.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58201 2023-07-29 09:42:52.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.149114 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:59.153114 mypy-boto3-ds-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-ds-1.28.15/LICENSE` & `mypy-boto3-ds-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15/PKG-INFO` & `mypy-boto3-ds-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ds
-Version: 1.28.15
-Summary: Type annotations for boto3.DirectoryService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DirectoryService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ds-1.28.15/README.md` & `mypy-boto3-ds-1.28.15.post1/README.md`

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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/__init__.py` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/__init__.pyi` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/__main__.py` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DirectoryService 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.DirectoryService 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService\nOther"
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

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/client.py` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ds.client import DirectoryServiceClient
 
     session = Session()
     client: DirectoryServiceClient = session.client("ds")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CertificateTypeType,
     ClientAuthenticationTypeType,
     DirectoryConfigurationStatusType,
@@ -69,24 +69,26 @@
     DescribeRegionsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
     DirectoryConnectSettingsTypeDef,
+    DirectoryVpcSettingsOutputTypeDef,
     DirectoryVpcSettingsTypeDef,
     GetDirectoryLimitsResultTypeDef,
     GetSnapshotLimitsResultTypeDef,
     IpRouteTypeDef,
     ListCertificatesResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     OSUpdateSettingsTypeDef,
+    RadiusSettingsOutputTypeDef,
     RadiusSettingsTypeDef,
     RegisterCertificateResultTypeDef,
     RejectSharedDirectoryResultTypeDef,
     SettingTypeDef,
     ShareDirectoryResultTypeDef,
     ShareTargetTypeDef,
     StartSchemaExtensionResultTypeDef,
@@ -197,15 +199,19 @@
         from your Microsoft AD on Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_ip_routes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#add_ip_routes)
         """
 
     def add_region(
-        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsTypeDef
+        self,
+        *,
+        DirectoryId: str,
+        RegionName: str,
+        VPCSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Adds two domain controllers in the specified Region for the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_region)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#add_region)
         """
@@ -303,15 +309,15 @@
         self,
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ShortName: str = ...,
         Description: str = ...,
-        VpcSettings: DirectoryVpcSettingsTypeDef = ...,
+        VpcSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDirectoryResultTypeDef:
         """
         Creates a Simple AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_directory)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#create_directory)
@@ -328,15 +334,15 @@
         """
 
     def create_microsoft_ad(
         self,
         *,
         Name: str,
         Password: str,
-        VpcSettings: DirectoryVpcSettingsTypeDef,
+        VpcSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef],
         ShortName: str = ...,
         Description: str = ...,
         Edition: DirectoryEditionType = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMicrosoftADResultTypeDef:
         """
         Creates a Microsoft AD directory in the Amazon Web Services Cloud.
@@ -663,15 +669,18 @@
         Activates the switch for the specific directory to always use LDAP secure calls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_ldaps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#enable_ldaps)
         """
 
     def enable_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
+        self,
+        *,
+        DirectoryId: str,
+        RadiusSettings: Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Enables multi-factor authentication (MFA) with the Remote Authentication Dial In
         User Service (RADIUS) server for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_radius)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#enable_radius)
@@ -923,15 +932,18 @@
         Adds or removes domain controllers to or from the directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_number_of_domain_controllers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#update_number_of_domain_controllers)
         """
 
     def update_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
+        self,
+        *,
+        DirectoryId: str,
+        RadiusSettings: Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates the Remote Authentication Dial In User Service (RADIUS) server
         information for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_radius)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#update_radius)
```

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/client.pyi` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ds.client import DirectoryServiceClient
 
     session = Session()
     client: DirectoryServiceClient = session.client("ds")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CertificateTypeType,
     ClientAuthenticationTypeType,
     DirectoryConfigurationStatusType,
@@ -69,24 +69,26 @@
     DescribeRegionsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
     DirectoryConnectSettingsTypeDef,
+    DirectoryVpcSettingsOutputTypeDef,
     DirectoryVpcSettingsTypeDef,
     GetDirectoryLimitsResultTypeDef,
     GetSnapshotLimitsResultTypeDef,
     IpRouteTypeDef,
     ListCertificatesResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     OSUpdateSettingsTypeDef,
+    RadiusSettingsOutputTypeDef,
     RadiusSettingsTypeDef,
     RegisterCertificateResultTypeDef,
     RejectSharedDirectoryResultTypeDef,
     SettingTypeDef,
     ShareDirectoryResultTypeDef,
     ShareTargetTypeDef,
     StartSchemaExtensionResultTypeDef,
@@ -190,15 +192,19 @@
         address, you must add a CIDR address block to correctly route traffic to and
         from your Microsoft AD on Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_ip_routes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#add_ip_routes)
         """
     def add_region(
-        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsTypeDef
+        self,
+        *,
+        DirectoryId: str,
+        RegionName: str,
+        VPCSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Adds two domain controllers in the specified Region for the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_region)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#add_region)
         """
@@ -287,15 +293,15 @@
         self,
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ShortName: str = ...,
         Description: str = ...,
-        VpcSettings: DirectoryVpcSettingsTypeDef = ...,
+        VpcSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDirectoryResultTypeDef:
         """
         Creates a Simple AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_directory)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#create_directory)
@@ -310,15 +316,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#create_log_subscription)
         """
     def create_microsoft_ad(
         self,
         *,
         Name: str,
         Password: str,
-        VpcSettings: DirectoryVpcSettingsTypeDef,
+        VpcSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef],
         ShortName: str = ...,
         Description: str = ...,
         Edition: DirectoryEditionType = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMicrosoftADResultTypeDef:
         """
         Creates a Microsoft AD directory in the Amazon Web Services Cloud.
@@ -616,15 +622,18 @@
         """
         Activates the switch for the specific directory to always use LDAP secure calls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_ldaps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#enable_ldaps)
         """
     def enable_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
+        self,
+        *,
+        DirectoryId: str,
+        RadiusSettings: Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Enables multi-factor authentication (MFA) with the Remote Authentication Dial In
         User Service (RADIUS) server for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_radius)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#enable_radius)
@@ -852,15 +861,18 @@
         """
         Adds or removes domain controllers to or from the directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_number_of_domain_controllers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#update_number_of_domain_controllers)
         """
     def update_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
+        self,
+        *,
+        DirectoryId: str,
+        RadiusSettings: Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates the Remote Authentication Dial In User Service (RADIUS) server
         information for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_radius)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#update_radius)
```

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/literals.py` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/literals.pyi` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/paginator.py` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/paginator.pyi` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/type_defs.py` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds/type_defs.pyi` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/PKG-INFO` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ds
-Version: 1.28.15
-Summary: Type annotations for boto3.DirectoryService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DirectoryService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ds-1.28.15/mypy_boto3_ds.egg-info/SOURCES.txt` & `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15/setup.py` & `mypy-boto3-ds-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ds",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_ds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DirectoryService 1.28.15 service generated with"
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

