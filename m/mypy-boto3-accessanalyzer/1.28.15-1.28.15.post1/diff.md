# Comparing `tmp/mypy-boto3-accessanalyzer-1.28.15.tar.gz` & `tmp/mypy-boto3-accessanalyzer-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-accessanalyzer-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
+gzip compressed data, was "mypy-boto3-accessanalyzer-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:24 2023, max compression
```

## Comparing `mypy-boto3-accessanalyzer-1.28.15.tar` & `mypy-boto3-accessanalyzer-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.660609 mypy-boto3-accessanalyzer-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-07-28 20:42:12.660609 mypy-boto3-accessanalyzer-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.660609 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24705 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-07-28 20:18:36.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47242 2023-07-28 20:18:37.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47161 2023-07-28 20:18:36.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.660609 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.660609 mypy-boto3-accessanalyzer-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.036978 mypy-boto3-accessanalyzer-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19378 2023-07-29 10:02:24.024978 mypy-boto3-accessanalyzer-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.012978 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24974 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-07-29 09:37:25.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47463 2023-07-29 09:37:27.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47382 2023-07-29 09:37:26.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.024978 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19378 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:02:23.000000 mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:24.036978 mypy-boto3-accessanalyzer-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:37:24.000000 mypy-boto3-accessanalyzer-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15/LICENSE` & `mypy-boto3-accessanalyzer-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15/PKG-INFO` & `mypy-boto3-accessanalyzer-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-accessanalyzer
-Version: 1.28.15
-Summary: Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15/README.md` & `mypy-boto3-accessanalyzer-1.28.15.post1/README.md`

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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__init__.py` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__init__.pyi` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__main__.py` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AccessAnalyzer 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.AccessAnalyzer 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer\nOther"
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

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/client.py` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_accessanalyzer.client import AccessAnalyzerClient
 
     session = Session()
     client: AccessAnalyzerClient = session.client("accessanalyzer")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     FindingStatusUpdateType,
     LocaleType,
     PolicyTypeType,
@@ -34,17 +34,19 @@
     ListArchiveRulesPaginator,
     ListFindingsPaginator,
     ListPolicyGenerationsPaginator,
     ValidatePolicyPaginator,
 )
 from .type_defs import (
     CloudTrailDetailsTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
+    CriterionOutputTypeDef,
     CriterionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccessPreviewResponseTypeDef,
     GetAnalyzedResourceResponseTypeDef,
     GetAnalyzerResponseTypeDef,
     GetArchiveRuleResponseTypeDef,
     GetFindingResponseTypeDef,
@@ -144,15 +146,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#close)
         """
 
     def create_access_preview(
         self,
         *,
         analyzerArn: str,
-        configurations: Mapping[str, ConfigurationTypeDef],
+        configurations: Mapping[str, Union[ConfigurationTypeDef, ConfigurationOutputTypeDef]],
         clientToken: str = ...
     ) -> CreateAccessPreviewResponseTypeDef:
         """
         Creates an access preview that allows you to preview IAM Access Analyzer
         findings for your resource before deploying resource permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_access_preview)
@@ -176,15 +178,15 @@
         """
 
     def create_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
-        filter: Mapping[str, CriterionTypeDef],
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates an archive rule for the specified analyzer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_archive_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#create_archive_rule)
@@ -285,15 +287,15 @@
         """
 
     def list_access_preview_findings(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
-        filter: Mapping[str, CriterionTypeDef] = ...,
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListAccessPreviewFindingsResponseTypeDef:
         """
         Retrieves a list of access preview findings generated by the specified access
         preview.
 
@@ -347,15 +349,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#list_archive_rules)
         """
 
     def list_findings(
         self,
         *,
         analyzerArn: str,
-        filter: Mapping[str, CriterionTypeDef] = ...,
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
         sort: SortCriteriaTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a list of findings generated by the specified analyzer.
 
@@ -422,15 +424,15 @@
         """
 
     def update_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
-        filter: Mapping[str, CriterionTypeDef],
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the criteria and values for the specified archive rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.update_archive_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#update_archive_rule)
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/client.pyi` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_accessanalyzer.client import AccessAnalyzerClient
 
     session = Session()
     client: AccessAnalyzerClient = session.client("accessanalyzer")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     FindingStatusUpdateType,
     LocaleType,
     PolicyTypeType,
