# Comparing `tmp/mypy-boto3-efs-1.28.15.tar.gz` & `tmp/mypy-boto3-efs-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-efs-1.28.15.tar", last modified: Fri Jul 28 20:42:43 2023, max compression
+gzip compressed data, was "mypy-boto3-efs-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
```

## Comparing `mypy-boto3-efs-1.28.15.tar` & `mypy-boto3-efs-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.889042 mypy-boto3-efs-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15677 2023-07-28 20:42:43.889042 mypy-boto3-efs-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.881042 mypy-boto3-efs-1.28.15/mypy_boto3_efs/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23463 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24584 2023-07-28 20:24:58.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-07-28 20:24:58.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.889042 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15677 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.889042 mypy-boto3-efs-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.509128 mypy-boto3-efs-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-29 10:03:02.509128 mypy-boto3-efs-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.497128 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23569 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24584 2023-07-29 09:44:28.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.509128 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.509128 mypy-boto3-efs-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-efs-1.28.15/LICENSE` & `mypy-boto3-efs-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15/PKG-INFO` & `mypy-boto3-efs-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.28.15
-Summary: Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-efs-1.28.15/README.md` & `mypy-boto3-efs-1.28.15.post1/README.md`

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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/__init__.py` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/__init__.pyi` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/__main__.py` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EFS 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.EFS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS\nOther"
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

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/client.py` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_efs.client import EFSClient
 
     session = Session()
     client: EFSClient = session.client("efs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PerformanceModeType, ResourceIdTypeType, ThroughputModeType
 from .paginator import (
     DescribeFileSystemsPaginator,
     DescribeMountTargetsPaginator,
@@ -39,14 +39,15 @@
     EmptyResponseMetadataTypeDef,
     FileSystemDescriptionResponseTypeDef,
     FileSystemPolicyDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceResponseTypeDef,
     MountTargetDescriptionResponseTypeDef,
+    PosixUserOutputTypeDef,
     PosixUserTypeDef,
     PutAccountPreferencesResponseTypeDef,
     ReplicationConfigurationDescriptionResponseTypeDef,
     RootDirectoryTypeDef,
     TagTypeDef,
 )
 
@@ -136,15 +137,15 @@
 
     def create_access_point(
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
-        PosixUser: PosixUserTypeDef = ...,
+        PosixUser: Union[PosixUserTypeDef, PosixUserOutputTypeDef] = ...,
         RootDirectory: RootDirectoryTypeDef = ...
     ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_access_point)
```

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/client.pyi` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_efs.client import EFSClient
 
     session = Session()
     client: EFSClient = session.client("efs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PerformanceModeType, ResourceIdTypeType, ThroughputModeType
 from .paginator import (
     DescribeFileSystemsPaginator,
     DescribeMountTargetsPaginator,
@@ -39,14 +39,15 @@
     EmptyResponseMetadataTypeDef,
     FileSystemDescriptionResponseTypeDef,
     FileSystemPolicyDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceResponseTypeDef,
     MountTargetDescriptionResponseTypeDef,
+    PosixUserOutputTypeDef,
     PosixUserTypeDef,
     PutAccountPreferencesResponseTypeDef,
     ReplicationConfigurationDescriptionResponseTypeDef,
     RootDirectoryTypeDef,
     TagTypeDef,
 )
 
@@ -129,15 +130,15 @@
         """
     def create_access_point(
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
-        PosixUser: PosixUserTypeDef = ...,
+        PosixUser: Union[PosixUserTypeDef, PosixUserOutputTypeDef] = ...,
         RootDirectory: RootDirectoryTypeDef = ...
     ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_access_point)
```

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/literals.py` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/literals.pyi` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/paginator.py` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/paginator.pyi` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/type_defs.py` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs/type_defs.pyi` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/PKG-INFO` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.28.15
-Summary: Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/SOURCES.txt` & `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15/setup.py` & `mypy-boto3-efs-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-efs",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_efs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

