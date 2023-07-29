# Comparing `tmp/mypy-boto3-amplifybackend-1.28.15.tar.gz` & `tmp/mypy-boto3-amplifybackend-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplifybackend-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
+gzip compressed data, was "mypy-boto3-amplifybackend-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:27 2023, max compression
```

## Comparing `mypy-boto3-amplifybackend-1.28.15.tar` & `mypy-boto3-amplifybackend-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.676609 mypy-boto3-amplifybackend-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-07-28 20:42:12.676609 mypy-boto3-amplifybackend-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.676609 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23022 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22983 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44075 2023-07-28 20:18:54.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44010 2023-07-28 20:18:53.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.676609 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.676609 mypy-boto3-amplifybackend-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.704993 mypy-boto3-amplifybackend-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17588 2023-07-29 10:02:27.700993 mypy-boto3-amplifybackend-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.688993 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-07-29 09:37:42.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-07-29 09:37:42.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-29 09:37:43.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-29 09:37:43.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-29 09:37:42.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-29 09:37:42.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44075 2023-07-29 09:37:44.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44010 2023-07-29 09:37:43.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.696993 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17588 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:02:27.000000 mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:27.704993 mypy-boto3-amplifybackend-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:37:41.000000 mypy-boto3-amplifybackend-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-amplifybackend-1.28.15/LICENSE` & `mypy-boto3-amplifybackend-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15/PKG-INFO` & `mypy-boto3-amplifybackend-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifybackend
-Version: 1.28.15
-Summary: Type annotations for boto3.AmplifyBackend 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AmplifyBackend 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-amplifybackend-1.28.15/README.md` & `mypy-boto3-amplifybackend-1.28.15.post1/README.md`

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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__init__.py` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__init__.pyi` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__main__.py` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AmplifyBackend 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.AmplifyBackend 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend\nOther"
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

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/client.py` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,25 @@
     from mypy_boto3_amplifybackend.client import AmplifyBackendClient
 
     session = Session()
     client: AmplifyBackendClient = session.client("amplifybackend")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Type
+from typing import Any, Dict, Mapping, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListBackendJobsPaginator
 from .type_defs import (
+    BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
+    CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResponseTypeDef,
     CreateTokenResponseTypeDef,
@@ -144,30 +146,34 @@
         """
 
     def create_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef,
+        ResourceConfig: Union[
+            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+        ],
         ResourceName: str
     ) -> CreateBackendAPIResponseTypeDef:
         """
         Creates a new backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#create_backend_api)
         """
 
     def create_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: CreateBackendAuthResourceConfigTypeDef,
+        ResourceConfig: Union[
+            CreateBackendAuthResourceConfigTypeDef, CreateBackendAuthResourceConfigOutputTypeDef
+        ],
         ResourceName: str
     ) -> CreateBackendAuthResponseTypeDef:
         """
         Creates a new backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#create_backend_auth)
@@ -219,15 +225,17 @@
 
     def delete_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: Union[
+            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+        ] = ...
     ) -> DeleteBackendAPIResponseTypeDef:
         """
         Deletes an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#delete_backend_api)
         """
@@ -301,15 +309,17 @@
 
     def get_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: Union[
+            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+        ] = ...
     ) -> GetBackendAPIResponseTypeDef:
         """
         Gets the details for a backend API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.get_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#get_backend_api)
         """
@@ -440,15 +450,17 @@
 
     def update_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: Union[
+            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+        ] = ...
     ) -> UpdateBackendAPIResponseTypeDef:
         """
         Updates an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#update_backend_api)
         """
```

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/client.pyi` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,25 @@
     from mypy_boto3_amplifybackend.client import AmplifyBackendClient
 
     session = Session()
     client: AmplifyBackendClient = session.client("amplifybackend")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Type
+from typing import Any, Dict, Mapping, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListBackendJobsPaginator
 from .type_defs import (
+    BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
+    CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResponseTypeDef,
     CreateTokenResponseTypeDef,
@@ -135,29 +137,33 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#create_backend)
         """
     def create_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef,
+        ResourceConfig: Union[
+            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+        ],
         ResourceName: str
     ) -> CreateBackendAPIResponseTypeDef:
         """
         Creates a new backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#create_backend_api)
         """
     def create_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: CreateBackendAuthResourceConfigTypeDef,
+        ResourceConfig: Union[
+            CreateBackendAuthResourceConfigTypeDef, CreateBackendAuthResourceConfigOutputTypeDef
+        ],
         ResourceName: str
     ) -> CreateBackendAuthResponseTypeDef:
         """
         Creates a new backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#create_backend_auth)
@@ -204,15 +210,17 @@
         """
     def delete_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: Union[
+            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+        ] = ...
     ) -> DeleteBackendAPIResponseTypeDef:
         """
         Deletes an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#delete_backend_api)
         """
@@ -279,15 +287,17 @@
         """
     def get_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: Union[
+            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+        ] = ...
     ) -> GetBackendAPIResponseTypeDef:
         """
         Gets the details for a backend API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.get_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#get_backend_api)
         """
@@ -406,15 +416,17 @@
         """
     def update_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
+        ResourceConfig: Union[
+            BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
+        ] = ...
     ) -> UpdateBackendAPIResponseTypeDef:
         """
         Updates an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/client/#update_backend_api)
         """
```

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/literals.py` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/literals.pyi` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/paginator.py` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/paginator.pyi` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/type_defs.py` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/type_defs.pyi` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/PKG-INFO` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifybackend
-Version: 1.28.15
-Summary: Type annotations for boto3.AmplifyBackend 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AmplifyBackend 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/SOURCES.txt` & `mypy-boto3-amplifybackend-1.28.15.post1/mypy_boto3_amplifybackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.15/setup.py` & `mypy-boto3-amplifybackend-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplifybackend",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_amplifybackend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AmplifyBackend 1.28.15 service generated with"
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

