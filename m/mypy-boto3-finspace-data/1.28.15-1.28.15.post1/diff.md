# Comparing `tmp/mypy-boto3-finspace-data-1.28.15.tar.gz` & `tmp/mypy-boto3-finspace-data-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-data-1.28.15.tar", last modified: Fri Jul 28 20:42:47 2023, max compression
+gzip compressed data, was "mypy-boto3-finspace-data-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:08 2023, max compression
```

## Comparing `mypy-boto3-finspace-data-1.28.15.tar` & `mypy-boto3-finspace-data-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.237089 mypy-boto3-finspace-data-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-07-28 20:42:47.237089 mypy-boto3-finspace-data-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.229089 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25240 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35600 2023-07-28 20:25:51.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35545 2023-07-28 20:25:51.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.237089 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:47.237089 mypy-boto3-finspace-data-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:08.061150 mypy-boto3-finspace-data-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-07-29 10:03:08.057150 mypy-boto3-finspace-data-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:08.045150 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25421 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35600 2023-07-29 09:45:23.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35545 2023-07-29 09:45:23.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:08.057150 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:08.061150 mypy-boto3-finspace-data-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-finspace-data-1.28.15/LICENSE` & `mypy-boto3-finspace-data-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15/PKG-INFO` & `mypy-boto3-finspace-data-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace-data
-Version: 1.28.15
-Summary: Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-finspace-data-1.28.15/README.md` & `mypy-boto3-finspace-data-1.28.15.post1/README.md`

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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__init__.py` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__init__.pyi` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__main__.py` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FinSpaceData 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.FinSpaceData 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData\nOther"
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

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/client.py` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_finspace_data.client import FinSpaceDataClient
 
     session = Session()
     client: FinSpaceDataClient = session.client("finspace-data")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApiAccessType,
     ApplicationPermissionType,
     ChangeTypeType,
@@ -37,14 +37,15 @@
     AssociateUserToPermissionGroupResponseTypeDef,
     CreateChangesetResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDataViewResponseTypeDef,
     CreatePermissionGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     DatasetOwnerInfoTypeDef,
+    DataViewDestinationTypeParamsOutputTypeDef,
     DataViewDestinationTypeParamsTypeDef,
     DeleteDatasetResponseTypeDef,
     DeletePermissionGroupResponseTypeDef,
     DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupResponseTypeDef,
     EnableUserResponseTypeDef,
     GetChangesetResponseTypeDef,
@@ -60,14 +61,15 @@
     ListDataViewsResponseTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ResetUserPasswordResponseTypeDef,
+    SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
     UpdateChangesetResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdatePermissionGroupResponseTypeDef,
     UpdateUserResponseTypeDef,
 )
 
@@ -159,15 +161,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#create_changeset)
         """
 
     def create_data_view(
         self,
         *,
         datasetId: str,
-        destinationTypeParams: DataViewDestinationTypeParamsTypeDef,
+        destinationTypeParams: Union[
+            DataViewDestinationTypeParamsTypeDef, DataViewDestinationTypeParamsOutputTypeDef
+        ],
         clientToken: str = ...,
         autoUpdate: bool = ...,
         sortColumns: Sequence[str] = ...,
         partitionColumns: Sequence[str] = ...,
         asOfTimestamp: int = ...
     ) -> CreateDataViewResponseTypeDef:
         """
@@ -183,15 +187,15 @@
         datasetTitle: str,
         kind: DatasetKindType,
         permissionGroupParams: PermissionGroupParamsTypeDef,
         clientToken: str = ...,
         datasetDescription: str = ...,
         ownerInfo: DatasetOwnerInfoTypeDef = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionTypeDef = ...
+        schemaDefinition: Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#create_dataset)
         """
@@ -461,15 +465,15 @@
         *,
         datasetId: str,
         datasetTitle: str,
         kind: DatasetKindType,
         clientToken: str = ...,
         datasetDescription: str = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionTypeDef = ...
+        schemaDefinition: Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef] = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Updates a FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#update_dataset)
         """
```

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/client.pyi` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_finspace_data.client import FinSpaceDataClient
 
     session = Session()
     client: FinSpaceDataClient = session.client("finspace-data")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApiAccessType,
     ApplicationPermissionType,
     ChangeTypeType,
@@ -37,14 +37,15 @@
     AssociateUserToPermissionGroupResponseTypeDef,
     CreateChangesetResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDataViewResponseTypeDef,
     CreatePermissionGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     DatasetOwnerInfoTypeDef,
+    DataViewDestinationTypeParamsOutputTypeDef,
     DataViewDestinationTypeParamsTypeDef,
     DeleteDatasetResponseTypeDef,
     DeletePermissionGroupResponseTypeDef,
     DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupResponseTypeDef,
     EnableUserResponseTypeDef,
     GetChangesetResponseTypeDef,
@@ -60,14 +61,15 @@
     ListDataViewsResponseTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ResetUserPasswordResponseTypeDef,
+    SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
     UpdateChangesetResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdatePermissionGroupResponseTypeDef,
     UpdateUserResponseTypeDef,
 )
 
@@ -150,15 +152,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_changeset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#create_changeset)
         """
     def create_data_view(
         self,
         *,
         datasetId: str,
-        destinationTypeParams: DataViewDestinationTypeParamsTypeDef,
+        destinationTypeParams: Union[
+            DataViewDestinationTypeParamsTypeDef, DataViewDestinationTypeParamsOutputTypeDef
+        ],
         clientToken: str = ...,
         autoUpdate: bool = ...,
         sortColumns: Sequence[str] = ...,
         partitionColumns: Sequence[str] = ...,
         asOfTimestamp: int = ...
     ) -> CreateDataViewResponseTypeDef:
         """
@@ -173,15 +177,15 @@
         datasetTitle: str,
         kind: DatasetKindType,
         permissionGroupParams: PermissionGroupParamsTypeDef,
         clientToken: str = ...,
         datasetDescription: str = ...,
         ownerInfo: DatasetOwnerInfoTypeDef = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionTypeDef = ...
+        schemaDefinition: Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#create_dataset)
         """
@@ -425,15 +429,15 @@
         *,
         datasetId: str,
         datasetTitle: str,
         kind: DatasetKindType,
         clientToken: str = ...,
         datasetDescription: str = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionTypeDef = ...
+        schemaDefinition: Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef] = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Updates a FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#update_dataset)
         """
```

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/literals.py` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/literals.pyi` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/paginator.py` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/paginator.pyi` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/type_defs.py` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/type_defs.pyi` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/PKG-INFO` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace-data
-Version: 1.28.15
-Summary: Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/SOURCES.txt` & `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15/setup.py` & `mypy-boto3-finspace-data-1.28.15.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace-data",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_finspace_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder"
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

