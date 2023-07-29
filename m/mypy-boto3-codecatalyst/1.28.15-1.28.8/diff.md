# Comparing `tmp/mypy-boto3-codecatalyst-1.28.15.tar.gz` & `tmp/mypy-boto3-codecatalyst-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codecatalyst-1.28.15.tar", last modified: Fri Jul 28 20:42:28 2023, max compression
+gzip compressed data, was "mypy-boto3-codecatalyst-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-codecatalyst-1.28.15.tar` & `mypy-boto3-codecatalyst-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.584825 mypy-boto3-codecatalyst-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-28 20:42:28.584825 mypy-boto3-codecatalyst-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.572825 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27809 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-28 20:21:22.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-07-28 20:21:22.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39199 2023-07-28 20:21:23.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39130 2023-07-28 20:21:22.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.584825 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-28 20:42:28.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:28.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:28.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:28.000000 mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:28.584825 mypy-boto3-codecatalyst-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:21:21.000000 mypy-boto3-codecatalyst-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.012775 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27809 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37203 2023-07-20 19:46:46.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37150 2023-07-20 19:46:46.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/setup.py
```

### Comparing `mypy-boto3-codecatalyst-1.28.15/LICENSE` & `mypy-boto3-codecatalyst-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.15/PKG-INFO` & `mypy-boto3-codecatalyst-1.28.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.28.15
-Summary: Type annotations for boto3.CodeCatalyst 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.8
+Summary: Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecatalyst)](https://pepy.tech/project/mypy-boto3-codecatalyst)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -388,14 +388,15 @@
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
     GetSourceRepositoryRequestRequestTypeDef,
     GetSpaceRequestRequestTypeDef,
     GetSubscriptionRequestRequestTypeDef,
     GetUserDetailsRequestRequestTypeDef,
+    IdeConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
@@ -427,24 +428,24 @@
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    UpdateDevEnvironmentResponseTypeDef,
     ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSpacesRequestListSpacesPaginateTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.15/README.md` & `mypy-boto3-codecatalyst-1.28.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecatalyst)](https://pepy.tech/project/mypy-boto3-codecatalyst)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,14 +356,15 @@
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
     GetSourceRepositoryRequestRequestTypeDef,
     GetSpaceRequestRequestTypeDef,
     GetSubscriptionRequestRequestTypeDef,
     GetUserDetailsRequestRequestTypeDef,
+    IdeConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
@@ -395,24 +396,24 @@
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    UpdateDevEnvironmentResponseTypeDef,
     ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSpacesRequestListSpacesPaginateTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/__init__.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/__init__.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/__main__.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeCatalyst 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.CodeCatalyst 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/client.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/client.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/literals.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,14 @@
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
@@ -264,15 +263,14 @@
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
```

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/literals.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,14 @@
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
@@ -262,15 +261,14 @@
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
```

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/paginator.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/paginator.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/type_defs.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     "GetSourceRepositoryRequestRequestTypeDef",
     "GetSpaceRequestRequestTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
+    "IdeConfigurationOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
     "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
@@ -102,24 +103,24 @@
     "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
     "UpdateProjectResponseTypeDef",
     "UpdateSpaceResponseTypeDef",
     "VerifySessionResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
-    "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
     "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
     "ListDevEnvironmentsRequestRequestTypeDef",
+    "UpdateDevEnvironmentResponseTypeDef",
     "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
     "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     "ListEventLogsRequestListEventLogsPaginateTypeDef",
     "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSpacesRequestListSpacesPaginateTypeDef",
@@ -130,36 +131,23 @@
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     "ListDevEnvironmentsResponseTypeDef",
     "ListEventLogsResponseTypeDef",
 )
 
-_RequiredAccessTokenSummaryTypeDef = TypedDict(
-    "_RequiredAccessTokenSummaryTypeDef",
+AccessTokenSummaryTypeDef = TypedDict(
+    "AccessTokenSummaryTypeDef",
     {
         "id": str,
         "name": str,
-    },
-)
-_OptionalAccessTokenSummaryTypeDef = TypedDict(
-    "_OptionalAccessTokenSummaryTypeDef",
-    {
         "expiresTime": datetime,
     },
-    total=False,
 )
 
-
-class AccessTokenSummaryTypeDef(
-    _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
-):
-    pass
-
-
 _RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
@@ -338,35 +326,22 @@
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
 
-_RequiredDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentRepositorySummaryTypeDef",
+DevEnvironmentRepositorySummaryTypeDef = TypedDict(
+    "DevEnvironmentRepositorySummaryTypeDef",
     {
         "repositoryName": str,
-    },
-)
-_OptionalDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentRepositorySummaryTypeDef",
-    {
         "branchName": str,
     },
-    total=False,
 )
 
