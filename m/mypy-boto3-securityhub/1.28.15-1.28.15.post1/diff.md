# Comparing `tmp/mypy-boto3-securityhub-1.28.15.tar.gz` & `tmp/mypy-boto3-securityhub-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securityhub-1.28.15.tar", last modified: Fri Jul 28 20:43:42 2023, max compression
+gzip compressed data, was "mypy-boto3-securityhub-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:09 2023, max compression
```

## Comparing `mypy-boto3-securityhub-1.28.15.tar` & `mypy-boto3-securityhub-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:42.957853 mypy-boto3-securityhub-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:38:48.000000 mypy-boto3-securityhub-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    61539 2023-07-28 20:43:42.957853 mypy-boto3-securityhub-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    60036 2023-07-28 20:38:48.000000 mypy-boto3-securityhub-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:42.953853 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-28 20:38:48.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   402725 2023-07-28 20:39:03.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   402652 2023-07-28 20:38:58.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:38:48.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:42.957853 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    61539 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:42.957853 mypy-boto3-securityhub-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:38:48.000000 mypy-boto3-securityhub-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:09.333392 mypy-boto3-securityhub-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    61545 2023-07-29 10:04:09.329392 mypy-boto3-securityhub-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    60036 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:09.325392 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52477 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52388 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18429 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-07-29 09:58:58.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   402830 2023-07-29 09:59:13.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   402757 2023-07-29 09:59:03.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:09.329392 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    61545 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:04:09.000000 mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:09.333392 mypy-boto3-securityhub-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:58:57.000000 mypy-boto3-securityhub-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-securityhub-1.28.15/LICENSE` & `mypy-boto3-securityhub-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15/PKG-INFO` & `mypy-boto3-securityhub-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.28.15
-Summary: Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-securityhub-1.28.15/README.md` & `mypy-boto3-securityhub-1.28.15.post1/README.md`

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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__init__.py` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__init__.pyi` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__main__.py` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityHub 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.SecurityHub 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\nOther"
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

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/client.py` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,22 @@
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
     ListSecurityControlDefinitionsPaginator,
     ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
+    AutomationRulesActionOutputTypeDef,
     AutomationRulesActionTypeDef,
+    AutomationRulesFindingFiltersOutputTypeDef,
     AutomationRulesFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersOutputTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
+    AwsSecurityFindingOutputTypeDef,
     AwsSecurityFindingTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
@@ -234,15 +238,17 @@
         is currently enabled or disabled in a standard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_standards_control_associations)
         """
 
     def batch_import_findings(
-        self, *, Findings: Sequence[AwsSecurityFindingTypeDef]
+        self,
+        *,
+        Findings: Sequence[Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]]
     ) -> BatchImportFindingsResponseTypeDef:
         """
         Imports security findings generated by a finding provider into Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_import_findings)
         """
@@ -323,16 +329,18 @@
 
     def create_automation_rule(
         self,
         *,
         RuleOrder: int,
         RuleName: str,
         Description: str,
-        Criteria: AutomationRulesFindingFiltersTypeDef,
-        Actions: Sequence[AutomationRulesActionTypeDef],
+        Criteria: Union[
+            AutomationRulesFindingFiltersTypeDef, AutomationRulesFindingFiltersOutputTypeDef
+        ],
+        Actions: Sequence[Union[AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef]],
         Tags: Mapping[str, str] = ...,
         RuleStatus: RuleStatusType = ...,
         IsTerminal: bool = ...
     ) -> CreateAutomationRuleResponseTypeDef:
         """
         Creates an automation rule based on input parameters.
 
@@ -347,15 +355,19 @@
         Used to enable finding aggregation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_finding_aggregator)
         """
 
     def create_insight(
-        self, *, Name: str, Filters: AwsSecurityFindingFiltersTypeDef, GroupByAttribute: str
+        self,
+        *,
+        Name: str,
+        Filters: Union[AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef],
+        GroupByAttribute: str
     ) -> CreateInsightResponseTypeDef:
         """
         Creates a custom insight in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_insight)
         """
@@ -626,15 +638,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_history)
         """
 
     def get_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: Union[
+            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
+        ] = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of findings that match the specified criteria.
 
@@ -823,15 +837,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_finding_aggregator)
         """
 
     def update_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef,
+        Filters: Union[AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef],
         Note: NoteUpdateTypeDef = ...,
         RecordState: RecordStateType = ...
     ) -> Dict[str, Any]:
         """
         `UpdateFindings` is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)
@@ -839,15 +853,17 @@
         """
 
     def update_insight(
         self,
         *,
         InsightArn: str,
         Name: str = ...,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: Union[
+            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
+        ] = ...,
         GroupByAttribute: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the Security Hub insight identified by the specified insight ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_insight)
```

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/client.pyi` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,22 @@
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
     ListSecurityControlDefinitionsPaginator,
     ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
+    AutomationRulesActionOutputTypeDef,
     AutomationRulesActionTypeDef,
+    AutomationRulesFindingFiltersOutputTypeDef,
     AutomationRulesFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersOutputTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
+    AwsSecurityFindingOutputTypeDef,
     AwsSecurityFindingTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
@@ -221,15 +225,17 @@
         For a batch of security controls and standards, identifies whether each control
         is currently enabled or disabled in a standard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_standards_control_associations)
         """
     def batch_import_findings(
-        self, *, Findings: Sequence[AwsSecurityFindingTypeDef]
+        self,
+        *,
+        Findings: Sequence[Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]]
     ) -> BatchImportFindingsResponseTypeDef:
         """
         Imports security findings generated by a finding provider into Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_import_findings)
         """
@@ -303,16 +309,18 @@
         """
     def create_automation_rule(
         self,
         *,
         RuleOrder: int,
         RuleName: str,
         Description: str,
-        Criteria: AutomationRulesFindingFiltersTypeDef,
-        Actions: Sequence[AutomationRulesActionTypeDef],
+        Criteria: Union[
+            AutomationRulesFindingFiltersTypeDef, AutomationRulesFindingFiltersOutputTypeDef
+        ],
+        Actions: Sequence[Union[AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef]],
         Tags: Mapping[str, str] = ...,
         RuleStatus: RuleStatusType = ...,
         IsTerminal: bool = ...
     ) -> CreateAutomationRuleResponseTypeDef:
         """
         Creates an automation rule based on input parameters.
 
@@ -325,15 +333,19 @@
         """
         Used to enable finding aggregation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_finding_aggregator)
         """
     def create_insight(
-        self, *, Name: str, Filters: AwsSecurityFindingFiltersTypeDef, GroupByAttribute: str
+        self,
+        *,
+        Name: str,
+        Filters: Union[AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef],
+        GroupByAttribute: str
     ) -> CreateInsightResponseTypeDef:
         """
         Creates a custom insight in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_insight)
         """
@@ -576,15 +588,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_history)
         """
     def get_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: Union[
+            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
+        ] = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of findings that match the specified criteria.
 
@@ -753,30 +767,32 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_finding_aggregator)
         """
     def update_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef,
+        Filters: Union[AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef],
         Note: NoteUpdateTypeDef = ...,
         RecordState: RecordStateType = ...
     ) -> Dict[str, Any]:
         """
         `UpdateFindings` is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_findings)
         """
     def update_insight(
         self,
         *,
         InsightArn: str,
         Name: str = ...,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: Union[
+            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
+        ] = ...,
         GroupByAttribute: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the Security Hub insight identified by the specified insight ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_insight)
```

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/literals.py` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/literals.pyi` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/paginator.py` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 """
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
+    AwsSecurityFindingFiltersOutputTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
@@ -209,15 +210,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: Union[
+            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
+        ] = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
         """
```

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/paginator.pyi` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 """
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
+    AwsSecurityFindingFiltersOutputTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
@@ -200,15 +201,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: Union[
+            AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
+        ] = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
         """
```

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/type_defs.py` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -11764,15 +11764,17 @@
 _RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutomationRuleRequestRequestTypeDef",
     {
         "RuleOrder": int,
         "RuleName": str,
         "Description": str,
         "Criteria": AutomationRulesFindingFiltersTypeDef,
-        "Actions": Sequence[AutomationRulesActionTypeDef],
+        "Actions": Sequence[
+            Union[AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef]
+        ],
     },
 )
 _OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAutomationRuleRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
         "RuleStatus": RuleStatusType,
@@ -12961,10 +12963,10 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchImportFindingsRequestRequestTypeDef = TypedDict(
     "BatchImportFindingsRequestRequestTypeDef",
     {
-        "Findings": Sequence[AwsSecurityFindingTypeDef],
+        "Findings": Sequence[Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]],
     },
 )
```

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/type_defs.pyi` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11707,15 +11707,17 @@
 _RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutomationRuleRequestRequestTypeDef",
     {
         "RuleOrder": int,
         "RuleName": str,
         "Description": str,
         "Criteria": AutomationRulesFindingFiltersTypeDef,
-        "Actions": Sequence[AutomationRulesActionTypeDef],
+        "Actions": Sequence[
+            Union[AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef]
+        ],
     },
 )
 _OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAutomationRuleRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
         "RuleStatus": RuleStatusType,
@@ -12888,10 +12890,10 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchImportFindingsRequestRequestTypeDef = TypedDict(
     "BatchImportFindingsRequestRequestTypeDef",
     {
-        "Findings": Sequence[AwsSecurityFindingTypeDef],
+        "Findings": Sequence[Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]],
     },
 )
```

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/PKG-INFO` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.28.15
-Summary: Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/SOURCES.txt` & `mypy-boto3-securityhub-1.28.15.post1/mypy_boto3_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.15/setup.py` & `mypy-boto3-securityhub-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securityhub",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder"
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

