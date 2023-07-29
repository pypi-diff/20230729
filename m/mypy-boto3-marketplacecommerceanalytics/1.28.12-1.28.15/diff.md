# Comparing `tmp/mypy-boto3-marketplacecommerceanalytics-1.28.12.tar.gz` & `tmp/mypy-boto3-marketplacecommerceanalytics-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-marketplacecommerceanalytics-1.28.12.tar", last modified: Thu Jul 27 05:35:00 2023, max compression
+gzip compressed data, was "mypy-boto3-marketplacecommerceanalytics-1.28.15.tar", last modified: Fri Jul 28 20:43:14 2023, max compression
```

## Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12.tar` & `mypy-boto3-marketplacecommerceanalytics-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.040445 mypy-boto3-marketplacecommerceanalytics-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-07-27 05:35:00.040445 mypy-boto3-marketplacecommerceanalytics-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.036445 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.040445 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-07-27 05:34:59.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-27 05:34:59.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:59.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 05:34:59.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:00.040445 mypy-boto3-marketplacecommerceanalytics-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-27 05:25:53.000000 mypy-boto3-marketplacecommerceanalytics-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.933469 mypy-boto3-marketplacecommerceanalytics-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:56.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-07-28 20:43:14.933469 mypy-boto3-marketplacecommerceanalytics-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-07-28 20:30:56.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.925469 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-28 20:30:56.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-28 20:30:56.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-28 20:30:57.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-28 20:30:57.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-28 20:30:57.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-28 20:30:57.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-07-28 20:30:57.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:57.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-28 20:30:59.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-28 20:30:57.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:56.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.933469 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-07-28 20:43:14.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-28 20:43:14.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:14.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:14.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:14.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 20:43:14.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:14.933469 mypy-boto3-marketplacecommerceanalytics-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-28 20:30:56.000000 mypy-boto3-marketplacecommerceanalytics-1.28.15/setup.py
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/LICENSE` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/PKG-INFO` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplacecommerceanalytics
-Version: 1.28.12
-Summary: Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplacecommerceanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplacecommerceanalytics)](https://pepy.tech/project/mypy-boto3-marketplacecommerceanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCommerceAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
+[boto3.MarketplaceCommerceAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
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
 [mypy-boto3-marketplacecommerceanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,17 +300,17 @@
 
 `mypy_boto3_marketplacecommerceanalytics.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplacecommerceanalytics.type_defs import (
     GenerateDataSetRequestRequestTypeDef,
-    GenerateDataSetResultTypeDef,
     ResponseMetadataTypeDef,
     StartSupportDataExportRequestRequestTypeDef,
+    GenerateDataSetResultTypeDef,
     StartSupportDataExportResultTypeDef,
 )
 
 
 def get_structure() -> GenerateDataSetRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/README.md` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplacecommerceanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplacecommerceanalytics)](https://pepy.tech/project/mypy-boto3-marketplacecommerceanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCommerceAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
+[boto3.MarketplaceCommerceAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
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
 [mypy-boto3-marketplacecommerceanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -268,17 +268,17 @@
 
 `mypy_boto3_marketplacecommerceanalytics.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplacecommerceanalytics.type_defs import (
     GenerateDataSetRequestRequestTypeDef,
-    GenerateDataSetResultTypeDef,
     ResponseMetadataTypeDef,
     StartSupportDataExportRequestRequestTypeDef,
+    GenerateDataSetResultTypeDef,
     StartSupportDataExportResultTypeDef,
 )
 
 
 def get_structure() -> GenerateDataSetRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/__init__.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/__init__.pyi` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/__main__.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics\nOther"
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

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/client.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/client.pyi` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/literals.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/literals.pyi` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/type_defs.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,19 @@
 from .literals import DataSetTypeType, SupportDataSetTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "GenerateDataSetRequestRequestTypeDef",
-    "GenerateDataSetResultTypeDef",
     "ResponseMetadataTypeDef",
     "StartSupportDataExportRequestRequestTypeDef",
+    "GenerateDataSetResultTypeDef",
     "StartSupportDataExportResultTypeDef",
 )
 
 _RequiredGenerateDataSetRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataSetRequestRequestTypeDef",
     {
         "dataSetType": DataSetTypeType,
@@ -46,29 +45,19 @@
     {
         "destinationS3Prefix": str,
         "customerDefinedValues": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GenerateDataSetRequestRequestTypeDef(
     _RequiredGenerateDataSetRequestRequestTypeDef, _OptionalGenerateDataSetRequestRequestTypeDef
 ):
     pass
 
-
-GenerateDataSetResultTypeDef = TypedDict(
-    "GenerateDataSetResultTypeDef",
-    {
-        "dataSetRequestId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -91,22 +80,28 @@
     {
         "destinationS3Prefix": str,
         "customerDefinedValues": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartSupportDataExportRequestRequestTypeDef(
     _RequiredStartSupportDataExportRequestRequestTypeDef,
     _OptionalStartSupportDataExportRequestRequestTypeDef,
 ):
     pass
 
+GenerateDataSetResultTypeDef = TypedDict(
+    "GenerateDataSetResultTypeDef",
+    {
+        "dataSetRequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 StartSupportDataExportResultTypeDef = TypedDict(
     "StartSupportDataExportResultTypeDef",
     {
         "dataSetRequestId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics/type_defs.pyi` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 from .literals import DataSetTypeType, SupportDataSetTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "GenerateDataSetRequestRequestTypeDef",
