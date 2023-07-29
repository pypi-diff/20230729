# Comparing `tmp/mypy-boto3-marketplace-entitlement-1.28.12.tar.gz` & `tmp/mypy-boto3-marketplace-entitlement-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-marketplace-entitlement-1.28.12.tar", last modified: Thu Jul 27 05:34:59 2023, max compression
+gzip compressed data, was "mypy-boto3-marketplace-entitlement-1.28.15.tar", last modified: Fri Jul 28 20:43:14 2023, max compression
```

## Comparing `mypy-boto3-marketplace-entitlement-1.28.12.tar` & `mypy-boto3-marketplace-entitlement-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.952445 mypy-boto3-marketplace-entitlement-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-07-27 05:34:59.948445 mypy-boto3-marketplace-entitlement-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.948445 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.948445 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 05:34:59.000000 mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:59.952445 mypy-boto3-marketplace-entitlement-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-27 05:25:53.000000 mypy-boto3-marketplace-entitlement-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.869468 mypy-boto3-marketplace-entitlement-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-07-28 20:43:14.865468 mypy-boto3-marketplace-entitlement-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.853468 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.865468 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 20:43:14.000000 mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:14.869468 mypy-boto3-marketplace-entitlement-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-28 20:30:56.000000 mypy-boto3-marketplace-entitlement-1.28.15/setup.py
```

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/LICENSE` & `mypy-boto3-marketplace-entitlement-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/PKG-INFO` & `mypy-boto3-marketplace-entitlement-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-entitlement
-Version: 1.28.12
-Summary: Type annotations for boto3.MarketplaceEntitlementService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MarketplaceEntitlementService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-entitlement)](https://pepy.tech/project/mypy-boto3-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceEntitlementService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[boto3.MarketplaceEntitlementService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
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
 [mypy-boto3-marketplace-entitlement docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,19 +322,19 @@
 
 `mypy_boto3_marketplace_entitlement.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_entitlement.type_defs import (
     EntitlementValueTypeDef,
-    GetEntitlementsRequestGetEntitlementsPaginateTypeDef,
-    GetEntitlementsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    GetEntitlementsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EntitlementTypeDef,
+    GetEntitlementsRequestGetEntitlementsPaginateTypeDef,
     GetEntitlementsResultTypeDef,
 )
 
 
 def get_structure() -> EntitlementValueTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/README.md` & `mypy-boto3-marketplace-entitlement-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-entitlement)](https://pepy.tech/project/mypy-boto3-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceEntitlementService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[boto3.MarketplaceEntitlementService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
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
 [mypy-boto3-marketplace-entitlement docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,19 +290,19 @@
 
 `mypy_boto3_marketplace_entitlement.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_entitlement.type_defs import (
     EntitlementValueTypeDef,
-    GetEntitlementsRequestGetEntitlementsPaginateTypeDef,
-    GetEntitlementsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    GetEntitlementsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EntitlementTypeDef,
+    GetEntitlementsRequestGetEntitlementsPaginateTypeDef,
     GetEntitlementsResultTypeDef,
 )
 
 
 def get_structure() -> EntitlementValueTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/__init__.py` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/__init__.pyi` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/__main__.py` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceEntitlementService 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MarketplaceEntitlementService 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService\nOther"
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

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/client.py` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/client.pyi` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/literals.py` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/literals.pyi` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/paginator.py` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,13 +46,13 @@
     """
 
     def paginate(
         self,
         *,
         ProductCode: str,
         Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetEntitlementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Paginator.GetEntitlements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/paginators/#getentitlementspaginator)
         """
```

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/paginator.pyi` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     """
 
     def paginate(
         self,
         *,
         ProductCode: str,
         Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetEntitlementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Paginator.GetEntitlements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/paginators/#getentitlementspaginator)
         """
```

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/type_defs.py` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,56 +21,43 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "EntitlementValueTypeDef",
-    "GetEntitlementsRequestGetEntitlementsPaginateTypeDef",
-    "GetEntitlementsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "GetEntitlementsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EntitlementTypeDef",
+    "GetEntitlementsRequestGetEntitlementsPaginateTypeDef",
     "GetEntitlementsResultTypeDef",
 )
 
 EntitlementValueTypeDef = TypedDict(
     "EntitlementValueTypeDef",
     {
         "IntegerValue": int,
         "DoubleValue": float,
         "BooleanValue": bool,
         "StringValue": str,
     },
     total=False,
 )
 
-_RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef = TypedDict(
-    "_RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef",
-    {
-        "ProductCode": str,
-    },
-)
-_OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef = TypedDict(
-    "_OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Filter": Mapping[GetEntitlementFilterNameType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetEntitlementsRequestGetEntitlementsPaginateTypeDef(
-    _RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef,
-    _OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetEntitlementsRequestRequestTypeDef = TypedDict(
     "_RequiredGetEntitlementsRequestRequestTypeDef",
     {
         "ProductCode": str,
     },
 )
 _OptionalGetEntitlementsRequestRequestTypeDef = TypedDict(
@@ -86,24 +73,14 @@
 
 class GetEntitlementsRequestRequestTypeDef(
     _RequiredGetEntitlementsRequestRequestTypeDef, _OptionalGetEntitlementsRequestRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -119,15 +96,38 @@
         "CustomerIdentifier": str,
         "Value": EntitlementValueTypeDef,
         "ExpirationDate": datetime,
     },
     total=False,
 )
 
+_RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef = TypedDict(
+    "_RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef",
+    {
+        "ProductCode": str,
+    },
+)
+_OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef = TypedDict(
+    "_OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef",
+    {
+        "Filter": Mapping[GetEntitlementFilterNameType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetEntitlementsRequestGetEntitlementsPaginateTypeDef(
+    _RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef,
+    _OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef,
+):
+    pass
+
+
 GetEntitlementsResultTypeDef = TypedDict(
     "GetEntitlementsResultTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement/type_defs.pyi` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,54 +20,43 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "EntitlementValueTypeDef",
-    "GetEntitlementsRequestGetEntitlementsPaginateTypeDef",
-    "GetEntitlementsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "GetEntitlementsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EntitlementTypeDef",
+    "GetEntitlementsRequestGetEntitlementsPaginateTypeDef",
     "GetEntitlementsResultTypeDef",
 )
 
 EntitlementValueTypeDef = TypedDict(
     "EntitlementValueTypeDef",
     {
         "IntegerValue": int,
         "DoubleValue": float,
         "BooleanValue": bool,
         "StringValue": str,
     },
     total=False,
 )
 
-_RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef = TypedDict(
-    "_RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef",
-    {
-        "ProductCode": str,
-    },
-)
-_OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef = TypedDict(
-    "_OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Filter": Mapping[GetEntitlementFilterNameType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetEntitlementsRequestGetEntitlementsPaginateTypeDef(
-    _RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef,
-    _OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetEntitlementsRequestRequestTypeDef = TypedDict(
     "_RequiredGetEntitlementsRequestRequestTypeDef",
     {
         "ProductCode": str,
     },
 )
 _OptionalGetEntitlementsRequestRequestTypeDef = TypedDict(
@@ -81,24 +70,14 @@
 )
 
 class GetEntitlementsRequestRequestTypeDef(
     _RequiredGetEntitlementsRequestRequestTypeDef, _OptionalGetEntitlementsRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -114,15 +93,36 @@
         "CustomerIdentifier": str,
         "Value": EntitlementValueTypeDef,
         "ExpirationDate": datetime,
     },
     total=False,
 )
 
+_RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef = TypedDict(
+    "_RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef",
+    {
+        "ProductCode": str,
+    },
+)
+_OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef = TypedDict(
+    "_OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef",
+    {
+        "Filter": Mapping[GetEntitlementFilterNameType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetEntitlementsRequestGetEntitlementsPaginateTypeDef(
+    _RequiredGetEntitlementsRequestGetEntitlementsPaginateTypeDef,
+    _OptionalGetEntitlementsRequestGetEntitlementsPaginateTypeDef,
+):
+    pass
+
 GetEntitlementsResultTypeDef = TypedDict(
     "GetEntitlementsResultTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement.egg-info/PKG-INFO` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-entitlement
-Version: 1.28.12
-Summary: Type annotations for boto3.MarketplaceEntitlementService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MarketplaceEntitlementService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplace-entitlement)](https://pepy.tech/project/mypy-boto3-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceEntitlementService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[boto3.MarketplaceEntitlementService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
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
 [mypy-boto3-marketplace-entitlement docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_entitlement/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,19 +322,19 @@
 
 `mypy_boto3_marketplace_entitlement.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_entitlement.type_defs import (
     EntitlementValueTypeDef,
-    GetEntitlementsRequestGetEntitlementsPaginateTypeDef,
-    GetEntitlementsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    GetEntitlementsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EntitlementTypeDef,
+    GetEntitlementsRequestGetEntitlementsPaginateTypeDef,
     GetEntitlementsResultTypeDef,
 )
 
 
 def get_structure() -> EntitlementValueTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/mypy_boto3_marketplace_entitlement.egg-info/SOURCES.txt` & `mypy-boto3-marketplace-entitlement-1.28.15/mypy_boto3_marketplace_entitlement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplace-entitlement-1.28.12/setup.py` & `mypy-boto3-marketplace-entitlement-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-marketplace-entitlement",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_marketplace_entitlement"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceEntitlementService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MarketplaceEntitlementService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

