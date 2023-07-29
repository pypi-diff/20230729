# Comparing `tmp/mypy-boto3-ce-1.28.15.tar.gz` & `tmp/mypy-boto3-ce-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ce-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
+gzip compressed data, was "mypy-boto3-ce-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:37 2023, max compression
```

## Comparing `mypy-boto3-ce-1.28.15.tar` & `mypy-boto3-ce-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.344738 mypy-boto3-ce-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-28 20:42:22.344738 mypy-boto3-ce-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.344738 mypy-boto3-ce-1.28.15/mypy_boto3_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32603 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68658 2023-07-28 20:20:24.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68585 2023-07-28 20:20:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.344738 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.344738 mypy-boto3-ce-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.969035 mypy-boto3-ce-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-07-29 10:02:37.965036 mypy-boto3-ce-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.961035 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33450 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33405 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68807 2023-07-29 09:39:16.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68734 2023-07-29 09:39:15.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.965036 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 10:02:37.000000 mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:37.969035 mypy-boto3-ce-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:39:13.000000 mypy-boto3-ce-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-ce-1.28.15/LICENSE` & `mypy-boto3-ce-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.15/PKG-INFO` & `mypy-boto3-ce-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.28.15
-Summary: Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ce-1.28.15/README.md` & `mypy-boto3-ce-1.28.15.post1/README.md`

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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ce-1.28.15/mypy_boto3_ce/__main__.py` & `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostExplorer 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.CostExplorer 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
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

### Comparing `mypy-boto3-ce-1.28.15/mypy_boto3_ce/client.py` & `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/client.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ce.client import CostExplorerClient
 
     session = Session()
     client: CostExplorerClient = session.client("ce")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccountScopeType,
     AnomalyFeedbackTypeType,
     AnomalySubscriptionFrequencyType,
@@ -34,24 +34,27 @@
     SavingsPlansDataTypeType,
     SupportedSavingsPlansTypeType,
     TermInYearsType,
 )
 from .type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
+    AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostCategoryRuleTypeDef,
+    CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     CreateAnomalyMonitorResponseTypeDef,
     CreateAnomalySubscriptionResponseTypeDef,
     CreateCostCategoryDefinitionResponseTypeDef,
     DateIntervalTypeDef,
     DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
+    ExpressionOutputTypeDef,
     ExpressionTypeDef,
     GetAnomaliesResponseTypeDef,
     GetAnomalyMonitorsResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetCostCategoriesResponseTypeDef,
@@ -88,26 +91,23 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CostExplorerClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BillExpirationException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     DataUnavailableException: Type[BotocoreClientError]
     GenerationExistsException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
@@ -115,15 +115,14 @@
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     UnknownMonitorException: Type[BotocoreClientError]
     UnknownSubscriptionException: Type[BotocoreClientError]
     UnresolvableUsageUnitException: Type[BotocoreClientError]
 
