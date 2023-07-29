# Comparing `tmp/mypy-boto3-codestar-notifications-1.28.12.tar.gz` & `tmp/mypy-boto3-codestar-notifications-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codestar-notifications-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
+gzip compressed data, was "mypy-boto3-codestar-notifications-1.28.15.tar", last modified: Fri Jul 28 20:42:31 2023, max compression
```

## Comparing `mypy-boto3-codestar-notifications-1.28.12.tar` & `mypy-boto3-codestar-notifications-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.400549 mypy-boto3-codestar-notifications-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-07-27 05:34:29.400549 mypy-boto3-codestar-notifications-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.392549 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.400549 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-07-27 05:34:29.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-27 05:34:29.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:29.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 05:34:29.000000 mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.400549 mypy-boto3-codestar-notifications-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-27 05:19:15.000000 mypy-boto3-codestar-notifications-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.640869 mypy-boto3-codestar-notifications-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-07-28 20:42:31.636869 mypy-boto3-codestar-notifications-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.632868 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-28 20:21:46.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.636869 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-07-28 20:42:31.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-28 20:42:31.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:31.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 20:42:31.000000 mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:31.640869 mypy-boto3-codestar-notifications-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-28 20:21:45.000000 mypy-boto3-codestar-notifications-1.28.15/setup.py
```

### Comparing `mypy-boto3-codestar-notifications-1.28.12/LICENSE` & `mypy-boto3-codestar-notifications-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.28.12/PKG-INFO` & `mypy-boto3-codestar-notifications-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-notifications
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeStarNotifications 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeStarNotifications 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-notifications.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-notifications)](https://pepy.tech/project/mypy-boto3-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarNotifications 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[boto3.CodeStarNotifications 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [mypy-boto3-codestar-notifications docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,43 +337,43 @@
 
 `mypy_boto3_codestar_notifications.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_notifications.type_defs import (
     TargetTypeDef,
-    CreateNotificationRuleResultTypeDef,
+    ResponseMetadataTypeDef,
     DeleteNotificationRuleRequestRequestTypeDef,
-    DeleteNotificationRuleResultTypeDef,
     DeleteTargetRequestRequestTypeDef,
     DescribeNotificationRuleRequestRequestTypeDef,
     EventTypeSummaryTypeDef,
     TargetSummaryTypeDef,
     ListEventTypesFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListNotificationRulesFilterTypeDef,
     NotificationRuleSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     ListTargetsFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    SubscribeResultTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResultTypeDef,
     UnsubscribeRequestRequestTypeDef,
-    UnsubscribeResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateNotificationRuleRequestRequestTypeDef,
     SubscribeRequestRequestTypeDef,
     UpdateNotificationRuleRequestRequestTypeDef,
+    CreateNotificationRuleResultTypeDef,
+    DeleteNotificationRuleResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    SubscribeResultTypeDef,
+    TagResourceResultTypeDef,
+    UnsubscribeResultTypeDef,
     ListEventTypesResultTypeDef,
     DescribeNotificationRuleResultTypeDef,
     ListTargetsResultTypeDef,
-    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListEventTypesRequestRequestTypeDef,
+    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
     ListNotificationRulesRequestRequestTypeDef,
     ListNotificationRulesResultTypeDef,
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-codestar-notifications-1.28.12/README.md` & `mypy-boto3-codestar-notifications-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-notifications.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-notifications)](https://pepy.tech/project/mypy-boto3-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarNotifications 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[boto3.CodeStarNotifications 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [mypy-boto3-codestar-notifications docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,43 +305,43 @@
 
 `mypy_boto3_codestar_notifications.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_notifications.type_defs import (
     TargetTypeDef,
-    CreateNotificationRuleResultTypeDef,
+    ResponseMetadataTypeDef,
     DeleteNotificationRuleRequestRequestTypeDef,
-    DeleteNotificationRuleResultTypeDef,
     DeleteTargetRequestRequestTypeDef,
     DescribeNotificationRuleRequestRequestTypeDef,
     EventTypeSummaryTypeDef,
     TargetSummaryTypeDef,
     ListEventTypesFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListNotificationRulesFilterTypeDef,
     NotificationRuleSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     ListTargetsFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    SubscribeResultTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResultTypeDef,
     UnsubscribeRequestRequestTypeDef,
-    UnsubscribeResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateNotificationRuleRequestRequestTypeDef,
     SubscribeRequestRequestTypeDef,
     UpdateNotificationRuleRequestRequestTypeDef,
+    CreateNotificationRuleResultTypeDef,
+    DeleteNotificationRuleResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    SubscribeResultTypeDef,
+    TagResourceResultTypeDef,
+    UnsubscribeResultTypeDef,
     ListEventTypesResultTypeDef,
     DescribeNotificationRuleResultTypeDef,
     ListTargetsResultTypeDef,
-    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListEventTypesRequestRequestTypeDef,
+    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
     ListNotificationRulesRequestRequestTypeDef,
     ListNotificationRulesResultTypeDef,
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/__init__.py` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/__init__.pyi` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/__main__.py` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeStarNotifications 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodeStarNotifications 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications\nOther"
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

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/client.py` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/client.pyi` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/literals.py` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/literals.pyi` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/paginator.py` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listeventtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListEventTypesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventTypesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listeventtypespaginator)
         """
 
 
@@ -74,15 +74,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listnotificationrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNotificationRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listnotificationrulespaginator)
         """
 
 
@@ -92,13 +92,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listtargetspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListTargetsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listtargetspaginator)
         """
```

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/paginator.pyi` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listeventtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListEventTypesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventTypesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listeventtypespaginator)
         """
 
 class ListNotificationRulesPaginator(Paginator):
