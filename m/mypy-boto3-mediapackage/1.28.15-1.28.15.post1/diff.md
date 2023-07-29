# Comparing `tmp/mypy-boto3-mediapackage-1.28.15.tar.gz` & `tmp/mypy-boto3-mediapackage-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-1.28.15.tar", last modified: Fri Jul 28 20:43:15 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:39 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-1.28.15.tar` & `mypy-boto3-mediapackage-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.261474 mypy-boto3-mediapackage-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-07-28 20:43:15.261474 mypy-boto3-mediapackage-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14559 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.245473 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30177 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30146 2023-07-28 20:31:34.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.261474 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:15.261474 mypy-boto3-mediapackage-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:31:33.000000 mypy-boto3-mediapackage-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:39.189277 mypy-boto3-mediapackage-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-07-29 10:03:39.185277 mypy-boto3-mediapackage-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14559 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:39.181277 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-29 09:51:13.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-29 09:51:13.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30177 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30146 2023-07-29 09:51:13.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:39.185277 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:38.000000 mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:39.189277 mypy-boto3-mediapackage-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:51:10.000000 mypy-boto3-mediapackage-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-mediapackage-1.28.15/LICENSE` & `mypy-boto3-mediapackage-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15/PKG-INFO` & `mypy-boto3-mediapackage-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.28.15
-Summary: Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediapackage-1.28.15/README.md` & `mypy-boto3-mediapackage-1.28.15.post1/README.md`

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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__init__.py` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__init__.pyi` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/__main__.py` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackage 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.MediaPackage 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage\nOther"
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

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/client.py` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,39 +10,42 @@
     from mypy_boto3_mediapackage.client import MediaPackageClient
 
     session = Session()
     client: MediaPackageClient = session.client("mediapackage")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import OriginationType
 from .paginator import ListChannelsPaginator, ListHarvestJobsPaginator, ListOriginEndpointsPaginator
 from .type_defs import (
     AuthorizationTypeDef,
     CmafPackageCreateOrUpdateParametersTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateHarvestJobResponseTypeDef,
     CreateOriginEndpointResponseTypeDef,
+    DashPackageOutputTypeDef,
     DashPackageTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
+    HlsPackageOutputTypeDef,
     HlsPackageTypeDef,
     IngressAccessLogsTypeDef,
     ListChannelsResponseTypeDef,
     ListHarvestJobsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MssPackageOutputTypeDef,
     MssPackageTypeDef,
     RotateChannelCredentialsResponseTypeDef,
     RotateIngestEndpointCredentialsResponseTypeDef,
     S3DestinationTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
 )
@@ -152,19 +155,19 @@
     def create_origin_endpoint(
         self,
         *,
         ChannelId: str,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: DashPackageTypeDef = ...,
+        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
         Description: str = ...,
-        HlsPackage: HlsPackageTypeDef = ...,
+        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
         ManifestName: str = ...,
-        MssPackage: MssPackageTypeDef = ...,
+        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         Tags: Mapping[str, str] = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> CreateOriginEndpointResponseTypeDef:
         """
@@ -323,19 +326,19 @@
 
     def update_origin_endpoint(
         self,
         *,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: DashPackageTypeDef = ...,
+        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
         Description: str = ...,
-        HlsPackage: HlsPackageTypeDef = ...,
+        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
         ManifestName: str = ...,
-        MssPackage: MssPackageTypeDef = ...,
+        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Updates an existing OriginEndpoint.
```

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/client.pyi` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,39 +10,42 @@
     from mypy_boto3_mediapackage.client import MediaPackageClient
 
     session = Session()
     client: MediaPackageClient = session.client("mediapackage")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import OriginationType
 from .paginator import ListChannelsPaginator, ListHarvestJobsPaginator, ListOriginEndpointsPaginator
 from .type_defs import (
     AuthorizationTypeDef,
     CmafPackageCreateOrUpdateParametersTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateHarvestJobResponseTypeDef,
     CreateOriginEndpointResponseTypeDef,
+    DashPackageOutputTypeDef,
     DashPackageTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
+    HlsPackageOutputTypeDef,
     HlsPackageTypeDef,
     IngressAccessLogsTypeDef,
     ListChannelsResponseTypeDef,
     ListHarvestJobsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MssPackageOutputTypeDef,
     MssPackageTypeDef,
     RotateChannelCredentialsResponseTypeDef,
     RotateIngestEndpointCredentialsResponseTypeDef,
     S3DestinationTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
 )
@@ -142,19 +145,19 @@
     def create_origin_endpoint(
         self,
         *,
         ChannelId: str,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: DashPackageTypeDef = ...,
+        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
         Description: str = ...,
-        HlsPackage: HlsPackageTypeDef = ...,
+        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
         ManifestName: str = ...,
-        MssPackage: MssPackageTypeDef = ...,
+        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         Tags: Mapping[str, str] = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> CreateOriginEndpointResponseTypeDef:
         """
@@ -297,19 +300,19 @@
         """
     def update_origin_endpoint(
         self,
         *,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: DashPackageTypeDef = ...,
+        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
         Description: str = ...,
-        HlsPackage: HlsPackageTypeDef = ...,
+        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
         ManifestName: str = ...,
-        MssPackage: MssPackageTypeDef = ...,
+        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Updates an existing OriginEndpoint.
```

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/literals.py` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/literals.pyi` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/paginator.py` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/paginator.pyi` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/type_defs.py` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage/type_defs.pyi` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.28.15
-Summary: Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediapackage-1.28.15/mypy_boto3_mediapackage.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-1.28.15.post1/mypy_boto3_mediapackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.15/setup.py` & `mypy-boto3-mediapackage-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_mediapackage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.MediaPackage 1.28.15 service generated with mypy-boto3-builder"
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

