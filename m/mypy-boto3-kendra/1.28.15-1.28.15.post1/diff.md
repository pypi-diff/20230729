# Comparing `tmp/mypy-boto3-kendra-1.28.15.tar.gz` & `tmp/mypy-boto3-kendra-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kendra-1.28.15.tar", last modified: Fri Jul 28 20:43:02 2023, max compression
+gzip compressed data, was "mypy-boto3-kendra-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:26 2023, max compression
```

## Comparing `mypy-boto3-kendra-1.28.15.tar` & `mypy-boto3-kendra-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.837303 mypy-boto3-kendra-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25916 2023-07-28 20:43:02.833303 mypy-boto3-kendra-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24433 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.821303 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47945 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47873 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   144224 2023-07-28 20:29:07.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   144013 2023-07-28 20:29:05.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.833303 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25916 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:02.837303 mypy-boto3-kendra-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:29:00.000000 mypy-boto3-kendra-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.297213 mypy-boto3-kendra-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25922 2023-07-29 10:03:26.293213 mypy-boto3-kendra-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24433 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.289213 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49177 2023-07-29 09:48:39.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49105 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-29 09:48:39.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-29 09:48:39.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   144427 2023-07-29 09:48:43.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144216 2023-07-29 09:48:41.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.293213 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25922 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:26.309213 mypy-boto3-kendra-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-kendra-1.28.15/LICENSE` & `mypy-boto3-kendra-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.15/PKG-INFO` & `mypy-boto3-kendra-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.28.15
-Summary: Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kendra-1.28.15/README.md` & `mypy-boto3-kendra-1.28.15.post1/README.md`

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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/__main__.py` & `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.kendra 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.kendra 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra\nOther"
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

### Comparing `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/client.py` & `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_kendra.client import kendraClient
 
     session = Session()
     client: kendraClient = session.client("kendra")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceSyncJobStatusType,
     DataSourceTypeType,
     FaqFileFormatType,
@@ -46,43 +46,49 @@
     CreateDataSourceResponseTypeDef,
     CreateExperienceResponseTypeDef,
     CreateFaqResponseTypeDef,
     CreateFeaturedResultsSetResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateQuerySuggestionsBlockListResponseTypeDef,
     CreateThesaurusResponseTypeDef,
+    CustomDocumentEnrichmentConfigurationOutputTypeDef,
     CustomDocumentEnrichmentConfigurationTypeDef,
+    DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
+    DataSourceVpcConfigurationOutputTypeDef,
     DataSourceVpcConfigurationTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     DescribeFaqResponseTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribeIndexResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DescribeQuerySuggestionsBlockListResponseTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
     DocumentInfoTypeDef,
+    DocumentMetadataConfigurationOutputTypeDef,
     DocumentMetadataConfigurationTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EntityConfigurationTypeDef,
     EntityPersonaConfigurationTypeDef,
+    ExperienceConfigurationOutputTypeDef,
     ExperienceConfigurationTypeDef,
     FacetTypeDef,
     FeaturedDocumentTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
+    HierarchicalPrincipalOutputTypeDef,
     HierarchicalPrincipalTypeDef,
     ListAccessControlConfigurationsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     ListExperiencesResponseTypeDef,
@@ -99,14 +105,15 @@
     RetrieveResultTypeDef,
     S3PathTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     StartDataSourceSyncJobResponseTypeDef,
     TagTypeDef,
+    TimeRangeOutputTypeDef,
     TimeRangeTypeDef,
     UpdateFeaturedResultsSetResponseTypeDef,
     UserContextTypeDef,
     UserGroupResolutionConfigurationTypeDef,
     UserTokenConfigurationTypeDef,
 )
 
@@ -214,15 +221,18 @@
 
     def batch_put_document(
         self,
         *,
         IndexId: str,
         Documents: Sequence[DocumentTypeDef],
         RoleArn: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: Union[
+            CustomDocumentEnrichmentConfigurationTypeDef,
+            CustomDocumentEnrichmentConfigurationOutputTypeDef,
+        ] = ...
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_put_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_put_document)
         """
@@ -254,15 +264,17 @@
     def create_access_control_configuration(
         self,
         *,
         IndexId: str,
         Name: str,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...,
+        HierarchicalAccessControlList: Sequence[
+            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
+        ] = ...,
         ClientToken: str = ...
     ) -> CreateAccessControlConfigurationResponseTypeDef:
         """
         Creates an access configuration for your documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_access_control_configuration)
