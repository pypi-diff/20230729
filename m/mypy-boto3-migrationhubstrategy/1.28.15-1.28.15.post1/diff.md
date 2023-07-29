# Comparing `tmp/mypy-boto3-migrationhubstrategy-1.28.15.tar.gz` & `tmp/mypy-boto3-migrationhubstrategy-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhubstrategy-1.28.15.tar", last modified: Fri Jul 28 20:43:20 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhubstrategy-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:44 2023, max compression
```

## Comparing `mypy-boto3-migrationhubstrategy-1.28.15.tar` & `mypy-boto3-migrationhubstrategy-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.841550 mypy-boto3-migrationhubstrategy-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19266 2023-07-28 20:43:20.841550 mypy-boto3-migrationhubstrategy-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.825550 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-07-28 20:32:06.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34508 2023-07-28 20:32:09.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34497 2023-07-28 20:32:06.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.841550 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19266 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:20.841550 mypy-boto3-migrationhubstrategy-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.229300 mypy-boto3-migrationhubstrategy-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19272 2023-07-29 10:03:44.221300 mypy-boto3-migrationhubstrategy-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.209300 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21098 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-07-29 09:51:47.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-07-29 09:51:47.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34564 2023-07-29 09:51:47.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.221300 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19272 2023-07-29 10:03:43.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 10:03:44.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:43.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-29 10:03:43.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:44.229300 mypy-boto3-migrationhubstrategy-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/LICENSE` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/PKG-INFO` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhubstrategy
-Version: 1.28.15
-Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/README.md` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/README.md`

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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__init__.py` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__init__.pyi` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__main__.py` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations\nOther"
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

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/client.py` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
 
     session = Session()
     client: MigrationHubStrategyRecommendationsClient = session.client("migrationhubstrategy")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApplicationComponentCriteriaType,
     ApplicationModeType,
     AppTypeType,
