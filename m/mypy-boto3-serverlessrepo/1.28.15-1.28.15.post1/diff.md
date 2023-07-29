# Comparing `tmp/mypy-boto3-serverlessrepo-1.28.15.tar.gz` & `tmp/mypy-boto3-serverlessrepo-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-serverlessrepo-1.28.15.tar", last modified: Fri Jul 28 20:43:43 2023, max compression
+gzip compressed data, was "mypy-boto3-serverlessrepo-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:10 2023, max compression
```

## Comparing `mypy-boto3-serverlessrepo-1.28.15.tar` & `mypy-boto3-serverlessrepo-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:43.025854 mypy-boto3-serverlessrepo-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-28 20:43:43.021854 mypy-boto3-serverlessrepo-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:43.021854 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19929 2023-07-28 20:39:06.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19897 2023-07-28 20:39:06.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:43.021854 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:43.025854 mypy-boto3-serverlessrepo-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:10.033395 mypy-boto3-serverlessrepo-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15374 2023-07-29 10:04:10.033395 mypy-boto3-serverlessrepo-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:10.033395 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-07-29 09:59:16.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:10.033395 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15374 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:10.033395 mypy-boto3-serverlessrepo-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15/LICENSE` & `mypy-boto3-serverlessrepo-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15/PKG-INFO` & `mypy-boto3-serverlessrepo-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-serverlessrepo
-Version: 1.28.15
-Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15/README.md` & `mypy-boto3-serverlessrepo-1.28.15.post1/README.md`

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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__init__.py` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__init__.pyi` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__main__.py` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.ServerlessApplicationRepository 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository\nOther"
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

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/client.py` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,24 +10,25 @@
     from mypy_boto3_serverlessrepo.client import ServerlessApplicationRepositoryClient
 
     session = Session()
     client: ServerlessApplicationRepositoryClient = session.client("serverlessrepo")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListApplicationDependenciesPaginator,
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
 )
 from .type_defs import (
+    ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     CreateApplicationResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
@@ -263,15 +264,20 @@
         Lists applications owned by the requester.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/client/#list_applications)
         """
 
     def put_application_policy(
-        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementTypeDef]
+        self,
+        *,
+        ApplicationId: str,
+        Statements: Sequence[
+            Union[ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef]
+        ]
     ) -> PutApplicationPolicyResponseTypeDef:
         """
         Sets the permission policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.put_application_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/client/#put_application_policy)
         """
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/client.pyi` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,25 @@
     from mypy_boto3_serverlessrepo.client import ServerlessApplicationRepositoryClient
 
     session = Session()
     client: ServerlessApplicationRepositoryClient = session.client("serverlessrepo")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListApplicationDependenciesPaginator,
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
 )
 from .type_defs import (
+    ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     CreateApplicationResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
@@ -244,15 +245,20 @@
         """
         Lists applications owned by the requester.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/client/#list_applications)
         """
     def put_application_policy(
-        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementTypeDef]
+        self,
+        *,
+        ApplicationId: str,
+        Statements: Sequence[
+            Union[ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef]
+        ]
     ) -> PutApplicationPolicyResponseTypeDef:
         """
         Sets the permission policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.put_application_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/client/#put_application_policy)
         """
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/literals.py` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/literals.pyi` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/paginator.py` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/paginator.pyi` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/type_defs.py` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
     data: ApplicationDependencySummaryTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import CapabilityType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -463,15 +463,17 @@
     pass
 
 
 PutApplicationPolicyRequestRequestTypeDef = TypedDict(
     "PutApplicationPolicyRequestRequestTypeDef",
     {
         "ApplicationId": str,
-        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
+        "Statements": Sequence[
+            Union[ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef]
+        ],
     },
 )
 
 CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
     "CreateCloudFormationChangeSetResponseTypeDef",
     {
         "ApplicationId": str,
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/type_defs.pyi` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
     data: ApplicationDependencySummaryTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import CapabilityType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -438,15 +438,17 @@
 ):
     pass
 
 PutApplicationPolicyRequestRequestTypeDef = TypedDict(
     "PutApplicationPolicyRequestRequestTypeDef",
     {
         "ApplicationId": str,
-        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
+        "Statements": Sequence[
+            Union[ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef]
+        ],
     },
 )
 
 CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
     "CreateCloudFormationChangeSetResponseTypeDef",
     {
         "ApplicationId": str,
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/PKG-INFO` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-serverlessrepo
-Version: 1.28.15
-Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt` & `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15/setup.py` & `mypy-boto3-serverlessrepo-1.28.15.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-serverlessrepo",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_serverlessrepo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with"
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

