# Comparing `tmp/mypy-boto3-lakeformation-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-lakeformation-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lakeformation-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:30 2023, max compression
+gzip compressed data, was "mypy-boto3-lakeformation-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-lakeformation-1.28.15.post1.tar` & `mypy-boto3-lakeformation-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.253230 mypy-boto3-lakeformation-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19230 2023-07-29 10:03:30.253230 mypy-boto3-lakeformation-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.253230 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38144 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38085 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-07-29 09:49:07.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-07-29 09:49:07.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54848 2023-07-29 09:49:08.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54749 2023-07-29 09:49:07.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.253230 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19230 2023-07-29 10:03:30.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-29 10:03:30.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:30.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:30.000000 mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:30.253230 mypy-boto3-lakeformation-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-29 09:49:06.000000 mypy-boto3-lakeformation-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19383 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37043 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53022 2023-07-18 01:01:31.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52937 2023-07-18 01:01:31.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19383 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-18 01:01:29.000000 mypy-boto3-lakeformation-1.28.4/setup.py
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/LICENSE` & `mypy-boto3-lakeformation-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/PKG-INFO` & `mypy-boto3-lakeformation-1.28.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LakeFormation 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.4
+Summary: Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,31 +351,35 @@
 ### Typed dictionaries
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
-    LFTagPairOutputTypeDef,
     LFTagPairTypeDef,
     ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
+    LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
@@ -412,30 +416,30 @@
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
     TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
-    ColumnLFTagTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     CommitTransactionResponseTypeDef,
     GetLFTagResponseTypeDef,
     GetQueryStateResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
-    ListLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
-    LFTagErrorTypeDef,
     PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    ColumnLFTagTypeDef,
+    LFTagErrorTypeDef,
+    ListLFTagsResponseTypeDef,
     TableWithColumnsResourceOutputTypeDef,
     TableWithColumnsResourceTypeDef,
     DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
     DeleteObjectsOnCancelRequestRequestTypeDef,
@@ -456,32 +460,32 @@
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
     StartQueryPlanningRequestRequestTypeDef,
+    DataLakeSettingsOutputTypeDef,
+    DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    DataLakeSettingsOutputTypeDef,
-    DataLakeSettingsTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
     CreateDataCellsFilterRequestRequestTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     GetTableObjectsResponseTypeDef,
-    SearchTablesByLFTagsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
+    SearchTablesByLFTagsResponseTypeDef,
     BatchPermissionsRequestEntryOutputTypeDef,
     PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
@@ -493,15 +497,15 @@
     BatchGrantPermissionsRequestRequestTypeDef,
     BatchRevokePermissionsRequestRequestTypeDef,
     BatchGrantPermissionsResponseTypeDef,
     BatchRevokePermissionsResponseTypeDef,
 )
 
 
-def get_structure() -> LFTagPairOutputTypeDef:
+def get_structure() -> LFTagPairTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/README.md` & `mypy-boto3-lakeformation-1.28.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,31 +319,35 @@
 ### Typed dictionaries
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
-    LFTagPairOutputTypeDef,
     LFTagPairTypeDef,
     ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
+    LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
@@ -380,30 +384,30 @@
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
     TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
-    ColumnLFTagTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     CommitTransactionResponseTypeDef,
     GetLFTagResponseTypeDef,
     GetQueryStateResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
-    ListLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
-    LFTagErrorTypeDef,
     PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    ColumnLFTagTypeDef,
+    LFTagErrorTypeDef,
+    ListLFTagsResponseTypeDef,
     TableWithColumnsResourceOutputTypeDef,
     TableWithColumnsResourceTypeDef,
     DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
     DeleteObjectsOnCancelRequestRequestTypeDef,
@@ -424,32 +428,32 @@
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
     StartQueryPlanningRequestRequestTypeDef,
+    DataLakeSettingsOutputTypeDef,
+    DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    DataLakeSettingsOutputTypeDef,
-    DataLakeSettingsTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
     CreateDataCellsFilterRequestRequestTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     GetTableObjectsResponseTypeDef,
-    SearchTablesByLFTagsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
+    SearchTablesByLFTagsResponseTypeDef,
     BatchPermissionsRequestEntryOutputTypeDef,
     PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
@@ -461,15 +465,15 @@
     BatchGrantPermissionsRequestRequestTypeDef,
     BatchRevokePermissionsRequestRequestTypeDef,
     BatchGrantPermissionsResponseTypeDef,
     BatchRevokePermissionsResponseTypeDef,
 )
 
 
-def get_structure() -> LFTagPairOutputTypeDef:
+def get_structure() -> LFTagPairTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/__init__.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/__init__.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/__main__.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LakeFormation 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.LakeFormation 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/client.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -36,22 +36,19 @@
     SearchTablesByLFTagsPaginator,
 )
 from .type_defs import (
     AddLFTagsToResourceResponseTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     BatchGrantPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryOutputTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     BatchRevokePermissionsResponseTypeDef,
     CommitTransactionResponseTypeDef,
-    DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     DataLakePrincipalTypeDef,
-    DataLakeSettingsOutputTypeDef,
     DataLakeSettingsTypeDef,
     DescribeResourceResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
@@ -60,57 +57,50 @@
     GetQueryStatisticsResponseTypeDef,
     GetResourceLFTagsResponseTypeDef,
     GetTableObjectsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
     GetWorkUnitsResponseTypeDef,
-    LFTagOutputTypeDef,
-    LFTagPairOutputTypeDef,
     LFTagPairTypeDef,
     LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     ListTransactionsResponseTypeDef,
     PartitionValueListTypeDef,
     QueryPlanningContextTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    ResourceOutputTypeDef,
     ResourceTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
-    TableResourceOutputTypeDef,
     TableResourceTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     VirtualObjectTypeDef,
     WriteOperationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LakeFormationClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConcurrentModificationException: Type[BotocoreClientError]
     EntityNotFoundException: Type[BotocoreClientError]
     ExpiredException: Type[BotocoreClientError]
@@ -124,15 +114,14 @@
     StatisticsNotReadyYetException: Type[BotocoreClientError]
     ThrottledException: Type[BotocoreClientError]
     TransactionCanceledException: Type[BotocoreClientError]
     TransactionCommitInProgressException: Type[BotocoreClientError]
     TransactionCommittedException: Type[BotocoreClientError]
     WorkUnitsNotReadyYetException: Type[BotocoreClientError]
 
-
 class LakeFormationClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/)
     """
 
     meta: ClientMeta
@@ -141,146 +130,117 @@
     def exceptions(self) -> Exceptions:
         """
         LakeFormationClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#exceptions)
         """
-
     def add_lf_tags_to_resource(
-        self,
-        *,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef],
-        LFTags: Sequence[Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> AddLFTagsToResourceResponseTypeDef:
         """
         Attaches one or more LF-tags to an existing resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.add_lf_tags_to_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#add_lf_tags_to_resource)
         """
-
     def assume_decorated_role_with_saml(
         self, *, SAMLAssertion: str, RoleArn: str, PrincipalArn: str, DurationSeconds: int = ...
     ) -> AssumeDecoratedRoleWithSAMLResponseTypeDef:
         """
         Allows a caller to assume an IAM role decorated as the SAML user specified in
         the SAML assertion included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.assume_decorated_role_with_saml)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#assume_decorated_role_with_saml)
         """
-
     def batch_grant_permissions(
-        self,
-        *,
-        Entries: Sequence[
-            Union[BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef]
-        ],
-        CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchGrantPermissionsResponseTypeDef:
         """
         Batch operation to grant permissions to the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_grant_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#batch_grant_permissions)
         """
-
     def batch_revoke_permissions(
-        self,
-        *,
-        Entries: Sequence[
-            Union[BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef]
-        ],
-        CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchRevokePermissionsResponseTypeDef:
         """
         Batch operation to revoke permissions from the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_revoke_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#batch_revoke_permissions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#can_paginate)
         """
-
     def cancel_transaction(self, *, TransactionId: str) -> Dict[str, Any]:
         """
         Attempts to cancel the specified transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.cancel_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#cancel_transaction)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#close)
         """
-
     def commit_transaction(self, *, TransactionId: str) -> CommitTransactionResponseTypeDef:
         """
         Attempts to commit the specified transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.commit_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#commit_transaction)
         """
-
-    def create_data_cells_filter(
-        self, *, TableData: Union[DataCellsFilterTypeDef, DataCellsFilterOutputTypeDef]
-    ) -> Dict[str, Any]:
+    def create_data_cells_filter(self, *, TableData: DataCellsFilterTypeDef) -> Dict[str, Any]:
         """
         Creates a data cell filter to allow one to grant access to certain columns on
         certain rows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#create_data_cells_filter)
         """
-
     def create_lf_tag(
         self, *, TagKey: str, TagValues: Sequence[str], CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Creates an LF-tag with the specified name and values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_lf_tag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#create_lf_tag)
         """
