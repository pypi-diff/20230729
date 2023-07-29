# Comparing `tmp/mypy-boto3-marketplace-catalog-1.28.12.tar.gz` & `tmp/mypy-boto3-marketplace-catalog-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-marketplace-catalog-1.28.12.tar", last modified: Thu Jul 27 05:34:59 2023, max compression
+gzip compressed data, was "mypy-boto3-marketplace-catalog-1.28.15.tar", last modified: Fri Jul 28 20:43:14 2023, max compression
```

## Comparing `mypy-boto3-marketplace-catalog-1.28.12.tar` & `mypy-boto3-marketplace-catalog-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.924445 mypy-boto3-marketplace-catalog-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-27 05:34:59.924445 mypy-boto3-marketplace-catalog-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.920445 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.924445 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:59.924445 mypy-boto3-marketplace-catalog-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 05:25:52.000000 mypy-boto3-marketplace-catalog-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.753467 mypy-boto3-marketplace-catalog-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-07-28 20:43:14.749467 mypy-boto3-marketplace-catalog-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.749467 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.749467 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:14.753467 mypy-boto3-marketplace-catalog-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-28 20:30:55.000000 mypy-boto3-marketplace-catalog-1.28.15/setup.py
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/LICENSE` & `mypy-boto3-marketplace-catalog-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/PKG-INFO` & `mypy-boto3-marketplace-catalog-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-catalog
-Version: 1.28.12
-Summary: Type annotations for boto3.MarketplaceCatalog 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MarketplaceCatalog 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-catalog)](https://pepy.tech/project/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,46 +327,44 @@
 
 `mypy_boto3_marketplace_catalog.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
-    EntityOutputTypeDef,
-    ErrorDetailTypeDef,
     EntityTypeDef,
+    ErrorDetailTypeDef,
     TagTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
-    DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartChangeSetResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CancelChangeSetResponseTypeDef,
+    DescribeEntityResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    StartChangeSetResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
     ListChangeSetsRequestListChangeSetsPaginateTypeDef,
     ListChangeSetsRequestRequestTypeDef,
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/README.md` & `mypy-boto3-marketplace-catalog-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-catalog)](https://pepy.tech/project/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,46 +295,44 @@
 
 `mypy_boto3_marketplace_catalog.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
-    EntityOutputTypeDef,
-    ErrorDetailTypeDef,
     EntityTypeDef,
+    ErrorDetailTypeDef,
     TagTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
-    DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartChangeSetResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CancelChangeSetResponseTypeDef,
+    DescribeEntityResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    StartChangeSetResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
     ListChangeSetsRequestListChangeSetsPaginateTypeDef,
     ListChangeSetsRequestRequestTypeDef,
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__init__.py` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__init__.pyi` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/__main__.py` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceCatalog 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MarketplaceCatalog 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/client.py` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/client.pyi` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/literals.py` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/literals.pyi` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/paginator.py` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def paginate(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChangeSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListChangeSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/paginators/#listchangesetspaginator)
         """
 
 
@@ -77,13 +77,13 @@
         self,
         *,
         Catalog: str,
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         OwnershipType: OwnershipTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListEntities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/paginators/#listentitiespaginator)
         """
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/paginator.pyi` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def paginate(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChangeSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListChangeSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/paginators/#listchangesetspaginator)
         """
 
 class ListEntitiesPaginator(Paginator):
@@ -73,13 +73,13 @@
         self,
         *,
         Catalog: str,
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         OwnershipType: OwnershipTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListEntities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/paginators/#listentitiespaginator)
         """
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/type_defs.py` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,64 +20,64 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
-    "CancelChangeSetResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ChangeSetSummaryListItemTypeDef",
-    "EntityOutputTypeDef",
-    "ErrorDetailTypeDef",
     "EntityTypeDef",
+    "ErrorDetailTypeDef",
     "TagTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeChangeSetRequestRequestTypeDef",
     "DescribeEntityRequestRequestTypeDef",
-    "DescribeEntityResponseTypeDef",
     "EntitySummaryTypeDef",
     "FilterTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SortTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartChangeSetResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CancelChangeSetResponseTypeDef",
+    "DescribeEntityResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "StartChangeSetResponseTypeDef",
     "ListChangeSetsResponseTypeDef",
     "ChangeSummaryTypeDef",
     "ChangeTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListChangeSetsRequestListChangeSetsPaginateTypeDef",
     "ListChangeSetsRequestRequestTypeDef",
     "ListEntitiesRequestListEntitiesPaginateTypeDef",
     "ListEntitiesRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "DescribeChangeSetResponseTypeDef",
     "StartChangeSetRequestRequestTypeDef",
 )
 
 CancelChangeSetRequestRequestTypeDef = TypedDict(
     "CancelChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
         "ChangeSetId": str,
     },
 )
 
