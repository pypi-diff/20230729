# Comparing `tmp/mypy-boto3-inspector2-1.28.15.tar.gz` & `tmp/mypy-boto3-inspector2-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector2-1.28.15.tar", last modified: Fri Jul 28 20:42:56 2023, max compression
+gzip compressed data, was "mypy-boto3-inspector2-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:16 2023, max compression
```

## Comparing `mypy-boto3-inspector2-1.28.15.tar` & `mypy-boto3-inspector2-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.377214 mypy-boto3-inspector2-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23307 2023-07-28 20:42:56.377214 mypy-boto3-inspector2-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.365214 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35728 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-07-28 20:27:47.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-28 20:27:47.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75649 2023-07-28 20:27:50.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75568 2023-07-28 20:27:48.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.377214 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23307 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:56.000000 mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:56.377214 mypy-boto3-inspector2-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:27:46.000000 mypy-boto3-inspector2-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.689174 mypy-boto3-inspector2-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-29 10:03:16.689174 mypy-boto3-inspector2-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.681174 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36019 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35957 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-29 09:47:20.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75649 2023-07-29 09:47:22.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75568 2023-07-29 09:47:21.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:18.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.689174 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:16.000000 mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:16.689174 mypy-boto3-inspector2-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:47:17.000000 mypy-boto3-inspector2-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-inspector2-1.28.15/LICENSE` & `mypy-boto3-inspector2-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15/PKG-INFO` & `mypy-boto3-inspector2-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.28.15
-Summary: Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-inspector2-1.28.15/README.md` & `mypy-boto3-inspector2-1.28.15.post1/README.md`

 * *Files 1% similar despite different names*

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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__init__.py` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__init__.pyi` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/__main__.py` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector2 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Inspector2 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\nOther"
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

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/client.py` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_inspector2.client import Inspector2Client
 
     session = Session()
     client: Inspector2Client = session.client("inspector2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AggregationTypeType,
     FilterActionType,
     GroupKeyType,
@@ -61,14 +61,15 @@
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     GetMemberResponseTypeDef,
@@ -80,14 +81,15 @@
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
+    ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
     UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateFilterResponseTypeDef,
@@ -235,15 +237,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#close)
         """
 
     def create_filter(
         self,
         *,
         action: FilterActionType,
-        filterCriteria: FilterCriteriaTypeDef,
+        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef],
         name: str,
         description: str = ...,
         reason: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
@@ -253,29 +255,31 @@
         """
 
     def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: FilterCriteriaTypeDef = ...
+        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_findings_report)
         """
 
     def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...
+        resourceFilterCriteria: Union[
+            ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
+        ] = ...
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_sbom_export)
         """
@@ -512,15 +516,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_finding_aggregations)
         """
 
     def list_findings(
         self,
         *,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
@@ -624,15 +628,15 @@
 
     def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         name: str = ...,
         reason: str = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
```

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/client.pyi` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_inspector2.client import Inspector2Client
 
     session = Session()
     client: Inspector2Client = session.client("inspector2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AggregationTypeType,
     FilterActionType,
     GroupKeyType,
@@ -61,14 +61,15 @@
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     GetMemberResponseTypeDef,
@@ -80,14 +81,15 @@
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
+    ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
     UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateFilterResponseTypeDef,
@@ -220,15 +222,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#close)
         """
     def create_filter(
         self,
         *,
         action: FilterActionType,
-        filterCriteria: FilterCriteriaTypeDef,
+        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef],
         name: str,
         description: str = ...,
         reason: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
@@ -237,28 +239,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_filter)
         """
     def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: FilterCriteriaTypeDef = ...
+        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_findings_report)
         """
     def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...
+        resourceFilterCriteria: Union[
+            ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
+        ] = ...
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_sbom_export)
         """
@@ -473,15 +477,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_finding_aggregations)
         """
     def list_findings(
         self,
         *,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
@@ -574,15 +578,15 @@
         """
     def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         name: str = ...,
         reason: str = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
```

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/literals.py` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/literals.pyi` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/paginator.py` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,22 +33,23 @@
     list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
     search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator("search_vulnerabilities")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AggregationTypeType, FilterActionType, GroupKeyType, ServiceType
 from .type_defs import (
     AggregationRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
@@ -197,15 +198,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/paginator.pyi` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -33,22 +33,23 @@
     list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
     search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator("search_vulnerabilities")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AggregationTypeType, FilterActionType, GroupKeyType, ServiceType
 from .type_defs import (
     AggregationRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
@@ -188,15 +189,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/type_defs.py` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2/type_defs.pyi` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/PKG-INFO` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.28.15
-Summary: Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-inspector2-1.28.15/mypy_boto3_inspector2.egg-info/SOURCES.txt` & `mypy-boto3-inspector2-1.28.15.post1/mypy_boto3_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.15/setup.py` & `mypy-boto3-inspector2-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector2",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Inspector2 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