@@ -34,17 +34,19 @@
     ListArchiveRulesPaginator,
     ListFindingsPaginator,
     ListPolicyGenerationsPaginator,
     ValidatePolicyPaginator,
 )
 from .type_defs import (
     CloudTrailDetailsTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
+    CriterionOutputTypeDef,
     CriterionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccessPreviewResponseTypeDef,
     GetAnalyzedResourceResponseTypeDef,
     GetAnalyzerResponseTypeDef,
     GetArchiveRuleResponseTypeDef,
     GetFindingResponseTypeDef,
@@ -135,15 +137,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#close)
         """
     def create_access_preview(
         self,
         *,
         analyzerArn: str,
-        configurations: Mapping[str, ConfigurationTypeDef],
+        configurations: Mapping[str, Union[ConfigurationTypeDef, ConfigurationOutputTypeDef]],
         clientToken: str = ...
     ) -> CreateAccessPreviewResponseTypeDef:
         """
         Creates an access preview that allows you to preview IAM Access Analyzer
         findings for your resource before deploying resource permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_access_preview)
@@ -165,15 +167,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#create_analyzer)
         """
     def create_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
-        filter: Mapping[str, CriterionTypeDef],
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates an archive rule for the specified analyzer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.create_archive_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#create_archive_rule)
@@ -264,15 +266,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#get_generated_policy)
         """
     def list_access_preview_findings(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
-        filter: Mapping[str, CriterionTypeDef] = ...,
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListAccessPreviewFindingsResponseTypeDef:
         """
         Retrieves a list of access preview findings generated by the specified access
         preview.
 
@@ -321,15 +323,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.list_archive_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#list_archive_rules)
         """
     def list_findings(
         self,
         *,
         analyzerArn: str,
-        filter: Mapping[str, CriterionTypeDef] = ...,
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
         sort: SortCriteriaTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a list of findings generated by the specified analyzer.
 
@@ -389,15 +391,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#untag_resource)
         """
     def update_archive_rule(
         self,
         *,
         analyzerName: str,
         ruleName: str,
-        filter: Mapping[str, CriterionTypeDef],
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the criteria and values for the specified archive rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.update_archive_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#update_archive_rule)
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/literals.py` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/literals.pyi` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/paginator.py` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,26 +29,27 @@
     list_analyzers_paginator: ListAnalyzersPaginator = client.get_paginator("list_analyzers")
     list_archive_rules_paginator: ListArchiveRulesPaginator = client.get_paginator("list_archive_rules")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_policy_generations_paginator: ListPolicyGenerationsPaginator = client.get_paginator("list_policy_generations")
     validate_policy_paginator: ValidatePolicyPaginator = client.get_paginator("validate_policy")
     ```
 """
-from typing import Generic, Iterator, Mapping, TypeVar
+from typing import Generic, Iterator, Mapping, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     LocaleType,
     PolicyTypeType,
     ResourceTypeType,
     TypeType,
     ValidatePolicyResourceTypeType,
 )
 from .type_defs import (
+    CriterionOutputTypeDef,
     CriterionTypeDef,
     ListAccessPreviewFindingsResponseTypeDef,
     ListAccessPreviewsResponseTypeDef,
     ListAnalyzedResourcesResponseTypeDef,
     ListAnalyzersResponseTypeDef,
     ListArchiveRulesResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -87,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
-        filter: Mapping[str, CriterionTypeDef] = ...,
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPreviewFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviewFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listaccesspreviewfindingspaginator)
         """
 
@@ -170,15 +171,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         analyzerArn: str,
-        filter: Mapping[str, CriterionTypeDef] = ...,
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
         sort: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/paginator.pyi` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,27 @@
     list_analyzers_paginator: ListAnalyzersPaginator = client.get_paginator("list_analyzers")
     list_archive_rules_paginator: ListArchiveRulesPaginator = client.get_paginator("list_archive_rules")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_policy_generations_paginator: ListPolicyGenerationsPaginator = client.get_paginator("list_policy_generations")
     validate_policy_paginator: ValidatePolicyPaginator = client.get_paginator("validate_policy")
     ```
 """
-from typing import Generic, Iterator, Mapping, TypeVar
+from typing import Generic, Iterator, Mapping, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     LocaleType,
     PolicyTypeType,
     ResourceTypeType,
     TypeType,
     ValidatePolicyResourceTypeType,
 )
 from .type_defs import (
+    CriterionOutputTypeDef,
     CriterionTypeDef,
     ListAccessPreviewFindingsResponseTypeDef,
     ListAccessPreviewsResponseTypeDef,
     ListAnalyzedResourcesResponseTypeDef,
     ListAnalyzersResponseTypeDef,
     ListArchiveRulesResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -84,15 +85,15 @@
     """
 
     def paginate(
         self,
         *,
         accessPreviewId: str,
         analyzerArn: str,
-        filter: Mapping[str, CriterionTypeDef] = ...,
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPreviewFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviewFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listaccesspreviewfindingspaginator)
         """
 
@@ -162,15 +163,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         analyzerArn: str,
-        filter: Mapping[str, CriterionTypeDef] = ...,
+        filter: Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]] = ...,
         sort: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/type_defs.py` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1001,15 +1001,15 @@
 )
 
 _RequiredCreateArchiveRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateArchiveRuleRequestRequestTypeDef",
     {
         "analyzerName": str,
         "ruleName": str,
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
     },
 )
 _OptionalCreateArchiveRuleRequestRequestTypeDef = TypedDict(
     "_OptionalCreateArchiveRuleRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -1037,15 +1037,15 @@
         "accessPreviewId": str,
         "analyzerArn": str,
     },
 )
 _OptionalListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalListAccessPreviewFindingsRequestRequestTypeDef",
     {
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
 
@@ -1057,15 +1057,15 @@
 
 
 _RequiredUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateArchiveRuleRequestRequestTypeDef",
     {
         "analyzerName": str,
         "ruleName": str,
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
     },
 )
 _OptionalUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateArchiveRuleRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -1174,15 +1174,15 @@
         "accessPreviewId": str,
         "analyzerArn": str,
     },
 )
 _OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef = TypedDict(
     "_OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
     {
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef(
@@ -1307,15 +1307,15 @@
     {
         "analyzerArn": str,
     },
 )
 _OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
     {
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         "sort": SortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
@@ -1331,15 +1331,15 @@
     {
         "analyzerArn": str,
     },
 )
 _OptionalListFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalListFindingsRequestRequestTypeDef",
     {
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         "sort": SortCriteriaTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
@@ -1843,15 +1843,15 @@
     pass
 
 
 _RequiredCreateAccessPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPreviewRequestRequestTypeDef",
     {
         "analyzerArn": str,
-        "configurations": Mapping[str, ConfigurationTypeDef],
+        "configurations": Mapping[str, Union[ConfigurationTypeDef, ConfigurationOutputTypeDef]],
     },
 )
 _OptionalCreateAccessPreviewRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAccessPreviewRequestRequestTypeDef",
     {
         "clientToken": str,
     },
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/type_defs.pyi` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -966,15 +966,15 @@
 )
 
 _RequiredCreateArchiveRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateArchiveRuleRequestRequestTypeDef",
     {
         "analyzerName": str,
         "ruleName": str,
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
     },
 )
 _OptionalCreateArchiveRuleRequestRequestTypeDef = TypedDict(
     "_OptionalCreateArchiveRuleRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -1000,15 +1000,15 @@
         "accessPreviewId": str,
         "analyzerArn": str,
     },
 )
 _OptionalListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalListAccessPreviewFindingsRequestRequestTypeDef",
     {
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
 class ListAccessPreviewFindingsRequestRequestTypeDef(
@@ -1018,15 +1018,15 @@
     pass
 
 _RequiredUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateArchiveRuleRequestRequestTypeDef",
     {
         "analyzerName": str,
         "ruleName": str,
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
     },
 )
 _OptionalUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateArchiveRuleRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -1125,15 +1125,15 @@
         "accessPreviewId": str,
         "analyzerArn": str,
     },
 )
 _OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef = TypedDict(
     "_OptionalListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
     {
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef(
     _RequiredListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
@@ -1248,15 +1248,15 @@
     {
         "analyzerArn": str,
     },
 )
 _OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
     {
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         "sort": SortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListFindingsRequestListFindingsPaginateTypeDef(
@@ -1270,15 +1270,15 @@
     {
         "analyzerArn": str,
     },
 )
 _OptionalListFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalListFindingsRequestRequestTypeDef",
     {
-        "filter": Mapping[str, CriterionTypeDef],
+        "filter": Mapping[str, Union[CriterionTypeDef, CriterionOutputTypeDef]],
         "sort": SortCriteriaTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
@@ -1764,15 +1764,15 @@
 class AccessPreviewTypeDef(_RequiredAccessPreviewTypeDef, _OptionalAccessPreviewTypeDef):
     pass
 
 _RequiredCreateAccessPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPreviewRequestRequestTypeDef",
     {
         "analyzerArn": str,
-        "configurations": Mapping[str, ConfigurationTypeDef],
+        "configurations": Mapping[str, Union[ConfigurationTypeDef, ConfigurationOutputTypeDef]],
     },
 )
 _OptionalCreateAccessPreviewRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAccessPreviewRequestRequestTypeDef",
     {
         "clientToken": str,
     },
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/PKG-INFO` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-accessanalyzer
-Version: 1.28.15
-Summary: Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt` & `mypy-boto3-accessanalyzer-1.28.15.post1/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.15/setup.py` & `mypy-boto3-accessanalyzer-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-accessanalyzer",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_accessanalyzer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with"
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

