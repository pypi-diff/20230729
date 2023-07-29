# Comparing `tmp/mypy-boto3-managedblockchain-query-1.28.12.tar.gz` & `tmp/mypy-boto3-managedblockchain-query-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-managedblockchain-query-1.28.12.tar", last modified: Thu Jul 27 05:34:59 2023, max compression
+gzip compressed data, was "mypy-boto3-managedblockchain-query-1.28.15.tar", last modified: Fri Jul 28 20:43:14 2023, max compression
```

## Comparing `mypy-boto3-managedblockchain-query-1.28.12.tar` & `mypy-boto3-managedblockchain-query-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.656446 mypy-boto3-managedblockchain-query-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-27 05:34:59.652446 mypy-boto3-managedblockchain-query-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13563 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-27 05:25:52.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-07-27 05:25:52.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.652446 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:59.656446 mypy-boto3-managedblockchain-query-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-query-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.265460 mypy-boto3-managedblockchain-query-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-28 20:43:14.265460 mypy-boto3-managedblockchain-query-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.257460 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:54.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.265460 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-28 20:43:14.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 20:43:14.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:14.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:14.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:14.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 20:43:14.000000 mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:14.265460 mypy-boto3-managedblockchain-query-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-28 20:30:53.000000 mypy-boto3-managedblockchain-query-1.28.15/setup.py
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/LICENSE` & `mypy-boto3-managedblockchain-query-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/PKG-INFO` & `mypy-boto3-managedblockchain-query-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain-query
-Version: 1.28.12
-Summary: Type annotations for boto3.ManagedBlockchainQuery 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ManagedBlockchainQuery 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain-query)](https://pepy.tech/project/mypy-boto3-managedblockchain-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchainQuery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
+[boto3.ManagedBlockchainQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
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
 [mypy-boto3-managedblockchain-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,37 +338,35 @@
 
 `mypy_boto3_managedblockchain_query.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain_query.type_defs import (
     BlockchainInstantOutputTypeDef,
-    OwnerIdentifierOutputTypeDef,
-    TokenIdentifierOutputTypeDef,
-    BlockchainInstantTypeDef,
     OwnerIdentifierTypeDef,
     TokenIdentifierTypeDef,
+    BlockchainInstantTypeDef,
+    ResponseMetadataTypeDef,
     GetTransactionInputRequestTypeDef,
     TransactionTypeDef,
     OwnerFilterTypeDef,
+    PaginatorConfigTypeDef,
     TokenFilterTypeDef,
-    ListTransactionEventsInputListTransactionEventsPaginateTypeDef,
     ListTransactionEventsInputRequestTypeDef,
     TransactionEventTypeDef,
     ListTransactionsSortTypeDef,
     TransactionOutputItemTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetTokenBalanceErrorItemTypeDef,
     BatchGetTokenBalanceOutputItemTypeDef,
-    GetTokenBalanceOutputTypeDef,
     TokenBalanceTypeDef,
     BatchGetTokenBalanceInputItemTypeDef,
     GetTokenBalanceInputRequestTypeDef,
+    GetTokenBalanceOutputTypeDef,
     GetTransactionOutputTypeDef,
+    ListTransactionEventsInputListTransactionEventsPaginateTypeDef,
     ListTokenBalancesInputListTokenBalancesPaginateTypeDef,
     ListTokenBalancesInputRequestTypeDef,
     ListTransactionEventsOutputTypeDef,
     ListTransactionsInputListTransactionsPaginateTypeDef,
     ListTransactionsInputRequestTypeDef,
     ListTransactionsOutputTypeDef,
     BatchGetTokenBalanceOutputTypeDef,
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/README.md` & `mypy-boto3-managedblockchain-query-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain-query)](https://pepy.tech/project/mypy-boto3-managedblockchain-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchainQuery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
+[boto3.ManagedBlockchainQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
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
 [mypy-boto3-managedblockchain-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,37 +306,35 @@
 
 `mypy_boto3_managedblockchain_query.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain_query.type_defs import (
     BlockchainInstantOutputTypeDef,
-    OwnerIdentifierOutputTypeDef,
-    TokenIdentifierOutputTypeDef,
-    BlockchainInstantTypeDef,
     OwnerIdentifierTypeDef,
     TokenIdentifierTypeDef,
+    BlockchainInstantTypeDef,
+    ResponseMetadataTypeDef,
     GetTransactionInputRequestTypeDef,
     TransactionTypeDef,
     OwnerFilterTypeDef,
+    PaginatorConfigTypeDef,
     TokenFilterTypeDef,
-    ListTransactionEventsInputListTransactionEventsPaginateTypeDef,
     ListTransactionEventsInputRequestTypeDef,
     TransactionEventTypeDef,
     ListTransactionsSortTypeDef,
     TransactionOutputItemTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetTokenBalanceErrorItemTypeDef,
     BatchGetTokenBalanceOutputItemTypeDef,
-    GetTokenBalanceOutputTypeDef,
     TokenBalanceTypeDef,
     BatchGetTokenBalanceInputItemTypeDef,
     GetTokenBalanceInputRequestTypeDef,
+    GetTokenBalanceOutputTypeDef,
     GetTransactionOutputTypeDef,
+    ListTransactionEventsInputListTransactionEventsPaginateTypeDef,
     ListTokenBalancesInputListTokenBalancesPaginateTypeDef,
     ListTokenBalancesInputRequestTypeDef,
     ListTransactionEventsOutputTypeDef,
     ListTransactionsInputListTransactionsPaginateTypeDef,
     ListTransactionsInputRequestTypeDef,
     ListTransactionsOutputTypeDef,
     BatchGetTokenBalanceOutputTypeDef,
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/__init__.py` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/__init__.pyi` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/__main__.py` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedBlockchainQuery 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ManagedBlockchainQuery 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery\nOther"
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

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/client.py` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/client.pyi` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/literals.py` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/literals.pyi` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/paginator.py` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
 
     def paginate(
         self,
         *,
         tokenFilter: TokenFilterTypeDef,
         ownerFilter: OwnerFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTokenBalancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTokenBalances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/paginators/#listtokenbalancespaginator)
         """
 
 
@@ -82,15 +82,15 @@
     """
 
     def paginate(
         self,
         *,
         transactionHash: str,
         network: QueryNetworkType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTransactionEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactionEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/paginators/#listtransactioneventspaginator)
         """
 
 
@@ -104,13 +104,13 @@
         self,
         *,
         address: str,
         network: QueryNetworkType,
         fromBlockchainInstant: BlockchainInstantTypeDef = ...,
         toBlockchainInstant: BlockchainInstantTypeDef = ...,
         sort: ListTransactionsSortTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTransactionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/paginators/#listtransactionspaginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/paginator.pyi` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     """
 
     def paginate(
         self,
         *,
         tokenFilter: TokenFilterTypeDef,
         ownerFilter: OwnerFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTokenBalancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTokenBalances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/paginators/#listtokenbalancespaginator)
         """
 
 class ListTransactionEventsPaginator(Paginator):
@@ -78,15 +78,15 @@
     """
 
     def paginate(
         self,
         *,
         transactionHash: str,
         network: QueryNetworkType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTransactionEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactionEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/paginators/#listtransactioneventspaginator)
         """
 
 class ListTransactionsPaginator(Paginator):
@@ -99,13 +99,13 @@
         self,
         *,
         address: str,
         network: QueryNetworkType,
         fromBlockchainInstant: BlockchainInstantTypeDef = ...,
         toBlockchainInstant: BlockchainInstantTypeDef = ...,
         sort: ListTransactionsSortTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTransactionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/paginators/#listtransactionspaginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/type_defs.py` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,37 +31,35 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BlockchainInstantOutputTypeDef",
-    "OwnerIdentifierOutputTypeDef",
-    "TokenIdentifierOutputTypeDef",
-    "BlockchainInstantTypeDef",
     "OwnerIdentifierTypeDef",
     "TokenIdentifierTypeDef",
+    "BlockchainInstantTypeDef",
+    "ResponseMetadataTypeDef",
     "GetTransactionInputRequestTypeDef",
     "TransactionTypeDef",
     "OwnerFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "TokenFilterTypeDef",
-    "ListTransactionEventsInputListTransactionEventsPaginateTypeDef",
     "ListTransactionEventsInputRequestTypeDef",
     "TransactionEventTypeDef",
     "ListTransactionsSortTypeDef",
     "TransactionOutputItemTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetTokenBalanceErrorItemTypeDef",
     "BatchGetTokenBalanceOutputItemTypeDef",
-    "GetTokenBalanceOutputTypeDef",
     "TokenBalanceTypeDef",
     "BatchGetTokenBalanceInputItemTypeDef",
     "GetTokenBalanceInputRequestTypeDef",
+    "GetTokenBalanceOutputTypeDef",
     "GetTransactionOutputTypeDef",
+    "ListTransactionEventsInputListTransactionEventsPaginateTypeDef",
     "ListTokenBalancesInputListTokenBalancesPaginateTypeDef",
     "ListTokenBalancesInputRequestTypeDef",
     "ListTransactionEventsOutputTypeDef",
     "ListTransactionsInputListTransactionsPaginateTypeDef",
     "ListTransactionsInputRequestTypeDef",
     "ListTransactionsOutputTypeDef",
     "BatchGetTokenBalanceOutputTypeDef",
@@ -73,78 +71,60 @@
     "BlockchainInstantOutputTypeDef",
     {
         "time": datetime,
     },
     total=False,
 )
 
-OwnerIdentifierOutputTypeDef = TypedDict(
-    "OwnerIdentifierOutputTypeDef",
+OwnerIdentifierTypeDef = TypedDict(
+    "OwnerIdentifierTypeDef",
     {
         "address": str,
     },
 )
 
-_RequiredTokenIdentifierOutputTypeDef = TypedDict(
-    "_RequiredTokenIdentifierOutputTypeDef",
+_RequiredTokenIdentifierTypeDef = TypedDict(
+    "_RequiredTokenIdentifierTypeDef",
     {
         "network": QueryNetworkType,
     },
 )
-_OptionalTokenIdentifierOutputTypeDef = TypedDict(
-    "_OptionalTokenIdentifierOutputTypeDef",
+_OptionalTokenIdentifierTypeDef = TypedDict(
+    "_OptionalTokenIdentifierTypeDef",
     {
         "contractAddress": str,
         "tokenId": str,
     },
     total=False,
 )
 
 
-class TokenIdentifierOutputTypeDef(
-    _RequiredTokenIdentifierOutputTypeDef, _OptionalTokenIdentifierOutputTypeDef
-):
+class TokenIdentifierTypeDef(_RequiredTokenIdentifierTypeDef, _OptionalTokenIdentifierTypeDef):
     pass
 
 
 BlockchainInstantTypeDef = TypedDict(
     "BlockchainInstantTypeDef",
     {
         "time": Union[datetime, str],
     },
     total=False,
 )
 
-OwnerIdentifierTypeDef = TypedDict(
-    "OwnerIdentifierTypeDef",
-    {
-        "address": str,
-    },
-)
-
-_RequiredTokenIdentifierTypeDef = TypedDict(
-    "_RequiredTokenIdentifierTypeDef",
-    {
-        "network": QueryNetworkType,
-    },
-)
-_OptionalTokenIdentifierTypeDef = TypedDict(
-    "_OptionalTokenIdentifierTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "contractAddress": str,
-        "tokenId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class TokenIdentifierTypeDef(_RequiredTokenIdentifierTypeDef, _OptionalTokenIdentifierTypeDef):
-    pass
-
-
 GetTransactionInputRequestTypeDef = TypedDict(
     "GetTransactionInputRequestTypeDef",
     {
         "transactionHash": str,
         "network": QueryNetworkType,
     },
 )
@@ -188,14 +168,24 @@
 OwnerFilterTypeDef = TypedDict(
     "OwnerFilterTypeDef",
     {
         "address": str,
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 _RequiredTokenFilterTypeDef = TypedDict(
     "_RequiredTokenFilterTypeDef",
     {
         "network": QueryNetworkType,
     },
 )
 _OptionalTokenFilterTypeDef = TypedDict(
@@ -208,37 +198,14 @@
 )
 
 
 class TokenFilterTypeDef(_RequiredTokenFilterTypeDef, _OptionalTokenFilterTypeDef):
     pass
 
 
-_RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef = TypedDict(
-    "_RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef",
-    {
-        "transactionHash": str,
-        "network": QueryNetworkType,
-    },
-)
-_OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef = TypedDict(
-    "_OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTransactionEventsInputListTransactionEventsPaginateTypeDef(
-    _RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef,
-    _OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTransactionEventsInputRequestTypeDef = TypedDict(
     "_RequiredListTransactionEventsInputRequestTypeDef",
     {
         "transactionHash": str,
         "network": QueryNetworkType,
     },
 )
@@ -300,48 +267,27 @@
     {
         "transactionHash": str,
         "network": QueryNetworkType,
         "transactionTimestamp": datetime,
     },
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
 _RequiredBatchGetTokenBalanceErrorItemTypeDef = TypedDict(
     "_RequiredBatchGetTokenBalanceErrorItemTypeDef",
     {
         "errorCode": str,
         "errorMessage": str,
         "errorType": ErrorTypeType,
     },
 )
 _OptionalBatchGetTokenBalanceErrorItemTypeDef = TypedDict(
     "_OptionalBatchGetTokenBalanceErrorItemTypeDef",
     {
-        "tokenIdentifier": TokenIdentifierOutputTypeDef,
-        "ownerIdentifier": OwnerIdentifierOutputTypeDef,
+        "tokenIdentifier": TokenIdentifierTypeDef,
+        "ownerIdentifier": OwnerIdentifierTypeDef,
         "atBlockchainInstant": BlockchainInstantOutputTypeDef,
     },
     total=False,
 )
 
 
 class BatchGetTokenBalanceErrorItemTypeDef(
@@ -356,52 +302,40 @@
         "balance": str,
         "atBlockchainInstant": BlockchainInstantOutputTypeDef,
     },
 )
 _OptionalBatchGetTokenBalanceOutputItemTypeDef = TypedDict(
     "_OptionalBatchGetTokenBalanceOutputItemTypeDef",
     {
-        "ownerIdentifier": OwnerIdentifierOutputTypeDef,
-        "tokenIdentifier": TokenIdentifierOutputTypeDef,
+        "ownerIdentifier": OwnerIdentifierTypeDef,
+        "tokenIdentifier": TokenIdentifierTypeDef,
         "lastUpdatedTime": BlockchainInstantOutputTypeDef,
     },
     total=False,
 )
 
 
 class BatchGetTokenBalanceOutputItemTypeDef(
     _RequiredBatchGetTokenBalanceOutputItemTypeDef, _OptionalBatchGetTokenBalanceOutputItemTypeDef
 ):
     pass
 
 
-GetTokenBalanceOutputTypeDef = TypedDict(
-    "GetTokenBalanceOutputTypeDef",
-    {
-        "ownerIdentifier": OwnerIdentifierOutputTypeDef,
-        "tokenIdentifier": TokenIdentifierOutputTypeDef,
-        "balance": str,
-        "atBlockchainInstant": BlockchainInstantOutputTypeDef,
-        "lastUpdatedTime": BlockchainInstantOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTokenBalanceTypeDef = TypedDict(
     "_RequiredTokenBalanceTypeDef",
     {
         "balance": str,
         "atBlockchainInstant": BlockchainInstantOutputTypeDef,
     },
 )
 _OptionalTokenBalanceTypeDef = TypedDict(
     "_OptionalTokenBalanceTypeDef",
     {
-        "ownerIdentifier": OwnerIdentifierOutputTypeDef,
-        "tokenIdentifier": TokenIdentifierOutputTypeDef,
+        "ownerIdentifier": OwnerIdentifierTypeDef,
+        "tokenIdentifier": TokenIdentifierTypeDef,
         "lastUpdatedTime": BlockchainInstantOutputTypeDef,
     },
     total=False,
 )
 
 
 class TokenBalanceTypeDef(_RequiredTokenBalanceTypeDef, _OptionalTokenBalanceTypeDef):
@@ -448,33 +382,68 @@
 
 class GetTokenBalanceInputRequestTypeDef(
     _RequiredGetTokenBalanceInputRequestTypeDef, _OptionalGetTokenBalanceInputRequestTypeDef
 ):
     pass
 
 
+GetTokenBalanceOutputTypeDef = TypedDict(
+    "GetTokenBalanceOutputTypeDef",
+    {
+        "ownerIdentifier": OwnerIdentifierTypeDef,
+        "tokenIdentifier": TokenIdentifierTypeDef,
+        "balance": str,
+        "atBlockchainInstant": BlockchainInstantOutputTypeDef,
+        "lastUpdatedTime": BlockchainInstantOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetTransactionOutputTypeDef = TypedDict(
     "GetTransactionOutputTypeDef",
     {
         "transaction": TransactionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef = TypedDict(
+    "_RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef",
+    {
+        "transactionHash": str,
+        "network": QueryNetworkType,
+    },
+)
+_OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef = TypedDict(
+    "_OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTransactionEventsInputListTransactionEventsPaginateTypeDef(
+    _RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef,
+    _OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTokenBalancesInputListTokenBalancesPaginateTypeDef = TypedDict(
     "_RequiredListTokenBalancesInputListTokenBalancesPaginateTypeDef",
     {
         "tokenFilter": TokenFilterTypeDef,
     },
 )
 _OptionalListTokenBalancesInputListTokenBalancesPaginateTypeDef = TypedDict(
     "_OptionalListTokenBalancesInputListTokenBalancesPaginateTypeDef",
     {
         "ownerFilter": OwnerFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListTokenBalancesInputListTokenBalancesPaginateTypeDef(
     _RequiredListTokenBalancesInputListTokenBalancesPaginateTypeDef,
@@ -507,15 +476,15 @@
 
 
 ListTransactionEventsOutputTypeDef = TypedDict(
     "ListTransactionEventsOutputTypeDef",
     {
         "events": List[TransactionEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListTransactionsInputListTransactionsPaginateTypeDef = TypedDict(
     "_RequiredListTransactionsInputListTransactionsPaginateTypeDef",
     {
         "address": str,
@@ -524,15 +493,15 @@
 )
 _OptionalListTransactionsInputListTransactionsPaginateTypeDef = TypedDict(
     "_OptionalListTransactionsInputListTransactionsPaginateTypeDef",
     {
         "fromBlockchainInstant": BlockchainInstantTypeDef,
         "toBlockchainInstant": BlockchainInstantTypeDef,
         "sort": ListTransactionsSortTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListTransactionsInputListTransactionsPaginateTypeDef(
     _RequiredListTransactionsInputListTransactionsPaginateTypeDef,
@@ -568,33 +537,33 @@
 
 
 ListTransactionsOutputTypeDef = TypedDict(
     "ListTransactionsOutputTypeDef",
     {
         "transactions": List[TransactionOutputItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetTokenBalanceOutputTypeDef = TypedDict(
     "BatchGetTokenBalanceOutputTypeDef",
     {
         "tokenBalances": List[BatchGetTokenBalanceOutputItemTypeDef],
         "errors": List[BatchGetTokenBalanceErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTokenBalancesOutputTypeDef = TypedDict(
     "ListTokenBalancesOutputTypeDef",
     {
         "tokenBalances": List[TokenBalanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetTokenBalanceInputRequestTypeDef = TypedDict(
     "BatchGetTokenBalanceInputRequestTypeDef",
     {
         "getTokenBalanceInputs": Sequence[BatchGetTokenBalanceInputItemTypeDef],
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query/type_defs.pyi` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -30,37 +30,35 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BlockchainInstantOutputTypeDef",
-    "OwnerIdentifierOutputTypeDef",
-    "TokenIdentifierOutputTypeDef",
-    "BlockchainInstantTypeDef",
     "OwnerIdentifierTypeDef",
     "TokenIdentifierTypeDef",
+    "BlockchainInstantTypeDef",
+    "ResponseMetadataTypeDef",
     "GetTransactionInputRequestTypeDef",
     "TransactionTypeDef",
     "OwnerFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "TokenFilterTypeDef",
-    "ListTransactionEventsInputListTransactionEventsPaginateTypeDef",
     "ListTransactionEventsInputRequestTypeDef",
     "TransactionEventTypeDef",
     "ListTransactionsSortTypeDef",
     "TransactionOutputItemTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetTokenBalanceErrorItemTypeDef",
     "BatchGetTokenBalanceOutputItemTypeDef",
-    "GetTokenBalanceOutputTypeDef",
     "TokenBalanceTypeDef",
     "BatchGetTokenBalanceInputItemTypeDef",
     "GetTokenBalanceInputRequestTypeDef",
+    "GetTokenBalanceOutputTypeDef",
     "GetTransactionOutputTypeDef",
+    "ListTransactionEventsInputListTransactionEventsPaginateTypeDef",
     "ListTokenBalancesInputListTokenBalancesPaginateTypeDef",
     "ListTokenBalancesInputRequestTypeDef",
     "ListTransactionEventsOutputTypeDef",
     "ListTransactionsInputListTransactionsPaginateTypeDef",
     "ListTransactionsInputRequestTypeDef",
     "ListTransactionsOutputTypeDef",
     "BatchGetTokenBalanceOutputTypeDef",
@@ -72,74 +70,58 @@
     "BlockchainInstantOutputTypeDef",
     {
         "time": datetime,
     },
     total=False,
 )
 
-OwnerIdentifierOutputTypeDef = TypedDict(
-    "OwnerIdentifierOutputTypeDef",
+OwnerIdentifierTypeDef = TypedDict(
+    "OwnerIdentifierTypeDef",
     {
         "address": str,
     },
 )
 
-_RequiredTokenIdentifierOutputTypeDef = TypedDict(
-    "_RequiredTokenIdentifierOutputTypeDef",
+_RequiredTokenIdentifierTypeDef = TypedDict(
+    "_RequiredTokenIdentifierTypeDef",
     {
         "network": QueryNetworkType,
     },
 )
-_OptionalTokenIdentifierOutputTypeDef = TypedDict(
-    "_OptionalTokenIdentifierOutputTypeDef",
+_OptionalTokenIdentifierTypeDef = TypedDict(
+    "_OptionalTokenIdentifierTypeDef",
     {
         "contractAddress": str,
         "tokenId": str,
     },
     total=False,
 )
 
-class TokenIdentifierOutputTypeDef(
-    _RequiredTokenIdentifierOutputTypeDef, _OptionalTokenIdentifierOutputTypeDef
-):
+class TokenIdentifierTypeDef(_RequiredTokenIdentifierTypeDef, _OptionalTokenIdentifierTypeDef):
     pass
 
 BlockchainInstantTypeDef = TypedDict(
     "BlockchainInstantTypeDef",
     {
         "time": Union[datetime, str],
     },
     total=False,
 )
 
-OwnerIdentifierTypeDef = TypedDict(
-    "OwnerIdentifierTypeDef",
-    {
-        "address": str,
-    },
-)
-
-_RequiredTokenIdentifierTypeDef = TypedDict(
-    "_RequiredTokenIdentifierTypeDef",
-    {
-        "network": QueryNetworkType,
-    },
-)
-_OptionalTokenIdentifierTypeDef = TypedDict(
-    "_OptionalTokenIdentifierTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "contractAddress": str,
-        "tokenId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class TokenIdentifierTypeDef(_RequiredTokenIdentifierTypeDef, _OptionalTokenIdentifierTypeDef):
-    pass
-
 GetTransactionInputRequestTypeDef = TypedDict(
     "GetTransactionInputRequestTypeDef",
     {
         "transactionHash": str,
         "network": QueryNetworkType,
     },
 )
@@ -181,14 +163,24 @@
 OwnerFilterTypeDef = TypedDict(
     "OwnerFilterTypeDef",
     {
         "address": str,
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 _RequiredTokenFilterTypeDef = TypedDict(
     "_RequiredTokenFilterTypeDef",
     {
         "network": QueryNetworkType,
     },
 )
 _OptionalTokenFilterTypeDef = TypedDict(
@@ -199,35 +191,14 @@
     },
     total=False,
 )
 
 class TokenFilterTypeDef(_RequiredTokenFilterTypeDef, _OptionalTokenFilterTypeDef):
     pass
 
-_RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef = TypedDict(
-    "_RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef",
-    {
-        "transactionHash": str,
-        "network": QueryNetworkType,
-    },
-)
-_OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef = TypedDict(
-    "_OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTransactionEventsInputListTransactionEventsPaginateTypeDef(
-    _RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef,
-    _OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredListTransactionEventsInputRequestTypeDef = TypedDict(
     "_RequiredListTransactionEventsInputRequestTypeDef",
     {
         "transactionHash": str,
         "network": QueryNetworkType,
     },
 )
@@ -285,48 +256,27 @@
     {
         "transactionHash": str,
         "network": QueryNetworkType,
         "transactionTimestamp": datetime,
     },
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
 _RequiredBatchGetTokenBalanceErrorItemTypeDef = TypedDict(
     "_RequiredBatchGetTokenBalanceErrorItemTypeDef",
     {
         "errorCode": str,
         "errorMessage": str,
         "errorType": ErrorTypeType,
     },
 )
 _OptionalBatchGetTokenBalanceErrorItemTypeDef = TypedDict(
     "_OptionalBatchGetTokenBalanceErrorItemTypeDef",
     {
-        "tokenIdentifier": TokenIdentifierOutputTypeDef,
-        "ownerIdentifier": OwnerIdentifierOutputTypeDef,
+        "tokenIdentifier": TokenIdentifierTypeDef,
+        "ownerIdentifier": OwnerIdentifierTypeDef,
         "atBlockchainInstant": BlockchainInstantOutputTypeDef,
     },
     total=False,
 )
 
 class BatchGetTokenBalanceErrorItemTypeDef(
     _RequiredBatchGetTokenBalanceErrorItemTypeDef, _OptionalBatchGetTokenBalanceErrorItemTypeDef
@@ -339,50 +289,38 @@
         "balance": str,
         "atBlockchainInstant": BlockchainInstantOutputTypeDef,
     },
 )
 _OptionalBatchGetTokenBalanceOutputItemTypeDef = TypedDict(
     "_OptionalBatchGetTokenBalanceOutputItemTypeDef",
     {
-        "ownerIdentifier": OwnerIdentifierOutputTypeDef,
-        "tokenIdentifier": TokenIdentifierOutputTypeDef,
+        "ownerIdentifier": OwnerIdentifierTypeDef,
+        "tokenIdentifier": TokenIdentifierTypeDef,
         "lastUpdatedTime": BlockchainInstantOutputTypeDef,
     },
     total=False,
 )
 
 class BatchGetTokenBalanceOutputItemTypeDef(
     _RequiredBatchGetTokenBalanceOutputItemTypeDef, _OptionalBatchGetTokenBalanceOutputItemTypeDef
 ):
     pass
 
-GetTokenBalanceOutputTypeDef = TypedDict(
-    "GetTokenBalanceOutputTypeDef",
-    {
-        "ownerIdentifier": OwnerIdentifierOutputTypeDef,
-        "tokenIdentifier": TokenIdentifierOutputTypeDef,
-        "balance": str,
-        "atBlockchainInstant": BlockchainInstantOutputTypeDef,
-        "lastUpdatedTime": BlockchainInstantOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTokenBalanceTypeDef = TypedDict(
     "_RequiredTokenBalanceTypeDef",
     {
         "balance": str,
         "atBlockchainInstant": BlockchainInstantOutputTypeDef,
     },
 )
 _OptionalTokenBalanceTypeDef = TypedDict(
     "_OptionalTokenBalanceTypeDef",
     {
-        "ownerIdentifier": OwnerIdentifierOutputTypeDef,
-        "tokenIdentifier": TokenIdentifierOutputTypeDef,
+        "ownerIdentifier": OwnerIdentifierTypeDef,
+        "tokenIdentifier": TokenIdentifierTypeDef,
         "lastUpdatedTime": BlockchainInstantOutputTypeDef,
     },
     total=False,
 )
 
 class TokenBalanceTypeDef(_RequiredTokenBalanceTypeDef, _OptionalTokenBalanceTypeDef):
     pass
@@ -423,33 +361,66 @@
 )
 
 class GetTokenBalanceInputRequestTypeDef(
     _RequiredGetTokenBalanceInputRequestTypeDef, _OptionalGetTokenBalanceInputRequestTypeDef
 ):
     pass
 
+GetTokenBalanceOutputTypeDef = TypedDict(
+    "GetTokenBalanceOutputTypeDef",
+    {
+        "ownerIdentifier": OwnerIdentifierTypeDef,
+        "tokenIdentifier": TokenIdentifierTypeDef,
+        "balance": str,
+        "atBlockchainInstant": BlockchainInstantOutputTypeDef,
+        "lastUpdatedTime": BlockchainInstantOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetTransactionOutputTypeDef = TypedDict(
     "GetTransactionOutputTypeDef",
     {
         "transaction": TransactionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef = TypedDict(
+    "_RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef",
+    {
+        "transactionHash": str,
+        "network": QueryNetworkType,
+    },
+)
+_OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef = TypedDict(
+    "_OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTransactionEventsInputListTransactionEventsPaginateTypeDef(
+    _RequiredListTransactionEventsInputListTransactionEventsPaginateTypeDef,
+    _OptionalListTransactionEventsInputListTransactionEventsPaginateTypeDef,
+):
+    pass
+
 _RequiredListTokenBalancesInputListTokenBalancesPaginateTypeDef = TypedDict(
     "_RequiredListTokenBalancesInputListTokenBalancesPaginateTypeDef",
     {
         "tokenFilter": TokenFilterTypeDef,
     },
 )
 _OptionalListTokenBalancesInputListTokenBalancesPaginateTypeDef = TypedDict(
     "_OptionalListTokenBalancesInputListTokenBalancesPaginateTypeDef",
     {
         "ownerFilter": OwnerFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListTokenBalancesInputListTokenBalancesPaginateTypeDef(
     _RequiredListTokenBalancesInputListTokenBalancesPaginateTypeDef,
     _OptionalListTokenBalancesInputListTokenBalancesPaginateTypeDef,
@@ -478,15 +449,15 @@
     pass
 
 ListTransactionEventsOutputTypeDef = TypedDict(
     "ListTransactionEventsOutputTypeDef",
     {
         "events": List[TransactionEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListTransactionsInputListTransactionsPaginateTypeDef = TypedDict(
     "_RequiredListTransactionsInputListTransactionsPaginateTypeDef",
     {
         "address": str,
@@ -495,15 +466,15 @@
 )
 _OptionalListTransactionsInputListTransactionsPaginateTypeDef = TypedDict(
     "_OptionalListTransactionsInputListTransactionsPaginateTypeDef",
     {
         "fromBlockchainInstant": BlockchainInstantTypeDef,
         "toBlockchainInstant": BlockchainInstantTypeDef,
         "sort": ListTransactionsSortTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListTransactionsInputListTransactionsPaginateTypeDef(
     _RequiredListTransactionsInputListTransactionsPaginateTypeDef,
     _OptionalListTransactionsInputListTransactionsPaginateTypeDef,
@@ -535,33 +506,33 @@
     pass
 
 ListTransactionsOutputTypeDef = TypedDict(
     "ListTransactionsOutputTypeDef",
     {
         "transactions": List[TransactionOutputItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetTokenBalanceOutputTypeDef = TypedDict(
     "BatchGetTokenBalanceOutputTypeDef",
     {
         "tokenBalances": List[BatchGetTokenBalanceOutputItemTypeDef],
         "errors": List[BatchGetTokenBalanceErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTokenBalancesOutputTypeDef = TypedDict(
     "ListTokenBalancesOutputTypeDef",
     {
         "tokenBalances": List[TokenBalanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetTokenBalanceInputRequestTypeDef = TypedDict(
     "BatchGetTokenBalanceInputRequestTypeDef",
     {
         "getTokenBalanceInputs": Sequence[BatchGetTokenBalanceInputItemTypeDef],
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query.egg-info/PKG-INFO` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain-query
-Version: 1.28.12
-Summary: Type annotations for boto3.ManagedBlockchainQuery 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ManagedBlockchainQuery 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain-query)](https://pepy.tech/project/mypy-boto3-managedblockchain-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchainQuery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
+[boto3.ManagedBlockchainQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
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
 [mypy-boto3-managedblockchain-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,37 +338,35 @@
 
 `mypy_boto3_managedblockchain_query.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain_query.type_defs import (
     BlockchainInstantOutputTypeDef,
-    OwnerIdentifierOutputTypeDef,
-    TokenIdentifierOutputTypeDef,
-    BlockchainInstantTypeDef,
     OwnerIdentifierTypeDef,
     TokenIdentifierTypeDef,
+    BlockchainInstantTypeDef,
+    ResponseMetadataTypeDef,
     GetTransactionInputRequestTypeDef,
     TransactionTypeDef,
     OwnerFilterTypeDef,
+    PaginatorConfigTypeDef,
     TokenFilterTypeDef,
-    ListTransactionEventsInputListTransactionEventsPaginateTypeDef,
     ListTransactionEventsInputRequestTypeDef,
     TransactionEventTypeDef,
     ListTransactionsSortTypeDef,
     TransactionOutputItemTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetTokenBalanceErrorItemTypeDef,
     BatchGetTokenBalanceOutputItemTypeDef,
-    GetTokenBalanceOutputTypeDef,
     TokenBalanceTypeDef,
     BatchGetTokenBalanceInputItemTypeDef,
     GetTokenBalanceInputRequestTypeDef,
+    GetTokenBalanceOutputTypeDef,
     GetTransactionOutputTypeDef,
+    ListTransactionEventsInputListTransactionEventsPaginateTypeDef,
     ListTokenBalancesInputListTokenBalancesPaginateTypeDef,
     ListTokenBalancesInputRequestTypeDef,
     ListTransactionEventsOutputTypeDef,
     ListTransactionsInputListTransactionsPaginateTypeDef,
     ListTransactionsInputRequestTypeDef,
     ListTransactionsOutputTypeDef,
     BatchGetTokenBalanceOutputTypeDef,
```

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/mypy_boto3_managedblockchain_query.egg-info/SOURCES.txt` & `mypy-boto3-managedblockchain-query-1.28.15/mypy_boto3_managedblockchain_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-query-1.28.12/setup.py` & `mypy-boto3-managedblockchain-query-1.28.15/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-managedblockchain-query",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_managedblockchain_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedBlockchainQuery 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ManagedBlockchainQuery 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

