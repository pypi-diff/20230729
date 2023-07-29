# Comparing `tmp/mypy-boto3-connectcases-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-connectcases-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcases-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:52 2023, max compression
+gzip compressed data, was "mypy-boto3-connectcases-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-connectcases-1.28.15.post1.tar` & `mypy-boto3-connectcases-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:52.101089 mypy-boto3-connectcases-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:43.000000 mypy-boto3-connectcases-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16578 2023-07-29 10:02:52.081089 mypy-boto3-connectcases-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15065 2023-07-29 09:41:43.000000 mypy-boto3-connectcases-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:52.081089 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-29 09:41:43.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-29 09:41:43.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:41:43.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-07-29 09:41:44.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22487 2023-07-29 09:41:44.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-29 09:41:44.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-29 09:41:44.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-29 09:41:44.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-29 09:41:44.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:43.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32323 2023-07-29 09:41:46.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32275 2023-07-29 09:41:46.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:43.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:52.081089 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16578 2023-07-29 10:02:51.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:02:51.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:51.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:51.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:51.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:02:51.000000 mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:52.101089 mypy-boto3-connectcases-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:41:43.000000 mypy-boto3-connectcases-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.012775 mypy-boto3-connectcases-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-20 19:47:56.004775 mypy-boto3-connectcases-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22068 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-07-20 19:46:48.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-07-20 19:46:48.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.004775 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.012775 mypy-boto3-connectcases-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/setup.py
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/LICENSE` & `mypy-boto3-connectcases-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.15.post1/PKG-INFO` & `mypy-boto3-connectcases-1.28.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ConnectCases 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.8
+Summary: Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,34 +336,41 @@
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
     ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
+    FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
+    CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateFieldRequestRequestTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
+    RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
+    FieldItemOutputTypeDef,
     FieldItemTypeDef,
+    FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionOutputTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
+    LayoutConfigurationOutputTypeDef,
+    RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
@@ -371,69 +378,69 @@
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
-    CaseEventIncludedDataOutputTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDomainResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
+    ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     FieldValueOutputTypeDef,
     FieldValueTypeDef,
+    GetTemplateResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
-    EventIncludedDataOutputTypeDef,
     EventIncludedDataTypeDef,
+    EventIncludedDataOutputTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
     SectionOutputTypeDef,
     SectionTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
     CreateCaseRequestRequestTypeDef,
     FieldFilterTypeDef,
     UpdateCaseRequestRequestTypeDef,
-    EventBridgeConfigurationOutputTypeDef,
     EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     SearchRelatedItemsResponseTypeDef,
     LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
     SearchCasesResponseTypeDef,
     CaseFilterTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    GetCaseEventConfigurationResponseTypeDef,
     BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
     LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
     GetLayoutResponseTypeDef,
     CreateLayoutRequestRequestTypeDef,
     UpdateLayoutRequestRequestTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/README.md` & `mypy-boto3-connectcases-1.28.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,34 +304,41 @@
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
     ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
+    FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
+    CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateFieldRequestRequestTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
+    RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
+    FieldItemOutputTypeDef,
     FieldItemTypeDef,
+    FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionOutputTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
+    LayoutConfigurationOutputTypeDef,
+    RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
@@ -339,69 +346,69 @@
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
-    CaseEventIncludedDataOutputTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDomainResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
+    ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     FieldValueOutputTypeDef,
     FieldValueTypeDef,
+    GetTemplateResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
-    EventIncludedDataOutputTypeDef,
     EventIncludedDataTypeDef,
+    EventIncludedDataOutputTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
     SectionOutputTypeDef,
     SectionTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
     CreateCaseRequestRequestTypeDef,
     FieldFilterTypeDef,
     UpdateCaseRequestRequestTypeDef,
-    EventBridgeConfigurationOutputTypeDef,
     EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     SearchRelatedItemsResponseTypeDef,
     LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
     SearchCasesResponseTypeDef,
     CaseFilterTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    GetCaseEventConfigurationResponseTypeDef,
     BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
     LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
     GetLayoutResponseTypeDef,
     CreateLayoutRequestRequestTypeDef,
     UpdateLayoutRequestRequestTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/__init__.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/__init__.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/__main__.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCases 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ConnectCases 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/client.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_connectcases.client import ConnectCasesClient
 
     session = Session()
     client: ConnectCasesClient = session.client("connectcases")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FieldTypeType, RelatedItemTypeType, TemplateStatusType
 from .paginator import SearchCasesPaginator, SearchRelatedItemsPaginator
 from .type_defs import (
     BatchGetFieldResponseTypeDef,
@@ -27,27 +27,24 @@
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventBridgeConfigurationOutputTypeDef,
     EventBridgeConfigurationTypeDef,
     FieldIdentifierTypeDef,
     FieldOptionTypeDef,
-    FieldValueOutputTypeDef,
     FieldValueTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
     GetCaseResponseTypeDef,
     GetDomainResponseTypeDef,
     GetLayoutResponseTypeDef,
     GetTemplateResponseTypeDef,
     LayoutConfigurationTypeDef,
-    LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
     ListCasesForContactResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -142,15 +139,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#close)
         """
 
     def create_case(
         self,
         *,
         domainId: str,
-        fields: Sequence[Union[FieldValueTypeDef, FieldValueOutputTypeDef]],
+        fields: Sequence[FieldValueTypeDef],
         templateId: str,
         clientToken: str = ...
     ) -> CreateCaseResponseTypeDef:
         """
         Creates a case in the specified Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_case)
