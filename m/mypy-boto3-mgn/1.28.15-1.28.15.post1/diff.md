# Comparing `tmp/mypy-boto3-mgn-1.28.15.tar.gz` & `tmp/mypy-boto3-mgn-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mgn-1.28.15.tar", last modified: Fri Jul 28 20:43:18 2023, max compression
+gzip compressed data, was "mypy-boto3-mgn-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:42 2023, max compression
```

## Comparing `mypy-boto3-mgn-1.28.15.tar` & `mypy-boto3-mgn-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.665521 mypy-boto3-mgn-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-07-28 20:43:18.665521 mypy-boto3-mgn-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22021 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.665521 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51698 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51611 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-28 20:31:56.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-07-28 20:31:56.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18006 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    80885 2023-07-28 20:32:00.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    80768 2023-07-28 20:31:57.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.665521 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:18.665521 mypy-boto3-mgn-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:31:54.000000 mypy-boto3-mgn-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:42.693293 mypy-boto3-mgn-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-07-29 10:03:42.693293 mypy-boto3-mgn-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22021 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:42.669293 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51858 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51771 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-29 09:51:36.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-07-29 09:51:36.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-07-29 09:51:36.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18006 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    80885 2023-07-29 09:51:38.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80768 2023-07-29 09:51:37.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:42.693293 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-07-29 10:03:42.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:03:42.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:42.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:42.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:42.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:42.000000 mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:42.693293 mypy-boto3-mgn-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:51:35.000000 mypy-boto3-mgn-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-mgn-1.28.15/LICENSE` & `mypy-boto3-mgn-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.15/PKG-INFO` & `mypy-boto3-mgn-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.28.15
-Summary: Type annotations for boto3.mgn 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.mgn 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mgn-1.28.15/README.md` & `mypy-boto3-mgn-1.28.15.post1/README.md`

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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__init__.py` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__init__.pyi` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__main__.py` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.mgn 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.mgn 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn\nOther"
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

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/client.py` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_mgn.client import mgnClient
 
     session = Session()
     client: mgnClient = session.client("mgn")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionCategoryType,
     BootModeType,
     LaunchDispositionType,
@@ -71,14 +71,15 @@
     ListImportsResponseTypeDef,
     ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
+    PostLaunchActionsOutputTypeDef,
     PostLaunchActionsTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTypeDef,
     S3BucketSourceTypeDef,
     SourceServerActionDocumentResponseTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
@@ -233,15 +234,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
-        postLaunchActions: PostLaunchActionsTypeDef = ...,
+        postLaunchActions: Union[PostLaunchActionsTypeDef, PostLaunchActionsOutputTypeDef] = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         tags: Mapping[str, str] = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
@@ -882,15 +883,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         name: str = ...,
-        postLaunchActions: PostLaunchActionsTypeDef = ...,
+        postLaunchActions: Union[PostLaunchActionsTypeDef, PostLaunchActionsOutputTypeDef] = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTypeDef:
         """
         Updates multiple LaunchConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration)
@@ -905,15 +906,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
-        postLaunchActions: PostLaunchActionsTypeDef = ...,
+        postLaunchActions: Union[PostLaunchActionsTypeDef, PostLaunchActionsOutputTypeDef] = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
```

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/client.pyi` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_mgn.client import mgnClient
 
     session = Session()
     client: mgnClient = session.client("mgn")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionCategoryType,
     BootModeType,
     LaunchDispositionType,
@@ -71,14 +71,15 @@
     ListImportsResponseTypeDef,
     ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
+    PostLaunchActionsOutputTypeDef,
     PostLaunchActionsTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTypeDef,
     S3BucketSourceTypeDef,
     SourceServerActionDocumentResponseTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
@@ -220,15 +221,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
-        postLaunchActions: PostLaunchActionsTypeDef = ...,
+        postLaunchActions: Union[PostLaunchActionsTypeDef, PostLaunchActionsOutputTypeDef] = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         tags: Mapping[str, str] = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
@@ -815,15 +816,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         name: str = ...,
-        postLaunchActions: PostLaunchActionsTypeDef = ...,
+        postLaunchActions: Union[PostLaunchActionsTypeDef, PostLaunchActionsOutputTypeDef] = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTypeDef:
         """
         Updates multiple LaunchConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration)
@@ -837,15 +838,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
-        postLaunchActions: PostLaunchActionsTypeDef = ...,
+        postLaunchActions: Union[PostLaunchActionsTypeDef, PostLaunchActionsOutputTypeDef] = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
```

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/literals.py` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/literals.pyi` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/paginator.py` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/paginator.pyi` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/type_defs.py` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/type_defs.pyi` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/PKG-INFO` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.28.15
-Summary: Type annotations for boto3.mgn 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.mgn 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/SOURCES.txt` & `mypy-boto3-mgn-1.28.15.post1/mypy_boto3_mgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.15/setup.py` & `mypy-boto3-mgn-1.28.15.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mgn",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_mgn"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.mgn 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.mgn 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