-
 class CostExplorerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/)
     """
 
     meta: ClientMeta
@@ -132,127 +131,118 @@
     def exceptions(self) -> Exceptions:
         """
         CostExplorerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#close)
         """
-
     def create_anomaly_monitor(
         self,
         *,
         AnomalyMonitor: AnomalyMonitorTypeDef,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateAnomalyMonitorResponseTypeDef:
         """
         Creates a new cost anomaly detection monitor with the requested type and monitor
         specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_anomaly_monitor)
         """
-
     def create_anomaly_subscription(
         self,
         *,
-        AnomalySubscription: AnomalySubscriptionTypeDef,
+        AnomalySubscription: Union[AnomalySubscriptionTypeDef, AnomalySubscriptionOutputTypeDef],
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateAnomalySubscriptionResponseTypeDef:
         """
         Adds an alert subscription to a cost anomaly detection monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_anomaly_subscription)
         """
-
     def create_cost_category_definition(
         self,
         *,
         Name: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,
+        SplitChargeRules: Sequence[
+            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
+        ] = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateCostCategoryDefinitionResponseTypeDef:
         """
         Creates a new Cost Category with the requested name and rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_cost_category_definition)
         """
-
     def delete_anomaly_monitor(self, *, MonitorArn: str) -> Dict[str, Any]:
         """
         Deletes a cost anomaly monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.delete_anomaly_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#delete_anomaly_monitor)
         """
-
     def delete_anomaly_subscription(self, *, SubscriptionArn: str) -> Dict[str, Any]:
         """
         Deletes a cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.delete_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#delete_anomaly_subscription)
         """
-
     def delete_cost_category_definition(
         self, *, CostCategoryArn: str
     ) -> DeleteCostCategoryDefinitionResponseTypeDef:
         """
         Deletes a Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.delete_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#delete_cost_category_definition)
         """
-
     def describe_cost_category_definition(
         self, *, CostCategoryArn: str, EffectiveOn: str = ...
     ) -> DescribeCostCategoryDefinitionResponseTypeDef:
         """
         Returns the name, Amazon Resource Name (ARN), rules, definition, and effective
         dates of a Cost Category that's defined in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.describe_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#describe_cost_category_definition)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#generate_presigned_url)
         """
-
     def get_anomalies(
         self,
         *,
         DateInterval: AnomalyDateIntervalTypeDef,
         MonitorArn: str = ...,
         Feedback: AnomalyFeedbackTypeType = ...,
         TotalImpact: TotalImpactFilterTypeDef = ...,
@@ -262,328 +252,309 @@
         """
         Retrieves all of the cost anomalies detected on your account during the time
         period that's specified by the `DateInterval` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomalies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_anomalies)
         """
-
     def get_anomaly_monitors(
         self,
         *,
         MonitorArnList: Sequence[str] = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetAnomalyMonitorsResponseTypeDef:
         """
         Retrieves the cost anomaly monitor definitions for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomaly_monitors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_anomaly_monitors)
         """
-
     def get_anomaly_subscriptions(
         self,
         *,
         SubscriptionArnList: Sequence[str] = ...,
         MonitorArn: str = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetAnomalySubscriptionsResponseTypeDef:
         """
         Retrieves the cost anomaly subscription objects for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomaly_subscriptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_anomaly_subscriptions)
         """
-
     def get_cost_and_usage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Metrics: Sequence[str],
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageResponseTypeDef:
         """
         Retrieves cost and usage metrics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_cost_and_usage)
         """
-
     def get_cost_and_usage_with_resources(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef",
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"],
         Metrics: Sequence[str] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageWithResourcesResponseTypeDef:
         """
         Retrieves cost and usage metrics with resources for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage_with_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_cost_and_usage_with_resources)
         """
-
     def get_cost_categories(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         CostCategoryName: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetCostCategoriesResponseTypeDef:
         """
         Retrieves an array of Cost Category names and values incurred cost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_categories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_cost_categories)
         """
-
     def get_cost_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetCostForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         spend over the forecast time period that you select, based on your past costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_cost_forecast)
         """
-
     def get_dimension_values(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Dimension: DimensionType,
         SearchString: str = ...,
         Context: ContextType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetDimensionValuesResponseTypeDef:
         """
         Retrieves all available filter values for a specified filter over a period of
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_dimension_values)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_dimension_values)
         """
-
     def get_reservation_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         Metrics: Sequence[str] = ...,
         NextPageToken: str = ...,
         SortBy: SortDefinitionTypeDef = ...,
         MaxResults: int = ...
     ) -> GetReservationCoverageResponseTypeDef:
         """
         Retrieves the reservation coverage for your account, which you can use to see
         how much of your Amazon Elastic Compute Cloud, Amazon ElastiCache, Amazon
         Relational Database Service, or Amazon Redshift usage is covered by a
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_coverage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_reservation_coverage)
         """
-
     def get_reservation_purchase_recommendation(
         self,
         *,
         Service: str,
         AccountId: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         AccountScope: AccountScopeType = ...,
         LookbackPeriodInDays: LookbackPeriodInDaysType = ...,
         TermInYears: TermInYearsType = ...,
         PaymentOption: PaymentOptionType = ...,
         ServiceSpecification: ServiceSpecificationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
     ) -> GetReservationPurchaseRecommendationResponseTypeDef:
         """
         Gets recommendations for reservation purchases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_purchase_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_reservation_purchase_recommendation)
         """