@@ -70,15 +70,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listnotificationrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNotificationRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listnotificationrulespaginator)
         """
 
 class ListTargetsPaginator(Paginator):
@@ -87,13 +87,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listtargetspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ListTargetsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/paginators/#listtargetspaginator)
         """
```

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/type_defs.py` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -25,46 +25,45 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TargetTypeDef",
-    "CreateNotificationRuleResultTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteNotificationRuleRequestRequestTypeDef",
-    "DeleteNotificationRuleResultTypeDef",
     "DeleteTargetRequestRequestTypeDef",
     "DescribeNotificationRuleRequestRequestTypeDef",
     "EventTypeSummaryTypeDef",
     "TargetSummaryTypeDef",
     "ListEventTypesFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListNotificationRulesFilterTypeDef",
     "NotificationRuleSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "ListTargetsFilterTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "SubscribeResultTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagResourceResultTypeDef",
     "UnsubscribeRequestRequestTypeDef",
-    "UnsubscribeResultTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateNotificationRuleRequestRequestTypeDef",
     "SubscribeRequestRequestTypeDef",
     "UpdateNotificationRuleRequestRequestTypeDef",
+    "CreateNotificationRuleResultTypeDef",
+    "DeleteNotificationRuleResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "SubscribeResultTypeDef",
+    "TagResourceResultTypeDef",
+    "UnsubscribeResultTypeDef",
     "ListEventTypesResultTypeDef",
     "DescribeNotificationRuleResultTypeDef",
     "ListTargetsResultTypeDef",
-    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     "ListEventTypesRequestRequestTypeDef",
+    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     "ListNotificationRulesRequestRequestTypeDef",
     "ListNotificationRulesResultTypeDef",
     "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
 )
 
@@ -73,58 +72,51 @@
     {
         "TargetType": str,
         "TargetAddress": str,
     },
     total=False,
 )
 
-CreateNotificationRuleResultTypeDef = TypedDict(
-    "CreateNotificationRuleResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteNotificationRuleRequestRequestTypeDef = TypedDict(
     "DeleteNotificationRuleRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteNotificationRuleResultTypeDef = TypedDict(
-    "DeleteNotificationRuleResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTargetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTargetRequestRequestTypeDef",
     {
         "TargetAddress": str,
     },
 )
 _OptionalDeleteTargetRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteTargetRequestRequestTypeDef",
     {
         "ForceUnsubscribeAll": bool,
     },
     total=False,
 )
 
-
 class DeleteTargetRequestRequestTypeDef(
     _RequiredDeleteTargetRequestRequestTypeDef, _OptionalDeleteTargetRequestRequestTypeDef
 ):
     pass
 