-CancelChangeSetResponseTypeDef = TypedDict(
-    "CancelChangeSetResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ChangeSetId": str,
-        "ChangeSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ChangeSetSummaryListItemTypeDef = TypedDict(
     "ChangeSetSummaryListItemTypeDef",
     {
         "ChangeSetId": str,
@@ -88,61 +88,42 @@
         "Status": ChangeStatusType,
         "EntityIdList": List[str],
         "FailureCode": FailureCodeType,
     },
     total=False,
 )
 
-_RequiredEntityOutputTypeDef = TypedDict(
-    "_RequiredEntityOutputTypeDef",
+_RequiredEntityTypeDef = TypedDict(
+    "_RequiredEntityTypeDef",
     {
         "Type": str,
     },
 )
-_OptionalEntityOutputTypeDef = TypedDict(
-    "_OptionalEntityOutputTypeDef",
+_OptionalEntityTypeDef = TypedDict(
+    "_OptionalEntityTypeDef",
     {
         "Identifier": str,
     },
     total=False,
 )
 
 
-class EntityOutputTypeDef(_RequiredEntityOutputTypeDef, _OptionalEntityOutputTypeDef):
+class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
     pass
 
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredEntityTypeDef = TypedDict(
-    "_RequiredEntityTypeDef",
-    {
-        "Type": str,
-    },
-)
-_OptionalEntityTypeDef = TypedDict(
-    "_OptionalEntityTypeDef",
-    {
-        "Identifier": str,
-    },
-    total=False,
-)
-
-
-class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
-    pass
-
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -166,26 +147,14 @@
     "DescribeEntityRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityId": str,
     },
 )
 