-
     def get_reservation_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         SortBy: SortDefinitionTypeDef = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetReservationUtilizationResponseTypeDef:
         """
         Retrieves the reservation utilization for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_utilization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_reservation_utilization)
         """
-
     def get_rightsizing_recommendation(
         self,
         *,
         Service: str,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         Configuration: RightsizingRecommendationConfigurationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
     ) -> GetRightsizingRecommendationResponseTypeDef:
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_rightsizing_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_rightsizing_recommendation)
         """
-
     def get_savings_plan_purchase_recommendation_details(
         self, *, RecommendationDetailId: str
     ) -> GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef:
         """
         Retrieves the details for a Savings Plan recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plan_purchase_recommendation_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plan_purchase_recommendation_details)
         """
-
     def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         Metrics: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansCoverageResponseTypeDef:
         """
         Retrieves the Savings Plans covered for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_coverage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_coverage)
         """
-
     def get_savings_plans_purchase_recommendation(
         self,
         *,
         SavingsPlansType: SupportedSavingsPlansTypeType,
         TermInYears: TermInYearsType,
         PaymentOption: PaymentOptionType,
         LookbackPeriodInDays: LookbackPeriodInDaysType,
         AccountScope: AccountScopeType = ...,
         NextPageToken: str = ...,
         PageSize: int = ...,
-        Filter: "ExpressionTypeDef" = ...
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...
     ) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:
         """
         Retrieves the Savings Plans recommendations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_purchase_recommendation)
         """
-
     def get_savings_plans_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationResponseTypeDef:
         """
         Retrieves the Savings Plans utilization for your account across date ranges with
         daily or monthly granularity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_utilization)
         """
-
     def get_savings_plans_utilization_details(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         DataType: Sequence[SavingsPlansDataTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:
         """
         Retrieves attribute data along with aggregate utilization and savings data for a
         given time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_utilization_details)
         """
-
     def get_tags(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         TagKey: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetTagsResponseTypeDef:
         """
         Queries for available tag keys and tag values for a specified period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_tags)
         """
-
     def get_usage_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetUsageForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will use
         over the forecast time period that you select, based on your past usage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_usage_forecast)
         """
-
     def list_cost_allocation_tags(
         self,
         *,
         Status: CostAllocationTagStatusType = ...,
         TagKeys: Sequence[str] = ...,
         Type: CostAllocationTagTypeType = ...,
         NextToken: str = ...,
@@ -591,26 +562,24 @@
     ) -> ListCostAllocationTagsResponseTypeDef:
         """
         Get a list of cost allocation tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_cost_allocation_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#list_cost_allocation_tags)
         """
