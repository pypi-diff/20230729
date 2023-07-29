# Comparing `tmp/mypy-boto3-appsync-1.28.15.tar.gz` & `tmp/mypy-boto3-appsync-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appsync-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
+gzip compressed data, was "mypy-boto3-appsync-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
```

## Comparing `mypy-boto3-appsync-1.28.15.tar` & `mypy-boto3-appsync-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.196694 mypy-boto3-appsync-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:41.000000 mypy-boto3-appsync-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-07-28 20:42:19.188695 mypy-boto3-appsync-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-28 20:19:41.000000 mypy-boto3-appsync-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.184694 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-28 20:19:41.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-28 20:19:41.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:19:41.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43388 2023-07-28 20:19:42.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43314 2023-07-28 20:19:42.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-07-28 20:19:42.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-07-28 20:19:42.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-28 20:19:42.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-07-28 20:19:42.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:41.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57726 2023-07-28 20:19:45.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57641 2023-07-28 20:19:43.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:41.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.188695 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-07-28 20:42:18.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:42:18.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:18.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:18.000000 mypy-boto3-appsync-1.28.15/mypy_boto3_appsync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.196694 mypy-boto3-appsync-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:19:41.000000 mypy-boto3-appsync-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.313020 mypy-boto3-appsync-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-07-29 10:02:34.305020 mypy-boto3-appsync-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.305020 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43595 2023-07-29 09:38:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43521 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-07-29 09:38:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-07-29 09:38:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-29 09:38:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-07-29 09:38:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57726 2023-07-29 09:38:36.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57641 2023-07-29 09:38:36.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.305020 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:34.000000 mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.313020 mypy-boto3-appsync-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:38:33.000000 mypy-boto3-appsync-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-appsync-1.28.15/LICENSE` & `mypy-boto3-appsync-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15/PKG-INFO` & `mypy-boto3-appsync-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appsync
-Version: 1.28.15
-Summary: Type annotations for boto3.AppSync 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppSync 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/
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
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appsync-1.28.15/README.md` & `mypy-boto3-appsync-1.28.15.post1/README.md`

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
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/__init__.py` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/__init__.pyi` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/__main__.py` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppSync 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.AppSync 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync\nOther"
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

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/client.py` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 )
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
+    CachingConfigOutputTypeDef,
     CachingConfigTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
@@ -86,14 +87,15 @@
     ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
+    PipelineConfigOutputTypeDef,
     PipelineConfigTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     SourceApiAssociationConfigTypeDef,
     StartSchemaCreationResponseTypeDef,
     StartSchemaMergeResponseTypeDef,
     SyncConfigTypeDef,
     UpdateApiCacheResponseTypeDef,
@@ -325,17 +327,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef] = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: Union[CachingConfigTypeDef, CachingConfigOutputTypeDef] = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
 
@@ -854,17 +856,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef] = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: Union[CachingConfigTypeDef, CachingConfigOutputTypeDef] = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
```

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/client.pyi` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 )
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
+    CachingConfigOutputTypeDef,
     CachingConfigTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
@@ -86,14 +87,15 @@
     ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
+    PipelineConfigOutputTypeDef,
     PipelineConfigTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     SourceApiAssociationConfigTypeDef,
     StartSchemaCreationResponseTypeDef,
     StartSchemaMergeResponseTypeDef,
     SyncConfigTypeDef,
     UpdateApiCacheResponseTypeDef,
@@ -309,17 +311,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef] = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: Union[CachingConfigTypeDef, CachingConfigOutputTypeDef] = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
 
@@ -789,17 +791,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef] = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: Union[CachingConfigTypeDef, CachingConfigOutputTypeDef] = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
```

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/literals.py` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/literals.pyi` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/paginator.py` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/paginator.pyi` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/type_defs.py` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync/type_defs.pyi` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync.egg-info/PKG-INFO` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appsync
-Version: 1.28.15
-Summary: Type annotations for boto3.AppSync 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppSync 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/
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
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appsync-1.28.15/mypy_boto3_appsync.egg-info/SOURCES.txt` & `mypy-boto3-appsync-1.28.15.post1/mypy_boto3_appsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.28.15/setup.py` & `mypy-boto3-appsync-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appsync",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_appsync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AppSync 1.28.15 service generated with mypy-boto3-builder"
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

