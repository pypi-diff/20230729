# Comparing `tmp/mypy-boto3-macie-1.28.12.tar.gz` & `tmp/mypy-boto3-macie-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-macie-1.28.12.tar", last modified: Thu Jul 27 05:34:59 2023, max compression
+gzip compressed data, was "mypy-boto3-macie-1.28.15.tar", last modified: Fri Jul 28 20:43:12 2023, max compression
```

## Comparing `mypy-boto3-macie-1.28.12.tar` & `mypy-boto3-macie-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.032448 mypy-boto3-macie-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-27 05:34:59.032448 mypy-boto3-macie-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.032448 mypy-boto3-macie-1.28.12/mypy_boto3_macie/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-07-27 05:25:45.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.032448 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:58.000000 mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:59.032448 mypy-boto3-macie-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:25:44.000000 mypy-boto3-macie-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:12.121431 mypy-boto3-macie-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-07-28 20:43:12.113431 mypy-boto3-macie-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:12.109430 mypy-boto3-macie-1.28.15/mypy_boto3_macie/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-28 20:30:45.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-07-28 20:30:45.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:12.113431 mypy-boto3-macie-1.28.15/mypy_boto3_macie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-07-28 20:43:11.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:43:11.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:11.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:11.000000 mypy-boto3-macie-1.28.15/mypy_boto3_macie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:12.121431 mypy-boto3-macie-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:30:44.000000 mypy-boto3-macie-1.28.15/setup.py
```

### Comparing `mypy-boto3-macie-1.28.12/LICENSE` & `mypy-boto3-macie-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.12/PKG-INFO` & `mypy-boto3-macie-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie
-Version: 1.28.12
-Summary: Type annotations for boto3.Macie 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Macie 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie)](https://pepy.tech/project/mypy-boto3-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
+[boto3.Macie 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [mypy-boto3-macie docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,36 +325,33 @@
 
 `mypy_boto3_macie.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
-    ClassificationTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
-    EmptyResponseMetadataTypeDef,
-    S3ResourceOutputTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    S3ResourceClassificationOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListMemberAccountsResultTypeDef,
-    ListS3ResourcesResultTypeDef,
     AssociateS3ResourcesRequestRequestTypeDef,
+    ListS3ResourcesResultTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
 )
```

### Comparing `mypy-boto3-macie-1.28.12/README.md` & `mypy-boto3-macie-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie)](https://pepy.tech/project/mypy-boto3-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
+[boto3.Macie 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [mypy-boto3-macie docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,36 +293,33 @@
 
 `mypy_boto3_macie.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
-    ClassificationTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
-    EmptyResponseMetadataTypeDef,
-    S3ResourceOutputTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    S3ResourceClassificationOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListMemberAccountsResultTypeDef,
-    ListS3ResourcesResultTypeDef,
     AssociateS3ResourcesRequestRequestTypeDef,
+    ListS3ResourcesResultTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
 )
```

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/__init__.py` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/__init__.pyi` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/__main__.py` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Macie 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Macie 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie\nOther"
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

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/client.py` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/client.pyi` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/literals.py` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/literals.pyi` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/paginator.py` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListMemberAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMemberAccountsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#listmemberaccountspaginator)
         """
 
 
 class ListS3ResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#lists3resourcespaginator)
     """
 
     def paginate(
-        self, *, memberAccountId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, memberAccountId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListS3ResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#lists3resourcespaginator)
         """
```

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/paginator.pyi` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListMemberAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMemberAccountsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#listmemberaccountspaginator)
         """
 
 class ListS3ResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#lists3resourcespaginator)
     """
 
     def paginate(
-        self, *, memberAccountId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, memberAccountId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListS3ResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/paginators/#lists3resourcespaginator)
         """
```

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/type_defs.py` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,54 +24,54 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateMemberAccountRequestRequestTypeDef",
-    "ClassificationTypeOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "ClassificationTypeTypeDef",
     "ClassificationTypeUpdateTypeDef",
     "DisassociateMemberAccountRequestRequestTypeDef",
     "S3ResourceTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "S3ResourceOutputTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
     "MemberAccountTypeDef",
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListS3ResourcesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "S3ResourceClassificationOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "S3ResourceClassificationTypeDef",
     "S3ResourceClassificationUpdateTypeDef",
     "DisassociateS3ResourcesRequestRequestTypeDef",
     "FailedS3ResourceTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListMemberAccountsResultTypeDef",
-    "ListS3ResourcesResultTypeDef",
     "AssociateS3ResourcesRequestRequestTypeDef",
+    "ListS3ResourcesResultTypeDef",
     "UpdateS3ResourcesRequestRequestTypeDef",
     "AssociateS3ResourcesResultTypeDef",
     "DisassociateS3ResourcesResultTypeDef",
     "UpdateS3ResourcesResultTypeDef",
 )
 
 AssociateMemberAccountRequestRequestTypeDef = TypedDict(
     "AssociateMemberAccountRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
 )
 
-ClassificationTypeOutputTypeDef = TypedDict(
-    "ClassificationTypeOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "oneTime": S3OneTimeClassificationTypeType,
-        "continuous": Literal["FULL"],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ClassificationTypeTypeDef = TypedDict(
     "ClassificationTypeTypeDef",
     {
         "oneTime": S3OneTimeClassificationTypeType,
@@ -110,44 +110,20 @@
 )
 
 
 class S3ResourceTypeDef(_RequiredS3ResourceTypeDef, _OptionalS3ResourceTypeDef):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredS3ResourceOutputTypeDef = TypedDict(
-    "_RequiredS3ResourceOutputTypeDef",
-    {
-        "bucketName": str,
-    },
-)
-_OptionalS3ResourceOutputTypeDef = TypedDict(
-    "_OptionalS3ResourceOutputTypeDef",
-    {
-        "prefix": str,
-    },
-    total=False,
-)
-
-
-class S3ResourceOutputTypeDef(_RequiredS3ResourceOutputTypeDef, _OptionalS3ResourceOutputTypeDef):
-    pass
-
-
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
@@ -161,76 +137,31 @@
     "MemberAccountTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
-    {
-        "memberAccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListS3ResourcesRequestRequestTypeDef = TypedDict(
     "ListS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
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
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-_RequiredS3ResourceClassificationOutputTypeDef = TypedDict(
-    "_RequiredS3ResourceClassificationOutputTypeDef",
-    {
-        "bucketName": str,
-        "classificationType": ClassificationTypeOutputTypeDef,
-    },
-)
-_OptionalS3ResourceClassificationOutputTypeDef = TypedDict(
-    "_OptionalS3ResourceClassificationOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "prefix": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class S3ResourceClassificationOutputTypeDef(
-    _RequiredS3ResourceClassificationOutputTypeDef, _OptionalS3ResourceClassificationOutputTypeDef
-):
-    pass
-
-
 _RequiredS3ResourceClassificationTypeDef = TypedDict(
     "_RequiredS3ResourceClassificationTypeDef",
     {
         "bucketName": str,
         "classificationType": ClassificationTypeTypeDef,
     },
 )
@@ -292,36 +223,44 @@
 ):
     pass
 
 
 FailedS3ResourceTypeDef = TypedDict(
     "FailedS3ResourceTypeDef",
     {
-        "failedItem": S3ResourceOutputTypeDef,
+        "failedItem": S3ResourceTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-ListMemberAccountsResultTypeDef = TypedDict(
-    "ListMemberAccountsResultTypeDef",
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     {
-        "memberAccounts": List[MemberAccountTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListS3ResourcesResultTypeDef = TypedDict(
-    "ListS3ResourcesResultTypeDef",
+ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     {
-        "s3Resources": List[S3ResourceClassificationOutputTypeDef],
+        "memberAccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMemberAccountsResultTypeDef = TypedDict(
+    "ListMemberAccountsResultTypeDef",
+    {
+        "memberAccounts": List[MemberAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateS3ResourcesRequestRequestTypeDef",
     {
         "s3Resources": Sequence[S3ResourceClassificationTypeDef],
@@ -339,14 +278,23 @@
 class AssociateS3ResourcesRequestRequestTypeDef(
     _RequiredAssociateS3ResourcesRequestRequestTypeDef,
     _OptionalAssociateS3ResourcesRequestRequestTypeDef,
 ):
     pass
 
 
+ListS3ResourcesResultTypeDef = TypedDict(
+    "ListS3ResourcesResultTypeDef",
+    {
+        "s3Resources": List[S3ResourceClassificationTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateS3ResourcesRequestRequestTypeDef",
     {
         "s3ResourcesUpdate": Sequence[S3ResourceClassificationUpdateTypeDef],
     },
 )
 _OptionalUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
@@ -364,26 +312,26 @@
     pass
 
 
 AssociateS3ResourcesResultTypeDef = TypedDict(
     "AssociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateS3ResourcesResultTypeDef = TypedDict(
     "DisassociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateS3ResourcesResultTypeDef = TypedDict(
     "UpdateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie/type_defs.pyi` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -23,54 +23,54 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateMemberAccountRequestRequestTypeDef",
-    "ClassificationTypeOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "ClassificationTypeTypeDef",
     "ClassificationTypeUpdateTypeDef",
     "DisassociateMemberAccountRequestRequestTypeDef",
     "S3ResourceTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "S3ResourceOutputTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
     "MemberAccountTypeDef",
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListS3ResourcesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "S3ResourceClassificationOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "S3ResourceClassificationTypeDef",
     "S3ResourceClassificationUpdateTypeDef",
     "DisassociateS3ResourcesRequestRequestTypeDef",
     "FailedS3ResourceTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListMemberAccountsResultTypeDef",
-    "ListS3ResourcesResultTypeDef",
     "AssociateS3ResourcesRequestRequestTypeDef",
+    "ListS3ResourcesResultTypeDef",
     "UpdateS3ResourcesRequestRequestTypeDef",
     "AssociateS3ResourcesResultTypeDef",
     "DisassociateS3ResourcesResultTypeDef",
     "UpdateS3ResourcesResultTypeDef",
 )
 
 AssociateMemberAccountRequestRequestTypeDef = TypedDict(
     "AssociateMemberAccountRequestRequestTypeDef",
     {
         "memberAccountId": str,
     },
 )
 
-ClassificationTypeOutputTypeDef = TypedDict(
-    "ClassificationTypeOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "oneTime": S3OneTimeClassificationTypeType,
-        "continuous": Literal["FULL"],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ClassificationTypeTypeDef = TypedDict(
     "ClassificationTypeTypeDef",
     {
         "oneTime": S3OneTimeClassificationTypeType,
@@ -107,42 +107,20 @@
     },
     total=False,
 )
 
 class S3ResourceTypeDef(_RequiredS3ResourceTypeDef, _OptionalS3ResourceTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredS3ResourceOutputTypeDef = TypedDict(
-    "_RequiredS3ResourceOutputTypeDef",
-    {
-        "bucketName": str,
-    },
-)
-_OptionalS3ResourceOutputTypeDef = TypedDict(
-    "_OptionalS3ResourceOutputTypeDef",
-    {
-        "prefix": str,
-    },
-    total=False,
-)
-
-class S3ResourceOutputTypeDef(_RequiredS3ResourceOutputTypeDef, _OptionalS3ResourceOutputTypeDef):
-    pass
-
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
@@ -156,74 +134,31 @@
     "MemberAccountTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
-    {
-        "memberAccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListS3ResourcesRequestRequestTypeDef = TypedDict(
     "ListS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
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
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-_RequiredS3ResourceClassificationOutputTypeDef = TypedDict(
-    "_RequiredS3ResourceClassificationOutputTypeDef",
-    {
-        "bucketName": str,
-        "classificationType": ClassificationTypeOutputTypeDef,
-    },
-)
-_OptionalS3ResourceClassificationOutputTypeDef = TypedDict(
-    "_OptionalS3ResourceClassificationOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "prefix": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class S3ResourceClassificationOutputTypeDef(
-    _RequiredS3ResourceClassificationOutputTypeDef, _OptionalS3ResourceClassificationOutputTypeDef
-):
-    pass
-
 _RequiredS3ResourceClassificationTypeDef = TypedDict(
     "_RequiredS3ResourceClassificationTypeDef",
     {
         "bucketName": str,
         "classificationType": ClassificationTypeTypeDef,
     },
 )
@@ -279,36 +214,44 @@
     _OptionalDisassociateS3ResourcesRequestRequestTypeDef,
 ):
     pass
 
 FailedS3ResourceTypeDef = TypedDict(
     "FailedS3ResourceTypeDef",
     {
-        "failedItem": S3ResourceOutputTypeDef,
+        "failedItem": S3ResourceTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-ListMemberAccountsResultTypeDef = TypedDict(
-    "ListMemberAccountsResultTypeDef",
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     {
-        "memberAccounts": List[MemberAccountTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListS3ResourcesResultTypeDef = TypedDict(
-    "ListS3ResourcesResultTypeDef",
+ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
+    {
+        "memberAccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMemberAccountsResultTypeDef = TypedDict(
+    "ListMemberAccountsResultTypeDef",
     {
-        "s3Resources": List[S3ResourceClassificationOutputTypeDef],
+        "memberAccounts": List[MemberAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateS3ResourcesRequestRequestTypeDef",
     {
         "s3Resources": Sequence[S3ResourceClassificationTypeDef],
@@ -324,14 +267,23 @@
 
 class AssociateS3ResourcesRequestRequestTypeDef(
     _RequiredAssociateS3ResourcesRequestRequestTypeDef,
     _OptionalAssociateS3ResourcesRequestRequestTypeDef,
 ):
     pass
 
+ListS3ResourcesResultTypeDef = TypedDict(
+    "ListS3ResourcesResultTypeDef",
+    {
+        "s3Resources": List[S3ResourceClassificationTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateS3ResourcesRequestRequestTypeDef",
     {
         "s3ResourcesUpdate": Sequence[S3ResourceClassificationUpdateTypeDef],
     },
 )
 _OptionalUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
@@ -347,26 +299,26 @@
 ):
     pass
 
 AssociateS3ResourcesResultTypeDef = TypedDict(
     "AssociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateS3ResourcesResultTypeDef = TypedDict(
     "DisassociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateS3ResourcesResultTypeDef = TypedDict(
     "UpdateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/PKG-INFO` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie
-Version: 1.28.12
-Summary: Type annotations for boto3.Macie 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Macie 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie)](https://pepy.tech/project/mypy-boto3-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
+[boto3.Macie 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [mypy-boto3-macie docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,36 +325,33 @@
 
 `mypy_boto3_macie.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
-    ClassificationTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
-    EmptyResponseMetadataTypeDef,
-    S3ResourceOutputTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    S3ResourceClassificationOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListMemberAccountsResultTypeDef,
-    ListS3ResourcesResultTypeDef,
     AssociateS3ResourcesRequestRequestTypeDef,
+    ListS3ResourcesResultTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
 )
```

### Comparing `mypy-boto3-macie-1.28.12/mypy_boto3_macie.egg-info/SOURCES.txt` & `mypy-boto3-macie-1.28.15/mypy_boto3_macie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie-1.28.12/setup.py` & `mypy-boto3-macie-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-macie",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_macie"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Macie 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Macie 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

