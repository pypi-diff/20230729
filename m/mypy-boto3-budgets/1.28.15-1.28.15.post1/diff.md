# Comparing `tmp/mypy-boto3-budgets-1.28.15.tar.gz` & `tmp/mypy-boto3-budgets-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-budgets-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
+gzip compressed data, was "mypy-boto3-budgets-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:37 2023, max compression
```

## Comparing `mypy-boto3-budgets-1.28.15.tar` & `mypy-boto3-budgets-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.328737 mypy-boto3-budgets-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-07-28 20:42:22.324737 mypy-boto3-budgets-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.320737 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-28 20:20:18.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-28 20:20:18.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34193 2023-07-28 20:20:19.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34138 2023-07-28 20:20:19.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.324737 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-07-28 20:42:22.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:42:22.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:22.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:22.000000 mypy-boto3-budgets-1.28.15/mypy_boto3_budgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.328737 mypy-boto3-budgets-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:20:17.000000 mypy-boto3-budgets-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.941035 mypy-boto3-budgets-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-29 10:02:37.941035 mypy-boto3-budgets-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.929035 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-07-29 09:39:10.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22215 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-29 09:39:10.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-29 09:39:10.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-29 09:39:10.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-29 09:39:10.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34193 2023-07-29 09:39:12.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34138 2023-07-29 09:39:11.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.941035 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:37.941035 mypy-boto3-budgets-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-budgets-1.28.15/LICENSE` & `mypy-boto3-budgets-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15/PKG-INFO` & `mypy-boto3-budgets-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-budgets
-Version: 1.28.15
-Summary: Type annotations for boto3.Budgets 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Budgets 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-budgets-1.28.15/README.md` & `mypy-boto3-budgets-1.28.15.post1/README.md`

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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/__init__.py` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/__init__.pyi` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/__main__.py` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Budgets 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Budgets 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
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

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/client.py` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_budgets.client import BudgetsClient
 
     session = Session()
     client: BudgetsClient = session.client("budgets")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ActionTypeType, ApprovalModelType, ExecutionTypeType, NotificationTypeType
 from .paginator import (
     DescribeBudgetActionHistoriesPaginator,
     DescribeBudgetActionsForAccountPaginator,
@@ -27,16 +27,18 @@
     DescribeBudgetPerformanceHistoryPaginator,
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 from .type_defs import (
     ActionThresholdTypeDef,
+    BudgetOutputTypeDef,
     BudgetTypeDef,
     CreateBudgetActionResponseTypeDef,
+    DefinitionOutputTypeDef,
     DefinitionTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
@@ -45,14 +47,15 @@
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     NotificationTypeDef,
     NotificationWithSubscribersTypeDef,
     SubscriberTypeDef,
+    TimePeriodOutputTypeDef,
     TimePeriodTypeDef,
     UpdateBudgetActionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -117,15 +120,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#close)
         """
 
     def create_budget(
         self,
         *,
         AccountId: str,
-        Budget: BudgetTypeDef,
+        Budget: Union[BudgetTypeDef, BudgetOutputTypeDef],
         NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_budget)
@@ -135,15 +138,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
-        Definition: DefinitionTypeDef,
+        Definition: Union[DefinitionTypeDef, DefinitionOutputTypeDef],
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
         Subscribers: Sequence[SubscriberTypeDef]
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
@@ -244,15 +247,15 @@
 
     def describe_budget_action_histories(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
@@ -290,15 +293,15 @@
         """
 
     def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
@@ -361,15 +364,17 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#generate_presigned_url)
         """
 
-    def update_budget(self, *, AccountId: str, NewBudget: BudgetTypeDef) -> Dict[str, Any]:
+    def update_budget(
+        self, *, AccountId: str, NewBudget: Union[BudgetTypeDef, BudgetOutputTypeDef]
+    ) -> Dict[str, Any]:
         """
         Updates a budget.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_budget)
         """
 
@@ -377,15 +382,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
-        Definition: DefinitionTypeDef = ...,
+        Definition: Union[DefinitionTypeDef, DefinitionOutputTypeDef] = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
```

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/client.pyi` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_budgets.client import BudgetsClient
 
     session = Session()
     client: BudgetsClient = session.client("budgets")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ActionTypeType, ApprovalModelType, ExecutionTypeType, NotificationTypeType
 from .paginator import (
     DescribeBudgetActionHistoriesPaginator,
     DescribeBudgetActionsForAccountPaginator,
@@ -27,16 +27,18 @@
     DescribeBudgetPerformanceHistoryPaginator,
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 from .type_defs import (
     ActionThresholdTypeDef,
+    BudgetOutputTypeDef,
     BudgetTypeDef,
     CreateBudgetActionResponseTypeDef,
+    DefinitionOutputTypeDef,
     DefinitionTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
@@ -45,14 +47,15 @@
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     NotificationTypeDef,
     NotificationWithSubscribersTypeDef,
     SubscriberTypeDef,
+    TimePeriodOutputTypeDef,
     TimePeriodTypeDef,
     UpdateBudgetActionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -110,15 +113,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#close)
         """
     def create_budget(
         self,
         *,
         AccountId: str,
-        Budget: BudgetTypeDef,
+        Budget: Union[BudgetTypeDef, BudgetOutputTypeDef],
         NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_budget)
@@ -127,15 +130,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
-        Definition: DefinitionTypeDef,
+        Definition: Union[DefinitionTypeDef, DefinitionOutputTypeDef],
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
         Subscribers: Sequence[SubscriberTypeDef]
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
@@ -227,15 +230,15 @@
         """
     def describe_budget_action_histories(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
@@ -269,15 +272,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#describe_budget_notifications_for_account)
         """
     def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
@@ -334,30 +337,32 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#generate_presigned_url)
         """
-    def update_budget(self, *, AccountId: str, NewBudget: BudgetTypeDef) -> Dict[str, Any]:
+    def update_budget(
+        self, *, AccountId: str, NewBudget: Union[BudgetTypeDef, BudgetOutputTypeDef]
+    ) -> Dict[str, Any]:
         """
         Updates a budget.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_budget)
         """
     def update_budget_action(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
-        Definition: DefinitionTypeDef = ...,
+        Definition: Union[DefinitionTypeDef, DefinitionOutputTypeDef] = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
```

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/literals.py` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/literals.pyi` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/paginator.py` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,29 +29,30 @@
     describe_budget_notifications_for_account_paginator: DescribeBudgetNotificationsForAccountPaginator = client.get_paginator("describe_budget_notifications_for_account")
     describe_budget_performance_history_paginator: DescribeBudgetPerformanceHistoryPaginator = client.get_paginator("describe_budget_performance_history")
     describe_budgets_paginator: DescribeBudgetsPaginator = client.get_paginator("describe_budgets")
     describe_notifications_for_budget_paginator: DescribeNotificationsForBudgetPaginator = client.get_paginator("describe_notifications_for_budget")
     describe_subscribers_for_notification_paginator: DescribeSubscribersForNotificationPaginator = client.get_paginator("describe_subscribers_for_notification")
     ```
 """
-from typing import Generic, Iterator, TypeVar
+from typing import Generic, Iterator, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     NotificationTypeDef,
     PaginatorConfigTypeDef,
+    TimePeriodOutputTypeDef,
     TimePeriodTypeDef,
 )
 
 __all__ = (
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
@@ -81,15 +82,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
@@ -146,15 +147,15 @@
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
```

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/paginator.pyi` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,29 +29,30 @@
     describe_budget_notifications_for_account_paginator: DescribeBudgetNotificationsForAccountPaginator = client.get_paginator("describe_budget_notifications_for_account")
     describe_budget_performance_history_paginator: DescribeBudgetPerformanceHistoryPaginator = client.get_paginator("describe_budget_performance_history")
     describe_budgets_paginator: DescribeBudgetsPaginator = client.get_paginator("describe_budgets")
     describe_notifications_for_budget_paginator: DescribeNotificationsForBudgetPaginator = client.get_paginator("describe_notifications_for_budget")
     describe_subscribers_for_notification_paginator: DescribeSubscribersForNotificationPaginator = client.get_paginator("describe_subscribers_for_notification")
     ```
 """
-from typing import Generic, Iterator, TypeVar
+from typing import Generic, Iterator, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     NotificationTypeDef,
     PaginatorConfigTypeDef,
+    TimePeriodOutputTypeDef,
     TimePeriodTypeDef,
 )
 
 __all__ = (
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
@@ -78,15 +79,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
@@ -139,15 +140,15 @@
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
```

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/type_defs.py` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets/type_defs.pyi` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets.egg-info/PKG-INFO` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-budgets
-Version: 1.28.15
-Summary: Type annotations for boto3.Budgets 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Budgets 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-budgets-1.28.15/mypy_boto3_budgets.egg-info/SOURCES.txt` & `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15/setup.py` & `mypy-boto3-budgets-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-budgets",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Budgets 1.28.15 service generated with mypy-boto3-builder"
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