-
-class DevEnvironmentRepositorySummaryTypeDef(
-    _RequiredDevEnvironmentRepositorySummaryTypeDef, _OptionalDevEnvironmentRepositorySummaryTypeDef
-):
-    pass
-
-
 _RequiredExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_RequiredExecuteCommandSessionConfigurationTypeDef",
     {
         "command": str,
     },
 )
 _OptionalExecuteCommandSessionConfigurationTypeDef = TypedDict(
@@ -398,15 +373,14 @@
 
 IdeTypeDef = TypedDict(
     "IdeTypeDef",
     {
         "runtime": str,
         "name": str,
     },
-    total=False,
 )
 
 PersistentStorageTypeDef = TypedDict(
     "PersistentStorageTypeDef",
     {
         "sizeInGiB": int,
     },
@@ -414,56 +388,42 @@
 
 EmailAddressTypeDef = TypedDict(
     "EmailAddressTypeDef",
     {
         "email": str,
         "verified": bool,
     },
-    total=False,
 )
 
 EventPayloadTypeDef = TypedDict(
     "EventPayloadTypeDef",
     {
         "contentType": str,
         "data": str,
     },
-    total=False,
 )
 
 ProjectInformationTypeDef = TypedDict(
     "ProjectInformationTypeDef",
     {
         "name": str,
         "projectId": str,
     },
-    total=False,
 )
 
-_RequiredUserIdentityTypeDef = TypedDict(
-    "_RequiredUserIdentityTypeDef",
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
     {
         "userType": UserTypeType,
         "principalId": str,
-    },
-)
-_OptionalUserIdentityTypeDef = TypedDict(
-    "_OptionalUserIdentityTypeDef",
-    {
         "userName": str,
         "awsAccountId": str,
     },
-    total=False,
 )
 
-
-class UserIdentityTypeDef(_RequiredUserIdentityTypeDef, _OptionalUserIdentityTypeDef):
-    pass
-
-
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "key": str,
         "values": Sequence[str],
     },
 )
@@ -534,14 +494,22 @@
     {
         "id": str,
         "userName": str,
     },
     total=False,
 )
 