-
     def delete_data_cells_filter(
         self,
         *,
         TableCatalogId: str = ...,
         DatabaseName: str = ...,
         TableName: str = ...,
         Name: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.delete_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#delete_data_cells_filter)
         """
-
     def delete_lf_tag(self, *, TagKey: str, CatalogId: str = ...) -> Dict[str, Any]:
         """
         Deletes the specified LF-tag given a key name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.delete_lf_tag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#delete_lf_tag)
         """
-
     def delete_objects_on_cancel(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         TransactionId: str,
         Objects: Sequence[VirtualObjectTypeDef],
@@ -290,131 +250,114 @@
         For a specific governed table, provides a list of Amazon S3 objects that will be
         written during the current transaction and that can be automatically deleted if
         the transaction is canceled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.delete_objects_on_cancel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#delete_objects_on_cancel)
         """
-
     def deregister_resource(self, *, ResourceArn: str) -> Dict[str, Any]:
         """
         Deregisters the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.deregister_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#deregister_resource)
         """
-
     def describe_resource(self, *, ResourceArn: str) -> DescribeResourceResponseTypeDef:
         """
         Retrieves the current data access role for the given resource registered in Lake
         Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.describe_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#describe_resource)
         """
-
     def describe_transaction(self, *, TransactionId: str) -> DescribeTransactionResponseTypeDef:
         """
         Returns the details of a single transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.describe_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#describe_transaction)
         """
-
     def extend_transaction(self, *, TransactionId: str = ...) -> Dict[str, Any]:
         """
         Indicates to the service that the specified transaction is still active and
         should not be treated as idle and aborted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.extend_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#extend_transaction)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#generate_presigned_url)
         """
-
     def get_data_cells_filter(
         self, *, TableCatalogId: str, DatabaseName: str, TableName: str, Name: str
     ) -> GetDataCellsFilterResponseTypeDef:
         """
         Returns a data cells filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_data_cells_filter)
         """
-
     def get_data_lake_settings(self, *, CatalogId: str = ...) -> GetDataLakeSettingsResponseTypeDef:
         """
         Retrieves the list of the data lake administrators of a Lake Formation-managed
         data lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_data_lake_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_data_lake_settings)
         """
-
     def get_effective_permissions_for_path(
         self, *, ResourceArn: str, CatalogId: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> GetEffectivePermissionsForPathResponseTypeDef:
         """
         Returns the Lake Formation permissions for a specified table or database
         resource located at a path in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_effective_permissions_for_path)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_effective_permissions_for_path)
         """
-
     def get_lf_tag(self, *, TagKey: str, CatalogId: str = ...) -> GetLFTagResponseTypeDef:
         """
         Returns an LF-tag definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_lf_tag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_lf_tag)
         """
-
     def get_query_state(self, *, QueryId: str) -> GetQueryStateResponseTypeDef:
         """
         Returns the state of a query previously submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_query_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_query_state)
         """
-
     def get_query_statistics(self, *, QueryId: str) -> GetQueryStatisticsResponseTypeDef:
         """
         Retrieves statistics on the planning and execution of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_query_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_query_statistics)
         """
-
     def get_resource_lf_tags(
-        self,
-        *,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef],
-        CatalogId: str = ...,
-        ShowAssignedLFTags: bool = ...
+        self, *, Resource: ResourceTypeDef, CatalogId: str = ..., ShowAssignedLFTags: bool = ...
     ) -> GetResourceLFTagsResponseTypeDef:
         """
         Returns the LF-tags applied to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_resource_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_resource_lf_tags)
         """
-
     def get_table_objects(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         TransactionId: str = ...,
@@ -425,15 +368,14 @@
     ) -> GetTableObjectsResponseTypeDef:
         """
         Returns the set of Amazon S3 objects that make up the specified governed table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_table_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_table_objects)
         """
-
     def get_temporary_glue_partition_credentials(
         self,
         *,
         TableArn: str,
         Partition: PartitionValueListTypeDef,
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
@@ -443,15 +385,14 @@
         """
         This API is identical to `GetTemporaryTableCredentials` except that this is used
         when the target Data Catalog resource is of type Partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_partition_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_temporary_glue_partition_credentials)
         """
-
     def get_temporary_glue_table_credentials(
         self,
         *,
         TableArn: str,
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
         AuditContext: AuditContextTypeDef = ...,
@@ -460,114 +401,102 @@
         """
         Allows a caller in a secure environment to assume a role with permission to
         access Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_table_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_temporary_glue_table_credentials)
         """
-
     def get_work_unit_results(
         self, *, QueryId: str, WorkUnitId: int, WorkUnitToken: str
     ) -> GetWorkUnitResultsResponseTypeDef:
         """
         Returns the work units resulting from the query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_work_unit_results)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_work_unit_results)
         """
-
     def get_work_units(
         self, *, QueryId: str, NextToken: str = ..., PageSize: int = ...
     ) -> GetWorkUnitsResponseTypeDef:
         """
         Retrieves the work units generated by the `StartQueryPlanning` operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_work_units)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_work_units)
         """
-
     def grant_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef],
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Grants permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.grant_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#grant_permissions)
         """
-
     def list_data_cells_filter(
-        self,
-        *,
-        Table: Union[TableResourceTypeDef, TableResourceOutputTypeDef] = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
+        self, *, Table: TableResourceTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCellsFilterResponseTypeDef:
         """
         Lists all the data cell filters on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_data_cells_filter)
         """
-
     def list_lf_tags(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListLFTagsResponseTypeDef:
         """
         Lists LF-tags that the requester has permission to view.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_lf_tags)
         """
-
     def list_permissions(
         self,
         *,
         CatalogId: str = ...,
         Principal: DataLakePrincipalTypeDef = ...,
         ResourceType: DataLakeResourceTypeType = ...,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef] = ...,
+        Resource: ResourceTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncludeRelated: str = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Returns a list of the principal permissions on the resource, filtered by the
         permissions of the caller.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_permissions)
         """
