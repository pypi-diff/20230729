# Comparing `tmp/mypy-boto3-license-manager-1.28.15.tar.gz` & `tmp/mypy-boto3-license-manager-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-1.28.15.tar", last modified: Fri Jul 28 20:43:08 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:32 2023, max compression
```

## Comparing `mypy-boto3-license-manager-1.28.15.tar` & `mypy-boto3-license-manager-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.965387 mypy-boto3-license-manager-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20362 2023-07-28 20:43:08.965387 mypy-boto3-license-manager-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18844 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.957387 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 20:30:06.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40707 2023-07-28 20:30:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-28 20:30:06.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-28 20:30:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-07-28 20:30:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-28 20:30:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-28 20:30:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:06.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56131 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56058 2023-07-28 20:30:09.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.965387 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20362 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:08.965387 mypy-boto3-license-manager-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-28 20:30:05.000000 mypy-boto3-license-manager-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:32.189242 mypy-boto3-license-manager-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-07-29 10:03:32.189242 mypy-boto3-license-manager-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18844 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:32.181242 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40977 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40915 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56262 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56189 2023-07-29 09:49:46.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:32.189242 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:32.189242 mypy-boto3-license-manager-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-29 09:49:44.000000 mypy-boto3-license-manager-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-license-manager-1.28.15/LICENSE` & `mypy-boto3-license-manager-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15/PKG-INFO` & `mypy-boto3-license-manager-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager
-Version: 1.28.15
-Summary: Type annotations for boto3.LicenseManager 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LicenseManager 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-license-manager-1.28.15/README.md` & `mypy-boto3-license-manager-1.28.15.post1/README.md`

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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__init__.py` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__init__.pyi` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/__main__.py` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManager 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.LicenseManager 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager\nOther"
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

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/client.py` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_license_manager.client import LicenseManagerClient
 
     session = Session()
     client: LicenseManagerClient = session.client("license-manager")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AllowedOperationType,
     CheckoutTypeType,
     GrantStatusType,
@@ -82,16 +82,18 @@
     ListResourceInventoryResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTokensResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     MetadataTypeDef,
     OptionsTypeDef,
     OrganizationConfigurationTypeDef,
+    ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
     RejectGrantResponseTypeDef,
+    ReportContextOutputTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -282,15 +284,17 @@
         LicenseCountingType: LicenseCountingTypeType,
         Description: str = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         LicenseRules: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...,
-        ProductInformationList: Sequence[ProductInformationTypeDef] = ...
+        ProductInformationList: Sequence[
+            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
+        ] = ...
     ) -> CreateLicenseConfigurationResponseTypeDef:
         """
         Creates a license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#create_license_configuration)
         """
@@ -310,15 +314,15 @@
         """
 
     def create_license_manager_report_generator(
         self,
         *,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextTypeDef,
+        ReportContext: Union[ReportContextTypeDef, ReportContextOutputTypeDef],
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateLicenseManagerReportGeneratorResponseTypeDef:
         """
         Creates a report generator.
@@ -751,15 +755,17 @@
         LicenseConfigurationArn: str,
         LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,
         LicenseRules: Sequence[str] = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         Name: str = ...,
         Description: str = ...,
-        ProductInformationList: Sequence[ProductInformationTypeDef] = ...,
+        ProductInformationList: Sequence[
+            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
+        ] = ...,
         DisassociateWhenNotFound: bool = ...
     ) -> Dict[str, Any]:
         """
         Modifies the attributes of an existing license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#update_license_configuration)
@@ -767,15 +773,15 @@
 
     def update_license_manager_report_generator(
         self,
         *,
         LicenseManagerReportGeneratorArn: str,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextTypeDef,
+        ReportContext: Union[ReportContextTypeDef, ReportContextOutputTypeDef],
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a report generator.
```

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/client.pyi` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_license_manager.client import LicenseManagerClient
 
     session = Session()
     client: LicenseManagerClient = session.client("license-manager")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AllowedOperationType,
     CheckoutTypeType,
     GrantStatusType,
@@ -82,16 +82,18 @@
     ListResourceInventoryResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTokensResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     MetadataTypeDef,
     OptionsTypeDef,
     OrganizationConfigurationTypeDef,
+    ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
     RejectGrantResponseTypeDef,
+    ReportContextOutputTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -268,15 +270,17 @@
         LicenseCountingType: LicenseCountingTypeType,
         Description: str = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         LicenseRules: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...,
-        ProductInformationList: Sequence[ProductInformationTypeDef] = ...
+        ProductInformationList: Sequence[
+            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
+        ] = ...
     ) -> CreateLicenseConfigurationResponseTypeDef:
         """
         Creates a license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#create_license_configuration)
         """
@@ -294,15 +298,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#create_license_conversion_task_for_resource)
         """
     def create_license_manager_report_generator(
         self,
         *,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextTypeDef,
+        ReportContext: Union[ReportContextTypeDef, ReportContextOutputTypeDef],
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateLicenseManagerReportGeneratorResponseTypeDef:
         """
         Creates a report generator.
@@ -697,30 +701,32 @@
         LicenseConfigurationArn: str,
         LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,
         LicenseRules: Sequence[str] = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         Name: str = ...,
         Description: str = ...,
-        ProductInformationList: Sequence[ProductInformationTypeDef] = ...,
+        ProductInformationList: Sequence[
+            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
+        ] = ...,
         DisassociateWhenNotFound: bool = ...
     ) -> Dict[str, Any]:
         """
         Modifies the attributes of an existing license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#update_license_configuration)
         """
     def update_license_manager_report_generator(
         self,
         *,
         LicenseManagerReportGeneratorArn: str,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextTypeDef,
+        ReportContext: Union[ReportContextTypeDef, ReportContextOutputTypeDef],
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a report generator.
```

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/literals.py` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/literals.pyi` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/paginator.py` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/paginator.pyi` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/type_defs.py` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_license_manager.type_defs import AcceptGrantRequestRequestTypeDef
 
     data: AcceptGrantRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     EntitlementDataUnitType,
     EntitlementUnitType,
@@ -1934,15 +1934,17 @@
     {
         "Description": str,
         "LicenseCount": int,
         "LicenseCountHardLimit": bool,
         "LicenseRules": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "DisassociateWhenNotFound": bool,
-        "ProductInformationList": Sequence[ProductInformationTypeDef],
+        "ProductInformationList": Sequence[
+            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class CreateLicenseConfigurationRequestRequestTypeDef(
     _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
@@ -1962,15 +1964,17 @@
     {
         "LicenseConfigurationStatus": LicenseConfigurationStatusType,
         "LicenseRules": Sequence[str],
         "LicenseCount": int,
         "LicenseCountHardLimit": bool,
         "Name": str,
         "Description": str,
-        "ProductInformationList": Sequence[ProductInformationTypeDef],
+        "ProductInformationList": Sequence[
+            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
+        ],
         "DisassociateWhenNotFound": bool,
     },
     total=False,
 )
 
 
 class UpdateLicenseConfigurationRequestRequestTypeDef(
```

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager/type_defs.pyi` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_license_manager.type_defs import AcceptGrantRequestRequestTypeDef
 
     data: AcceptGrantRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     EntitlementDataUnitType,
     EntitlementUnitType,
@@ -1865,15 +1865,17 @@
     {
         "Description": str,
         "LicenseCount": int,
         "LicenseCountHardLimit": bool,
         "LicenseRules": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "DisassociateWhenNotFound": bool,
-        "ProductInformationList": Sequence[ProductInformationTypeDef],
+        "ProductInformationList": Sequence[
+            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class CreateLicenseConfigurationRequestRequestTypeDef(
     _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
     _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
@@ -1891,15 +1893,17 @@
     {
         "LicenseConfigurationStatus": LicenseConfigurationStatusType,
         "LicenseRules": Sequence[str],
         "LicenseCount": int,
         "LicenseCountHardLimit": bool,
         "Name": str,
         "Description": str,
-        "ProductInformationList": Sequence[ProductInformationTypeDef],
+        "ProductInformationList": Sequence[
+            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
+        ],
         "DisassociateWhenNotFound": bool,
     },
     total=False,
 )
 
 class UpdateLicenseConfigurationRequestRequestTypeDef(
     _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/PKG-INFO` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager
-Version: 1.28.15
-Summary: Type annotations for boto3.LicenseManager 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LicenseManager 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-license-manager-1.28.15/mypy_boto3_license_manager.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15/setup.py` & `mypy-boto3-license-manager-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_license_manager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.LicenseManager 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

