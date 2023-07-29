# Comparing `tmp/mypy-boto3-codeguru-security-1.28.15.tar.gz` & `tmp/mypy-boto3-codeguru-security-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguru-security-1.28.15.tar", last modified: Fri Jul 28 20:42:28 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguru-security-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-codeguru-security-1.28.15.tar` & `mypy-boto3-codeguru-security-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.684826 mypy-boto3-codeguru-security-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-28 20:42:28.684826 mypy-boto3-codeguru-security-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.684826 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-28 20:21:36.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-07-28 20:21:36.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-07-28 20:21:36.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-07-28 20:21:36.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.684826 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:28.000000 mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:28.684826 mypy-boto3-codeguru-security-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 20:21:35.000000 mypy-boto3-codeguru-security-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.754719 mypy-boto3-codeguru-security-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-18 19:32:41.754719 mypy-boto3-codeguru-security-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.754719 mypy-boto3-codeguru-security-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/setup.py
```

### Comparing `mypy-boto3-codeguru-security-1.28.15/LICENSE` & `mypy-boto3-codeguru-security-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.15/PKG-INFO` & `mypy-boto3-codeguru-security-1.28.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-security
-Version: 1.28.15
-Summary: Type annotations for boto3.CodeGuruSecurity 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.5
+Summary: Type annotations for boto3.CodeGuruSecurity 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,15 +342,17 @@
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
     ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
+    ResourceIdOutputTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
     PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
     ListFindingsMetricsRequestRequestTypeDef,
@@ -367,16 +369,16 @@
     CreateUploadUrlResponseTypeDef,
     GetScanResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
+    UpdateAccountConfigurationRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.28.15/README.md` & `mypy-boto3-codeguru-security-1.28.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,15 +310,17 @@
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
     ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
+    ResourceIdOutputTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
     PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
     ListFindingsMetricsRequestRequestTypeDef,
@@ -335,16 +337,16 @@
     CreateUploadUrlResponseTypeDef,
     GetScanResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
+    UpdateAccountConfigurationRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/__init__.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/__init__.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/__main__.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruSecurity 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.CodeGuruSecurity 1.28.5\nVersion:         1.28.5\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/client.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/client.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/literals.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AnalysisTypeType",
     "ErrorCodeType",
     "GetFindingsPaginatorName",
     "ListFindingsMetricsPaginatorName",
     "ListScansPaginatorName",
     "ScanStateType",
@@ -31,15 +30,14 @@
     "StatusType",
     "CodeGuruSecurityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AnalysisTypeType = Literal["All", "Security"]
 ErrorCodeType = Literal[
     "DUPLICATE_IDENTIFIER",
     "INTERNAL_ERROR",
     "INVALID_FINDING_ID",
     "INVALID_SCAN_NAME",
     "ITEM_DOES_NOT_EXIST",
@@ -167,15 +165,14 @@
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
@@ -254,28 +251,26 @@
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

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/literals.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AnalysisTypeType",
     "ErrorCodeType",
     "GetFindingsPaginatorName",
     "ListFindingsMetricsPaginatorName",
     "ListScansPaginatorName",
     "ScanStateType",
@@ -30,14 +31,15 @@
     "StatusType",
     "CodeGuruSecurityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 AnalysisTypeType = Literal["All", "Security"]
 ErrorCodeType = Literal[
     "DUPLICATE_IDENTIFIER",
     "INTERNAL_ERROR",
     "INVALID_FINDING_ID",
     "INVALID_SCAN_NAME",
     "ITEM_DOES_NOT_EXIST",
@@ -165,15 +167,14 @@
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
@@ -252,28 +253,26 @@
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

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/paginator.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/paginator.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/type_defs.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,25 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
     "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
     "ResourceIdTypeDef",
+    "ResourceIdOutputTypeDef",
     "CreateUploadUrlRequestRequestTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "ResourceTypeDef",
     "PaginatorConfigTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "GetMetricsSummaryRequestRequestTypeDef",
     "GetScanRequestRequestTypeDef",
     "ListFindingsMetricsRequestRequestTypeDef",
@@ -59,16 +60,16 @@
     "CreateUploadUrlResponseTypeDef",
     "GetScanResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "FilePathTypeDef",
     "CreateScanRequestRequestTypeDef",
     "CreateScanResponseTypeDef",
     "GetAccountConfigurationResponseTypeDef",
-    "UpdateAccountConfigurationRequestRequestTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
+    "UpdateAccountConfigurationRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     "ListScansRequestListScansPaginateTypeDef",
     "ListScansResponseTypeDef",
     "MetricsSummaryTypeDef",
     "RemediationTypeDef",
     "ListFindingsMetricsResponseTypeDef",
@@ -84,15 +85,14 @@
     {
         "critical": float,
         "high": float,
         "info": float,
         "low": float,
         "medium": float,
     },
-    total=False,
 )
 
 BatchGetFindingsErrorTypeDef = TypedDict(
     "BatchGetFindingsErrorTypeDef",
     {
         "errorCode": ErrorCodeType,
         "findingId": str,
@@ -122,56 +122,67 @@
 
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": str,
         "findingNumber": int,
     },
-    total=False,
 )
 
 CodeLineTypeDef = TypedDict(
     "CodeLineTypeDef",
     {
         "content": str,
         "number": int,
     },
-    total=False,
 )
 
 ResourceIdTypeDef = TypedDict(
     "ResourceIdTypeDef",
     {
         "codeArtifactId": str,
     },
     total=False,
 )
 
+ResourceIdOutputTypeDef = TypedDict(
+    "ResourceIdOutputTypeDef",
+    {
+        "codeArtifactId": str,
+    },
+)
+
 CreateUploadUrlRequestRequestTypeDef = TypedDict(
     "CreateUploadUrlRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
+    {
+        "kmsKeyArn": str,
+    },
+)
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "id": str,
         "subResourceId": str,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -192,21 +203,19 @@
         "maxResults": int,
         "nextToken": str,
         "status": StatusType,
     },
     total=False,
 )
 