-
     def list_cost_category_definitions(
         self, *, EffectiveOn: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListCostCategoryDefinitionsResponseTypeDef:
         """
         Returns the name, Amazon Resource Name (ARN), `NumberOfRules` and effective
         dates of all Cost Categories defined in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_cost_category_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#list_cost_category_definitions)
         """
-
     def list_savings_plans_purchase_recommendation_generation(
         self,
         *,
         GenerationStatus: GenerationStatusType = ...,
         RecommendationIds: Sequence[str] = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
@@ -618,109 +587,102 @@
         """
         Retrieves a list of your historical recommendation generations within the past
         30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_savings_plans_purchase_recommendation_generation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#list_savings_plans_purchase_recommendation_generation)
         """
-
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of resource tags associated with the resource specified by the
         Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#list_tags_for_resource)
         """
-
     def provide_anomaly_feedback(
         self, *, AnomalyId: str, Feedback: AnomalyFeedbackTypeType
     ) -> ProvideAnomalyFeedbackResponseTypeDef:
         """
         Modifies the feedback property of a given cost anomaly.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.provide_anomaly_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#provide_anomaly_feedback)
         """
-
     def start_savings_plans_purchase_recommendation_generation(
         self,
     ) -> StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef:
         """
         Requests a Savings Plans recommendation generation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.start_savings_plans_purchase_recommendation_generation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#start_savings_plans_purchase_recommendation_generation)
         """
-
     def tag_resource(
         self, *, ResourceArn: str, ResourceTags: Sequence[ResourceTagTypeDef]
     ) -> Dict[str, Any]:
         """
         An API operation for adding one or more tags (key-value pairs) to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceArn: str, ResourceTagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#untag_resource)
         """
-
     def update_anomaly_monitor(
         self, *, MonitorArn: str, MonitorName: str = ...
     ) -> UpdateAnomalyMonitorResponseTypeDef:
         """
         Updates an existing cost anomaly monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_anomaly_monitor)
         """
-
     def update_anomaly_subscription(
         self,
         *,
         SubscriptionArn: str,
         Threshold: float = ...,
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
-        ThresholdExpression: "ExpressionTypeDef" = ...
+        ThresholdExpression: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
         Updates an existing cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_anomaly_subscription)
         """
-
     def update_cost_allocation_tags_status(
         self, *, CostAllocationTagsStatus: Sequence[CostAllocationTagStatusEntryTypeDef]
     ) -> UpdateCostAllocationTagsStatusResponseTypeDef:
         """
         Updates status for cost allocation tags in bulk, with maximum batch size of 20.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_allocation_tags_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_cost_allocation_tags_status)
         """
-
     def update_cost_category_definition(
         self,
         *,
         CostCategoryArn: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...
+        SplitChargeRules: Sequence[
+            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
+        ] = ...
     ) -> UpdateCostCategoryDefinitionResponseTypeDef:
         """
         Updates an existing Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_cost_category_definition)
         """
```

### Comparing `mypy-boto3-ce-1.28.15/mypy_boto3_ce/client.pyi` & `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ce.client import CostExplorerClient
 
     session = Session()
     client: CostExplorerClient = session.client("ce")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccountScopeType,
     AnomalyFeedbackTypeType,
     AnomalySubscriptionFrequencyType,
@@ -34,24 +34,27 @@
     SavingsPlansDataTypeType,
     SupportedSavingsPlansTypeType,
     TermInYearsType,
 )
 from .type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
+    AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostCategoryRuleTypeDef,
+    CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     CreateAnomalyMonitorResponseTypeDef,
     CreateAnomalySubscriptionResponseTypeDef,
     CreateCostCategoryDefinitionResponseTypeDef,
     DateIntervalTypeDef,
     DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
+    ExpressionOutputTypeDef,
     ExpressionTypeDef,
     GetAnomaliesResponseTypeDef,
     GetAnomalyMonitorsResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetCostCategoriesResponseTypeDef,
@@ -88,23 +91,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("CostExplorerClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BillExpirationException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     DataUnavailableException: Type[BotocoreClientError]
     GenerationExistsException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
@@ -112,14 +118,15 @@
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     UnknownMonitorException: Type[BotocoreClientError]
     UnknownSubscriptionException: Type[BotocoreClientError]
     UnresolvableUsageUnitException: Type[BotocoreClientError]
 
+
 class CostExplorerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/)
     """
 
     meta: ClientMeta
@@ -128,116 +135,129 @@
     def exceptions(self) -> Exceptions:
         """
         CostExplorerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#close)
         """
+
     def create_anomaly_monitor(
         self,
         *,
         AnomalyMonitor: AnomalyMonitorTypeDef,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateAnomalyMonitorResponseTypeDef:
         """
         Creates a new cost anomaly detection monitor with the requested type and monitor
         specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_anomaly_monitor)
         """
+
     def create_anomaly_subscription(
         self,
         *,
-        AnomalySubscription: AnomalySubscriptionTypeDef,
+        AnomalySubscription: Union[AnomalySubscriptionTypeDef, AnomalySubscriptionOutputTypeDef],
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateAnomalySubscriptionResponseTypeDef:
         """
         Adds an alert subscription to a cost anomaly detection monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_anomaly_subscription)
         """
+
     def create_cost_category_definition(
         self,
         *,
         Name: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,
+        SplitChargeRules: Sequence[
+            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
+        ] = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateCostCategoryDefinitionResponseTypeDef:
         """
         Creates a new Cost Category with the requested name and rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#create_cost_category_definition)
         """
+
     def delete_anomaly_monitor(self, *, MonitorArn: str) -> Dict[str, Any]:
         """
         Deletes a cost anomaly monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.delete_anomaly_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#delete_anomaly_monitor)
         """
+
     def delete_anomaly_subscription(self, *, SubscriptionArn: str) -> Dict[str, Any]:
         """
         Deletes a cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.delete_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#delete_anomaly_subscription)
         """
+
     def delete_cost_category_definition(
         self, *, CostCategoryArn: str
     ) -> DeleteCostCategoryDefinitionResponseTypeDef:
         """
         Deletes a Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.delete_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#delete_cost_category_definition)
         """
+
     def describe_cost_category_definition(
         self, *, CostCategoryArn: str, EffectiveOn: str = ...
     ) -> DescribeCostCategoryDefinitionResponseTypeDef:
         """
         Returns the name, Amazon Resource Name (ARN), rules, definition, and effective
         dates of a Cost Category that's defined in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.describe_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#describe_cost_category_definition)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#generate_presigned_url)
         """
+
     def get_anomalies(
         self,
         *,
         DateInterval: AnomalyDateIntervalTypeDef,
         MonitorArn: str = ...,
         Feedback: AnomalyFeedbackTypeType = ...,
         TotalImpact: TotalImpactFilterTypeDef = ...,
@@ -247,309 +267,328 @@
         """
         Retrieves all of the cost anomalies detected on your account during the time
         period that's specified by the `DateInterval` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomalies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_anomalies)
         """
+
     def get_anomaly_monitors(
         self,
         *,
         MonitorArnList: Sequence[str] = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetAnomalyMonitorsResponseTypeDef:
         """
         Retrieves the cost anomaly monitor definitions for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomaly_monitors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_anomaly_monitors)
         """
+
     def get_anomaly_subscriptions(
         self,
         *,
         SubscriptionArnList: Sequence[str] = ...,
         MonitorArn: str = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetAnomalySubscriptionsResponseTypeDef:
         """
         Retrieves the cost anomaly subscription objects for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomaly_subscriptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_anomaly_subscriptions)
         """
+
     def get_cost_and_usage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Metrics: Sequence[str],
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageResponseTypeDef:
         """
         Retrieves cost and usage metrics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_cost_and_usage)
         """
+
     def get_cost_and_usage_with_resources(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef",
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"],
         Metrics: Sequence[str] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageWithResourcesResponseTypeDef:
         """
         Retrieves cost and usage metrics with resources for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage_with_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_cost_and_usage_with_resources)
         """
+
     def get_cost_categories(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         CostCategoryName: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetCostCategoriesResponseTypeDef:
         """
         Retrieves an array of Cost Category names and values incurred cost.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_categories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_cost_categories)
         """
+
     def get_cost_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetCostForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         spend over the forecast time period that you select, based on your past costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_cost_forecast)
         """
+
     def get_dimension_values(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Dimension: DimensionType,
         SearchString: str = ...,
         Context: ContextType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetDimensionValuesResponseTypeDef:
         """
         Retrieves all available filter values for a specified filter over a period of
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_dimension_values)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_dimension_values)
         """
+
     def get_reservation_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         Metrics: Sequence[str] = ...,
         NextPageToken: str = ...,
         SortBy: SortDefinitionTypeDef = ...,
         MaxResults: int = ...
     ) -> GetReservationCoverageResponseTypeDef:
         """
         Retrieves the reservation coverage for your account, which you can use to see
         how much of your Amazon Elastic Compute Cloud, Amazon ElastiCache, Amazon
         Relational Database Service, or Amazon Redshift usage is covered by a
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_coverage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_reservation_coverage)
         """