@@ -173,19 +170,15 @@
         Creates a field in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_field)
         """
 
     def create_layout(
-        self,
-        *,
-        content: Union[LayoutContentTypeDef, LayoutContentOutputTypeDef],
-        domainId: str,
-        name: str
+        self, *, content: LayoutContentTypeDef, domainId: str, name: str
     ) -> CreateLayoutResponseTypeDef:
         """
         Creates a layout in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_layout)
         """
@@ -370,18 +363,15 @@
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_templates)
         """
 
     def put_case_event_configuration(
-        self,
-        *,
-        domainId: str,
-        eventBridge: Union[EventBridgeConfigurationTypeDef, EventBridgeConfigurationOutputTypeDef]
+        self, *, domainId: str, eventBridge: EventBridgeConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         API for adding case event publishing configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/connectcases-2022-10-03/PutCaseEventConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.put_case_event_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#put_case_event_configuration)
@@ -434,19 +424,15 @@
         Untags a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#untag_resource)
         """
 
     def update_case(
-        self,
-        *,
-        caseId: str,
-        domainId: str,
-        fields: Sequence[Union[FieldValueTypeDef, FieldValueOutputTypeDef]]
+        self, *, caseId: str, domainId: str, fields: Sequence[FieldValueTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates the values of fields on a case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_case)
         """
@@ -458,20 +444,15 @@
         Updates the properties of an existing field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_field)
         """
 
     def update_layout(
-        self,
-        *,
-        domainId: str,
-        layoutId: str,
-        content: Union[LayoutContentTypeDef, LayoutContentOutputTypeDef] = ...,
-        name: str = ...
+        self, *, domainId: str, layoutId: str, content: LayoutContentTypeDef = ..., name: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_layout)
         """
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/client.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_connectcases.client import ConnectCasesClient
 
     session = Session()
     client: ConnectCasesClient = session.client("connectcases")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FieldTypeType, RelatedItemTypeType, TemplateStatusType
 from .paginator import SearchCasesPaginator, SearchRelatedItemsPaginator
 from .type_defs import (
     BatchGetFieldResponseTypeDef,
@@ -27,27 +27,24 @@
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventBridgeConfigurationOutputTypeDef,
     EventBridgeConfigurationTypeDef,
     FieldIdentifierTypeDef,
     FieldOptionTypeDef,
-    FieldValueOutputTypeDef,
     FieldValueTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
     GetCaseResponseTypeDef,
     GetDomainResponseTypeDef,
     GetLayoutResponseTypeDef,
     GetTemplateResponseTypeDef,
     LayoutConfigurationTypeDef,
-    LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
     ListCasesForContactResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -133,15 +130,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#close)
         """
     def create_case(
         self,
         *,
         domainId: str,
-        fields: Sequence[Union[FieldValueTypeDef, FieldValueOutputTypeDef]],
+        fields: Sequence[FieldValueTypeDef],
         templateId: str,
         clientToken: str = ...
     ) -> CreateCaseResponseTypeDef:
         """
         Creates a case in the specified Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_case)
@@ -161,19 +158,15 @@
         """
         Creates a field in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_field)
         """
     def create_layout(
-        self,
-        *,
-        content: Union[LayoutContentTypeDef, LayoutContentOutputTypeDef],
-        domainId: str,
-        name: str
+        self, *, content: LayoutContentTypeDef, domainId: str, name: str
     ) -> CreateLayoutResponseTypeDef:
         """
         Creates a layout in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_layout)
         """