-
 DescribeNotificationRuleRequestRequestTypeDef = TypedDict(
     "DescribeNotificationRuleRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -153,14 +145,24 @@
     "ListEventTypesFilterTypeDef",
     {
         "Name": ListEventTypesFilterNameType,
         "Value": str,
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
 ListNotificationRulesFilterTypeDef = TypedDict(
     "ListNotificationRulesFilterTypeDef",
     {
         "Name": ListNotificationRulesFilterNameType,
         "Value": str,
     },
 )
@@ -177,91 +179,38 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTargetsFilterTypeDef = TypedDict(
     "ListTargetsFilterTypeDef",
     {
         "Name": ListTargetsFilterNameType,
         "Value": str,
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
-SubscribeResultTypeDef = TypedDict(
-    "SubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
-TagResourceResultTypeDef = TypedDict(
-    "TagResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnsubscribeRequestRequestTypeDef = TypedDict(
     "UnsubscribeRequestRequestTypeDef",
     {
         "Arn": str,
         "TargetAddress": str,
     },
 )
 
-UnsubscribeResultTypeDef = TypedDict(
-    "UnsubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -282,22 +231,20 @@
         "ClientRequestToken": str,
         "Tags": Mapping[str, str],
         "Status": NotificationRuleStatusType,
     },
     total=False,
 )
 
-
 class CreateNotificationRuleRequestRequestTypeDef(
     _RequiredCreateNotificationRuleRequestRequestTypeDef,
     _OptionalCreateNotificationRuleRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSubscribeRequestRequestTypeDef = TypedDict(
     "_RequiredSubscribeRequestRequestTypeDef",
     {
         "Arn": str,
         "Target": TargetTypeDef,
     },
 )
@@ -305,21 +252,19 @@
     "_OptionalSubscribeRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class SubscribeRequestRequestTypeDef(
     _RequiredSubscribeRequestRequestTypeDef, _OptionalSubscribeRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateNotificationRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNotificationRuleRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalUpdateNotificationRuleRequestRequestTypeDef = TypedDict(
@@ -330,28 +275,74 @@
         "EventTypeIds": Sequence[str],
         "Targets": Sequence[TargetTypeDef],
         "DetailType": DetailTypeType,
     },
     total=False,
 )
 
-
 class UpdateNotificationRuleRequestRequestTypeDef(
     _RequiredUpdateNotificationRuleRequestRequestTypeDef,
     _OptionalUpdateNotificationRuleRequestRequestTypeDef,
 ):
     pass
 
+CreateNotificationRuleResultTypeDef = TypedDict(
+    "CreateNotificationRuleResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteNotificationRuleResultTypeDef = TypedDict(
+    "DeleteNotificationRuleResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubscribeResultTypeDef = TypedDict(
+    "SubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceResultTypeDef = TypedDict(
+    "TagResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnsubscribeResultTypeDef = TypedDict(
+    "UnsubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListEventTypesResultTypeDef = TypedDict(
     "ListEventTypesResultTypeDef",
     {
         "EventTypes": List[EventTypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationRuleResultTypeDef = TypedDict(
     "DescribeNotificationRuleResultTypeDef",
     {
         "Arn": str,
@@ -361,51 +352,51 @@
         "Targets": List[TargetSummaryTypeDef],
         "DetailType": DetailTypeType,
         "CreatedBy": str,
         "Status": NotificationRuleStatusType,
         "CreatedTimestamp": datetime,
         "LastModifiedTimestamp": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsResultTypeDef = TypedDict(
     "ListTargetsResultTypeDef",
     {
         "Targets": List[TargetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
-    "ListEventTypesRequestListEventTypesPaginateTypeDef",
+ListEventTypesRequestRequestTypeDef = TypedDict(
+    "ListEventTypesRequestRequestTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
-ListEventTypesRequestRequestTypeDef = TypedDict(
-    "ListEventTypesRequestRequestTypeDef",
+ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
+    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNotificationRulesRequestListNotificationRulesPaginateTypeDef = TypedDict(
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     {
         "Filters": Sequence[ListNotificationRulesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNotificationRulesRequestRequestTypeDef = TypedDict(
     "ListNotificationRulesRequestRequestTypeDef",
     {
@@ -417,23 +408,23 @@
 )
 
 ListNotificationRulesResultTypeDef = TypedDict(
     "ListNotificationRulesResultTypeDef",
     {
         "NextToken": str,
         "NotificationRules": List[NotificationRuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
     "ListTargetsRequestListTargetsPaginateTypeDef",
     {
         "Filters": Sequence[ListTargetsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTargetsRequestRequestTypeDef = TypedDict(
     "ListTargetsRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications/type_defs.pyi` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,45 +25,46 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TargetTypeDef",
-    "CreateNotificationRuleResultTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteNotificationRuleRequestRequestTypeDef",
-    "DeleteNotificationRuleResultTypeDef",
     "DeleteTargetRequestRequestTypeDef",
     "DescribeNotificationRuleRequestRequestTypeDef",
     "EventTypeSummaryTypeDef",
     "TargetSummaryTypeDef",
     "ListEventTypesFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListNotificationRulesFilterTypeDef",
     "NotificationRuleSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "ListTargetsFilterTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "SubscribeResultTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagResourceResultTypeDef",
     "UnsubscribeRequestRequestTypeDef",
-    "UnsubscribeResultTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateNotificationRuleRequestRequestTypeDef",
     "SubscribeRequestRequestTypeDef",
     "UpdateNotificationRuleRequestRequestTypeDef",
+    "CreateNotificationRuleResultTypeDef",
+    "DeleteNotificationRuleResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "SubscribeResultTypeDef",
+    "TagResourceResultTypeDef",
+    "UnsubscribeResultTypeDef",
     "ListEventTypesResultTypeDef",
     "DescribeNotificationRuleResultTypeDef",
     "ListTargetsResultTypeDef",
-    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     "ListEventTypesRequestRequestTypeDef",
+    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     "ListNotificationRulesRequestRequestTypeDef",
     "ListNotificationRulesResultTypeDef",
     "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
 )
 
@@ -72,56 +73,53 @@
     {
         "TargetType": str,
         "TargetAddress": str,
     },
     total=False,
 )
 
-CreateNotificationRuleResultTypeDef = TypedDict(
-    "CreateNotificationRuleResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteNotificationRuleRequestRequestTypeDef = TypedDict(
     "DeleteNotificationRuleRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteNotificationRuleResultTypeDef = TypedDict(
-    "DeleteNotificationRuleResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTargetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTargetRequestRequestTypeDef",
     {
         "TargetAddress": str,
     },
 )
 _OptionalDeleteTargetRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteTargetRequestRequestTypeDef",
     {
         "ForceUnsubscribeAll": bool,
     },
     total=False,
 )
 
+
 class DeleteTargetRequestRequestTypeDef(
     _RequiredDeleteTargetRequestRequestTypeDef, _OptionalDeleteTargetRequestRequestTypeDef
 ):
     pass
 
+
 DescribeNotificationRuleRequestRequestTypeDef = TypedDict(
     "DescribeNotificationRuleRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -150,14 +148,24 @@
     "ListEventTypesFilterTypeDef",
     {
         "Name": ListEventTypesFilterNameType,
         "Value": str,
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
 ListNotificationRulesFilterTypeDef = TypedDict(
     "ListNotificationRulesFilterTypeDef",
     {
         "Name": ListNotificationRulesFilterNameType,
         "Value": str,
     },
 )
@@ -174,91 +182,38 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTargetsFilterTypeDef = TypedDict(
     "ListTargetsFilterTypeDef",
     {
         "Name": ListTargetsFilterNameType,
         "Value": str,
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
-SubscribeResultTypeDef = TypedDict(
-    "SubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
-TagResourceResultTypeDef = TypedDict(
-    "TagResourceResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnsubscribeRequestRequestTypeDef = TypedDict(
     "UnsubscribeRequestRequestTypeDef",
     {
         "Arn": str,
         "TargetAddress": str,
     },
 )
 
-UnsubscribeResultTypeDef = TypedDict(
-    "UnsubscribeResultTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -279,20 +234,22 @@
         "ClientRequestToken": str,
         "Tags": Mapping[str, str],
         "Status": NotificationRuleStatusType,
     },
     total=False,
 )
 
+
 class CreateNotificationRuleRequestRequestTypeDef(
     _RequiredCreateNotificationRuleRequestRequestTypeDef,
     _OptionalCreateNotificationRuleRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSubscribeRequestRequestTypeDef = TypedDict(
     "_RequiredSubscribeRequestRequestTypeDef",
     {
         "Arn": str,
         "Target": TargetTypeDef,
     },
 )
@@ -300,19 +257,21 @@
     "_OptionalSubscribeRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class SubscribeRequestRequestTypeDef(
     _RequiredSubscribeRequestRequestTypeDef, _OptionalSubscribeRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateNotificationRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNotificationRuleRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalUpdateNotificationRuleRequestRequestTypeDef = TypedDict(
@@ -323,26 +282,76 @@
         "EventTypeIds": Sequence[str],
         "Targets": Sequence[TargetTypeDef],
         "DetailType": DetailTypeType,
     },
     total=False,
 )
 
+
 class UpdateNotificationRuleRequestRequestTypeDef(
     _RequiredUpdateNotificationRuleRequestRequestTypeDef,
     _OptionalUpdateNotificationRuleRequestRequestTypeDef,
 ):
     pass
 
+
+CreateNotificationRuleResultTypeDef = TypedDict(
+    "CreateNotificationRuleResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteNotificationRuleResultTypeDef = TypedDict(
+    "DeleteNotificationRuleResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubscribeResultTypeDef = TypedDict(
+    "SubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceResultTypeDef = TypedDict(
+    "TagResourceResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnsubscribeResultTypeDef = TypedDict(
+    "UnsubscribeResultTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEventTypesResultTypeDef = TypedDict(
     "ListEventTypesResultTypeDef",
     {
         "EventTypes": List[EventTypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationRuleResultTypeDef = TypedDict(
     "DescribeNotificationRuleResultTypeDef",
     {
         "Arn": str,
@@ -352,51 +361,51 @@
         "Targets": List[TargetSummaryTypeDef],
         "DetailType": DetailTypeType,
         "CreatedBy": str,
         "Status": NotificationRuleStatusType,
         "CreatedTimestamp": datetime,
         "LastModifiedTimestamp": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsResultTypeDef = TypedDict(
     "ListTargetsResultTypeDef",
     {
         "Targets": List[TargetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
-    "ListEventTypesRequestListEventTypesPaginateTypeDef",
+ListEventTypesRequestRequestTypeDef = TypedDict(
+    "ListEventTypesRequestRequestTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
-ListEventTypesRequestRequestTypeDef = TypedDict(
-    "ListEventTypesRequestRequestTypeDef",
+ListEventTypesRequestListEventTypesPaginateTypeDef = TypedDict(
+    "ListEventTypesRequestListEventTypesPaginateTypeDef",
     {
         "Filters": Sequence[ListEventTypesFilterTypeDef],
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNotificationRulesRequestListNotificationRulesPaginateTypeDef = TypedDict(
     "ListNotificationRulesRequestListNotificationRulesPaginateTypeDef",
     {
         "Filters": Sequence[ListNotificationRulesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNotificationRulesRequestRequestTypeDef = TypedDict(
     "ListNotificationRulesRequestRequestTypeDef",
     {
@@ -408,23 +417,23 @@
 )
 
 ListNotificationRulesResultTypeDef = TypedDict(
     "ListNotificationRulesResultTypeDef",
     {
         "NextToken": str,
         "NotificationRules": List[NotificationRuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
     "ListTargetsRequestListTargetsPaginateTypeDef",
     {
         "Filters": Sequence[ListTargetsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTargetsRequestRequestTypeDef = TypedDict(
     "ListTargetsRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications.egg-info/PKG-INFO` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-notifications
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeStarNotifications 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeStarNotifications 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-notifications.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-notifications)](https://pepy.tech/project/mypy-boto3-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarNotifications 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[boto3.CodeStarNotifications 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
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
 [mypy-boto3-codestar-notifications docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,43 +337,43 @@
 
 `mypy_boto3_codestar_notifications.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar_notifications.type_defs import (
     TargetTypeDef,
-    CreateNotificationRuleResultTypeDef,
+    ResponseMetadataTypeDef,
     DeleteNotificationRuleRequestRequestTypeDef,
-    DeleteNotificationRuleResultTypeDef,
     DeleteTargetRequestRequestTypeDef,
     DescribeNotificationRuleRequestRequestTypeDef,
     EventTypeSummaryTypeDef,
     TargetSummaryTypeDef,
     ListEventTypesFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListNotificationRulesFilterTypeDef,
     NotificationRuleSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     ListTargetsFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    SubscribeResultTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResultTypeDef,
     UnsubscribeRequestRequestTypeDef,
-    UnsubscribeResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateNotificationRuleRequestRequestTypeDef,
     SubscribeRequestRequestTypeDef,
     UpdateNotificationRuleRequestRequestTypeDef,
+    CreateNotificationRuleResultTypeDef,
+    DeleteNotificationRuleResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    SubscribeResultTypeDef,
+    TagResourceResultTypeDef,
+    UnsubscribeResultTypeDef,
     ListEventTypesResultTypeDef,
     DescribeNotificationRuleResultTypeDef,
     ListTargetsResultTypeDef,
-    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListEventTypesRequestRequestTypeDef,
+    ListEventTypesRequestListEventTypesPaginateTypeDef,
     ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
     ListNotificationRulesRequestRequestTypeDef,
     ListNotificationRulesResultTypeDef,
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-codestar-notifications-1.28.12/mypy_boto3_codestar_notifications.egg-info/SOURCES.txt` & `mypy-boto3-codestar-notifications-1.28.15/mypy_boto3_codestar_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-notifications-1.28.12/setup.py` & `mypy-boto3-codestar-notifications-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codestar-notifications",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_codestar_notifications"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeStarNotifications 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CodeStarNotifications 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