@@ -270,23 +282,30 @@
 
     def create_data_source(
         self,
         *,
         Name: str,
         IndexId: str,
         Type: DataSourceTypeType,
-        Configuration: DataSourceConfigurationTypeDef = ...,
-        VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
+        Configuration: Union[
+            DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
+        ] = ...,
+        VpcConfiguration: Union[
+            DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
+        ] = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: Union[
+            CustomDocumentEnrichmentConfigurationTypeDef,
+            CustomDocumentEnrichmentConfigurationOutputTypeDef,
+        ] = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector that you want to use with an Amazon Kendra
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_data_source)
@@ -294,15 +313,17 @@
 
     def create_experience(
         self,
         *,
         Name: str,
         IndexId: str,
         RoleArn: str = ...,
-        Configuration: ExperienceConfigurationTypeDef = ...,
+        Configuration: Union[
+            ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
+        ] = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> CreateExperienceResponseTypeDef:
         """
         Creates an Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_experience)
@@ -651,15 +672,15 @@
     def list_data_source_sync_jobs(
         self,
         *,
         Id: str,
         IndexId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartTimeFilter: TimeRangeTypeDef = ...,
+        StartTimeFilter: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
         StatusFilter: DataSourceSyncJobStatusType = ...
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Gets statistics about synchronizing a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_source_sync_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_data_source_sync_jobs)
@@ -901,36 +922,45 @@
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...
+        HierarchicalAccessControlList: Sequence[
+            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Updates an access control configuration for your documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_access_control_configuration)
         """
 
     def update_data_source(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
-        Configuration: DataSourceConfigurationTypeDef = ...,
-        VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
+        Configuration: Union[
+            DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
+        ] = ...,
+        VpcConfiguration: Union[
+            DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
+        ] = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: Union[
+            CustomDocumentEnrichmentConfigurationTypeDef,
+            CustomDocumentEnrichmentConfigurationOutputTypeDef,
+        ] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_data_source)
         """
@@ -938,15 +968,17 @@
     def update_experience(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         RoleArn: str = ...,
-        Configuration: ExperienceConfigurationTypeDef = ...,
+        Configuration: Union[
+            ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
+        ] = ...,
         Description: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_experience)
@@ -973,15 +1005,17 @@
     def update_index(
         self,
         *,
         Id: str,
         Name: str = ...,
         RoleArn: str = ...,
         Description: str = ...,
-        DocumentMetadataConfigurationUpdates: Sequence[DocumentMetadataConfigurationTypeDef] = ...,
+        DocumentMetadataConfigurationUpdates: Sequence[
+            Union[DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef]
+        ] = ...,
         CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
         UserTokenConfigurations: Sequence[UserTokenConfigurationTypeDef] = ...,
         UserContextPolicy: UserContextPolicyType = ...,
         UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra index.
```

### Comparing `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/client.pyi` & `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_kendra.client import kendraClient
 
     session = Session()
     client: kendraClient = session.client("kendra")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceSyncJobStatusType,
     DataSourceTypeType,
     FaqFileFormatType,
@@ -46,43 +46,49 @@
     CreateDataSourceResponseTypeDef,
     CreateExperienceResponseTypeDef,
     CreateFaqResponseTypeDef,
     CreateFeaturedResultsSetResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateQuerySuggestionsBlockListResponseTypeDef,
     CreateThesaurusResponseTypeDef,
+    CustomDocumentEnrichmentConfigurationOutputTypeDef,
     CustomDocumentEnrichmentConfigurationTypeDef,
+    DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
+    DataSourceVpcConfigurationOutputTypeDef,
     DataSourceVpcConfigurationTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     DescribeFaqResponseTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribeIndexResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DescribeQuerySuggestionsBlockListResponseTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
     DocumentInfoTypeDef,
+    DocumentMetadataConfigurationOutputTypeDef,
     DocumentMetadataConfigurationTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EntityConfigurationTypeDef,
     EntityPersonaConfigurationTypeDef,
+    ExperienceConfigurationOutputTypeDef,
     ExperienceConfigurationTypeDef,
     FacetTypeDef,
     FeaturedDocumentTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
+    HierarchicalPrincipalOutputTypeDef,
     HierarchicalPrincipalTypeDef,
     ListAccessControlConfigurationsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     ListExperiencesResponseTypeDef,
@@ -99,14 +105,15 @@
     RetrieveResultTypeDef,
     S3PathTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     StartDataSourceSyncJobResponseTypeDef,
     TagTypeDef,
+    TimeRangeOutputTypeDef,
     TimeRangeTypeDef,
     UpdateFeaturedResultsSetResponseTypeDef,
     UserContextTypeDef,
     UserGroupResolutionConfigurationTypeDef,
     UserTokenConfigurationTypeDef,
 )
 
@@ -205,15 +212,18 @@
         """
     def batch_put_document(
         self,
         *,
         IndexId: str,
         Documents: Sequence[DocumentTypeDef],
         RoleArn: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: Union[
+            CustomDocumentEnrichmentConfigurationTypeDef,
+            CustomDocumentEnrichmentConfigurationOutputTypeDef,
+        ] = ...
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_put_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_put_document)
         """
@@ -241,53 +251,64 @@
     def create_access_control_configuration(
         self,
         *,
         IndexId: str,
         Name: str,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...,
+        HierarchicalAccessControlList: Sequence[
+            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
+        ] = ...,
         ClientToken: str = ...
     ) -> CreateAccessControlConfigurationResponseTypeDef:
         """
         Creates an access configuration for your documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_access_control_configuration)
         """
     def create_data_source(
         self,
         *,
         Name: str,
         IndexId: str,
         Type: DataSourceTypeType,
-        Configuration: DataSourceConfigurationTypeDef = ...,
-        VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
+        Configuration: Union[
+            DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
+        ] = ...,
+        VpcConfiguration: Union[
+            DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
+        ] = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: Union[
+            CustomDocumentEnrichmentConfigurationTypeDef,
+            CustomDocumentEnrichmentConfigurationOutputTypeDef,
+        ] = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector that you want to use with an Amazon Kendra
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_data_source)
         """
     def create_experience(
         self,
         *,
         Name: str,
         IndexId: str,
         RoleArn: str = ...,
-        Configuration: ExperienceConfigurationTypeDef = ...,
+        Configuration: Union[
+            ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
+        ] = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> CreateExperienceResponseTypeDef:
         """
         Creates an Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_experience)
@@ -606,15 +627,15 @@
     def list_data_source_sync_jobs(
         self,
         *,
         Id: str,
         IndexId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartTimeFilter: TimeRangeTypeDef = ...,
+        StartTimeFilter: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
         StatusFilter: DataSourceSyncJobStatusType = ...
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Gets statistics about synchronizing a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_source_sync_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_data_source_sync_jobs)
@@ -836,50 +857,61 @@
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...
+        HierarchicalAccessControlList: Sequence[
+            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Updates an access control configuration for your documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_access_control_configuration)
         """
     def update_data_source(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
-        Configuration: DataSourceConfigurationTypeDef = ...,
-        VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
+        Configuration: Union[
+            DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
+        ] = ...,
+        VpcConfiguration: Union[
+            DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
+        ] = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: Union[
+            CustomDocumentEnrichmentConfigurationTypeDef,
+            CustomDocumentEnrichmentConfigurationOutputTypeDef,
+        ] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_data_source)
         """
     def update_experience(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         RoleArn: str = ...,
-        Configuration: ExperienceConfigurationTypeDef = ...,
+        Configuration: Union[
+            ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
+        ] = ...,
         Description: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_experience)
@@ -904,15 +936,17 @@
     def update_index(
         self,
         *,
         Id: str,
         Name: str = ...,
         RoleArn: str = ...,
         Description: str = ...,
-        DocumentMetadataConfigurationUpdates: Sequence[DocumentMetadataConfigurationTypeDef] = ...,
+        DocumentMetadataConfigurationUpdates: Sequence[
+            Union[DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef]
+        ] = ...,
         CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
         UserTokenConfigurations: Sequence[UserTokenConfigurationTypeDef] = ...,
         UserContextPolicy: UserContextPolicyType = ...,
         UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra index.
```

### Comparing `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/literals.py` & `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/literals.pyi` & `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/type_defs.py` & `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4265,15 +4265,17 @@
     },
 )
 _OptionalCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAccessControlConfigurationRequestRequestTypeDef",
     {
         "Description": str,
         "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[
+            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
+        ],
         "ClientToken": str,
     },
     total=False,
 )
 
 
 class CreateAccessControlConfigurationRequestRequestTypeDef(
@@ -4292,15 +4294,17 @@
 )
 _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef",
     {
         "Name": str,
         "Description": str,
         "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[
+            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
@@ -4733,15 +4737,17 @@
 )
 _OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateIndexRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
         "Description": str,
-        "DocumentMetadataConfigurationUpdates": Sequence[DocumentMetadataConfigurationTypeDef],
+        "DocumentMetadataConfigurationUpdates": Sequence[
+            Union[DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef]
+        ],
         "CapacityUnits": CapacityUnitsConfigurationTypeDef,
         "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/type_defs.pyi` & `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4096,15 +4096,17 @@
     },
 )
 _OptionalCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAccessControlConfigurationRequestRequestTypeDef",
     {
         "Description": str,
         "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[
+            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
+        ],
         "ClientToken": str,
     },
     total=False,
 )
 
 class CreateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
@@ -4121,15 +4123,17 @@
 )
 _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef",
     {
         "Name": str,
         "Description": str,
         "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[
+            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
     _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
@@ -4540,15 +4544,17 @@
 )
 _OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateIndexRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
         "Description": str,
-        "DocumentMetadataConfigurationUpdates": Sequence[DocumentMetadataConfigurationTypeDef],
+        "DocumentMetadataConfigurationUpdates": Sequence[
+            Union[DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef]
+        ],
         "CapacityUnits": CapacityUnitsConfigurationTypeDef,
         "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/PKG-INFO` & `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.28.15
-Summary: Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/SOURCES.txt` & `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.15/setup.py` & `mypy-boto3-kendra-1.28.15.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kendra",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_kendra"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