-    "GenerateDataSetResultTypeDef",
     "ResponseMetadataTypeDef",
     "StartSupportDataExportRequestRequestTypeDef",
+    "GenerateDataSetResultTypeDef",
     "StartSupportDataExportResultTypeDef",
 )
 
 _RequiredGenerateDataSetRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataSetRequestRequestTypeDef",
     {
         "dataSetType": DataSetTypeType,
@@ -45,26 +46,20 @@
     {
         "destinationS3Prefix": str,
         "customerDefinedValues": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GenerateDataSetRequestRequestTypeDef(
     _RequiredGenerateDataSetRequestRequestTypeDef, _OptionalGenerateDataSetRequestRequestTypeDef
 ):
     pass
 
-GenerateDataSetResultTypeDef = TypedDict(
-    "GenerateDataSetResultTypeDef",
-    {
-        "dataSetRequestId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
@@ -88,20 +83,30 @@
     {
         "destinationS3Prefix": str,
         "customerDefinedValues": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartSupportDataExportRequestRequestTypeDef(
     _RequiredStartSupportDataExportRequestRequestTypeDef,
     _OptionalStartSupportDataExportRequestRequestTypeDef,
 ):
     pass
 
+
+GenerateDataSetResultTypeDef = TypedDict(
+    "GenerateDataSetResultTypeDef",
+    {
+        "dataSetRequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartSupportDataExportResultTypeDef = TypedDict(
     "StartSupportDataExportResultTypeDef",
     {
         "dataSetRequestId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics.egg-info/PKG-INFO` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplacecommerceanalytics
-Version: 1.28.12
-Summary: Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplacecommerceanalytics.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplacecommerceanalytics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-marketplacecommerceanalytics)](https://pepy.tech/project/mypy-boto3-marketplacecommerceanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCommerceAnalytics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
+[boto3.MarketplaceCommerceAnalytics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics)
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
 [mypy-boto3-marketplacecommerceanalytics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplacecommerceanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,17 +300,17 @@
 
 `mypy_boto3_marketplacecommerceanalytics.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplacecommerceanalytics.type_defs import (
     GenerateDataSetRequestRequestTypeDef,
-    GenerateDataSetResultTypeDef,
     ResponseMetadataTypeDef,
     StartSupportDataExportRequestRequestTypeDef,
+    GenerateDataSetResultTypeDef,
     StartSupportDataExportResultTypeDef,
 )
 
 
 def get_structure() -> GenerateDataSetRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/mypy_boto3_marketplacecommerceanalytics.egg-info/SOURCES.txt` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/mypy_boto3_marketplacecommerceanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-marketplacecommerceanalytics-1.28.12/setup.py` & `mypy-boto3-marketplacecommerceanalytics-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-marketplacecommerceanalytics",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_marketplacecommerceanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MarketplaceCommerceAnalytics 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

