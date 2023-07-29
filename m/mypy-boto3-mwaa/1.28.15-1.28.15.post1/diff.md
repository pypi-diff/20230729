# Comparing `tmp/mypy-boto3-mwaa-1.28.15.tar.gz` & `tmp/mypy-boto3-mwaa-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mwaa-1.28.15.tar", last modified: Fri Jul 28 20:43:21 2023, max compression
+gzip compressed data, was "mypy-boto3-mwaa-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:45 2023, max compression
```

## Comparing `mypy-boto3-mwaa-1.28.15.tar` & `mypy-boto3-mwaa-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.429558 mypy-boto3-mwaa-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-28 20:43:21.429558 mypy-boto3-mwaa-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.429558 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.429558 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:21.429558 mypy-boto3-mwaa-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-28 20:32:14.000000 mypy-boto3-mwaa-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:45.185304 mypy-boto3-mwaa-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-07-29 10:03:45.177304 mypy-boto3-mwaa-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:45.173304 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:56.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:45.177304 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:03:44.000000 mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:45.185304 mypy-boto3-mwaa-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-29 09:51:55.000000 mypy-boto3-mwaa-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-mwaa-1.28.15/LICENSE` & `mypy-boto3-mwaa-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15/PKG-INFO` & `mypy-boto3-mwaa-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.28.15
-Summary: Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
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
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mwaa-1.28.15/README.md` & `mypy-boto3-mwaa-1.28.15.post1/README.md`

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
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__init__.py` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__init__.pyi` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__main__.py` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MWAA 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.MWAA 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA\nOther"
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

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/client.py` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,30 @@
     from mypy_boto3_mwaa.client import MWAAClient
 
     session = Session()
     client: MWAAClient = session.client("mwaa")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import WebserverAccessModeType
 from .paginator import ListEnvironmentsPaginator
 from .type_defs import (
     CreateCliTokenResponseTypeDef,
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     GetEnvironmentOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationInputTypeDef,
     MetricDatumTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -102,15 +103,15 @@
 
     def create_environment(
         self,
         *,
         DagS3Path: str,
         ExecutionRoleArn: str,
         Name: str,
-        NetworkConfiguration: NetworkConfigurationTypeDef,
+        NetworkConfiguration: Union[NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef],
         SourceBucketArn: str,
         AirflowConfigurationOptions: Mapping[str, str] = ...,
         AirflowVersion: str = ...,
         EnvironmentClass: str = ...,
         KmsKey: str = ...,
         LoggingConfiguration: LoggingConfigurationInputTypeDef = ...,
         MaxWorkers: int = ...,
```

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/client.pyi` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,30 @@
     from mypy_boto3_mwaa.client import MWAAClient
 
     session = Session()
     client: MWAAClient = session.client("mwaa")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import WebserverAccessModeType
 from .paginator import ListEnvironmentsPaginator
 from .type_defs import (
     CreateCliTokenResponseTypeDef,
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     GetEnvironmentOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationInputTypeDef,
     MetricDatumTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -94,15 +95,15 @@
         """
     def create_environment(
         self,
         *,
         DagS3Path: str,
         ExecutionRoleArn: str,
         Name: str,
-        NetworkConfiguration: NetworkConfigurationTypeDef,
+        NetworkConfiguration: Union[NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef],
         SourceBucketArn: str,
         AirflowConfigurationOptions: Mapping[str, str] = ...,
         AirflowVersion: str = ...,
         EnvironmentClass: str = ...,
         KmsKey: str = ...,
         LoggingConfiguration: LoggingConfigurationInputTypeDef = ...,
         MaxWorkers: int = ...,
```

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/literals.py` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/literals.pyi` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/paginator.py` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/paginator.pyi` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/type_defs.py` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/type_defs.pyi` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/PKG-INFO` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.28.15
-Summary: Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
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
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/SOURCES.txt` & `mypy-boto3-mwaa-1.28.15.post1/mypy_boto3_mwaa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.15/setup.py` & `mypy-boto3-mwaa-1.28.15.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mwaa",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_mwaa"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