-
     def list_resources(
         self,
         *,
         FilterConditionList: Sequence[FilterConditionTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListResourcesResponseTypeDef:
         """
         Lists the resources registered to be managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_resources)
         """
-
     def list_table_storage_optimizers(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         StorageOptimizerType: OptimizerTypeType = ...,
@@ -577,176 +506,154 @@
         """
         Returns the configuration of all storage optimizers associated with a specified
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_table_storage_optimizers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_table_storage_optimizers)
         """
-
     def list_transactions(
         self,
         *,
         CatalogId: str = ...,
         StatusFilter: TransactionStatusFilterType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListTransactionsResponseTypeDef:
         """
         Returns metadata about transactions and their status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_transactions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_transactions)
         """
-
     def put_data_lake_settings(
-        self,
-        *,
-        DataLakeSettings: Union[DataLakeSettingsTypeDef, DataLakeSettingsOutputTypeDef],
-        CatalogId: str = ...
+        self, *, DataLakeSettings: DataLakeSettingsTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Sets the list of data lake administrators who have admin privileges on all
         resources managed by Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.put_data_lake_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#put_data_lake_settings)
         """
-
     def register_resource(
         self,
         *,
         ResourceArn: str,
         UseServiceLinkedRole: bool = ...,
         RoleArn: str = ...,
         WithFederation: bool = ...
     ) -> Dict[str, Any]:
         """
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#register_resource)
         """
-
     def remove_lf_tags_from_resource(
-        self,
-        *,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef],
-        LFTags: Sequence[Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> RemoveLFTagsFromResourceResponseTypeDef:
         """
         Removes an LF-tag from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.remove_lf_tags_from_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#remove_lf_tags_from_resource)
         """
-
     def revoke_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef],
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Revokes permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.revoke_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#revoke_permissions)
         """
-
     def search_databases_by_lf_tags(
         self,
         *,
-        Expression: Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchDatabasesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `DATABASE` resources by `TagCondition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_databases_by_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#search_databases_by_lf_tags)
         """
-
     def search_tables_by_lf_tags(
         self,
         *,
-        Expression: Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `TABLE` resources by `LFTag`s.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_tables_by_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#search_tables_by_lf_tags)
         """
-
     def start_query_planning(
         self, *, QueryPlanningContext: QueryPlanningContextTypeDef, QueryString: str
     ) -> StartQueryPlanningResponseTypeDef:
         """
         Submits a request to process a query statement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.start_query_planning)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#start_query_planning)
         """
-
     def start_transaction(
         self, *, TransactionType: TransactionTypeType = ...
     ) -> StartTransactionResponseTypeDef:
         """
         Starts a new transaction and returns its transaction ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.start_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#start_transaction)
         """
-
-    def update_data_cells_filter(
-        self, *, TableData: Union[DataCellsFilterTypeDef, DataCellsFilterOutputTypeDef]
-    ) -> Dict[str, Any]:
+    def update_data_cells_filter(self, *, TableData: DataCellsFilterTypeDef) -> Dict[str, Any]:
         """
         Updates a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_data_cells_filter)
         """
-
     def update_lf_tag(
         self,
         *,
         TagKey: str,
         CatalogId: str = ...,
         TagValuesToDelete: Sequence[str] = ...,
         TagValuesToAdd: Sequence[str] = ...
     ) -> Dict[str, Any]:
         """
         Updates the list of possible values for the specified LF-tag key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_lf_tag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_lf_tag)
         """
-
     def update_resource(
         self, *, RoleArn: str, ResourceArn: str, WithFederation: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the data access role used for vending access to the given (registered)
         resource in Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_resource)
         """
-
     def update_table_objects(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         WriteOperations: Sequence[WriteOperationTypeDef],
         CatalogId: str = ...,
@@ -755,62 +662,56 @@
         """
         Updates the manifest of Amazon S3 objects that make up the specified governed
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_table_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_table_objects)
         """
-
     def update_table_storage_optimizer(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         StorageOptimizerConfig: Mapping[OptimizerTypeType, Mapping[str, str]],
         CatalogId: str = ...
     ) -> UpdateTableStorageOptimizerResponseTypeDef:
         """
         Updates the configuration of the storage optimizers for a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_table_storage_optimizer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_table_storage_optimizer)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["get_work_units"]) -> GetWorkUnitsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_data_cells_filter"]
     ) -> ListDataCellsFilterPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_lf_tags"]) -> ListLFTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["search_databases_by_lf_tags"]
     ) -> SearchDatabasesByLFTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["search_tables_by_lf_tags"]
     ) -> SearchTablesByLFTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_paginator)
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/client.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,22 +36,19 @@
     SearchTablesByLFTagsPaginator,
 )
 from .type_defs import (
     AddLFTagsToResourceResponseTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     BatchGrantPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryOutputTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     BatchRevokePermissionsResponseTypeDef,
     CommitTransactionResponseTypeDef,
-    DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     DataLakePrincipalTypeDef,
-    DataLakeSettingsOutputTypeDef,
     DataLakeSettingsTypeDef,
     DescribeResourceResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
@@ -60,54 +57,53 @@
     GetQueryStatisticsResponseTypeDef,
     GetResourceLFTagsResponseTypeDef,
     GetTableObjectsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
     GetWorkUnitsResponseTypeDef,
-    LFTagOutputTypeDef,
-    LFTagPairOutputTypeDef,
     LFTagPairTypeDef,
     LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     ListTransactionsResponseTypeDef,
     PartitionValueListTypeDef,
     QueryPlanningContextTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    ResourceOutputTypeDef,
     ResourceTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
-    TableResourceOutputTypeDef,
     TableResourceTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     VirtualObjectTypeDef,
     WriteOperationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("LakeFormationClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConcurrentModificationException: Type[BotocoreClientError]
     EntityNotFoundException: Type[BotocoreClientError]
     ExpiredException: Type[BotocoreClientError]
@@ -121,14 +117,15 @@
     StatisticsNotReadyYetException: Type[BotocoreClientError]
     ThrottledException: Type[BotocoreClientError]
     TransactionCanceledException: Type[BotocoreClientError]
     TransactionCommitInProgressException: Type[BotocoreClientError]
     TransactionCommittedException: Type[BotocoreClientError]
     WorkUnitsNotReadyYetException: Type[BotocoreClientError]
 
+
 class LakeFormationClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/)
     """
 
     meta: ClientMeta
@@ -137,133 +134,130 @@
     def exceptions(self) -> Exceptions:
         """
         LakeFormationClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#exceptions)
         """
+
     def add_lf_tags_to_resource(
-        self,
-        *,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef],
-        LFTags: Sequence[Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> AddLFTagsToResourceResponseTypeDef:
         """
         Attaches one or more LF-tags to an existing resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.add_lf_tags_to_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#add_lf_tags_to_resource)
         """
+
     def assume_decorated_role_with_saml(
         self, *, SAMLAssertion: str, RoleArn: str, PrincipalArn: str, DurationSeconds: int = ...
     ) -> AssumeDecoratedRoleWithSAMLResponseTypeDef:
         """
         Allows a caller to assume an IAM role decorated as the SAML user specified in
         the SAML assertion included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.assume_decorated_role_with_saml)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#assume_decorated_role_with_saml)
         """
+
     def batch_grant_permissions(
-        self,
-        *,
-        Entries: Sequence[
-            Union[BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef]
-        ],
-        CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchGrantPermissionsResponseTypeDef:
         """
         Batch operation to grant permissions to the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_grant_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#batch_grant_permissions)
         """
+
     def batch_revoke_permissions(
-        self,
-        *,
-        Entries: Sequence[
-            Union[BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef]
-        ],
-        CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchRevokePermissionsResponseTypeDef:
         """
         Batch operation to revoke permissions from the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_revoke_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#batch_revoke_permissions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#can_paginate)
         """
+
     def cancel_transaction(self, *, TransactionId: str) -> Dict[str, Any]:
         """
         Attempts to cancel the specified transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.cancel_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#cancel_transaction)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#close)
         """
+
     def commit_transaction(self, *, TransactionId: str) -> CommitTransactionResponseTypeDef:
         """
         Attempts to commit the specified transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.commit_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#commit_transaction)
         """
-    def create_data_cells_filter(
-        self, *, TableData: Union[DataCellsFilterTypeDef, DataCellsFilterOutputTypeDef]
-    ) -> Dict[str, Any]:
+
+    def create_data_cells_filter(self, *, TableData: DataCellsFilterTypeDef) -> Dict[str, Any]:
         """
         Creates a data cell filter to allow one to grant access to certain columns on
         certain rows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#create_data_cells_filter)
         """
+
     def create_lf_tag(
         self, *, TagKey: str, TagValues: Sequence[str], CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Creates an LF-tag with the specified name and values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_lf_tag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#create_lf_tag)
         """
+
     def delete_data_cells_filter(
         self,
         *,
         TableCatalogId: str = ...,
         DatabaseName: str = ...,
         TableName: str = ...,
         Name: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.delete_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#delete_data_cells_filter)
         """
+
     def delete_lf_tag(self, *, TagKey: str, CatalogId: str = ...) -> Dict[str, Any]:
         """
         Deletes the specified LF-tag given a key name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.delete_lf_tag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#delete_lf_tag)
         """
+
     def delete_objects_on_cancel(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         TransactionId: str,
         Objects: Sequence[VirtualObjectTypeDef],
@@ -273,118 +267,127 @@
         For a specific governed table, provides a list of Amazon S3 objects that will be
         written during the current transaction and that can be automatically deleted if
         the transaction is canceled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.delete_objects_on_cancel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#delete_objects_on_cancel)
         """
+
     def deregister_resource(self, *, ResourceArn: str) -> Dict[str, Any]:
         """
         Deregisters the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.deregister_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#deregister_resource)
         """
+
     def describe_resource(self, *, ResourceArn: str) -> DescribeResourceResponseTypeDef:
         """
         Retrieves the current data access role for the given resource registered in Lake
         Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.describe_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#describe_resource)
         """
+
     def describe_transaction(self, *, TransactionId: str) -> DescribeTransactionResponseTypeDef:
         """
         Returns the details of a single transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.describe_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#describe_transaction)
         """
+
     def extend_transaction(self, *, TransactionId: str = ...) -> Dict[str, Any]:
         """
         Indicates to the service that the specified transaction is still active and
         should not be treated as idle and aborted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.extend_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#extend_transaction)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#generate_presigned_url)
         """
+
     def get_data_cells_filter(
         self, *, TableCatalogId: str, DatabaseName: str, TableName: str, Name: str
     ) -> GetDataCellsFilterResponseTypeDef:
         """
         Returns a data cells filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_data_cells_filter)
         """
+
     def get_data_lake_settings(self, *, CatalogId: str = ...) -> GetDataLakeSettingsResponseTypeDef:
         """
         Retrieves the list of the data lake administrators of a Lake Formation-managed
         data lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_data_lake_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_data_lake_settings)
         """
+
     def get_effective_permissions_for_path(
         self, *, ResourceArn: str, CatalogId: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> GetEffectivePermissionsForPathResponseTypeDef:
         """
         Returns the Lake Formation permissions for a specified table or database
         resource located at a path in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_effective_permissions_for_path)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_effective_permissions_for_path)
         """
+
     def get_lf_tag(self, *, TagKey: str, CatalogId: str = ...) -> GetLFTagResponseTypeDef:
         """
         Returns an LF-tag definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_lf_tag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_lf_tag)
         """
+
     def get_query_state(self, *, QueryId: str) -> GetQueryStateResponseTypeDef:
         """
         Returns the state of a query previously submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_query_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_query_state)
         """
+
     def get_query_statistics(self, *, QueryId: str) -> GetQueryStatisticsResponseTypeDef:
         """
         Retrieves statistics on the planning and execution of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_query_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_query_statistics)
         """
+
     def get_resource_lf_tags(
-        self,
-        *,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef],
-        CatalogId: str = ...,
-        ShowAssignedLFTags: bool = ...
+        self, *, Resource: ResourceTypeDef, CatalogId: str = ..., ShowAssignedLFTags: bool = ...
     ) -> GetResourceLFTagsResponseTypeDef:
         """
         Returns the LF-tags applied to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_resource_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_resource_lf_tags)
         """
+
     def get_table_objects(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         TransactionId: str = ...,
@@ -395,14 +398,15 @@
     ) -> GetTableObjectsResponseTypeDef:
         """
         Returns the set of Amazon S3 objects that make up the specified governed table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_table_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_table_objects)
         """
+
     def get_temporary_glue_partition_credentials(
         self,
         *,
         TableArn: str,
         Partition: PartitionValueListTypeDef,
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
@@ -412,14 +416,15 @@
         """
         This API is identical to `GetTemporaryTableCredentials` except that this is used
         when the target Data Catalog resource is of type Partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_partition_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_temporary_glue_partition_credentials)
         """
+
     def get_temporary_glue_table_credentials(
         self,
         *,
         TableArn: str,
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
         AuditContext: AuditContextTypeDef = ...,
@@ -428,106 +433,110 @@
         """
         Allows a caller in a secure environment to assume a role with permission to
         access Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_table_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_temporary_glue_table_credentials)
         """
+
     def get_work_unit_results(
         self, *, QueryId: str, WorkUnitId: int, WorkUnitToken: str
     ) -> GetWorkUnitResultsResponseTypeDef:
         """
         Returns the work units resulting from the query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_work_unit_results)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_work_unit_results)
         """
+
     def get_work_units(
         self, *, QueryId: str, NextToken: str = ..., PageSize: int = ...
     ) -> GetWorkUnitsResponseTypeDef:
         """
         Retrieves the work units generated by the `StartQueryPlanning` operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_work_units)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_work_units)
         """
+
     def grant_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef],
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Grants permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.grant_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#grant_permissions)
         """
+
     def list_data_cells_filter(
-        self,
-        *,
-        Table: Union[TableResourceTypeDef, TableResourceOutputTypeDef] = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
+        self, *, Table: TableResourceTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCellsFilterResponseTypeDef:
         """
         Lists all the data cell filters on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_data_cells_filter)
         """
+
     def list_lf_tags(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListLFTagsResponseTypeDef:
         """
         Lists LF-tags that the requester has permission to view.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_lf_tags)
         """
+
     def list_permissions(
         self,
         *,
         CatalogId: str = ...,
         Principal: DataLakePrincipalTypeDef = ...,
         ResourceType: DataLakeResourceTypeType = ...,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef] = ...,
+        Resource: ResourceTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncludeRelated: str = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Returns a list of the principal permissions on the resource, filtered by the
         permissions of the caller.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_permissions)
         """
+
     def list_resources(
         self,
         *,
         FilterConditionList: Sequence[FilterConditionTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListResourcesResponseTypeDef:
         """
         Lists the resources registered to be managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_resources)
         """
+
     def list_table_storage_optimizers(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         StorageOptimizerType: OptimizerTypeType = ...,
@@ -537,163 +546,167 @@
         """
         Returns the configuration of all storage optimizers associated with a specified
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_table_storage_optimizers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_table_storage_optimizers)
         """
+
     def list_transactions(
         self,
         *,
         CatalogId: str = ...,
         StatusFilter: TransactionStatusFilterType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListTransactionsResponseTypeDef:
         """
         Returns metadata about transactions and their status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_transactions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_transactions)
         """
+
     def put_data_lake_settings(
-        self,
-        *,
-        DataLakeSettings: Union[DataLakeSettingsTypeDef, DataLakeSettingsOutputTypeDef],
-        CatalogId: str = ...
+        self, *, DataLakeSettings: DataLakeSettingsTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Sets the list of data lake administrators who have admin privileges on all
         resources managed by Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.put_data_lake_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#put_data_lake_settings)
         """
+
     def register_resource(
         self,
         *,
         ResourceArn: str,
         UseServiceLinkedRole: bool = ...,
         RoleArn: str = ...,
         WithFederation: bool = ...
     ) -> Dict[str, Any]:
         """
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#register_resource)
         """
+
     def remove_lf_tags_from_resource(
-        self,
-        *,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef],
-        LFTags: Sequence[Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> RemoveLFTagsFromResourceResponseTypeDef:
         """
         Removes an LF-tag from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.remove_lf_tags_from_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#remove_lf_tags_from_resource)
         """
+
     def revoke_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: Union[ResourceTypeDef, ResourceOutputTypeDef],
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Revokes permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.revoke_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#revoke_permissions)
         """
+
     def search_databases_by_lf_tags(
         self,
         *,
-        Expression: Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchDatabasesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `DATABASE` resources by `TagCondition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_databases_by_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#search_databases_by_lf_tags)
         """
+
     def search_tables_by_lf_tags(
         self,
         *,
-        Expression: Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `TABLE` resources by `LFTag`s.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_tables_by_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#search_tables_by_lf_tags)
         """
+
     def start_query_planning(
         self, *, QueryPlanningContext: QueryPlanningContextTypeDef, QueryString: str
     ) -> StartQueryPlanningResponseTypeDef:
         """
         Submits a request to process a query statement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.start_query_planning)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#start_query_planning)
         """
+
     def start_transaction(
         self, *, TransactionType: TransactionTypeType = ...
     ) -> StartTransactionResponseTypeDef:
         """
         Starts a new transaction and returns its transaction ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.start_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#start_transaction)
         """
-    def update_data_cells_filter(
-        self, *, TableData: Union[DataCellsFilterTypeDef, DataCellsFilterOutputTypeDef]
-    ) -> Dict[str, Any]:
+
+    def update_data_cells_filter(self, *, TableData: DataCellsFilterTypeDef) -> Dict[str, Any]:
         """
         Updates a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_data_cells_filter)
         """
+
     def update_lf_tag(
         self,
         *,
         TagKey: str,
         CatalogId: str = ...,
         TagValuesToDelete: Sequence[str] = ...,
         TagValuesToAdd: Sequence[str] = ...
     ) -> Dict[str, Any]:
         """
         Updates the list of possible values for the specified LF-tag key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_lf_tag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_lf_tag)
         """
+
     def update_resource(
         self, *, RoleArn: str, ResourceArn: str, WithFederation: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the data access role used for vending access to the given (registered)
         resource in Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_resource)
         """
+
     def update_table_objects(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         WriteOperations: Sequence[WriteOperationTypeDef],
         CatalogId: str = ...,
@@ -702,56 +715,62 @@
         """
         Updates the manifest of Amazon S3 objects that make up the specified governed
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_table_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_table_objects)
         """
+
     def update_table_storage_optimizer(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         StorageOptimizerConfig: Mapping[OptimizerTypeType, Mapping[str, str]],
         CatalogId: str = ...
     ) -> UpdateTableStorageOptimizerResponseTypeDef:
         """
         Updates the configuration of the storage optimizers for a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_table_storage_optimizer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_table_storage_optimizer)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["get_work_units"]) -> GetWorkUnitsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_data_cells_filter"]
     ) -> ListDataCellsFilterPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_lf_tags"]) -> ListLFTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["search_databases_by_lf_tags"]
     ) -> SearchDatabasesByLFTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["search_tables_by_lf_tags"]
     ) -> SearchTablesByLFTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_paginator)
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/literals.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -292,28 +291,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/literals.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -290,28 +289,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/paginator.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,29 +23,27 @@
     get_work_units_paginator: GetWorkUnitsPaginator = client.get_paginator("get_work_units")
     list_data_cells_filter_paginator: ListDataCellsFilterPaginator = client.get_paginator("list_data_cells_filter")
     list_lf_tags_paginator: ListLFTagsPaginator = client.get_paginator("list_lf_tags")
     search_databases_by_lf_tags_paginator: SearchDatabasesByLFTagsPaginator = client.get_paginator("search_databases_by_lf_tags")
     search_tables_by_lf_tags_paginator: SearchTablesByLFTagsPaginator = client.get_paginator("search_tables_by_lf_tags")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ResourceShareTypeType
 from .type_defs import (
     GetWorkUnitsResponseTypeDef,
-    LFTagOutputTypeDef,
     LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     PaginatorConfigTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
-    TableResourceOutputTypeDef,
     TableResourceTypeDef,
 )
 
 __all__ = (
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
@@ -82,18 +80,15 @@
 class ListDataCellsFilterPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Table: Union[TableResourceTypeDef, TableResourceOutputTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
 
@@ -121,15 +116,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
@@ -140,15 +135,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/paginator.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,27 @@
     get_work_units_paginator: GetWorkUnitsPaginator = client.get_paginator("get_work_units")
     list_data_cells_filter_paginator: ListDataCellsFilterPaginator = client.get_paginator("list_data_cells_filter")
     list_lf_tags_paginator: ListLFTagsPaginator = client.get_paginator("list_lf_tags")
     search_databases_by_lf_tags_paginator: SearchDatabasesByLFTagsPaginator = client.get_paginator("search_databases_by_lf_tags")
     search_tables_by_lf_tags_paginator: SearchTablesByLFTagsPaginator = client.get_paginator("search_tables_by_lf_tags")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ResourceShareTypeType
 from .type_defs import (
     GetWorkUnitsResponseTypeDef,
-    LFTagOutputTypeDef,
     LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     PaginatorConfigTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
-    TableResourceOutputTypeDef,
     TableResourceTypeDef,
 )
 
 __all__ = (
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
@@ -78,18 +76,15 @@
 class ListDataCellsFilterPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Table: Union[TableResourceTypeDef, TableResourceOutputTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
 class ListLFTagsPaginator(Paginator):
@@ -115,15 +110,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
@@ -133,15 +128,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/type_defs.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lakeformation service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lakeformation.type_defs import LFTagPairOutputTypeDef
+    from mypy_boto3_lakeformation.type_defs import LFTagPairTypeDef
 
-    data: LFTagPairOutputTypeDef = {...}
+    data: LFTagPairTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -35,31 +35,35 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "LFTagPairOutputTypeDef",
     "LFTagPairTypeDef",
     "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
+    "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
+    "LFTagPairOutputTypeDef",
     "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
     "CreateLFTagRequestRequestTypeDef",
     "RowFilterOutputTypeDef",
+    "DataCellsFilterResourceOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
+    "DataLocationResourceOutputTypeDef",
     "DataLocationResourceTypeDef",
+    "DatabaseResourceOutputTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
     "VirtualObjectTypeDef",
     "DeregisterResourceRequestRequestTypeDef",
     "DescribeResourceRequestRequestTypeDef",
@@ -96,30 +100,30 @@
     "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
     "TableResourceOutputTypeDef",
     "StartTransactionRequestRequestTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
-    "ColumnLFTagTypeDef",
     "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "CommitTransactionResponseTypeDef",
     "GetLFTagResponseTypeDef",
     "GetQueryStateResponseTypeDef",
     "GetTemporaryGluePartitionCredentialsResponseTypeDef",
     "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsResponseTypeDef",
-    "ListLFTagsResponseTypeDef",
     "StartQueryPlanningResponseTypeDef",
     "StartTransactionResponseTypeDef",
     "UpdateTableStorageOptimizerResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
-    "LFTagErrorTypeDef",
     "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
+    "ColumnLFTagTypeDef",
+    "LFTagErrorTypeDef",
+    "ListLFTagsResponseTypeDef",
     "TableWithColumnsResourceOutputTypeDef",
     "TableWithColumnsResourceTypeDef",
     "DataCellsFilterOutputTypeDef",
     "DataCellsFilterTypeDef",
     "TaggedDatabaseTypeDef",
     "WriteOperationTypeDef",
     "DeleteObjectsOnCancelRequestRequestTypeDef",
@@ -140,32 +144,32 @@
     "SearchTablesByLFTagsRequestRequestTypeDef",
     "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     "ListDataCellsFilterRequestRequestTypeDef",
     "ListTableStorageOptimizersResponseTypeDef",
     "PartitionObjectsTypeDef",
     "StartQueryPlanningRequestRequestTypeDef",
+    "DataLakeSettingsOutputTypeDef",
+    "DataLakeSettingsTypeDef",
     "GetResourceLFTagsResponseTypeDef",
     "TaggedTableTypeDef",
     "AddLFTagsToResourceResponseTypeDef",
     "RemoveLFTagsFromResourceResponseTypeDef",
-    "DataLakeSettingsOutputTypeDef",
-    "DataLakeSettingsTypeDef",
     "GetDataCellsFilterResponseTypeDef",
     "ListDataCellsFilterResponseTypeDef",
     "CreateDataCellsFilterRequestRequestTypeDef",
     "UpdateDataCellsFilterRequestRequestTypeDef",
     "SearchDatabasesByLFTagsResponseTypeDef",
     "UpdateTableObjectsRequestRequestTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "GetTableObjectsResponseTypeDef",
-    "SearchTablesByLFTagsResponseTypeDef",
     "GetDataLakeSettingsResponseTypeDef",
     "PutDataLakeSettingsRequestRequestTypeDef",
+    "SearchTablesByLFTagsResponseTypeDef",
     "BatchPermissionsRequestEntryOutputTypeDef",
     "PrincipalResourcePermissionsTypeDef",
     "AddLFTagsToResourceRequestRequestTypeDef",
     "BatchPermissionsRequestEntryTypeDef",
     "GetResourceLFTagsRequestRequestTypeDef",
     "GrantPermissionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
@@ -176,34 +180,14 @@
     "ListPermissionsResponseTypeDef",
     "BatchGrantPermissionsRequestRequestTypeDef",
     "BatchRevokePermissionsRequestRequestTypeDef",
     "BatchGrantPermissionsResponseTypeDef",
     "BatchRevokePermissionsResponseTypeDef",
 )
 
-_RequiredLFTagPairOutputTypeDef = TypedDict(
-    "_RequiredLFTagPairOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": List[str],
-    },
-)
-_OptionalLFTagPairOutputTypeDef = TypedDict(
-    "_OptionalLFTagPairOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
-    pass
-
-
 _RequiredLFTagPairTypeDef = TypedDict(
     "_RequiredLFTagPairTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -286,15 +270,21 @@
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+DataLakePrincipalOutputTypeDef = TypedDict(
+    "DataLakePrincipalOutputTypeDef",
+    {
+        "DataLakePrincipalIdentifier": str,
+    },
 )
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
@@ -304,20 +294,28 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
+LFTagPairOutputTypeDef = TypedDict(
+    "LFTagPairOutputTypeDef",
+    {
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
 ColumnWildcardOutputTypeDef = TypedDict(
     "ColumnWildcardOutputTypeDef",
     {
         "ExcludedColumnNames": List[str],
     },
-    total=False,
 )
 
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
@@ -355,15 +353,24 @@
 
 RowFilterOutputTypeDef = TypedDict(
     "RowFilterOutputTypeDef",
     {
         "FilterExpression": str,
         "AllRowsWildcard": Dict[str, Any],
     },
-    total=False,
+)
+
+DataCellsFilterResourceOutputTypeDef = TypedDict(
+    "DataCellsFilterResourceOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+    },
 )
 
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
@@ -378,14 +385,22 @@
     {
         "FilterExpression": str,
         "AllRowsWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
+DataLocationResourceOutputTypeDef = TypedDict(
+    "DataLocationResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredDataLocationResourceTypeDef = TypedDict(
     "_RequiredDataLocationResourceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalDataLocationResourceTypeDef = TypedDict(
@@ -399,14 +414,22 @@
 
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
 
+DatabaseResourceOutputTypeDef = TypedDict(
+    "DatabaseResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "Name": str,
+    },
+)
+
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
@@ -513,15 +536,14 @@
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
         "WithFederation": bool,
     },
-    total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -531,33 +553,30 @@
     "TransactionDescriptionTypeDef",
     {
         "TransactionId": str,
         "TransactionStatus": TransactionStatusType,
         "TransactionStartTime": datetime,
         "TransactionEndTime": datetime,
     },
-    total=False,
 )
 
 DetailsMapTypeDef = TypedDict(
     "DetailsMapTypeDef",
     {
         "ResourceShare": List[str],
     },
-    total=False,
 )
 
 ExecutionStatisticsTypeDef = TypedDict(
     "ExecutionStatisticsTypeDef",
     {
         "AverageExecutionTimeMillis": int,
         "DataScannedBytes": int,
         "WorkUnitsExecutedCount": int,
     },
-    total=False,
 )
 
 ExtendTransactionRequestRequestTypeDef = TypedDict(
     "ExtendTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -655,15 +674,14 @@
     "PlanningStatisticsTypeDef",
     {
         "EstimatedDataToScanBytes": int,
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
-    total=False,
 )
 
 _RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
@@ -742,35 +760,22 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
-_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagKeyResourceOutputTypeDef",
+LFTagKeyResourceOutputTypeDef = TypedDict(
+    "LFTagKeyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagKeyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagKeyResourceOutputTypeDef(
-    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
-):
-    pass
-
 
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
@@ -867,15 +872,14 @@
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
         "LastRunDetails": str,
     },
-    total=False,
 )
 
 ListTransactionsRequestRequestTypeDef = TypedDict(
     "ListTransactionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "StatusFilter": TransactionStatusFilterType,
@@ -888,15 +892,14 @@
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
-    total=False,
 )
 
 _RequiredQueryPlanningContextTypeDef = TypedDict(
     "_RequiredQueryPlanningContextTypeDef",
     {
         "DatabaseName": str,
     },
@@ -938,37 +941,24 @@
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredTableResourceOutputTypeDef = TypedDict(
-    "_RequiredTableResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalTableResourceOutputTypeDef = TypedDict(
-    "_OptionalTableResourceOutputTypeDef",
+TableResourceOutputTypeDef = TypedDict(
+    "TableResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "DatabaseName": str,
         "Name": str,
         "TableWildcard": Dict[str, Any],
     },
-    total=False,
 )
 
-
-class TableResourceOutputTypeDef(
-    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
-):
-    pass
-
-
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
@@ -1038,23 +1028,14 @@
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
 
-ColumnLFTagTypeDef = TypedDict(
-    "ColumnLFTagTypeDef",
-    {
-        "Name": str,
-        "LFTags": List[LFTagPairOutputTypeDef],
-    },
-    total=False,
-)
-
 AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
     "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     {
         "AccessKeyId": str,
         "SecretAccessKey": str,
         "SessionToken": str,
         "Expiration": datetime,
@@ -1115,23 +1096,14 @@
     "GetWorkUnitResultsResponseTypeDef",
     {
         "ResultStream": StreamingBody,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListLFTagsResponseTypeDef = TypedDict(
-    "ListLFTagsResponseTypeDef",
-    {
-        "LFTags": List[LFTagPairOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 StartQueryPlanningResponseTypeDef = TypedDict(
     "StartQueryPlanningResponseTypeDef",
     {
         "QueryId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1173,65 +1145,67 @@
 class GetTemporaryGlueTableCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
 ):
     pass
 
 
-LFTagErrorTypeDef = TypedDict(
-    "LFTagErrorTypeDef",
-    {
-        "LFTag": LFTagPairOutputTypeDef,
-        "Error": ErrorDetailTypeDef,
-    },
-    total=False,
-)
-
 PrincipalPermissionsOutputTypeDef = TypedDict(
     "PrincipalPermissionsOutputTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Permissions": List[PermissionType],
     },
-    total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Permissions": Sequence[PermissionType],
     },
     total=False,
 )
 
-_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_RequiredTableWithColumnsResourceOutputTypeDef",
+ColumnLFTagTypeDef = TypedDict(
+    "ColumnLFTagTypeDef",
     {
-        "DatabaseName": str,
         "Name": str,
+        "LFTags": List[LFTagPairOutputTypeDef],
     },
 )
-_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_OptionalTableWithColumnsResourceOutputTypeDef",
+
+LFTagErrorTypeDef = TypedDict(
+    "LFTagErrorTypeDef",
+    {
+        "LFTag": LFTagPairOutputTypeDef,
+        "Error": ErrorDetailTypeDef,
+    },
+)
+
+ListLFTagsResponseTypeDef = TypedDict(
+    "ListLFTagsResponseTypeDef",
+    {
+        "LFTags": List[LFTagPairOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableWithColumnsResourceOutputTypeDef = TypedDict(
+    "TableWithColumnsResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "DatabaseName": str,
+        "Name": str,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
     },
-    total=False,
 )
 
-
-class TableWithColumnsResourceOutputTypeDef(
-    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1248,41 +1222,28 @@
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
 
-_RequiredDataCellsFilterOutputTypeDef = TypedDict(
-    "_RequiredDataCellsFilterOutputTypeDef",
+DataCellsFilterOutputTypeDef = TypedDict(
+    "DataCellsFilterOutputTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
-    },
-)
-_OptionalDataCellsFilterOutputTypeDef = TypedDict(
-    "_OptionalDataCellsFilterOutputTypeDef",
-    {
         "RowFilter": RowFilterOutputTypeDef,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
         "VersionId": str,
     },
-    total=False,
 )
 
-
-class DataCellsFilterOutputTypeDef(
-    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
-):
-    pass
-
-
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1303,18 +1264,17 @@
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
         "AddObject": AddObjectInputTypeDef,
         "DeleteObject": DeleteObjectInputTypeDef,
@@ -1465,35 +1425,22 @@
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceOutputTypeDef",
+LFTagPolicyResourceOutputTypeDef = TypedDict(
+    "LFTagPolicyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "ResourceType": ResourceTypeType,
         "Expression": List[LFTagOutputTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagPolicyResourceOutputTypeDef(
-    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
-):
-    pass
-
 
 _RequiredLFTagPolicyResourceTypeDef = TypedDict(
     "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
@@ -1512,15 +1459,15 @@
 ):
     pass
 
 
 _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
-        "Expression": Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
     "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -1536,15 +1483,15 @@
 ):
     pass
 
 
 _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
     "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
-        "Expression": Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -1559,15 +1506,15 @@
 ):
     pass
 
 
 _RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
     {
-        "Expression": Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
     "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -1583,15 +1530,15 @@
 ):
     pass
 
 
 _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
     "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     {
-        "Expression": Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -1637,25 +1584,57 @@
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
-    total=False,
 )
 
 StartQueryPlanningRequestRequestTypeDef = TypedDict(
     "StartQueryPlanningRequestRequestTypeDef",
     {
         "QueryPlanningContext": QueryPlanningContextTypeDef,
         "QueryString": str,
     },
 )
 
+DataLakeSettingsOutputTypeDef = TypedDict(
+    "DataLakeSettingsOutputTypeDef",
+    {
+        "DataLakeAdmins": List[DataLakePrincipalOutputTypeDef],
+        "ReadOnlyAdmins": List[DataLakePrincipalOutputTypeDef],
+        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "Parameters": Dict[str, str],
+        "TrustedResourceOwners": List[str],
+        "AllowExternalDataFiltering": bool,
+        "AllowFullTableExternalDataAccess": bool,
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalOutputTypeDef],
+        "AuthorizedSessionTagValueList": List[str],
+    },
+)
+
+DataLakeSettingsTypeDef = TypedDict(
+    "DataLakeSettingsTypeDef",
+    {
+        "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
+        "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
+        "CreateDatabaseDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "Parameters": Mapping[str, str],
+        "TrustedResourceOwners": Sequence[str],
+        "AllowExternalDataFiltering": bool,
+        "AllowFullTableExternalDataAccess": bool,
+        "ExternalDataFilteringAllowList": Sequence[DataLakePrincipalTypeDef],
+        "AuthorizedSessionTagValueList": Sequence[str],
+    },
+    total=False,
+)
+
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1666,15 +1645,14 @@
     "TaggedTableTypeDef",
     {
         "Table": TableResourceOutputTypeDef,
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
-    total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1685,48 +1663,14 @@
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataLakeSettingsOutputTypeDef = TypedDict(
-    "DataLakeSettingsOutputTypeDef",
-    {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "ReadOnlyAdmins": List[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
-        "Parameters": Dict[str, str],
-        "TrustedResourceOwners": List[str],
-        "AllowExternalDataFiltering": bool,
-        "AllowFullTableExternalDataAccess": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": List[str],
-    },
-    total=False,
-)
-
-DataLakeSettingsTypeDef = TypedDict(
-    "DataLakeSettingsTypeDef",
-    {
-        "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
-        "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
-        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
-        "Parameters": Mapping[str, str],
-        "TrustedResourceOwners": Sequence[str],
-        "AllowExternalDataFiltering": bool,
-        "AllowFullTableExternalDataAccess": bool,
-        "ExternalDataFilteringAllowList": Sequence[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": Sequence[str],
-    },
-    total=False,
-)
-
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
         "DataCellsFilter": DataCellsFilterOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1788,23 +1732,22 @@
     pass
 
 
 ResourceOutputTypeDef = TypedDict(
     "ResourceOutputTypeDef",
     {
         "Catalog": Dict[str, Any],
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "Table": TableResourceOutputTypeDef,
         "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
-        "DataLocation": DataLocationResourceTypeDef,
-        "DataCellsFilter": DataCellsFilterResourceTypeDef,
+        "DataLocation": DataLocationResourceOutputTypeDef,
+        "DataCellsFilter": DataCellsFilterResourceOutputTypeDef,
         "LFTag": LFTagKeyResourceOutputTypeDef,
         "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
     },
-    total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
@@ -1823,23 +1766,14 @@
     {
         "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SearchTablesByLFTagsResponseTypeDef = TypedDict(
-    "SearchTablesByLFTagsResponseTypeDef",
-    {
-        "NextToken": str,
-        "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1862,56 +1796,50 @@
 class PutDataLakeSettingsRequestRequestTypeDef(
     _RequiredPutDataLakeSettingsRequestRequestTypeDef,
     _OptionalPutDataLakeSettingsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
+SearchTablesByLFTagsResponseTypeDef = TypedDict(
+    "SearchTablesByLFTagsResponseTypeDef",
     {
-        "Id": str,
+        "NextToken": str,
+        "TableList": List[TaggedTableTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
+
+BatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "BatchPermissionsRequestEntryOutputTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Id": str,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
     },
-    total=False,
 )
 
-
-class BatchPermissionsRequestEntryOutputTypeDef(
-    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
-    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
-):
-    pass
-
-
 PrincipalResourcePermissionsTypeDef = TypedDict(
     "PrincipalResourcePermissionsTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
         "AdditionalDetails": DetailsMapTypeDef,
     },
-    total=False,
 )
 
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_OptionalAddLFTagsToResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -2010,15 +1938,15 @@
     total=False,
 )
 
 _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_OptionalRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -2059,15 +1987,14 @@
 
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
         "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
@@ -2083,17 +2010,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
     {
-        "Entries": Sequence[
-            Union[BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef]
-        ],
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -2107,17 +2032,15 @@
 ):
     pass
 
 
 _RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
     {
-        "Entries": Sequence[
-            Union[BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef]
-        ],
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation/type_defs.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lakeformation service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lakeformation.type_defs import LFTagPairOutputTypeDef
+    from mypy_boto3_lakeformation.type_defs import LFTagPairTypeDef
 
-    data: LFTagPairOutputTypeDef = {...}
+    data: LFTagPairTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -34,31 +34,35 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "LFTagPairOutputTypeDef",
     "LFTagPairTypeDef",
     "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
+    "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
+    "LFTagPairOutputTypeDef",
     "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
     "CreateLFTagRequestRequestTypeDef",
     "RowFilterOutputTypeDef",
+    "DataCellsFilterResourceOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
+    "DataLocationResourceOutputTypeDef",
     "DataLocationResourceTypeDef",
+    "DatabaseResourceOutputTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
     "VirtualObjectTypeDef",
     "DeregisterResourceRequestRequestTypeDef",
     "DescribeResourceRequestRequestTypeDef",
@@ -95,30 +99,30 @@
     "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
     "TableResourceOutputTypeDef",
     "StartTransactionRequestRequestTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
-    "ColumnLFTagTypeDef",
     "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "CommitTransactionResponseTypeDef",
     "GetLFTagResponseTypeDef",
     "GetQueryStateResponseTypeDef",
     "GetTemporaryGluePartitionCredentialsResponseTypeDef",
     "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsResponseTypeDef",
-    "ListLFTagsResponseTypeDef",
     "StartQueryPlanningResponseTypeDef",
     "StartTransactionResponseTypeDef",
     "UpdateTableStorageOptimizerResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
-    "LFTagErrorTypeDef",
     "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
+    "ColumnLFTagTypeDef",
+    "LFTagErrorTypeDef",
+    "ListLFTagsResponseTypeDef",
     "TableWithColumnsResourceOutputTypeDef",
     "TableWithColumnsResourceTypeDef",
     "DataCellsFilterOutputTypeDef",
     "DataCellsFilterTypeDef",
     "TaggedDatabaseTypeDef",
     "WriteOperationTypeDef",
     "DeleteObjectsOnCancelRequestRequestTypeDef",
@@ -139,32 +143,32 @@
     "SearchTablesByLFTagsRequestRequestTypeDef",
     "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     "ListDataCellsFilterRequestRequestTypeDef",
     "ListTableStorageOptimizersResponseTypeDef",
     "PartitionObjectsTypeDef",
     "StartQueryPlanningRequestRequestTypeDef",
+    "DataLakeSettingsOutputTypeDef",
+    "DataLakeSettingsTypeDef",
     "GetResourceLFTagsResponseTypeDef",
     "TaggedTableTypeDef",
     "AddLFTagsToResourceResponseTypeDef",
     "RemoveLFTagsFromResourceResponseTypeDef",
-    "DataLakeSettingsOutputTypeDef",
-    "DataLakeSettingsTypeDef",
     "GetDataCellsFilterResponseTypeDef",
     "ListDataCellsFilterResponseTypeDef",
     "CreateDataCellsFilterRequestRequestTypeDef",
     "UpdateDataCellsFilterRequestRequestTypeDef",
     "SearchDatabasesByLFTagsResponseTypeDef",
     "UpdateTableObjectsRequestRequestTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "GetTableObjectsResponseTypeDef",
-    "SearchTablesByLFTagsResponseTypeDef",
     "GetDataLakeSettingsResponseTypeDef",
     "PutDataLakeSettingsRequestRequestTypeDef",
+    "SearchTablesByLFTagsResponseTypeDef",
     "BatchPermissionsRequestEntryOutputTypeDef",
     "PrincipalResourcePermissionsTypeDef",
     "AddLFTagsToResourceRequestRequestTypeDef",
     "BatchPermissionsRequestEntryTypeDef",
     "GetResourceLFTagsRequestRequestTypeDef",
     "GrantPermissionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
@@ -175,32 +179,14 @@
     "ListPermissionsResponseTypeDef",
     "BatchGrantPermissionsRequestRequestTypeDef",
     "BatchRevokePermissionsRequestRequestTypeDef",
     "BatchGrantPermissionsResponseTypeDef",
     "BatchRevokePermissionsResponseTypeDef",
 )
 
-_RequiredLFTagPairOutputTypeDef = TypedDict(
-    "_RequiredLFTagPairOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": List[str],
-    },
-)
-_OptionalLFTagPairOutputTypeDef = TypedDict(
-    "_OptionalLFTagPairOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
-    pass
-
 _RequiredLFTagPairTypeDef = TypedDict(
     "_RequiredLFTagPairTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -277,15 +263,21 @@
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+DataLakePrincipalOutputTypeDef = TypedDict(
+    "DataLakePrincipalOutputTypeDef",
+    {
+        "DataLakePrincipalIdentifier": str,
+    },
 )
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
@@ -295,20 +287,28 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
+LFTagPairOutputTypeDef = TypedDict(
+    "LFTagPairOutputTypeDef",
+    {
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
 ColumnWildcardOutputTypeDef = TypedDict(
     "ColumnWildcardOutputTypeDef",
     {
         "ExcludedColumnNames": List[str],
     },
-    total=False,
 )
 
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
@@ -344,15 +344,24 @@
 
 RowFilterOutputTypeDef = TypedDict(
     "RowFilterOutputTypeDef",
     {
         "FilterExpression": str,
         "AllRowsWildcard": Dict[str, Any],
     },
-    total=False,
+)
+
+DataCellsFilterResourceOutputTypeDef = TypedDict(
+    "DataCellsFilterResourceOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+    },
 )
 
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
@@ -367,14 +376,22 @@
     {
         "FilterExpression": str,
         "AllRowsWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
+DataLocationResourceOutputTypeDef = TypedDict(
+    "DataLocationResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredDataLocationResourceTypeDef = TypedDict(
     "_RequiredDataLocationResourceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalDataLocationResourceTypeDef = TypedDict(
@@ -386,14 +403,22 @@
 )
 
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
+DatabaseResourceOutputTypeDef = TypedDict(
+    "DatabaseResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "Name": str,
+    },
+)
+
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
@@ -492,15 +517,14 @@
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
         "WithFederation": bool,
     },
-    total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -510,33 +534,30 @@
     "TransactionDescriptionTypeDef",
     {
         "TransactionId": str,
         "TransactionStatus": TransactionStatusType,
         "TransactionStartTime": datetime,
         "TransactionEndTime": datetime,
     },
-    total=False,
 )
 
 DetailsMapTypeDef = TypedDict(
     "DetailsMapTypeDef",
     {
         "ResourceShare": List[str],
     },
-    total=False,
 )
 
 ExecutionStatisticsTypeDef = TypedDict(
     "ExecutionStatisticsTypeDef",
     {
         "AverageExecutionTimeMillis": int,
         "DataScannedBytes": int,
         "WorkUnitsExecutedCount": int,
     },
-    total=False,
 )
 
 ExtendTransactionRequestRequestTypeDef = TypedDict(
     "ExtendTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -630,15 +651,14 @@
     "PlanningStatisticsTypeDef",
     {
         "EstimatedDataToScanBytes": int,
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
-    total=False,
 )
 
 _RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
@@ -713,33 +733,22 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
-_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagKeyResourceOutputTypeDef",
+LFTagKeyResourceOutputTypeDef = TypedDict(
+    "LFTagKeyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagKeyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagKeyResourceOutputTypeDef(
-    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
-):
-    pass
 
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
@@ -830,15 +839,14 @@
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
         "LastRunDetails": str,
     },
-    total=False,
 )
 
 ListTransactionsRequestRequestTypeDef = TypedDict(
     "ListTransactionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "StatusFilter": TransactionStatusFilterType,
@@ -851,15 +859,14 @@
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
-    total=False,
 )
 
 _RequiredQueryPlanningContextTypeDef = TypedDict(
     "_RequiredQueryPlanningContextTypeDef",
     {
         "DatabaseName": str,
     },
@@ -897,35 +904,24 @@
 )
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
-_RequiredTableResourceOutputTypeDef = TypedDict(
-    "_RequiredTableResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalTableResourceOutputTypeDef = TypedDict(
-    "_OptionalTableResourceOutputTypeDef",
+TableResourceOutputTypeDef = TypedDict(
+    "TableResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "DatabaseName": str,
         "Name": str,
         "TableWildcard": Dict[str, Any],
     },
-    total=False,
 )
 
-class TableResourceOutputTypeDef(
-    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
-):
-    pass
-
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
@@ -989,23 +985,14 @@
 
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
-ColumnLFTagTypeDef = TypedDict(
-    "ColumnLFTagTypeDef",
-    {
-        "Name": str,
-        "LFTags": List[LFTagPairOutputTypeDef],
-    },
-    total=False,
-)
-
 AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
     "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     {
         "AccessKeyId": str,
         "SecretAccessKey": str,
         "SessionToken": str,
         "Expiration": datetime,
@@ -1066,23 +1053,14 @@
     "GetWorkUnitResultsResponseTypeDef",
     {
         "ResultStream": StreamingBody,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListLFTagsResponseTypeDef = TypedDict(
-    "ListLFTagsResponseTypeDef",
-    {
-        "LFTags": List[LFTagPairOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 StartQueryPlanningResponseTypeDef = TypedDict(
     "StartQueryPlanningResponseTypeDef",
     {
         "QueryId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1122,63 +1100,67 @@
 
 class GetTemporaryGlueTableCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
 ):
     pass
 
-LFTagErrorTypeDef = TypedDict(
-    "LFTagErrorTypeDef",
-    {
-        "LFTag": LFTagPairOutputTypeDef,
-        "Error": ErrorDetailTypeDef,
-    },
-    total=False,
-)
-
 PrincipalPermissionsOutputTypeDef = TypedDict(
     "PrincipalPermissionsOutputTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Permissions": List[PermissionType],
     },
-    total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Permissions": Sequence[PermissionType],
     },
     total=False,
 )
 
-_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_RequiredTableWithColumnsResourceOutputTypeDef",
+ColumnLFTagTypeDef = TypedDict(
+    "ColumnLFTagTypeDef",
     {
-        "DatabaseName": str,
         "Name": str,
+        "LFTags": List[LFTagPairOutputTypeDef],
     },
 )
-_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_OptionalTableWithColumnsResourceOutputTypeDef",
+
+LFTagErrorTypeDef = TypedDict(
+    "LFTagErrorTypeDef",
+    {
+        "LFTag": LFTagPairOutputTypeDef,
+        "Error": ErrorDetailTypeDef,
+    },
+)
+
+ListLFTagsResponseTypeDef = TypedDict(
+    "ListLFTagsResponseTypeDef",
+    {
+        "LFTags": List[LFTagPairOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableWithColumnsResourceOutputTypeDef = TypedDict(
+    "TableWithColumnsResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "DatabaseName": str,
+        "Name": str,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
     },
-    total=False,
 )
 
-class TableWithColumnsResourceOutputTypeDef(
-    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
-):
-    pass
-
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1193,39 +1175,28 @@
 )
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
-_RequiredDataCellsFilterOutputTypeDef = TypedDict(
-    "_RequiredDataCellsFilterOutputTypeDef",
+DataCellsFilterOutputTypeDef = TypedDict(
+    "DataCellsFilterOutputTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
-    },
-)
-_OptionalDataCellsFilterOutputTypeDef = TypedDict(
-    "_OptionalDataCellsFilterOutputTypeDef",
-    {
         "RowFilter": RowFilterOutputTypeDef,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
         "VersionId": str,
     },
-    total=False,
 )
 
-class DataCellsFilterOutputTypeDef(
-    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
-):
-    pass
-
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1244,18 +1215,17 @@
 
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
         "AddObject": AddObjectInputTypeDef,
         "DeleteObject": DeleteObjectInputTypeDef,
@@ -1400,33 +1370,22 @@
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceOutputTypeDef",
+LFTagPolicyResourceOutputTypeDef = TypedDict(
+    "LFTagPolicyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "ResourceType": ResourceTypeType,
         "Expression": List[LFTagOutputTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagPolicyResourceOutputTypeDef(
-    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
-):
-    pass
 
 _RequiredLFTagPolicyResourceTypeDef = TypedDict(
     "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
@@ -1443,15 +1402,15 @@
     _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
 ):
     pass
 
 _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
-        "Expression": Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
     "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -1465,15 +1424,15 @@
     _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
 ):
     pass
 
 _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
     "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
-        "Expression": Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -1486,15 +1445,15 @@
     _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
 ):
     pass
 
 _RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
     {
-        "Expression": Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
     "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -1508,15 +1467,15 @@
     _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
 ):
     pass
 
 _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
     "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     {
-        "Expression": Sequence[Union[LFTagTypeDef, LFTagOutputTypeDef]],
+        "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -1560,25 +1519,57 @@
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
-    total=False,
 )
 
 StartQueryPlanningRequestRequestTypeDef = TypedDict(
     "StartQueryPlanningRequestRequestTypeDef",
     {
         "QueryPlanningContext": QueryPlanningContextTypeDef,
         "QueryString": str,
     },
 )
 
+DataLakeSettingsOutputTypeDef = TypedDict(
+    "DataLakeSettingsOutputTypeDef",
+    {
+        "DataLakeAdmins": List[DataLakePrincipalOutputTypeDef],
+        "ReadOnlyAdmins": List[DataLakePrincipalOutputTypeDef],
+        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "Parameters": Dict[str, str],
+        "TrustedResourceOwners": List[str],
+        "AllowExternalDataFiltering": bool,
+        "AllowFullTableExternalDataAccess": bool,
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalOutputTypeDef],
+        "AuthorizedSessionTagValueList": List[str],
+    },
+)
+
+DataLakeSettingsTypeDef = TypedDict(
+    "DataLakeSettingsTypeDef",
+    {
+        "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
+        "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
+        "CreateDatabaseDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "Parameters": Mapping[str, str],
+        "TrustedResourceOwners": Sequence[str],
+        "AllowExternalDataFiltering": bool,
+        "AllowFullTableExternalDataAccess": bool,
+        "ExternalDataFilteringAllowList": Sequence[DataLakePrincipalTypeDef],
+        "AuthorizedSessionTagValueList": Sequence[str],
+    },
+    total=False,
+)
+
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1589,15 +1580,14 @@
     "TaggedTableTypeDef",
     {
         "Table": TableResourceOutputTypeDef,
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
-    total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1608,48 +1598,14 @@
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataLakeSettingsOutputTypeDef = TypedDict(
-    "DataLakeSettingsOutputTypeDef",
-    {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "ReadOnlyAdmins": List[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
-        "Parameters": Dict[str, str],
-        "TrustedResourceOwners": List[str],
-        "AllowExternalDataFiltering": bool,
-        "AllowFullTableExternalDataAccess": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": List[str],
-    },
-    total=False,
-)
-
-DataLakeSettingsTypeDef = TypedDict(
-    "DataLakeSettingsTypeDef",
-    {
-        "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
-        "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
-        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
-        "Parameters": Mapping[str, str],
-        "TrustedResourceOwners": Sequence[str],
-        "AllowExternalDataFiltering": bool,
-        "AllowFullTableExternalDataAccess": bool,
-        "ExternalDataFilteringAllowList": Sequence[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": Sequence[str],
-    },
-    total=False,
-)
-
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
         "DataCellsFilter": DataCellsFilterOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1709,23 +1665,22 @@
 ):
     pass
 
 ResourceOutputTypeDef = TypedDict(
     "ResourceOutputTypeDef",
     {
         "Catalog": Dict[str, Any],
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "Table": TableResourceOutputTypeDef,
         "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
-        "DataLocation": DataLocationResourceTypeDef,
-        "DataCellsFilter": DataCellsFilterResourceTypeDef,
+        "DataLocation": DataLocationResourceOutputTypeDef,
+        "DataCellsFilter": DataCellsFilterResourceOutputTypeDef,
         "LFTag": LFTagKeyResourceOutputTypeDef,
         "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
     },
-    total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
@@ -1744,23 +1699,14 @@
     {
         "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SearchTablesByLFTagsResponseTypeDef = TypedDict(
-    "SearchTablesByLFTagsResponseTypeDef",
-    {
-        "NextToken": str,
-        "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1781,54 +1727,50 @@
 
 class PutDataLakeSettingsRequestRequestTypeDef(
     _RequiredPutDataLakeSettingsRequestRequestTypeDef,
     _OptionalPutDataLakeSettingsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
+SearchTablesByLFTagsResponseTypeDef = TypedDict(
+    "SearchTablesByLFTagsResponseTypeDef",
     {
-        "Id": str,
+        "NextToken": str,
+        "TableList": List[TaggedTableTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
+
+BatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "BatchPermissionsRequestEntryOutputTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Id": str,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
     },
-    total=False,
 )
 
-class BatchPermissionsRequestEntryOutputTypeDef(
-    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
-    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
-):
-    pass
-
 PrincipalResourcePermissionsTypeDef = TypedDict(
     "PrincipalResourcePermissionsTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
         "AdditionalDetails": DetailsMapTypeDef,
     },
-    total=False,
 )
 
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_OptionalAddLFTagsToResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -1919,15 +1861,15 @@
     total=False,
 )
 
 _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_OptionalRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -1964,15 +1906,14 @@
 
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
         "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
@@ -1988,17 +1929,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
     {
-        "Entries": Sequence[
-            Union[BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef]
-        ],
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -2010,17 +1949,15 @@
     _OptionalBatchGrantPermissionsRequestRequestTypeDef,
 ):
     pass
 
 _RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
     {
-        "Entries": Sequence[
-            Union[BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef]
-        ],
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation.egg-info/PKG-INFO` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LakeFormation 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.4
+Summary: Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,31 +351,35 @@
 ### Typed dictionaries
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
-    LFTagPairOutputTypeDef,
     LFTagPairTypeDef,
     ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
+    LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
@@ -412,30 +416,30 @@
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
     TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
-    ColumnLFTagTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     CommitTransactionResponseTypeDef,
     GetLFTagResponseTypeDef,
     GetQueryStateResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
-    ListLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
-    LFTagErrorTypeDef,
     PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    ColumnLFTagTypeDef,
+    LFTagErrorTypeDef,
+    ListLFTagsResponseTypeDef,
     TableWithColumnsResourceOutputTypeDef,
     TableWithColumnsResourceTypeDef,
     DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
     DeleteObjectsOnCancelRequestRequestTypeDef,
@@ -456,32 +460,32 @@
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
     StartQueryPlanningRequestRequestTypeDef,
+    DataLakeSettingsOutputTypeDef,
+    DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    DataLakeSettingsOutputTypeDef,
-    DataLakeSettingsTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
     CreateDataCellsFilterRequestRequestTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     GetTableObjectsResponseTypeDef,
-    SearchTablesByLFTagsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
+    SearchTablesByLFTagsResponseTypeDef,
     BatchPermissionsRequestEntryOutputTypeDef,
     PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
@@ -493,15 +497,15 @@
     BatchGrantPermissionsRequestRequestTypeDef,
     BatchRevokePermissionsRequestRequestTypeDef,
     BatchGrantPermissionsResponseTypeDef,
     BatchRevokePermissionsResponseTypeDef,
 )
 
 
-def get_structure() -> LFTagPairOutputTypeDef:
+def get_structure() -> LFTagPairTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/mypy_boto3_lakeformation.egg-info/SOURCES.txt` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15.post1/setup.py` & `mypy-boto3-lakeformation-1.28.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lakeformation",
-    version="1.28.15.post1",
+    version="1.28.4",
     packages=["mypy_boto3_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LakeFormation 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

