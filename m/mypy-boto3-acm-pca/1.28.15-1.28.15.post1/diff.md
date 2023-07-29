# Comparing `tmp/mypy-boto3-acm-pca-1.28.15.tar.gz` & `tmp/mypy-boto3-acm-pca-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-pca-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
+gzip compressed data, was "mypy-boto3-acm-pca-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:23 2023, max compression
```

## Comparing `mypy-boto3-acm-pca-1.28.15.tar` & `mypy-boto3-acm-pca-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.724609 mypy-boto3-acm-pca-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-07-28 20:42:12.716609 mypy-boto3-acm-pca-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.712609 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22345 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-07-28 20:18:41.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-28 20:18:41.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29584 2023-07-28 20:18:42.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29539 2023-07-28 20:18:41.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.712609 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.724609 mypy-boto3-acm-pca-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.940978 mypy-boto3-acm-pca-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-29 10:02:23.940978 mypy-boto3-acm-pca-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.924978 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22510 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22474 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-07-29 09:37:31.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-29 09:37:31.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29584 2023-07-29 09:37:32.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29539 2023-07-29 09:37:32.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.940978 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:23.940978 mypy-boto3-acm-pca-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-acm-pca-1.28.15/LICENSE` & `mypy-boto3-acm-pca-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/PKG-INFO` & `mypy-boto3-acm-pca-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.28.15
-Summary: Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-acm-pca-1.28.15/README.md` & `mypy-boto3-acm-pca-1.28.15.post1/README.md`

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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__init__.py` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__init__.pyi` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__main__.py` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACMPCA 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.ACMPCA 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\nOther"
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

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/client.py` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from .paginator import (
     ListCertificateAuthoritiesPaginator,
     ListPermissionsPaginator,
     ListTagsPaginator,
 )
 from .type_defs import (
     ApiPassthroughTypeDef,
+    CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
@@ -133,15 +134,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#close)
         """
 
     def create_certificate_authority(
         self,
         *,
-        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,
+        CertificateAuthorityConfiguration: Union[
+            CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationOutputTypeDef
+        ],
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UsageMode: CertificateAuthorityUsageModeType = ...
     ) -> CreateCertificateAuthorityResponseTypeDef:
```

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/client.pyi` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from .paginator import (
     ListCertificateAuthoritiesPaginator,
     ListPermissionsPaginator,
     ListTagsPaginator,
 )
 from .type_defs import (
     ApiPassthroughTypeDef,
+    CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
@@ -126,15 +127,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#close)
         """
     def create_certificate_authority(
         self,
         *,
-        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,
+        CertificateAuthorityConfiguration: Union[
+            CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationOutputTypeDef
+        ],
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UsageMode: CertificateAuthorityUsageModeType = ...
     ) -> CreateCertificateAuthorityResponseTypeDef:
```

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/literals.py` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/literals.pyi` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/paginator.py` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/paginator.pyi` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/type_defs.py` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/type_defs.pyi` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/waiter.py` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/waiter.pyi` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/PKG-INFO` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.28.15
-Summary: Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/SOURCES.txt` & `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15/setup.py` & `mypy-boto3-acm-pca-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm-pca",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_acm_pca"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