-
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
-
 GetMetricsSummaryRequestRequestTypeDef = TypedDict(
     "GetMetricsSummaryRequestRequestTypeDef",
     {
         "date": Union[datetime, str],
     },
 )
 
@@ -220,21 +229,19 @@
     "_OptionalGetScanRequestRequestTypeDef",
     {
         "runId": str,
     },
     total=False,
 )
 
-
 class GetScanRequestRequestTypeDef(
     _RequiredGetScanRequestRequestTypeDef, _OptionalGetScanRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsMetricsRequestRequestTypeDef",
     {
         "endDate": Union[datetime, str],
         "startDate": Union[datetime, str],
     },
 )
@@ -243,86 +250,70 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListFindingsMetricsRequestRequestTypeDef(
     _RequiredListFindingsMetricsRequestRequestTypeDef,
     _OptionalListFindingsMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 ListScansRequestRequestTypeDef = TypedDict(
     "ListScansRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredScanSummaryTypeDef = TypedDict(
-    "_RequiredScanSummaryTypeDef",
+ScanSummaryTypeDef = TypedDict(
+    "ScanSummaryTypeDef",
     {
         "createdAt": datetime,
         "runId": str,
         "scanName": str,
-        "scanState": ScanStateType,
-    },
-)
-_OptionalScanSummaryTypeDef = TypedDict(
-    "_OptionalScanSummaryTypeDef",
-    {
         "scanNameArn": str,
+        "scanState": ScanStateType,
         "updatedAt": datetime,
     },
-    total=False,
 )
 
-
-class ScanSummaryTypeDef(_RequiredScanSummaryTypeDef, _OptionalScanSummaryTypeDef):
-    pass
-
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
 ScanNameWithFindingNumTypeDef = TypedDict(
     "ScanNameWithFindingNumTypeDef",
     {
         "findingNumber": int,
         "scanName": str,
     },
-    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
-    total=False,
 )
 
 SuggestedFixTypeDef = TypedDict(
     "SuggestedFixTypeDef",
     {
         "code": str,
         "description": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -342,15 +333,14 @@
     {
         "closedFindings": FindingMetricsValuePerSeverityTypeDef,
         "date": datetime,
         "meanTimeToClose": FindingMetricsValuePerSeverityTypeDef,
         "newFindings": FindingMetricsValuePerSeverityTypeDef,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsRequestRequestTypeDef = TypedDict(
     "BatchGetFindingsRequestRequestTypeDef",
     {
         "findingIdentifiers": Sequence[FindingIdentifierTypeDef],
     },
@@ -394,15 +384,14 @@
     {
         "codeSnippet": List[CodeLineTypeDef],
         "endLine": int,
         "name": str,
         "path": str,
         "startLine": int,
     },
-    total=False,
 )
 
 _RequiredCreateScanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScanRequestRequestTypeDef",
     {
         "resourceId": ResourceIdTypeDef,
         "scanName": str,
@@ -415,53 +404,51 @@
         "clientToken": str,
         "scanType": ScanTypeType,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateScanRequestRequestTypeDef(
     _RequiredCreateScanRequestRequestTypeDef, _OptionalCreateScanRequestRequestTypeDef
 ):
     pass
 
-
 CreateScanResponseTypeDef = TypedDict(
     "CreateScanResponseTypeDef",
     {
-        "resourceId": ResourceIdTypeDef,
+        "resourceId": ResourceIdOutputTypeDef,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
-        "encryptionConfig": EncryptionConfigTypeDef,
+        "encryptionConfig": EncryptionConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateAccountConfigurationRequestRequestTypeDef",
+UpdateAccountConfigurationResponseTypeDef = TypedDict(
+    "UpdateAccountConfigurationResponseTypeDef",
     {
-        "encryptionConfig": EncryptionConfigTypeDef,
+        "encryptionConfig": EncryptionConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccountConfigurationResponseTypeDef = TypedDict(
-    "UpdateAccountConfigurationResponseTypeDef",
+UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
     "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
     {
         "scanName": str,
@@ -472,22 +459,20 @@
     {
         "status": StatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetFindingsRequestGetFindingsPaginateTypeDef(
     _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
     _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
     "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     {
         "endDate": Union[datetime, str],
         "startDate": Union[datetime, str],
     },
 )
@@ -495,22 +480,20 @@
     "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
     _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
 ):
     pass
 
-
 ListScansRequestListScansPaginateTypeDef = TypedDict(
     "ListScansRequestListScansPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -529,24 +512,22 @@
     {
         "categoriesWithMostFindings": List[CategoryWithFindingNumTypeDef],
         "date": datetime,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
         "scansWithMostOpenCriticalFindings": List[ScanNameWithFindingNumTypeDef],
         "scansWithMostOpenFindings": List[ScanNameWithFindingNumTypeDef],
     },
-    total=False,
 )
 
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
         "suggestedFixes": List[SuggestedFixTypeDef],
     },
-    total=False,
 )
 
 ListFindingsMetricsResponseTypeDef = TypedDict(
     "ListFindingsMetricsResponseTypeDef",
     {
         "findingsMetrics": List[AccountFindingsMetricTypeDef],
         "nextToken": str,
@@ -559,15 +540,14 @@
     {
         "filePath": FilePathTypeDef,
         "id": str,
         "itemCount": int,
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
     },
-    total=False,
 )
 
 GetMetricsSummaryResponseTypeDef = TypedDict(
     "GetMetricsSummaryResponseTypeDef",
     {
         "metricsSummary": MetricsSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -590,15 +570,14 @@
         "severity": SeverityType,
         "status": StatusType,
         "title": str,
         "type": str,
         "updatedAt": datetime,
         "vulnerability": VulnerabilityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsResponseTypeDef = TypedDict(
     "BatchGetFindingsResponseTypeDef",
     {
         "failedFindings": List[BatchGetFindingsErrorTypeDef],
         "findings": List[FindingTypeDef],
```

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security/type_defs.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,23 +25,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
     "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
     "ResourceIdTypeDef",
+    "ResourceIdOutputTypeDef",
     "CreateUploadUrlRequestRequestTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "ResourceTypeDef",
     "PaginatorConfigTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "GetMetricsSummaryRequestRequestTypeDef",
     "GetScanRequestRequestTypeDef",
     "ListFindingsMetricsRequestRequestTypeDef",
@@ -58,16 +61,16 @@
     "CreateUploadUrlResponseTypeDef",
     "GetScanResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "FilePathTypeDef",
     "CreateScanRequestRequestTypeDef",
     "CreateScanResponseTypeDef",
     "GetAccountConfigurationResponseTypeDef",
-    "UpdateAccountConfigurationRequestRequestTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
+    "UpdateAccountConfigurationRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     "ListScansRequestListScansPaginateTypeDef",
     "ListScansResponseTypeDef",
     "MetricsSummaryTypeDef",
     "RemediationTypeDef",
     "ListFindingsMetricsResponseTypeDef",
@@ -83,15 +86,14 @@
     {
         "critical": float,
         "high": float,
         "info": float,
         "low": float,
         "medium": float,
     },
-    total=False,
 )
 
 BatchGetFindingsErrorTypeDef = TypedDict(
     "BatchGetFindingsErrorTypeDef",
     {
         "errorCode": ErrorCodeType,
         "findingId": str,
@@ -121,56 +123,67 @@
 
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": str,
         "findingNumber": int,
     },
-    total=False,
 )
 
 CodeLineTypeDef = TypedDict(
     "CodeLineTypeDef",
     {
         "content": str,
         "number": int,
     },
-    total=False,
 )
 
 ResourceIdTypeDef = TypedDict(
     "ResourceIdTypeDef",
     {
         "codeArtifactId": str,
     },
     total=False,
 )
 
+ResourceIdOutputTypeDef = TypedDict(
+    "ResourceIdOutputTypeDef",
+    {
+        "codeArtifactId": str,
+    },
+)
+
 CreateUploadUrlRequestRequestTypeDef = TypedDict(
     "CreateUploadUrlRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
+    {
+        "kmsKeyArn": str,
+    },
+)
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "id": str,
         "subResourceId": str,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -191,19 +204,21 @@
         "maxResults": int,
         "nextToken": str,
         "status": StatusType,
     },
     total=False,
 )
 
+
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
+
 GetMetricsSummaryRequestRequestTypeDef = TypedDict(
     "GetMetricsSummaryRequestRequestTypeDef",
     {
         "date": Union[datetime, str],
     },
 )
 
@@ -217,19 +232,21 @@
     "_OptionalGetScanRequestRequestTypeDef",
     {
         "runId": str,
     },
     total=False,
 )
 
+
 class GetScanRequestRequestTypeDef(
     _RequiredGetScanRequestRequestTypeDef, _OptionalGetScanRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsMetricsRequestRequestTypeDef",
     {
         "endDate": Union[datetime, str],
         "startDate": Union[datetime, str],
     },
 )
@@ -238,82 +255,72 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListFindingsMetricsRequestRequestTypeDef(
     _RequiredListFindingsMetricsRequestRequestTypeDef,
     _OptionalListFindingsMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 ListScansRequestRequestTypeDef = TypedDict(
     "ListScansRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredScanSummaryTypeDef = TypedDict(
-    "_RequiredScanSummaryTypeDef",
+ScanSummaryTypeDef = TypedDict(
+    "ScanSummaryTypeDef",
     {
         "createdAt": datetime,
         "runId": str,
         "scanName": str,
-        "scanState": ScanStateType,
-    },
-)
-_OptionalScanSummaryTypeDef = TypedDict(
-    "_OptionalScanSummaryTypeDef",
-    {
         "scanNameArn": str,
+        "scanState": ScanStateType,
         "updatedAt": datetime,
     },
-    total=False,
 )
 
-class ScanSummaryTypeDef(_RequiredScanSummaryTypeDef, _OptionalScanSummaryTypeDef):
-    pass
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
 ScanNameWithFindingNumTypeDef = TypedDict(
     "ScanNameWithFindingNumTypeDef",
     {
         "findingNumber": int,
         "scanName": str,
     },
-    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
-    total=False,
 )
 
 SuggestedFixTypeDef = TypedDict(
     "SuggestedFixTypeDef",
     {
         "code": str,
         "description": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -333,15 +340,14 @@
     {
         "closedFindings": FindingMetricsValuePerSeverityTypeDef,
         "date": datetime,
         "meanTimeToClose": FindingMetricsValuePerSeverityTypeDef,
         "newFindings": FindingMetricsValuePerSeverityTypeDef,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsRequestRequestTypeDef = TypedDict(
     "BatchGetFindingsRequestRequestTypeDef",
     {
         "findingIdentifiers": Sequence[FindingIdentifierTypeDef],
     },
@@ -385,15 +391,14 @@
     {
         "codeSnippet": List[CodeLineTypeDef],
         "endLine": int,
         "name": str,
         "path": str,
         "startLine": int,
     },
-    total=False,
 )
 
 _RequiredCreateScanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScanRequestRequestTypeDef",
     {
         "resourceId": ResourceIdTypeDef,
         "scanName": str,
@@ -406,51 +411,53 @@
         "clientToken": str,
         "scanType": ScanTypeType,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateScanRequestRequestTypeDef(
     _RequiredCreateScanRequestRequestTypeDef, _OptionalCreateScanRequestRequestTypeDef
 ):
     pass
 
+
 CreateScanResponseTypeDef = TypedDict(
     "CreateScanResponseTypeDef",
     {
-        "resourceId": ResourceIdTypeDef,
+        "resourceId": ResourceIdOutputTypeDef,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
-        "encryptionConfig": EncryptionConfigTypeDef,
+        "encryptionConfig": EncryptionConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateAccountConfigurationRequestRequestTypeDef",
+UpdateAccountConfigurationResponseTypeDef = TypedDict(
+    "UpdateAccountConfigurationResponseTypeDef",
     {
-        "encryptionConfig": EncryptionConfigTypeDef,
+        "encryptionConfig": EncryptionConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccountConfigurationResponseTypeDef = TypedDict(
-    "UpdateAccountConfigurationResponseTypeDef",
+UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
     "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
     {
         "scanName": str,
@@ -461,20 +468,22 @@
     {
         "status": StatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetFindingsRequestGetFindingsPaginateTypeDef(
     _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
     _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
     "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     {
         "endDate": Union[datetime, str],
         "startDate": Union[datetime, str],
     },
 )
@@ -482,20 +491,22 @@
     "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
     _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
 ):
     pass
 
+
 ListScansRequestListScansPaginateTypeDef = TypedDict(
     "ListScansRequestListScansPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -514,24 +525,22 @@
     {
         "categoriesWithMostFindings": List[CategoryWithFindingNumTypeDef],
         "date": datetime,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
         "scansWithMostOpenCriticalFindings": List[ScanNameWithFindingNumTypeDef],
         "scansWithMostOpenFindings": List[ScanNameWithFindingNumTypeDef],
     },
-    total=False,
 )
 
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
         "suggestedFixes": List[SuggestedFixTypeDef],
     },
-    total=False,
 )
 
 ListFindingsMetricsResponseTypeDef = TypedDict(
     "ListFindingsMetricsResponseTypeDef",
     {
         "findingsMetrics": List[AccountFindingsMetricTypeDef],
         "nextToken": str,
@@ -544,15 +553,14 @@
     {
         "filePath": FilePathTypeDef,
         "id": str,
         "itemCount": int,
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
     },
-    total=False,
 )
 
 GetMetricsSummaryResponseTypeDef = TypedDict(
     "GetMetricsSummaryResponseTypeDef",
     {
         "metricsSummary": MetricsSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -575,15 +583,14 @@
         "severity": SeverityType,
         "status": StatusType,
         "title": str,
         "type": str,
         "updatedAt": datetime,
         "vulnerability": VulnerabilityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsResponseTypeDef = TypedDict(
     "BatchGetFindingsResponseTypeDef",
     {
         "failedFindings": List[BatchGetFindingsErrorTypeDef],
         "findings": List[FindingTypeDef],
```

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security.egg-info/PKG-INFO` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-security
-Version: 1.28.15
-Summary: Type annotations for boto3.CodeGuruSecurity 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.5
+Summary: Type annotations for boto3.CodeGuruSecurity 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,15 +342,17 @@
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
     ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
+    ResourceIdOutputTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
     PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
     ListFindingsMetricsRequestRequestTypeDef,
@@ -367,16 +369,16 @@
     CreateUploadUrlResponseTypeDef,
     GetScanResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
+    UpdateAccountConfigurationRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.28.15/mypy_boto3_codeguru_security.egg-info/SOURCES.txt` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.15/setup.py` & `mypy-boto3-codeguru-security-1.28.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguru-security",
-    version="1.28.15",
+    version="1.28.5",
     packages=["mypy_boto3_codeguru_security"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruSecurity 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.CodeGuruSecurity 1.28.5 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

