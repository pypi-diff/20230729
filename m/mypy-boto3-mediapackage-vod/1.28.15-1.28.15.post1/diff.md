# Comparing `tmp/mypy-boto3-mediapackage-vod-1.28.15.tar.gz` & `tmp/mypy-boto3-mediapackage-vod-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-vod-1.28.15.tar", last modified: Fri Jul 28 20:43:15 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-vod-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:40 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-vod-1.28.15.tar` & `mypy-boto3-mediapackage-vod-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.345475 mypy-boto3-mediapackage-vod-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-07-28 20:43:15.345475 mypy-boto3-mediapackage-vod-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.341475 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-28 20:31:36.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-28 20:31:36.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-07-28 20:31:36.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-07-28 20:31:36.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:15.345475 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:15.000000 mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:15.345475 mypy-boto3-mediapackage-vod-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 20:31:35.000000 mypy-boto3-mediapackage-vod-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.209282 mypy-boto3-mediapackage-vod-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15978 2023-07-29 10:03:40.205282 mypy-boto3-mediapackage-vod-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.197282 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-29 09:51:15.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-29 09:51:15.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-07-29 09:51:15.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-07-29 09:51:15.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.205282 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15978 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:03:39.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:40.209282 mypy-boto3-mediapackage-vod-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 09:51:14.000000 mypy-boto3-mediapackage-vod-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/LICENSE` & `mypy-boto3-mediapackage-vod-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/PKG-INFO` & `mypy-boto3-mediapackage-vod-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage-vod
-Version: 1.28.15
-Summary: Type annotations for boto3.MediaPackageVod 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MediaPackageVod 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/README.md` & `mypy-boto3-mediapackage-vod-1.28.15.post1/README.md`

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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__init__.py` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__init__.pyi` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/__main__.py` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackageVod 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.MediaPackageVod 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod\nOther"
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

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/client.py` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,41 +10,45 @@
     from mypy_boto3_mediapackage_vod.client import MediaPackageVodClient
 
     session = Session()
     client: MediaPackageVodClient = session.client("mediapackage-vod")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListAssetsPaginator,
     ListPackagingConfigurationsPaginator,
     ListPackagingGroupsPaginator,
 )
 from .type_defs import (
     AuthorizationTypeDef,
+    CmafPackageOutputTypeDef,
     CmafPackageTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateAssetResponseTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
+    DashPackageOutputTypeDef,
     DashPackageTypeDef,
     DescribeAssetResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
+    HlsPackageOutputTypeDef,
     HlsPackageTypeDef,
     ListAssetsResponseTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
     ListPackagingGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MssPackageOutputTypeDef,
     MssPackageTypeDef,
     UpdatePackagingGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -136,18 +140,18 @@
         """
 
     def create_packaging_configuration(
         self,
         *,
         Id: str,
         PackagingGroupId: str,
-        CmafPackage: CmafPackageTypeDef = ...,
-        DashPackage: DashPackageTypeDef = ...,
-        HlsPackage: HlsPackageTypeDef = ...,
-        MssPackage: MssPackageTypeDef = ...,
+        CmafPackage: Union[CmafPackageTypeDef, CmafPackageOutputTypeDef] = ...,
+        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
+        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
+        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePackagingConfigurationResponseTypeDef:
         """
         Creates a new MediaPackage VOD PackagingConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/client/#create_packaging_configuration)
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/client.pyi` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,41 +10,45 @@
     from mypy_boto3_mediapackage_vod.client import MediaPackageVodClient
 
     session = Session()
     client: MediaPackageVodClient = session.client("mediapackage-vod")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListAssetsPaginator,
     ListPackagingConfigurationsPaginator,
     ListPackagingGroupsPaginator,
 )
 from .type_defs import (
     AuthorizationTypeDef,
+    CmafPackageOutputTypeDef,
     CmafPackageTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateAssetResponseTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
+    DashPackageOutputTypeDef,
     DashPackageTypeDef,
     DescribeAssetResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
+    HlsPackageOutputTypeDef,
     HlsPackageTypeDef,
     ListAssetsResponseTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
     ListPackagingGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MssPackageOutputTypeDef,
     MssPackageTypeDef,
     UpdatePackagingGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -127,18 +131,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/client/#create_asset)
         """
     def create_packaging_configuration(
         self,
         *,
         Id: str,
         PackagingGroupId: str,
-        CmafPackage: CmafPackageTypeDef = ...,
-        DashPackage: DashPackageTypeDef = ...,
-        HlsPackage: HlsPackageTypeDef = ...,
-        MssPackage: MssPackageTypeDef = ...,
+        CmafPackage: Union[CmafPackageTypeDef, CmafPackageOutputTypeDef] = ...,
+        DashPackage: Union[DashPackageTypeDef, DashPackageOutputTypeDef] = ...,
+        HlsPackage: Union[HlsPackageTypeDef, HlsPackageOutputTypeDef] = ...,
+        MssPackage: Union[MssPackageTypeDef, MssPackageOutputTypeDef] = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePackagingConfigurationResponseTypeDef:
         """
         Creates a new MediaPackage VOD PackagingConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/client/#create_packaging_configuration)
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/literals.py` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/literals.pyi` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/paginator.py` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/paginator.pyi` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/type_defs.py` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod/type_defs.pyi` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage-vod
-Version: 1.28.15
-Summary: Type annotations for boto3.MediaPackageVod 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MediaPackageVod 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-vod-1.28.15.post1/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.15/setup.py` & `mypy-boto3-mediapackage-vod-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage-vod",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_mediapackage_vod"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.MediaPackageVod 1.28.15 service generated with"
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