-DescribeEntityResponseTypeDef = TypedDict(
-    "DescribeEntityResponseTypeDef",
-    {
-        "EntityType": str,
-        "EntityIdentifier": str,
-        "EntityArn": str,
-        "LastModifiedDate": str,
-        "Details": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EntitySummaryTypeDef = TypedDict(
     "EntitySummaryTypeDef",
     {
         "Name": str,
         "EntityType": str,
         "EntityId": str,
         "EntityArn": str,
@@ -207,20 +176,22 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "SortBy": str,
         "SortOrder": SortOrderType,
@@ -231,82 +202,82 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+PutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "PutResourcePolicyRequestRequestTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "ResourceArn": str,
+        "Policy": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
-    total=False,
 )
 
-PutResourcePolicyRequestRequestTypeDef = TypedDict(
-    "PutResourcePolicyRequestRequestTypeDef",
+CancelChangeSetResponseTypeDef = TypedDict(
+    "CancelChangeSetResponseTypeDef",
     {
-        "ResourceArn": str,
-        "Policy": str,
+        "ChangeSetId": str,
+        "ChangeSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeEntityResponseTypeDef = TypedDict(
+    "DescribeEntityResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "EntityType": str,
+        "EntityIdentifier": str,
+        "EntityArn": str,
+        "LastModifiedDate": str,
+        "Details": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartChangeSetResponseTypeDef = TypedDict(
-    "StartChangeSetResponseTypeDef",
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
     {
-        "ChangeSetId": str,
-        "ChangeSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartChangeSetResponseTypeDef = TypedDict(
+    "StartChangeSetResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "ChangeSetId": str,
+        "ChangeSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChangeSetsResponseTypeDef = TypedDict(
     "ListChangeSetsResponseTypeDef",
     {
         "ChangeSetSummaryList": List[ChangeSetSummaryListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeSummaryTypeDef = TypedDict(
     "ChangeSummaryTypeDef",
     {
         "ChangeType": str,
-        "Entity": EntityOutputTypeDef,
+        "Entity": EntityTypeDef,
         "Details": str,
         "ErrorDetailList": List[ErrorDetailTypeDef],
         "ChangeName": str,
     },
     total=False,
 )
 
@@ -328,43 +299,52 @@
 )
 
 
 class ChangeTypeDef(_RequiredChangeTypeDef, _OptionalChangeTypeDef):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "EntitySummaryList": List[EntitySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
     "_RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef",
     {
         "Catalog": str,
     },
 )
 _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
     "_OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListChangeSetsRequestListChangeSetsPaginateTypeDef(
     _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef,
@@ -406,15 +386,15 @@
 )
 _OptionalListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
     "_OptionalListEntitiesRequestListEntitiesPaginateTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
         "OwnershipType": OwnershipTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListEntitiesRequestListEntitiesPaginateTypeDef(
     _RequiredListEntitiesRequestListEntitiesPaginateTypeDef,
@@ -445,36 +425,27 @@
 
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeChangeSetResponseTypeDef = TypedDict(
     "DescribeChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ChangeSetName": str,
         "StartTime": str,
         "EndTime": str,
         "Status": ChangeStatusType,
         "FailureCode": FailureCodeType,
         "FailureDescription": str,
         "ChangeSet": List[ChangeSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredStartChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog/type_defs.pyi` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -19,64 +19,64 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
-    "CancelChangeSetResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ChangeSetSummaryListItemTypeDef",
-    "EntityOutputTypeDef",
-    "ErrorDetailTypeDef",
     "EntityTypeDef",
+    "ErrorDetailTypeDef",
     "TagTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeChangeSetRequestRequestTypeDef",
     "DescribeEntityRequestRequestTypeDef",
-    "DescribeEntityResponseTypeDef",
     "EntitySummaryTypeDef",
     "FilterTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SortTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartChangeSetResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CancelChangeSetResponseTypeDef",
+    "DescribeEntityResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "StartChangeSetResponseTypeDef",
     "ListChangeSetsResponseTypeDef",
     "ChangeSummaryTypeDef",
     "ChangeTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListChangeSetsRequestListChangeSetsPaginateTypeDef",
     "ListChangeSetsRequestRequestTypeDef",
     "ListEntitiesRequestListEntitiesPaginateTypeDef",
     "ListEntitiesRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "DescribeChangeSetResponseTypeDef",
     "StartChangeSetRequestRequestTypeDef",
 )
 
 CancelChangeSetRequestRequestTypeDef = TypedDict(
     "CancelChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
         "ChangeSetId": str,
     },
 )
 
-CancelChangeSetResponseTypeDef = TypedDict(
-    "CancelChangeSetResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ChangeSetId": str,
-        "ChangeSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ChangeSetSummaryListItemTypeDef = TypedDict(
     "ChangeSetSummaryListItemTypeDef",
     {
         "ChangeSetId": str,
@@ -87,57 +87,40 @@
         "Status": ChangeStatusType,
         "EntityIdList": List[str],
         "FailureCode": FailureCodeType,
     },
     total=False,
 )
 
-_RequiredEntityOutputTypeDef = TypedDict(
-    "_RequiredEntityOutputTypeDef",
+_RequiredEntityTypeDef = TypedDict(
+    "_RequiredEntityTypeDef",
     {
         "Type": str,
     },
 )
-_OptionalEntityOutputTypeDef = TypedDict(
-    "_OptionalEntityOutputTypeDef",
+_OptionalEntityTypeDef = TypedDict(
+    "_OptionalEntityTypeDef",
     {
         "Identifier": str,
     },
     total=False,
 )
 
-class EntityOutputTypeDef(_RequiredEntityOutputTypeDef, _OptionalEntityOutputTypeDef):
+class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
     pass
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredEntityTypeDef = TypedDict(
-    "_RequiredEntityTypeDef",
-    {
-        "Type": str,
-    },
-)
-_OptionalEntityTypeDef = TypedDict(
-    "_OptionalEntityTypeDef",
-    {
-        "Identifier": str,
-    },
-    total=False,
-)
-
-class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
-    pass
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -161,26 +144,14 @@
     "DescribeEntityRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityId": str,
     },
 )
 
-DescribeEntityResponseTypeDef = TypedDict(
-    "DescribeEntityResponseTypeDef",
-    {
-        "EntityType": str,
-        "EntityIdentifier": str,
-        "EntityArn": str,
-        "LastModifiedDate": str,
-        "Details": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EntitySummaryTypeDef = TypedDict(
     "EntitySummaryTypeDef",
     {
         "Name": str,
         "EntityType": str,
         "EntityId": str,
         "EntityArn": str,
@@ -202,20 +173,22 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "SortBy": str,
         "SortOrder": SortOrderType,
@@ -226,82 +199,82 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+PutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "PutResourcePolicyRequestRequestTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "ResourceArn": str,
+        "Policy": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
-    total=False,
 )
 
-PutResourcePolicyRequestRequestTypeDef = TypedDict(
-    "PutResourcePolicyRequestRequestTypeDef",
+CancelChangeSetResponseTypeDef = TypedDict(
+    "CancelChangeSetResponseTypeDef",
     {
-        "ResourceArn": str,
-        "Policy": str,
+        "ChangeSetId": str,
+        "ChangeSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeEntityResponseTypeDef = TypedDict(
+    "DescribeEntityResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "EntityType": str,
+        "EntityIdentifier": str,
+        "EntityArn": str,
+        "LastModifiedDate": str,
+        "Details": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartChangeSetResponseTypeDef = TypedDict(
-    "StartChangeSetResponseTypeDef",
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
     {
-        "ChangeSetId": str,
-        "ChangeSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartChangeSetResponseTypeDef = TypedDict(
+    "StartChangeSetResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "ChangeSetId": str,
+        "ChangeSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChangeSetsResponseTypeDef = TypedDict(
     "ListChangeSetsResponseTypeDef",
     {
         "ChangeSetSummaryList": List[ChangeSetSummaryListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeSummaryTypeDef = TypedDict(
     "ChangeSummaryTypeDef",
     {
         "ChangeType": str,
-        "Entity": EntityOutputTypeDef,
+        "Entity": EntityTypeDef,
         "Details": str,
         "ErrorDetailList": List[ErrorDetailTypeDef],
         "ChangeName": str,
     },
     total=False,
 )
 
@@ -321,43 +294,52 @@
     },
     total=False,
 )
 
 class ChangeTypeDef(_RequiredChangeTypeDef, _OptionalChangeTypeDef):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "EntitySummaryList": List[EntitySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
     "_RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef",
     {
         "Catalog": str,
     },
 )
 _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
     "_OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListChangeSetsRequestListChangeSetsPaginateTypeDef(
     _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef,
     _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef,
@@ -395,15 +377,15 @@
 )
 _OptionalListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
     "_OptionalListEntitiesRequestListEntitiesPaginateTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
         "OwnershipType": OwnershipTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListEntitiesRequestListEntitiesPaginateTypeDef(
     _RequiredListEntitiesRequestListEntitiesPaginateTypeDef,
     _OptionalListEntitiesRequestListEntitiesPaginateTypeDef,
@@ -430,36 +412,27 @@
 )
 
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeChangeSetResponseTypeDef = TypedDict(
     "DescribeChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ChangeSetName": str,
         "StartTime": str,
         "EndTime": str,
         "Status": ChangeStatusType,
         "FailureCode": FailureCodeType,
         "FailureDescription": str,
         "ChangeSet": List[ChangeSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredStartChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-catalog
-Version: 1.28.12
-Summary: Type annotations for boto3.MarketplaceCatalog 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MarketplaceCatalog 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-catalog)](https://pepy.tech/project/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,46 +327,44 @@
 
 `mypy_boto3_marketplace_catalog.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
-    EntityOutputTypeDef,
-    ErrorDetailTypeDef,
     EntityTypeDef,
+    ErrorDetailTypeDef,
     TagTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
-    DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartChangeSetResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CancelChangeSetResponseTypeDef,
+    DescribeEntityResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    StartChangeSetResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
     ListChangeSetsRequestListChangeSetsPaginateTypeDef,
     ListChangeSetsRequestRequestTypeDef,
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt` & `mypy-boto3-marketplace-catalog-1.28.15/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-catalog-1.28.12/setup.py` & `mypy-boto3-marketplace-catalog-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-marketplace-catalog",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_marketplace_catalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceCatalog 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MarketplaceCatalog 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