@@ -341,18 +334,15 @@
         """
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_templates)
         """
     def put_case_event_configuration(
-        self,
-        *,
-        domainId: str,
-        eventBridge: Union[EventBridgeConfigurationTypeDef, EventBridgeConfigurationOutputTypeDef]
+        self, *, domainId: str, eventBridge: EventBridgeConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         API for adding case event publishing configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/connectcases-2022-10-03/PutCaseEventConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.put_case_event_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#put_case_event_configuration)
@@ -400,19 +390,15 @@
         """
         Untags a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#untag_resource)
         """
     def update_case(
-        self,
-        *,
-        caseId: str,
-        domainId: str,
-        fields: Sequence[Union[FieldValueTypeDef, FieldValueOutputTypeDef]]
+        self, *, caseId: str, domainId: str, fields: Sequence[FieldValueTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates the values of fields on a case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_case)
         """
@@ -422,20 +408,15 @@
         """
         Updates the properties of an existing field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_field)
         """
     def update_layout(
-        self,
-        *,
-        domainId: str,
-        layoutId: str,
-        content: Union[LayoutContentTypeDef, LayoutContentOutputTypeDef] = ...,
-        name: str = ...
+        self, *, domainId: str, layoutId: str, content: LayoutContentTypeDef = ..., name: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_layout)
         """
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/literals.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,14 @@
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
@@ -249,15 +248,14 @@
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
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/literals.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,14 @@
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
@@ -247,15 +246,14 @@
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
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/paginator.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/paginator.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/type_defs.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_connectcases.type_defs import FieldIdentifierTypeDef
 
     data: FieldIdentifierTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     DomainStatusType,
     FieldNamespaceType,
     FieldTypeType,
     OrderType,
     RelatedItemTypeType,
@@ -37,34 +37,41 @@
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
     "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
+    "FieldIdentifierOutputTypeDef",
     "CaseSummaryTypeDef",
+    "CommentContentOutputTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateFieldRequestRequestTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
+    "RelatedItemEventIncludedDataOutputTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
+    "FieldItemOutputTypeDef",
     "FieldItemTypeDef",
+    "FieldOptionOutputTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
+    "LayoutConfigurationOutputTypeDef",
+    "RequiredFieldOutputTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
@@ -72,69 +79,69 @@
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
-    "CaseEventIncludedDataOutputTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "CreateFieldResponseTypeDef",
     "CreateLayoutResponseTypeDef",
     "CreateRelatedItemResponseTypeDef",
     "CreateTemplateResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetDomainResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
-    "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
+    "CaseEventIncludedDataOutputTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
+    "ListFieldOptionsResponseTypeDef",
     "ListFieldsResponseTypeDef",
     "FieldValueOutputTypeDef",
     "FieldValueTypeDef",
+    "GetTemplateResponseTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
-    "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
+    "EventIncludedDataOutputTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
     "SectionOutputTypeDef",
     "SectionTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "FieldFilterTypeDef",
     "UpdateCaseRequestRequestTypeDef",
-    "EventBridgeConfigurationOutputTypeDef",
     "EventBridgeConfigurationTypeDef",
+    "EventBridgeConfigurationOutputTypeDef",
     "SearchRelatedItemsResponseTypeDef",
     "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
     "SearchCasesResponseTypeDef",
     "CaseFilterTypeDef",
-    "GetCaseEventConfigurationResponseTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
+    "GetCaseEventConfigurationResponseTypeDef",
     "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
     "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
     "GetLayoutResponseTypeDef",
     "CreateLayoutRequestRequestTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
@@ -143,58 +150,36 @@
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredFieldErrorTypeDef = TypedDict(
-    "_RequiredFieldErrorTypeDef",
+FieldErrorTypeDef = TypedDict(
+    "FieldErrorTypeDef",
     {
         "errorCode": str,
         "id": str,
-    },
-)
-_OptionalFieldErrorTypeDef = TypedDict(
-    "_OptionalFieldErrorTypeDef",
-    {
         "message": str,
     },
-    total=False,
 )
 
-
-class FieldErrorTypeDef(_RequiredFieldErrorTypeDef, _OptionalFieldErrorTypeDef):
-    pass
-
-
-_RequiredGetFieldResponseTypeDef = TypedDict(
-    "_RequiredGetFieldResponseTypeDef",
+GetFieldResponseTypeDef = TypedDict(
+    "GetFieldResponseTypeDef",
     {
+        "description": str,
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
-        "type": FieldTypeType,
-    },
-)
-_OptionalGetFieldResponseTypeDef = TypedDict(
-    "_OptionalGetFieldResponseTypeDef",
-    {
-        "description": str,
         "tags": Dict[str, str],
+        "type": FieldTypeType,
     },
-    total=False,
 )
 
-
-class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
-    pass
-
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -216,22 +201,37 @@
     {
         "errorCode": str,
         "message": str,
         "value": str,
     },
 )
 
+FieldIdentifierOutputTypeDef = TypedDict(
+    "FieldIdentifierOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 CaseSummaryTypeDef = TypedDict(
     "CaseSummaryTypeDef",
     {
         "caseId": str,
         "templateId": str,
     },
 )
 
+CommentContentOutputTypeDef = TypedDict(
+    "CommentContentOutputTypeDef",
+    {
+        "body": str,
+        "contentType": Literal["Text/Plain"],
+    },
+)
+
 CommentContentTypeDef = TypedDict(
     "CommentContentTypeDef",
     {
         "body": str,
         "contentType": Literal["Text/Plain"],
     },
 )
@@ -318,28 +318,51 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
+RelatedItemEventIncludedDataOutputTypeDef = TypedDict(
+    "RelatedItemEventIncludedDataOutputTypeDef",
+    {
+        "includeContent": bool,
+    },
+)
+
 RelatedItemEventIncludedDataTypeDef = TypedDict(
     "RelatedItemEventIncludedDataTypeDef",
     {
         "includeContent": bool,
     },
 )
 
+FieldItemOutputTypeDef = TypedDict(
+    "FieldItemOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 FieldItemTypeDef = TypedDict(
     "FieldItemTypeDef",
     {
         "id": str,
     },
 )
 
+FieldOptionOutputTypeDef = TypedDict(
+    "FieldOptionOutputTypeDef",
+    {
+        "active": bool,
+        "name": str,
+        "value": str,
+    },
+)
+
 FieldSummaryTypeDef = TypedDict(
     "FieldSummaryTypeDef",
     {
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
@@ -351,15 +374,14 @@
     "FieldValueUnionOutputTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "emptyValue": Dict[str, Any],
         "stringValue": str,
     },
-    total=False,
 )
 
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
@@ -395,14 +417,28 @@
     "GetTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
 
+LayoutConfigurationOutputTypeDef = TypedDict(
+    "LayoutConfigurationOutputTypeDef",
+    {
+        "defaultLayout": str,
+    },
+)
+
+RequiredFieldOutputTypeDef = TypedDict(
+    "RequiredFieldOutputTypeDef",
+    {
+        "fieldId": str,
+    },
+)
+
 LayoutSummaryTypeDef = TypedDict(
     "LayoutSummaryTypeDef",
     {
         "layoutArn": str,
         "layoutId": str,
         "name": str,
     },
@@ -610,21 +646,14 @@
     "BatchGetFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
-CaseEventIncludedDataOutputTypeDef = TypedDict(
-    "CaseEventIncludedDataOutputTypeDef",
-    {
-        "fields": List[FieldIdentifierTypeDef],
-    },
-)
-
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
@@ -748,28 +777,26 @@
     {
         "domainId": str,
         "fieldId": str,
         "options": Sequence[FieldOptionTypeDef],
     },
 )
 
-ListFieldOptionsResponseTypeDef = TypedDict(
-    "ListFieldOptionsResponseTypeDef",
+BatchPutFieldOptionsResponseTypeDef = TypedDict(
+    "BatchPutFieldOptionsResponseTypeDef",
     {
-        "nextToken": str,
-        "options": List[FieldOptionTypeDef],
+        "errors": List[FieldOptionErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutFieldOptionsResponseTypeDef = TypedDict(
-    "BatchPutFieldOptionsResponseTypeDef",
+CaseEventIncludedDataOutputTypeDef = TypedDict(
+    "CaseEventIncludedDataOutputTypeDef",
     {
-        "errors": List[FieldOptionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "fields": List[FieldIdentifierOutputTypeDef],
     },
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
@@ -777,18 +804,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
-        "comment": CommentContentTypeDef,
+        "comment": CommentContentOutputTypeDef,
         "contact": ContactContentTypeDef,
     },
-    total=False,
 )
 
 RelatedItemTypeFilterTypeDef = TypedDict(
     "RelatedItemTypeFilterTypeDef",
     {
         "comment": Mapping[str, Any],
         "contact": ContactFilterTypeDef,
@@ -826,29 +852,14 @@
 
 class CreateTemplateRequestRequestTypeDef(
     _RequiredCreateTemplateRequestRequestTypeDef, _OptionalCreateTemplateRequestRequestTypeDef
 ):
     pass
 
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "description": str,
-        "layoutConfiguration": LayoutConfigurationTypeDef,
-        "name": str,
-        "requiredFields": List[RequiredFieldTypeDef],
-        "status": TemplateStatusType,
-        "tags": Dict[str, str],
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
@@ -876,33 +887,22 @@
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldGroupOutputTypeDef = TypedDict(
-    "_RequiredFieldGroupOutputTypeDef",
-    {
-        "fields": List[FieldItemTypeDef],
-    },
-)
-_OptionalFieldGroupOutputTypeDef = TypedDict(
-    "_OptionalFieldGroupOutputTypeDef",
+FieldGroupOutputTypeDef = TypedDict(
+    "FieldGroupOutputTypeDef",
     {
+        "fields": List[FieldItemOutputTypeDef],
         "name": str,
     },
-    total=False,
 )
 
-
-class FieldGroupOutputTypeDef(_RequiredFieldGroupOutputTypeDef, _OptionalFieldGroupOutputTypeDef):
-    pass
-
-
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
     },
 )
 _OptionalFieldGroupTypeDef = TypedDict(
@@ -914,14 +914,23 @@
 )
 
 
 class FieldGroupTypeDef(_RequiredFieldGroupTypeDef, _OptionalFieldGroupTypeDef):
     pass
 
 
+ListFieldOptionsResponseTypeDef = TypedDict(
+    "ListFieldOptionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "options": List[FieldOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -939,14 +948,29 @@
     "FieldValueTypeDef",
     {
         "id": str,
         "value": FieldValueUnionTypeDef,
     },
 )
 
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "description": str,
+        "layoutConfiguration": LayoutConfigurationOutputTypeDef,
+        "name": str,
+        "requiredFields": List[RequiredFieldOutputTypeDef],
+        "status": TemplateStatusType,
+        "tags": Dict[str, str],
+        "templateArn": str,
+        "templateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1009,55 +1033,41 @@
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
 ):
     pass
 
 
-EventIncludedDataOutputTypeDef = TypedDict(
-    "EventIncludedDataOutputTypeDef",
+EventIncludedDataTypeDef = TypedDict(
+    "EventIncludedDataTypeDef",
     {
-        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "caseData": CaseEventIncludedDataTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataTypeDef,
     },
     total=False,
 )
 
-EventIncludedDataTypeDef = TypedDict(
-    "EventIncludedDataTypeDef",
+EventIncludedDataOutputTypeDef = TypedDict(
+    "EventIncludedDataOutputTypeDef",
     {
-        "caseData": CaseEventIncludedDataTypeDef,
-        "relatedItemData": RelatedItemEventIncludedDataTypeDef,
+        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "relatedItemData": RelatedItemEventIncludedDataOutputTypeDef,
     },
-    total=False,
 )
 
-_RequiredSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_RequiredSearchRelatedItemsResponseItemTypeDef",
+SearchRelatedItemsResponseItemTypeDef = TypedDict(
+    "SearchRelatedItemsResponseItemTypeDef",
     {
         "associationTime": datetime,
         "content": RelatedItemContentTypeDef,
         "relatedItemId": str,
+        "tags": Dict[str, str],
         "type": RelatedItemTypeType,
     },
 )
-_OptionalSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_OptionalSearchRelatedItemsResponseItemTypeDef",
-    {
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class SearchRelatedItemsResponseItemTypeDef(
-    _RequiredSearchRelatedItemsResponseItemTypeDef, _OptionalSearchRelatedItemsResponseItemTypeDef
-):
-    pass
-
 
 _RequiredSearchRelatedItemsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRelatedItemsRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
     },
@@ -1115,15 +1125,14 @@
 )
 
 SectionOutputTypeDef = TypedDict(
     "SectionOutputTypeDef",
     {
         "fieldGroup": FieldGroupOutputTypeDef,
     },
-    total=False,
 )
 
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
@@ -1137,42 +1146,29 @@
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSearchCasesResponseItemTypeDef = TypedDict(
-    "_RequiredSearchCasesResponseItemTypeDef",
+SearchCasesResponseItemTypeDef = TypedDict(
+    "SearchCasesResponseItemTypeDef",
     {
         "caseId": str,
         "fields": List[FieldValueOutputTypeDef],
-        "templateId": str,
-    },
-)
-_OptionalSearchCasesResponseItemTypeDef = TypedDict(
-    "_OptionalSearchCasesResponseItemTypeDef",
-    {
         "tags": Dict[str, str],
+        "templateId": str,
     },
-    total=False,
 )
 
-
-class SearchCasesResponseItemTypeDef(
-    _RequiredSearchCasesResponseItemTypeDef, _OptionalSearchCasesResponseItemTypeDef
-):
-    pass
-
-
 _RequiredCreateCaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCaseRequestRequestTypeDef",
     {
         "domainId": str,
-        "fields": Sequence[Union[FieldValueTypeDef, FieldValueOutputTypeDef]],
+        "fields": Sequence[FieldValueTypeDef],
         "templateId": str,
     },
 )
 _OptionalCreateCaseRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCaseRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -1201,39 +1197,18 @@
 )
 
 UpdateCaseRequestRequestTypeDef = TypedDict(
     "UpdateCaseRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
-        "fields": Sequence[Union[FieldValueTypeDef, FieldValueOutputTypeDef]],
+        "fields": Sequence[FieldValueTypeDef],
     },
 )
 
-_RequiredEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEventBridgeConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEventBridgeConfigurationOutputTypeDef",
-    {
-        "includedData": EventIncludedDataOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EventBridgeConfigurationOutputTypeDef(
-    _RequiredEventBridgeConfigurationOutputTypeDef, _OptionalEventBridgeConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredEventBridgeConfigurationTypeDef = TypedDict(
     "_RequiredEventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEventBridgeConfigurationTypeDef = TypedDict(
@@ -1247,29 +1222,36 @@
 
 class EventBridgeConfigurationTypeDef(
     _RequiredEventBridgeConfigurationTypeDef, _OptionalEventBridgeConfigurationTypeDef
 ):
     pass
 
 
+EventBridgeConfigurationOutputTypeDef = TypedDict(
+    "EventBridgeConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "includedData": EventIncludedDataOutputTypeDef,
+    },
+)
+
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LayoutSectionsOutputTypeDef = TypedDict(
     "LayoutSectionsOutputTypeDef",
     {
         "sections": List[SectionOutputTypeDef],
     },
-    total=False,
 )
 
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
@@ -1292,37 +1274,36 @@
         "field": FieldFilterTypeDef,
         "not": Dict[str, Any],
         "orAll": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-GetCaseEventConfigurationResponseTypeDef = TypedDict(
-    "GetCaseEventConfigurationResponseTypeDef",
-    {
-        "eventBridge": EventBridgeConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
         "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
 
+GetCaseEventConfigurationResponseTypeDef = TypedDict(
+    "GetCaseEventConfigurationResponseTypeDef",
+    {
+        "eventBridge": EventBridgeConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BasicLayoutOutputTypeDef = TypedDict(
     "BasicLayoutOutputTypeDef",
     {
         "moreInfo": LayoutSectionsOutputTypeDef,
         "topPanel": LayoutSectionsOutputTypeDef,
     },
-    total=False,
 )
 
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
@@ -1331,15 +1312,14 @@
 )
 
 LayoutContentOutputTypeDef = TypedDict(
     "LayoutContentOutputTypeDef",
     {
         "basic": BasicLayoutOutputTypeDef,
     },
-    total=False,
 )
 
 LayoutContentTypeDef = TypedDict(
     "LayoutContentTypeDef",
     {
         "basic": BasicLayoutTypeDef,
     },
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases/type_defs.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_connectcases.type_defs import FieldIdentifierTypeDef
 
     data: FieldIdentifierTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     DomainStatusType,
     FieldNamespaceType,
     FieldTypeType,
     OrderType,
     RelatedItemTypeType,
@@ -36,34 +36,41 @@
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
     "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
+    "FieldIdentifierOutputTypeDef",
     "CaseSummaryTypeDef",
+    "CommentContentOutputTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateFieldRequestRequestTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
+    "RelatedItemEventIncludedDataOutputTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
+    "FieldItemOutputTypeDef",
     "FieldItemTypeDef",
+    "FieldOptionOutputTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
+    "LayoutConfigurationOutputTypeDef",
+    "RequiredFieldOutputTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
@@ -71,69 +78,69 @@
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
-    "CaseEventIncludedDataOutputTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "CreateFieldResponseTypeDef",
     "CreateLayoutResponseTypeDef",
     "CreateRelatedItemResponseTypeDef",
     "CreateTemplateResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetDomainResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
-    "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
+    "CaseEventIncludedDataOutputTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
+    "ListFieldOptionsResponseTypeDef",
     "ListFieldsResponseTypeDef",
     "FieldValueOutputTypeDef",
     "FieldValueTypeDef",
+    "GetTemplateResponseTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
-    "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
+    "EventIncludedDataOutputTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
     "SectionOutputTypeDef",
     "SectionTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "FieldFilterTypeDef",
     "UpdateCaseRequestRequestTypeDef",
-    "EventBridgeConfigurationOutputTypeDef",
     "EventBridgeConfigurationTypeDef",
+    "EventBridgeConfigurationOutputTypeDef",
     "SearchRelatedItemsResponseTypeDef",
     "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
     "SearchCasesResponseTypeDef",
     "CaseFilterTypeDef",
-    "GetCaseEventConfigurationResponseTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
+    "GetCaseEventConfigurationResponseTypeDef",
     "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
     "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
     "GetLayoutResponseTypeDef",
     "CreateLayoutRequestRequestTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
@@ -142,54 +149,36 @@
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredFieldErrorTypeDef = TypedDict(
-    "_RequiredFieldErrorTypeDef",
+FieldErrorTypeDef = TypedDict(
+    "FieldErrorTypeDef",
     {
         "errorCode": str,
         "id": str,
-    },
-)
-_OptionalFieldErrorTypeDef = TypedDict(
-    "_OptionalFieldErrorTypeDef",
-    {
         "message": str,
     },
-    total=False,
 )
 
-class FieldErrorTypeDef(_RequiredFieldErrorTypeDef, _OptionalFieldErrorTypeDef):
-    pass
-
-_RequiredGetFieldResponseTypeDef = TypedDict(
-    "_RequiredGetFieldResponseTypeDef",
+GetFieldResponseTypeDef = TypedDict(
+    "GetFieldResponseTypeDef",
     {
+        "description": str,
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
-        "type": FieldTypeType,
-    },
-)
-_OptionalGetFieldResponseTypeDef = TypedDict(
-    "_OptionalGetFieldResponseTypeDef",
-    {
-        "description": str,
         "tags": Dict[str, str],
+        "type": FieldTypeType,
     },
-    total=False,
 )
 
-class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
-    pass
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -211,22 +200,37 @@
     {
         "errorCode": str,
         "message": str,
         "value": str,
     },
 )
 
+FieldIdentifierOutputTypeDef = TypedDict(
+    "FieldIdentifierOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 CaseSummaryTypeDef = TypedDict(
     "CaseSummaryTypeDef",
     {
         "caseId": str,
         "templateId": str,
     },
 )
 
+CommentContentOutputTypeDef = TypedDict(
+    "CommentContentOutputTypeDef",
+    {
+        "body": str,
+        "contentType": Literal["Text/Plain"],
+    },
+)
+
 CommentContentTypeDef = TypedDict(
     "CommentContentTypeDef",
     {
         "body": str,
         "contentType": Literal["Text/Plain"],
     },
 )
@@ -311,28 +315,51 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
+RelatedItemEventIncludedDataOutputTypeDef = TypedDict(
+    "RelatedItemEventIncludedDataOutputTypeDef",
+    {
+        "includeContent": bool,
+    },
+)
+
 RelatedItemEventIncludedDataTypeDef = TypedDict(
     "RelatedItemEventIncludedDataTypeDef",
     {
         "includeContent": bool,
     },
 )
 
+FieldItemOutputTypeDef = TypedDict(
+    "FieldItemOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 FieldItemTypeDef = TypedDict(
     "FieldItemTypeDef",
     {
         "id": str,
     },
 )
 
+FieldOptionOutputTypeDef = TypedDict(
+    "FieldOptionOutputTypeDef",
+    {
+        "active": bool,
+        "name": str,
+        "value": str,
+    },
+)
+
 FieldSummaryTypeDef = TypedDict(
     "FieldSummaryTypeDef",
     {
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
@@ -344,15 +371,14 @@
     "FieldValueUnionOutputTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "emptyValue": Dict[str, Any],
         "stringValue": str,
     },
-    total=False,
 )
 
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
@@ -388,14 +414,28 @@
     "GetTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
 
+LayoutConfigurationOutputTypeDef = TypedDict(
+    "LayoutConfigurationOutputTypeDef",
+    {
+        "defaultLayout": str,
+    },
+)
+
+RequiredFieldOutputTypeDef = TypedDict(
+    "RequiredFieldOutputTypeDef",
+    {
+        "fieldId": str,
+    },
+)
+
 LayoutSummaryTypeDef = TypedDict(
     "LayoutSummaryTypeDef",
     {
         "layoutArn": str,
         "layoutId": str,
         "name": str,
     },
@@ -591,21 +631,14 @@
     "BatchGetFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
-CaseEventIncludedDataOutputTypeDef = TypedDict(
-    "CaseEventIncludedDataOutputTypeDef",
-    {
-        "fields": List[FieldIdentifierTypeDef],
-    },
-)
-
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
@@ -727,28 +760,26 @@
     {
         "domainId": str,
         "fieldId": str,
         "options": Sequence[FieldOptionTypeDef],
     },
 )
 
-ListFieldOptionsResponseTypeDef = TypedDict(
-    "ListFieldOptionsResponseTypeDef",
+BatchPutFieldOptionsResponseTypeDef = TypedDict(
+    "BatchPutFieldOptionsResponseTypeDef",
     {
-        "nextToken": str,
-        "options": List[FieldOptionTypeDef],
+        "errors": List[FieldOptionErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutFieldOptionsResponseTypeDef = TypedDict(
-    "BatchPutFieldOptionsResponseTypeDef",
+CaseEventIncludedDataOutputTypeDef = TypedDict(
+    "CaseEventIncludedDataOutputTypeDef",
     {
-        "errors": List[FieldOptionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "fields": List[FieldIdentifierOutputTypeDef],
     },
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
@@ -756,18 +787,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
-        "comment": CommentContentTypeDef,
+        "comment": CommentContentOutputTypeDef,
         "contact": ContactContentTypeDef,
     },
-    total=False,
 )
 
 RelatedItemTypeFilterTypeDef = TypedDict(
     "RelatedItemTypeFilterTypeDef",
     {
         "comment": Mapping[str, Any],
         "contact": ContactFilterTypeDef,
@@ -803,29 +833,14 @@
 )
 
 class CreateTemplateRequestRequestTypeDef(
     _RequiredCreateTemplateRequestRequestTypeDef, _OptionalCreateTemplateRequestRequestTypeDef
 ):
     pass
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "description": str,
-        "layoutConfiguration": LayoutConfigurationTypeDef,
-        "name": str,
-        "requiredFields": List[RequiredFieldTypeDef],
-        "status": TemplateStatusType,
-        "tags": Dict[str, str],
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
@@ -851,31 +866,22 @@
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldGroupOutputTypeDef = TypedDict(
-    "_RequiredFieldGroupOutputTypeDef",
-    {
-        "fields": List[FieldItemTypeDef],
-    },
-)
-_OptionalFieldGroupOutputTypeDef = TypedDict(
-    "_OptionalFieldGroupOutputTypeDef",
+FieldGroupOutputTypeDef = TypedDict(
+    "FieldGroupOutputTypeDef",
     {
+        "fields": List[FieldItemOutputTypeDef],
         "name": str,
     },
-    total=False,
 )
 
-class FieldGroupOutputTypeDef(_RequiredFieldGroupOutputTypeDef, _OptionalFieldGroupOutputTypeDef):
-    pass
-
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
     },
 )
 _OptionalFieldGroupTypeDef = TypedDict(
@@ -885,14 +891,23 @@
     },
     total=False,
 )
 
 class FieldGroupTypeDef(_RequiredFieldGroupTypeDef, _OptionalFieldGroupTypeDef):
     pass
 
+ListFieldOptionsResponseTypeDef = TypedDict(
+    "ListFieldOptionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "options": List[FieldOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -910,14 +925,29 @@
     "FieldValueTypeDef",
     {
         "id": str,
         "value": FieldValueUnionTypeDef,
     },
 )
 
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "description": str,
+        "layoutConfiguration": LayoutConfigurationOutputTypeDef,
+        "name": str,
+        "requiredFields": List[RequiredFieldOutputTypeDef],
+        "status": TemplateStatusType,
+        "tags": Dict[str, str],
+        "templateArn": str,
+        "templateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -976,54 +1006,42 @@
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
 ):
     pass
 
-EventIncludedDataOutputTypeDef = TypedDict(
-    "EventIncludedDataOutputTypeDef",
+EventIncludedDataTypeDef = TypedDict(
+    "EventIncludedDataTypeDef",
     {
-        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "caseData": CaseEventIncludedDataTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataTypeDef,
     },
     total=False,
 )
 
-EventIncludedDataTypeDef = TypedDict(
-    "EventIncludedDataTypeDef",
+EventIncludedDataOutputTypeDef = TypedDict(
+    "EventIncludedDataOutputTypeDef",
     {
-        "caseData": CaseEventIncludedDataTypeDef,
-        "relatedItemData": RelatedItemEventIncludedDataTypeDef,
+        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "relatedItemData": RelatedItemEventIncludedDataOutputTypeDef,
     },
-    total=False,
 )
 
-_RequiredSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_RequiredSearchRelatedItemsResponseItemTypeDef",
+SearchRelatedItemsResponseItemTypeDef = TypedDict(
+    "SearchRelatedItemsResponseItemTypeDef",
     {
         "associationTime": datetime,
         "content": RelatedItemContentTypeDef,
         "relatedItemId": str,
-        "type": RelatedItemTypeType,
-    },
-)
-_OptionalSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_OptionalSearchRelatedItemsResponseItemTypeDef",
-    {
         "tags": Dict[str, str],
+        "type": RelatedItemTypeType,
     },
-    total=False,
 )
 
-class SearchRelatedItemsResponseItemTypeDef(
-    _RequiredSearchRelatedItemsResponseItemTypeDef, _OptionalSearchRelatedItemsResponseItemTypeDef
-):
-    pass
-
 _RequiredSearchRelatedItemsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRelatedItemsRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
     },
 )
@@ -1076,15 +1094,14 @@
 )
 
 SectionOutputTypeDef = TypedDict(
     "SectionOutputTypeDef",
     {
         "fieldGroup": FieldGroupOutputTypeDef,
     },
-    total=False,
 )
 
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
@@ -1098,40 +1115,29 @@
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSearchCasesResponseItemTypeDef = TypedDict(
-    "_RequiredSearchCasesResponseItemTypeDef",
+SearchCasesResponseItemTypeDef = TypedDict(
+    "SearchCasesResponseItemTypeDef",
     {
         "caseId": str,
         "fields": List[FieldValueOutputTypeDef],
-        "templateId": str,
-    },
-)
-_OptionalSearchCasesResponseItemTypeDef = TypedDict(
-    "_OptionalSearchCasesResponseItemTypeDef",
-    {
         "tags": Dict[str, str],
+        "templateId": str,
     },
-    total=False,
 )
 
-class SearchCasesResponseItemTypeDef(
-    _RequiredSearchCasesResponseItemTypeDef, _OptionalSearchCasesResponseItemTypeDef
-):
-    pass
-
 _RequiredCreateCaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCaseRequestRequestTypeDef",
     {
         "domainId": str,
-        "fields": Sequence[Union[FieldValueTypeDef, FieldValueOutputTypeDef]],
+        "fields": Sequence[FieldValueTypeDef],
         "templateId": str,
     },
 )
 _OptionalCreateCaseRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCaseRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -1158,36 +1164,17 @@
 )
 
 UpdateCaseRequestRequestTypeDef = TypedDict(
     "UpdateCaseRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
-        "fields": Sequence[Union[FieldValueTypeDef, FieldValueOutputTypeDef]],
-    },
-)
-
-_RequiredEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEventBridgeConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
+        "fields": Sequence[FieldValueTypeDef],
     },
 )
-_OptionalEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEventBridgeConfigurationOutputTypeDef",
-    {
-        "includedData": EventIncludedDataOutputTypeDef,
-    },
-    total=False,
-)
-
-class EventBridgeConfigurationOutputTypeDef(
-    _RequiredEventBridgeConfigurationOutputTypeDef, _OptionalEventBridgeConfigurationOutputTypeDef
-):
-    pass
 
 _RequiredEventBridgeConfigurationTypeDef = TypedDict(
     "_RequiredEventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
@@ -1200,29 +1187,36 @@
 )
 
 class EventBridgeConfigurationTypeDef(
     _RequiredEventBridgeConfigurationTypeDef, _OptionalEventBridgeConfigurationTypeDef
 ):
     pass
 
+EventBridgeConfigurationOutputTypeDef = TypedDict(
+    "EventBridgeConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "includedData": EventIncludedDataOutputTypeDef,
+    },
+)
+
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LayoutSectionsOutputTypeDef = TypedDict(
     "LayoutSectionsOutputTypeDef",
     {
         "sections": List[SectionOutputTypeDef],
     },
-    total=False,
 )
 
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
@@ -1245,37 +1239,36 @@
         "field": FieldFilterTypeDef,
         "not": Dict[str, Any],
         "orAll": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-GetCaseEventConfigurationResponseTypeDef = TypedDict(
-    "GetCaseEventConfigurationResponseTypeDef",
-    {
-        "eventBridge": EventBridgeConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
         "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
 
+GetCaseEventConfigurationResponseTypeDef = TypedDict(
+    "GetCaseEventConfigurationResponseTypeDef",
+    {
+        "eventBridge": EventBridgeConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BasicLayoutOutputTypeDef = TypedDict(
     "BasicLayoutOutputTypeDef",
     {
         "moreInfo": LayoutSectionsOutputTypeDef,
         "topPanel": LayoutSectionsOutputTypeDef,
     },
-    total=False,
 )
 
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
@@ -1284,15 +1277,14 @@
 )
 
 LayoutContentOutputTypeDef = TypedDict(
     "LayoutContentOutputTypeDef",
     {
         "basic": BasicLayoutOutputTypeDef,
     },
-    total=False,
 )
 
 LayoutContentTypeDef = TypedDict(
     "LayoutContentTypeDef",
     {
         "basic": BasicLayoutTypeDef,
     },
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases.egg-info/PKG-INFO` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ConnectCases 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.8
+Summary: Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,34 +336,41 @@
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
     ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
+    FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
+    CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateFieldRequestRequestTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
+    RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
+    FieldItemOutputTypeDef,
     FieldItemTypeDef,
+    FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionOutputTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
+    LayoutConfigurationOutputTypeDef,
+    RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
@@ -371,69 +378,69 @@
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
-    CaseEventIncludedDataOutputTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDomainResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
+    ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     FieldValueOutputTypeDef,
     FieldValueTypeDef,
+    GetTemplateResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
-    EventIncludedDataOutputTypeDef,
     EventIncludedDataTypeDef,
+    EventIncludedDataOutputTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
     SectionOutputTypeDef,
     SectionTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
     CreateCaseRequestRequestTypeDef,
     FieldFilterTypeDef,
     UpdateCaseRequestRequestTypeDef,
-    EventBridgeConfigurationOutputTypeDef,
     EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     SearchRelatedItemsResponseTypeDef,
     LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
     SearchCasesResponseTypeDef,
     CaseFilterTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    GetCaseEventConfigurationResponseTypeDef,
     BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
     LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
     GetLayoutResponseTypeDef,
     CreateLayoutRequestRequestTypeDef,
     UpdateLayoutRequestRequestTypeDef,
```

### Comparing `mypy-boto3-connectcases-1.28.15.post1/mypy_boto3_connectcases.egg-info/SOURCES.txt` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.15.post1/setup.py` & `mypy-boto3-connectcases-1.28.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcases",
-    version="1.28.15.post1",
+    version="1.28.8",
     packages=["mypy_boto3_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectCases 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