@@ -32,16 +32,19 @@
     GetServerDetailsPaginator,
     ListApplicationComponentsPaginator,
     ListCollectorsPaginator,
     ListImportFileTaskPaginator,
     ListServersPaginator,
 )
 from .type_defs import (
+    ApplicationPreferencesOutputTypeDef,
     ApplicationPreferencesTypeDef,
+    AssessmentTargetOutputTypeDef,
     AssessmentTargetTypeDef,
+    DatabasePreferencesOutputTypeDef,
     DatabasePreferencesTypeDef,
     GetApplicationComponentDetailsResponseTypeDef,
     GetApplicationComponentStrategiesResponseTypeDef,
     GetAssessmentResponseTypeDef,
     GetImportFileTaskResponseTypeDef,
     GetLatestAssessmentIdResponseTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
@@ -283,29 +286,35 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/client/#list_servers)
         """
 
     def put_portfolio_preferences(
         self,
         *,
         applicationMode: ApplicationModeType = ...,
-        applicationPreferences: ApplicationPreferencesTypeDef = ...,
-        databasePreferences: DatabasePreferencesTypeDef = ...,
+        applicationPreferences: Union[
+            ApplicationPreferencesTypeDef, ApplicationPreferencesOutputTypeDef
+        ] = ...,
+        databasePreferences: Union[
+            DatabasePreferencesTypeDef, DatabasePreferencesOutputTypeDef
+        ] = ...,
         prioritizeBusinessGoals: PrioritizeBusinessGoalsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Saves the specified migration and modernization preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.put_portfolio_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/client/#put_portfolio_preferences)
         """
 
     def start_assessment(
         self,
         *,
-        assessmentTargets: Sequence[AssessmentTargetTypeDef] = ...,
+        assessmentTargets: Sequence[
+            Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
+        ] = ...,
         s3bucketForAnalysisData: str = ...,
         s3bucketForReportData: str = ...
     ) -> StartAssessmentResponseTypeDef:
         """
         Starts the assessment of an on-premises environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.start_assessment)
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/client.pyi` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
 
     session = Session()
     client: MigrationHubStrategyRecommendationsClient = session.client("migrationhubstrategy")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApplicationComponentCriteriaType,
     ApplicationModeType,
     AppTypeType,
@@ -32,16 +32,19 @@
     GetServerDetailsPaginator,
     ListApplicationComponentsPaginator,
     ListCollectorsPaginator,
     ListImportFileTaskPaginator,
     ListServersPaginator,
 )
 from .type_defs import (
+    ApplicationPreferencesOutputTypeDef,
     ApplicationPreferencesTypeDef,
+    AssessmentTargetOutputTypeDef,
     AssessmentTargetTypeDef,
+    DatabasePreferencesOutputTypeDef,
     DatabasePreferencesTypeDef,
     GetApplicationComponentDetailsResponseTypeDef,
     GetApplicationComponentStrategiesResponseTypeDef,
     GetAssessmentResponseTypeDef,
     GetImportFileTaskResponseTypeDef,
     GetLatestAssessmentIdResponseTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
@@ -261,28 +264,34 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.list_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/client/#list_servers)
         """
     def put_portfolio_preferences(
         self,
         *,
         applicationMode: ApplicationModeType = ...,
-        applicationPreferences: ApplicationPreferencesTypeDef = ...,
-        databasePreferences: DatabasePreferencesTypeDef = ...,
+        applicationPreferences: Union[
+            ApplicationPreferencesTypeDef, ApplicationPreferencesOutputTypeDef
+        ] = ...,
+        databasePreferences: Union[
+            DatabasePreferencesTypeDef, DatabasePreferencesOutputTypeDef
+        ] = ...,
         prioritizeBusinessGoals: PrioritizeBusinessGoalsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Saves the specified migration and modernization preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.put_portfolio_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/client/#put_portfolio_preferences)
         """
     def start_assessment(
         self,
         *,
-        assessmentTargets: Sequence[AssessmentTargetTypeDef] = ...,
+        assessmentTargets: Sequence[
+            Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
+        ] = ...,
         s3bucketForAnalysisData: str = ...,
         s3bucketForReportData: str = ...
     ) -> StartAssessmentResponseTypeDef:
         """
         Starts the assessment of an on-premises environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.start_assessment)
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/literals.py` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/literals.pyi` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/paginator.py` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/paginator.pyi` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/type_defs.py` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_migrationhubstrategy.type_defs import AnalysisStatusUnionTypeDef
 
     data: AnalysisStatusUnionTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AnalysisTypeType,
     AntipatternReportStatusType,
     ApplicationComponentCriteriaType,
     ApplicationModeType,
     AppTypeType,
@@ -707,15 +707,17 @@
     },
     total=False,
 )
 
 StartAssessmentRequestRequestTypeDef = TypedDict(
     "StartAssessmentRequestRequestTypeDef",
     {
-        "assessmentTargets": Sequence[AssessmentTargetTypeDef],
+        "assessmentTargets": Sequence[
+            Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
+        ],
         "s3bucketForAnalysisData": str,
         "s3bucketForReportData": str,
     },
     total=False,
 )
 
 PrioritizeBusinessGoalsTypeDef = TypedDict(
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/type_defs.pyi` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_migrationhubstrategy.type_defs import AnalysisStatusUnionTypeDef
 
     data: AnalysisStatusUnionTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AnalysisTypeType,
     AntipatternReportStatusType,
     ApplicationComponentCriteriaType,
     ApplicationModeType,
     AppTypeType,
@@ -704,15 +704,17 @@
     },
     total=False,
 )
 
 StartAssessmentRequestRequestTypeDef = TypedDict(
     "StartAssessmentRequestRequestTypeDef",
     {
-        "assessmentTargets": Sequence[AssessmentTargetTypeDef],
+        "assessmentTargets": Sequence[
+            Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
+        ],
         "s3bucketForAnalysisData": str,
         "s3bucketForReportData": str,
     },
     total=False,
 )
 
 PrioritizeBusinessGoalsTypeDef = TypedDict(
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhubstrategy
-Version: 1.28.15
-Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15/setup.py` & `mypy-boto3-migrationhubstrategy-1.28.15.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhubstrategy",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_migrationhubstrategy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated"
-        " with mypy-boto3-builder 7.16.1"
+        " with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