+IdeConfigurationOutputTypeDef = TypedDict(
+    "IdeConfigurationOutputTypeDef",
+    {
+        "runtime": str,
+        "name": str,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -625,57 +593,33 @@
 
 class ProjectListFilterTypeDef(
     _RequiredProjectListFilterTypeDef, _OptionalProjectListFilterTypeDef
 ):
     pass
 
 
-_RequiredProjectSummaryTypeDef = TypedDict(
-    "_RequiredProjectSummaryTypeDef",
+ProjectSummaryTypeDef = TypedDict(
+    "ProjectSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalProjectSummaryTypeDef = TypedDict(
-    "_OptionalProjectSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-
-class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
-    pass
-
-
-_RequiredListSourceRepositoriesItemTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesItemTypeDef",
+ListSourceRepositoriesItemTypeDef = TypedDict(
+    "ListSourceRepositoriesItemTypeDef",
     {
         "id": str,
         "name": str,
+        "description": str,
         "lastUpdatedTime": datetime,
         "createdTime": datetime,
     },
 )
-_OptionalListSourceRepositoriesItemTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesItemTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoriesItemTypeDef(
-    _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
-):
-    pass
-
 
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
@@ -701,15 +645,14 @@
     "ListSourceRepositoryBranchesItemTypeDef",
     {
         "ref": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
-    total=False,
 )
 
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
@@ -737,35 +680,24 @@
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredSpaceSummaryTypeDef = TypedDict(
-    "_RequiredSpaceSummaryTypeDef",
+SpaceSummaryTypeDef = TypedDict(
+    "SpaceSummaryTypeDef",
     {
         "name": str,
         "regionName": str,
-    },
-)
-_OptionalSpaceSummaryTypeDef = TypedDict(
-    "_OptionalSpaceSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-
-class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
-    pass
-
-
 StopDevEnvironmentRequestRequestTypeDef = TypedDict(
     "StopDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
@@ -1090,29 +1022,14 @@
 class UpdateDevEnvironmentRequestRequestTypeDef(
     _RequiredUpdateDevEnvironmentRequestRequestTypeDef,
     _OptionalUpdateDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateDevEnvironmentResponseTypeDef = TypedDict(
-    "UpdateDevEnvironmentResponseTypeDef",
-    {
-        "id": str,
-        "spaceName": str,
-        "projectName": str,
-        "alias": str,
-        "ides": List[IdeConfigurationTypeDef],
-        "instanceType": InstanceTypeType,
-        "inactivityTimeoutMinutes": int,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "instanceType": InstanceTypeType,
         "persistentStorage": PersistentStorageConfigurationTypeDef,
@@ -1177,45 +1094,32 @@
     {
         "items": List[DevEnvironmentSessionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDevEnvironmentSummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentSummaryTypeDef",
+DevEnvironmentSummaryTypeDef = TypedDict(
+    "DevEnvironmentSummaryTypeDef",
     {
+        "spaceName": str,
+        "projectName": str,
         "id": str,
         "lastUpdatedTime": datetime,
         "creatorId": str,
         "status": DevEnvironmentStatusType,
+        "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
+        "alias": str,
+        "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
     },
 )
-_OptionalDevEnvironmentSummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentSummaryTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "statusReason": str,
-        "alias": str,
-        "ides": List[IdeTypeDef],
-    },
-    total=False,
-)
-
-
-class DevEnvironmentSummaryTypeDef(
-    _RequiredDevEnvironmentSummaryTypeDef, _OptionalDevEnvironmentSummaryTypeDef
-):
-    pass
-
 
 GetDevEnvironmentResponseTypeDef = TypedDict(
     "GetDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
@@ -1241,46 +1145,35 @@
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEventLogEntryTypeDef = TypedDict(
-    "_RequiredEventLogEntryTypeDef",
+EventLogEntryTypeDef = TypedDict(
+    "EventLogEntryTypeDef",
     {
         "id": str,
         "eventName": str,
         "eventType": str,
         "eventCategory": str,
         "eventSource": str,
         "eventTime": datetime,
         "operationType": OperationTypeType,
         "userIdentity": UserIdentityTypeDef,
-    },
-)
-_OptionalEventLogEntryTypeDef = TypedDict(
-    "_OptionalEventLogEntryTypeDef",
-    {
         "projectInformation": ProjectInformationTypeDef,
         "requestId": str,
         "requestPayload": EventPayloadTypeDef,
         "responsePayload": EventPayloadTypeDef,
         "errorCode": str,
         "sourceIpAddress": str,
         "userAgent": str,
     },
-    total=False,
 )
 
-
-class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
-    pass
-
-
 _RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
@@ -1298,14 +1191,29 @@
 class ListDevEnvironmentsRequestRequestTypeDef(
     _RequiredListDevEnvironmentsRequestRequestTypeDef,
     _OptionalListDevEnvironmentsRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateDevEnvironmentResponseTypeDef = TypedDict(
+    "UpdateDevEnvironmentResponseTypeDef",
+    {
+        "id": str,
+        "spaceName": str,
+        "projectName": str,
+        "alias": str,
+        "ides": List[IdeConfigurationOutputTypeDef],
+        "instanceType": InstanceTypeType,
+        "inactivityTimeoutMinutes": int,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
     "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst/type_defs.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     "GetSourceRepositoryRequestRequestTypeDef",
     "GetSpaceRequestRequestTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
+    "IdeConfigurationOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
     "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
@@ -101,24 +102,24 @@
     "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
     "UpdateProjectResponseTypeDef",
     "UpdateSpaceResponseTypeDef",
     "VerifySessionResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
-    "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
     "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
     "ListDevEnvironmentsRequestRequestTypeDef",
+    "UpdateDevEnvironmentResponseTypeDef",
     "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
     "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     "ListEventLogsRequestListEventLogsPaginateTypeDef",
     "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSpacesRequestListSpacesPaginateTypeDef",
@@ -129,34 +130,23 @@
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     "ListDevEnvironmentsResponseTypeDef",
     "ListEventLogsResponseTypeDef",
 )
 
-_RequiredAccessTokenSummaryTypeDef = TypedDict(
-    "_RequiredAccessTokenSummaryTypeDef",
+AccessTokenSummaryTypeDef = TypedDict(
+    "AccessTokenSummaryTypeDef",
     {
         "id": str,
         "name": str,
-    },
-)
-_OptionalAccessTokenSummaryTypeDef = TypedDict(
-    "_OptionalAccessTokenSummaryTypeDef",
-    {
         "expiresTime": datetime,
     },
-    total=False,
 )
 
-class AccessTokenSummaryTypeDef(
-    _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
-):
-    pass
-
 _RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
@@ -325,33 +315,22 @@
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
 
-_RequiredDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentRepositorySummaryTypeDef",
+DevEnvironmentRepositorySummaryTypeDef = TypedDict(
+    "DevEnvironmentRepositorySummaryTypeDef",
     {
         "repositoryName": str,
-    },
-)
-_OptionalDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentRepositorySummaryTypeDef",
-    {
         "branchName": str,
     },
-    total=False,
 )
 
-class DevEnvironmentRepositorySummaryTypeDef(
-    _RequiredDevEnvironmentRepositorySummaryTypeDef, _OptionalDevEnvironmentRepositorySummaryTypeDef
-):
-    pass
-
 _RequiredExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_RequiredExecuteCommandSessionConfigurationTypeDef",
     {
         "command": str,
     },
 )
 _OptionalExecuteCommandSessionConfigurationTypeDef = TypedDict(
@@ -381,15 +360,14 @@
 
 IdeTypeDef = TypedDict(
     "IdeTypeDef",
     {
         "runtime": str,
         "name": str,
     },
-    total=False,
 )
 
 PersistentStorageTypeDef = TypedDict(
     "PersistentStorageTypeDef",
     {
         "sizeInGiB": int,
     },
@@ -397,54 +375,42 @@
 
 EmailAddressTypeDef = TypedDict(
     "EmailAddressTypeDef",
     {
         "email": str,
         "verified": bool,
     },
-    total=False,
 )
 
 EventPayloadTypeDef = TypedDict(
     "EventPayloadTypeDef",
     {
         "contentType": str,
         "data": str,
     },
-    total=False,
 )
 
 ProjectInformationTypeDef = TypedDict(
     "ProjectInformationTypeDef",
     {
         "name": str,
         "projectId": str,
     },
-    total=False,
 )
 
-_RequiredUserIdentityTypeDef = TypedDict(
-    "_RequiredUserIdentityTypeDef",
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
     {
         "userType": UserTypeType,
         "principalId": str,
-    },
-)
-_OptionalUserIdentityTypeDef = TypedDict(
-    "_OptionalUserIdentityTypeDef",
-    {
         "userName": str,
         "awsAccountId": str,
     },
-    total=False,
 )
 
-class UserIdentityTypeDef(_RequiredUserIdentityTypeDef, _OptionalUserIdentityTypeDef):
-    pass
-
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "key": str,
         "values": Sequence[str],
     },
 )
@@ -513,14 +479,22 @@
     {
         "id": str,
         "userName": str,
     },
     total=False,
 )
 
+IdeConfigurationOutputTypeDef = TypedDict(
+    "IdeConfigurationOutputTypeDef",
+    {
+        "runtime": str,
+        "name": str,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -598,53 +572,33 @@
 )
 
 class ProjectListFilterTypeDef(
     _RequiredProjectListFilterTypeDef, _OptionalProjectListFilterTypeDef
 ):
     pass
 
-_RequiredProjectSummaryTypeDef = TypedDict(
-    "_RequiredProjectSummaryTypeDef",
+ProjectSummaryTypeDef = TypedDict(
+    "ProjectSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalProjectSummaryTypeDef = TypedDict(
-    "_OptionalProjectSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
-    pass
-
-_RequiredListSourceRepositoriesItemTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesItemTypeDef",
+ListSourceRepositoriesItemTypeDef = TypedDict(
+    "ListSourceRepositoriesItemTypeDef",
     {
         "id": str,
         "name": str,
+        "description": str,
         "lastUpdatedTime": datetime,
         "createdTime": datetime,
     },
 )
-_OptionalListSourceRepositoriesItemTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesItemTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-class ListSourceRepositoriesItemTypeDef(
-    _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
-):
-    pass
 
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
@@ -668,15 +622,14 @@
     "ListSourceRepositoryBranchesItemTypeDef",
     {
         "ref": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
-    total=False,
 )
 
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
@@ -702,33 +655,24 @@
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredSpaceSummaryTypeDef = TypedDict(
-    "_RequiredSpaceSummaryTypeDef",
+SpaceSummaryTypeDef = TypedDict(
+    "SpaceSummaryTypeDef",
     {
         "name": str,
         "regionName": str,
-    },
-)
-_OptionalSpaceSummaryTypeDef = TypedDict(
-    "_OptionalSpaceSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
-    pass
-
 StopDevEnvironmentRequestRequestTypeDef = TypedDict(
     "StopDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
@@ -1045,29 +989,14 @@
 
 class UpdateDevEnvironmentRequestRequestTypeDef(
     _RequiredUpdateDevEnvironmentRequestRequestTypeDef,
     _OptionalUpdateDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
-UpdateDevEnvironmentResponseTypeDef = TypedDict(
-    "UpdateDevEnvironmentResponseTypeDef",
-    {
-        "id": str,
-        "spaceName": str,
-        "projectName": str,
-        "alias": str,
-        "ides": List[IdeConfigurationTypeDef],
-        "instanceType": InstanceTypeType,
-        "inactivityTimeoutMinutes": int,
-        "clientToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "instanceType": InstanceTypeType,
         "persistentStorage": PersistentStorageConfigurationTypeDef,
@@ -1128,43 +1057,32 @@
     {
         "items": List[DevEnvironmentSessionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDevEnvironmentSummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentSummaryTypeDef",
+DevEnvironmentSummaryTypeDef = TypedDict(
+    "DevEnvironmentSummaryTypeDef",
     {
+        "spaceName": str,
+        "projectName": str,
         "id": str,
         "lastUpdatedTime": datetime,
         "creatorId": str,
         "status": DevEnvironmentStatusType,
+        "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
+        "alias": str,
+        "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
     },
 )
-_OptionalDevEnvironmentSummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentSummaryTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "statusReason": str,
-        "alias": str,
-        "ides": List[IdeTypeDef],
-    },
-    total=False,
-)
-
-class DevEnvironmentSummaryTypeDef(
-    _RequiredDevEnvironmentSummaryTypeDef, _OptionalDevEnvironmentSummaryTypeDef
-):
-    pass
 
 GetDevEnvironmentResponseTypeDef = TypedDict(
     "GetDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
@@ -1190,44 +1108,35 @@
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEventLogEntryTypeDef = TypedDict(
-    "_RequiredEventLogEntryTypeDef",
+EventLogEntryTypeDef = TypedDict(
+    "EventLogEntryTypeDef",
     {
         "id": str,
         "eventName": str,
         "eventType": str,
         "eventCategory": str,
         "eventSource": str,
         "eventTime": datetime,
         "operationType": OperationTypeType,
         "userIdentity": UserIdentityTypeDef,
-    },
-)
-_OptionalEventLogEntryTypeDef = TypedDict(
-    "_OptionalEventLogEntryTypeDef",
-    {
         "projectInformation": ProjectInformationTypeDef,
         "requestId": str,
         "requestPayload": EventPayloadTypeDef,
         "responsePayload": EventPayloadTypeDef,
         "errorCode": str,
         "sourceIpAddress": str,
         "userAgent": str,
     },
-    total=False,
 )
 
-class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
-    pass
-
 _RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
@@ -1243,14 +1152,29 @@
 
 class ListDevEnvironmentsRequestRequestTypeDef(
     _RequiredListDevEnvironmentsRequestRequestTypeDef,
     _OptionalListDevEnvironmentsRequestRequestTypeDef,
 ):
     pass
 
+UpdateDevEnvironmentResponseTypeDef = TypedDict(
+    "UpdateDevEnvironmentResponseTypeDef",
+    {
+        "id": str,
+        "spaceName": str,
+        "projectName": str,
+        "alias": str,
+        "ides": List[IdeConfigurationOutputTypeDef],
+        "instanceType": InstanceTypeType,
+        "inactivityTimeoutMinutes": int,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
     "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst.egg-info/PKG-INFO` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.28.15
-Summary: Type annotations for boto3.CodeCatalyst 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.8
+Summary: Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecatalyst)](https://pepy.tech/project/mypy-boto3-codecatalyst)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -388,14 +388,15 @@
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
     GetSourceRepositoryRequestRequestTypeDef,
     GetSpaceRequestRequestTypeDef,
     GetSubscriptionRequestRequestTypeDef,
     GetUserDetailsRequestRequestTypeDef,
+    IdeConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
@@ -427,24 +428,24 @@
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    UpdateDevEnvironmentResponseTypeDef,
     ListAccessTokensRequestListAccessTokensPaginateTypeDef,
     ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSpacesRequestListSpacesPaginateTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.15/mypy_boto3_codecatalyst.egg-info/SOURCES.txt` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.15/setup.py` & `mypy-boto3-codecatalyst-1.28.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codecatalyst",
-    version="1.28.15",
+    version="1.28.8",
     packages=["mypy_boto3_codecatalyst"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeCatalyst 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        "Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