+
     def get_reservation_purchase_recommendation(
         self,
         *,
         Service: str,
         AccountId: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         AccountScope: AccountScopeType = ...,
         LookbackPeriodInDays: LookbackPeriodInDaysType = ...,
         TermInYears: TermInYearsType = ...,
         PaymentOption: PaymentOptionType = ...,
         ServiceSpecification: ServiceSpecificationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
     ) -> GetReservationPurchaseRecommendationResponseTypeDef:
         """
         Gets recommendations for reservation purchases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_purchase_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_reservation_purchase_recommendation)
         """
+
     def get_reservation_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         SortBy: SortDefinitionTypeDef = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetReservationUtilizationResponseTypeDef:
         """
         Retrieves the reservation utilization for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_utilization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_reservation_utilization)
         """
+
     def get_rightsizing_recommendation(
         self,
         *,
         Service: str,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         Configuration: RightsizingRecommendationConfigurationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
     ) -> GetRightsizingRecommendationResponseTypeDef:
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_rightsizing_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_rightsizing_recommendation)
         """
+
     def get_savings_plan_purchase_recommendation_details(
         self, *, RecommendationDetailId: str
     ) -> GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef:
         """
         Retrieves the details for a Savings Plan recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plan_purchase_recommendation_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plan_purchase_recommendation_details)
         """
+
     def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         Metrics: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansCoverageResponseTypeDef:
         """
         Retrieves the Savings Plans covered for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_coverage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_coverage)
         """
+
     def get_savings_plans_purchase_recommendation(
         self,
         *,
         SavingsPlansType: SupportedSavingsPlansTypeType,
         TermInYears: TermInYearsType,
         PaymentOption: PaymentOptionType,
         LookbackPeriodInDays: LookbackPeriodInDaysType,
         AccountScope: AccountScopeType = ...,
         NextPageToken: str = ...,
         PageSize: int = ...,
-        Filter: "ExpressionTypeDef" = ...
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...
     ) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:
         """
         Retrieves the Savings Plans recommendations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_purchase_recommendation)
         """
+
     def get_savings_plans_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationResponseTypeDef:
         """
         Retrieves the Savings Plans utilization for your account across date ranges with
         daily or monthly granularity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_utilization)
         """
+
     def get_savings_plans_utilization_details(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         DataType: Sequence[SavingsPlansDataTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:
         """
         Retrieves attribute data along with aggregate utilization and savings data for a
         given time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_savings_plans_utilization_details)
         """
+
     def get_tags(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         TagKey: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetTagsResponseTypeDef:
         """
         Queries for available tag keys and tag values for a specified period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_tags)
         """
+
     def get_usage_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetUsageForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will use
         over the forecast time period that you select, based on your past usage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#get_usage_forecast)
         """
+
     def list_cost_allocation_tags(
         self,
         *,
         Status: CostAllocationTagStatusType = ...,
         TagKeys: Sequence[str] = ...,
         Type: CostAllocationTagTypeType = ...,
         NextToken: str = ...,
@@ -557,24 +596,26 @@
     ) -> ListCostAllocationTagsResponseTypeDef:
         """
         Get a list of cost allocation tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_cost_allocation_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#list_cost_allocation_tags)
         """
