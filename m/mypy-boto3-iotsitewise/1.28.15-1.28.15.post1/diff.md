# Comparing `tmp/mypy-boto3-iotsitewise-1.28.15.tar.gz` & `tmp/mypy-boto3-iotsitewise-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotsitewise-1.28.15.tar", last modified: Fri Jul 28 20:43:01 2023, max compression
+gzip compressed data, was "mypy-boto3-iotsitewise-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:23 2023, max compression
```

## Comparing `mypy-boto3-iotsitewise-1.28.15.tar` & `mypy-boto3-iotsitewise-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:01.917291 mypy-boto3-iotsitewise-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-07-28 20:43:01.917291 mypy-boto3-iotsitewise-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27116 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:01.917291 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62559 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    62456 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21879 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   108808 2023-07-28 20:28:39.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   108600 2023-07-28 20:28:37.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-28 20:28:34.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:01.917291 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:01.000000 mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:01.917291 mypy-boto3-iotsitewise-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:28:33.000000 mypy-boto3-iotsitewise-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.305196 mypy-boto3-iotsitewise-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28625 2023-07-29 10:03:23.305196 mypy-boto3-iotsitewise-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27116 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.285196 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62842 2023-07-29 09:48:07.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62739 2023-07-29 09:48:07.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-07-29 09:48:08.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-07-29 09:48:08.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-07-29 09:48:07.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21879 2023-07-29 09:48:07.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   108938 2023-07-29 09:48:11.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108730 2023-07-29 09:48:09.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:05.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-29 09:48:08.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-29 09:48:08.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.285196 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28625 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:03:23.000000 mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:23.305196 mypy-boto3-iotsitewise-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:48:04.000000 mypy-boto3-iotsitewise-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-iotsitewise-1.28.15/LICENSE` & `mypy-boto3-iotsitewise-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15/PKG-INFO` & `mypy-boto3-iotsitewise-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsitewise
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotsitewise-1.28.15/README.md` & `mypy-boto3-iotsitewise-1.28.15.post1/README.md`

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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__init__.py` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__init__.pyi` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/__main__.py` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTSiteWise 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.IoTSiteWise 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise\nOther"
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

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/client.py` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,18 +56,20 @@
     ListProjectAssetsPaginator,
     ListProjectsPaginator,
     ListTimeSeriesPaginator,
 )
 from .type_defs import (
     AlarmsTypeDef,
     AssetModelCompositeModelDefinitionTypeDef,
+    AssetModelCompositeModelOutputTypeDef,
     AssetModelCompositeModelTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
     AssetModelHierarchyTypeDef,
     AssetModelPropertyDefinitionTypeDef,
+    AssetModelPropertyOutputTypeDef,
     AssetModelPropertyTypeDef,
     BatchAssociateProjectAssetsResponseTypeDef,
     BatchDisassociateProjectAssetsResponseTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueHistoryEntryTypeDef,
@@ -106,14 +108,15 @@
     GetAssetPropertyAggregatesResponseTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
     IdentityTypeDef,
     ImageFileTypeDef,
     ImageTypeDef,
+    JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     ListAccessPoliciesResponseTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
     ListAssetModelsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetsResponseTypeDef,
@@ -356,15 +359,15 @@
     def create_bulk_import_job(
         self,
         *,
         jobName: str,
         jobRoleArn: str,
         files: Sequence[FileTypeDef],
         errorReportLocation: ErrorReportLocationTypeDef,
-        jobConfiguration: JobConfigurationTypeDef
+        jobConfiguration: Union[JobConfigurationTypeDef, JobConfigurationOutputTypeDef]
     ) -> CreateBulkImportJobResponseTypeDef:
         """
         Defines a job to ingest data to IoT SiteWise from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_bulk_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/client/#create_bulk_import_job)
         """
@@ -1022,17 +1025,21 @@
 
     def update_asset_model(
         self,
         *,
         assetModelId: str,
         assetModelName: str,
         assetModelDescription: str = ...,
-        assetModelProperties: Sequence[AssetModelPropertyTypeDef] = ...,
+        assetModelProperties: Sequence[
+            Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
+        ] = ...,
         assetModelHierarchies: Sequence[AssetModelHierarchyTypeDef] = ...,
-        assetModelCompositeModels: Sequence[AssetModelCompositeModelTypeDef] = ...,
+        assetModelCompositeModels: Sequence[
+            Union[AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef]
+        ] = ...,
         clientToken: str = ...
     ) -> UpdateAssetModelResponseTypeDef:
         """
         Updates an asset model and all of the assets that were created from the model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/client/#update_asset_model)
```

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/client.pyi` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,20 @@
     ListProjectAssetsPaginator,
     ListProjectsPaginator,
     ListTimeSeriesPaginator,
 )
 from .type_defs import (
     AlarmsTypeDef,
     AssetModelCompositeModelDefinitionTypeDef,
+    AssetModelCompositeModelOutputTypeDef,
     AssetModelCompositeModelTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
     AssetModelHierarchyTypeDef,
     AssetModelPropertyDefinitionTypeDef,
+    AssetModelPropertyOutputTypeDef,
     AssetModelPropertyTypeDef,
     BatchAssociateProjectAssetsResponseTypeDef,
     BatchDisassociateProjectAssetsResponseTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueHistoryEntryTypeDef,
@@ -106,14 +108,15 @@
     GetAssetPropertyAggregatesResponseTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
     IdentityTypeDef,
     ImageFileTypeDef,
     ImageTypeDef,
+    JobConfigurationOutputTypeDef,
     JobConfigurationTypeDef,
     ListAccessPoliciesResponseTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
     ListAssetModelsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetsResponseTypeDef,
@@ -338,15 +341,15 @@
     def create_bulk_import_job(
         self,
         *,
         jobName: str,
         jobRoleArn: str,
         files: Sequence[FileTypeDef],
         errorReportLocation: ErrorReportLocationTypeDef,
-        jobConfiguration: JobConfigurationTypeDef
+        jobConfiguration: Union[JobConfigurationTypeDef, JobConfigurationOutputTypeDef]
     ) -> CreateBulkImportJobResponseTypeDef:
         """
         Defines a job to ingest data to IoT SiteWise from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_bulk_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/client/#create_bulk_import_job)
         """
@@ -948,17 +951,21 @@
         """
     def update_asset_model(
         self,
         *,
         assetModelId: str,
         assetModelName: str,
         assetModelDescription: str = ...,
-        assetModelProperties: Sequence[AssetModelPropertyTypeDef] = ...,
+        assetModelProperties: Sequence[
+            Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
+        ] = ...,
         assetModelHierarchies: Sequence[AssetModelHierarchyTypeDef] = ...,
-        assetModelCompositeModels: Sequence[AssetModelCompositeModelTypeDef] = ...,
+        assetModelCompositeModels: Sequence[
+            Union[AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef]
+        ] = ...,
         clientToken: str = ...
     ) -> UpdateAssetModelResponseTypeDef:
         """
         Updates an asset model and all of the assets that were created from the model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/client/#update_asset_model)
```

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/literals.py` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/literals.pyi` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/paginator.py` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/paginator.pyi` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/type_defs.py` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4170,17 +4170,21 @@
         "assetModelName": str,
     },
 )
 _OptionalUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelDescription": str,
-        "assetModelProperties": Sequence[AssetModelPropertyTypeDef],
+        "assetModelProperties": Sequence[
+            Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
+        ],
         "assetModelHierarchies": Sequence[AssetModelHierarchyTypeDef],
-        "assetModelCompositeModels": Sequence[AssetModelCompositeModelTypeDef],
+        "assetModelCompositeModels": Sequence[
+            Union[AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef]
+        ],
         "clientToken": str,
     },
     total=False,
 )
 
 
 class UpdateAssetModelRequestRequestTypeDef(
```

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/type_defs.pyi` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -3963,17 +3963,21 @@
         "assetModelName": str,
     },
 )
 _OptionalUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelDescription": str,
-        "assetModelProperties": Sequence[AssetModelPropertyTypeDef],
+        "assetModelProperties": Sequence[
+            Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
+        ],
         "assetModelHierarchies": Sequence[AssetModelHierarchyTypeDef],
-        "assetModelCompositeModels": Sequence[AssetModelCompositeModelTypeDef],
+        "assetModelCompositeModels": Sequence[
+            Union[AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef]
+        ],
         "clientToken": str,
     },
     total=False,
 )
 
 class UpdateAssetModelRequestRequestTypeDef(
     _RequiredUpdateAssetModelRequestRequestTypeDef, _OptionalUpdateAssetModelRequestRequestTypeDef
```

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/waiter.py` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise/waiter.pyi` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/PKG-INFO` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsitewise
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/
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
 [mypy-boto3-iotsitewise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsitewise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotsitewise-1.28.15/mypy_boto3_iotsitewise.egg-info/SOURCES.txt` & `mypy-boto3-iotsitewise-1.28.15.post1/mypy_boto3_iotsitewise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsitewise-1.28.15/setup.py` & `mypy-boto3-iotsitewise-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotsitewise",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_iotsitewise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.IoTSiteWise 1.28.15 service generated with mypy-boto3-builder"
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