+
     def list_cost_category_definitions(
         self, *, EffectiveOn: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListCostCategoryDefinitionsResponseTypeDef:
         """
         Returns the name, Amazon Resource Name (ARN), `NumberOfRules` and effective
         dates of all Cost Categories defined in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_cost_category_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#list_cost_category_definitions)
         """
+
     def list_savings_plans_purchase_recommendation_generation(
         self,
         *,
         GenerationStatus: GenerationStatusType = ...,
         RecommendationIds: Sequence[str] = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
@@ -582,100 +623,111 @@
         """
         Retrieves a list of your historical recommendation generations within the past
         30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_savings_plans_purchase_recommendation_generation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#list_savings_plans_purchase_recommendation_generation)
         """
+
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of resource tags associated with the resource specified by the
         Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#list_tags_for_resource)
         """
+
     def provide_anomaly_feedback(
         self, *, AnomalyId: str, Feedback: AnomalyFeedbackTypeType
     ) -> ProvideAnomalyFeedbackResponseTypeDef:
         """
         Modifies the feedback property of a given cost anomaly.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.provide_anomaly_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#provide_anomaly_feedback)
         """
+
     def start_savings_plans_purchase_recommendation_generation(
         self,
     ) -> StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef:
         """
         Requests a Savings Plans recommendation generation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.start_savings_plans_purchase_recommendation_generation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#start_savings_plans_purchase_recommendation_generation)
         """
+
     def tag_resource(
         self, *, ResourceArn: str, ResourceTags: Sequence[ResourceTagTypeDef]
     ) -> Dict[str, Any]:
         """
         An API operation for adding one or more tags (key-value pairs) to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceArn: str, ResourceTagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#untag_resource)
         """
+
     def update_anomaly_monitor(
         self, *, MonitorArn: str, MonitorName: str = ...
     ) -> UpdateAnomalyMonitorResponseTypeDef:
         """
         Updates an existing cost anomaly monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_anomaly_monitor)
         """
+
     def update_anomaly_subscription(
         self,
         *,
         SubscriptionArn: str,
         Threshold: float = ...,
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
-        ThresholdExpression: "ExpressionTypeDef" = ...
+        ThresholdExpression: Union["ExpressionTypeDef", "ExpressionOutputTypeDef"] = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
         Updates an existing cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_anomaly_subscription)
         """
+
     def update_cost_allocation_tags_status(
         self, *, CostAllocationTagsStatus: Sequence[CostAllocationTagStatusEntryTypeDef]
     ) -> UpdateCostAllocationTagsStatusResponseTypeDef:
         """
         Updates status for cost allocation tags in bulk, with maximum batch size of 20.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_allocation_tags_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_cost_allocation_tags_status)
         """
+
     def update_cost_category_definition(
         self,
         *,
         CostCategoryArn: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...
+        SplitChargeRules: Sequence[
+            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
+        ] = ...
     ) -> UpdateCostCategoryDefinitionResponseTypeDef:
         """
         Updates an existing Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/client/#update_cost_category_definition)
         """
```

### Comparing `mypy-boto3-ce-1.28.15/mypy_boto3_ce/literals.py` & `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.15/mypy_boto3_ce/literals.pyi` & `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.15/mypy_boto3_ce/type_defs.py` & `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_ce.type_defs import AnomalyDateIntervalTypeDef
 
     data: AnomalyDateIntervalTypeDef = {...}
     ```
 """
 import sys
-from typing import Any, Dict, List, Sequence
+from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
     AccountScopeType,
     AnomalyFeedbackTypeType,
     AnomalySubscriptionFrequencyType,
     ContextType,
     CostAllocationTagStatusType,
@@ -2109,15 +2109,17 @@
     },
 )
 _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
     {
         "EffectiveStart": str,
         "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
+        "SplitChargeRules": Sequence[
+            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
+        ],
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
 
 class CreateCostCategoryDefinitionRequestRequestTypeDef(
@@ -2136,15 +2138,17 @@
     },
 )
 _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
     {
         "EffectiveStart": str,
         "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
+        "SplitChargeRules": Sequence[
+            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class UpdateCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.15/mypy_boto3_ce/type_defs.pyi` & `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_ce.type_defs import AnomalyDateIntervalTypeDef
 
     data: AnomalyDateIntervalTypeDef = {...}
     ```
 """
 import sys
-from typing import Any, Dict, List, Sequence
+from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
     AccountScopeType,
     AnomalyFeedbackTypeType,
     AnomalySubscriptionFrequencyType,
     ContextType,
     CostAllocationTagStatusType,
@@ -2042,15 +2042,17 @@
     },
 )
 _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
     {
         "EffectiveStart": str,
         "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
+        "SplitChargeRules": Sequence[
+            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
+        ],
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
 class CreateCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
@@ -2067,15 +2069,17 @@
     },
 )
 _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
     {
         "EffectiveStart": str,
         "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
+        "SplitChargeRules": Sequence[
+            Union[CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class UpdateCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/PKG-INFO` & `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.28.15
-Summary: Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/SOURCES.txt` & `mypy-boto3-ce-1.28.15.post1/mypy_boto3_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.15/setup.py` & `mypy-boto3-ce-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ce",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder"
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

