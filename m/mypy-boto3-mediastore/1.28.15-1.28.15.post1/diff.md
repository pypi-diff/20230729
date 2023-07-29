# Comparing `tmp/mypy-boto3-mediastore-1.28.15.tar.gz` & `tmp/mypy-boto3-mediastore-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediastore-1.28.15.tar", last modified: Fri Jul 28 20:43:17 2023, max compression
+gzip compressed data, was "mypy-boto3-mediastore-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:40 2023, max compression
```

## Comparing `mypy-boto3-mediastore-1.28.15.tar` & `mypy-boto3-mediastore-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:17.785508 mypy-boto3-mediastore-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-07-28 20:43:17.777508 mypy-boto3-mediastore-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:17.777508 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:17.777508 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:17.785508 mypy-boto3-mediastore-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.749284 mypy-boto3-mediastore-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-07-29 10:03:40.749284 mypy-boto3-mediastore-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.749284 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.749284 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:40.749284 mypy-boto3-mediastore-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:51:17.000000 mypy-boto3-mediastore-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-mediastore-1.28.15/LICENSE` & `mypy-boto3-mediastore-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15/PKG-INFO` & `mypy-boto3-mediastore-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore
-Version: 1.28.15
-Summary: Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediastore-1.28.15/README.md` & `mypy-boto3-mediastore-1.28.15.post1/README.md`

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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__init__.py` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__init__.pyi` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__main__.py` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaStore 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.MediaStore 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore\nOther"
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

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/client.py` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,31 @@
     from mypy_boto3_mediastore.client import MediaStoreClient
 
     session = Session()
     client: MediaStoreClient = session.client("mediastore")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListContainersPaginator
 from .type_defs import (
+    CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     GetContainerPolicyOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyOutputTypeDef,
     ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -223,15 +225,18 @@
         clients that can access it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_container_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_container_policy)
         """
 
     def put_cors_policy(
-        self, *, ContainerName: str, CorsPolicy: Sequence[CorsRuleTypeDef]
+        self,
+        *,
+        ContainerName: str,
+        CorsPolicy: Sequence[Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]]
     ) -> Dict[str, Any]:
         """
         Sets the cross-origin resource sharing (CORS) configuration on a container so
         that the container can service cross-origin requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_cors_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_cors_policy)
@@ -242,15 +247,18 @@
         Writes an object lifecycle policy to a container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_lifecycle_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_lifecycle_policy)
         """
 
     def put_metric_policy(
-        self, *, ContainerName: str, MetricPolicy: MetricPolicyTypeDef
+        self,
+        *,
+        ContainerName: str,
+        MetricPolicy: Union[MetricPolicyTypeDef, MetricPolicyOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         The metric policy that you want to add to the container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_metric_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_metric_policy)
         """
```

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/client.pyi` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,31 @@
     from mypy_boto3_mediastore.client import MediaStoreClient
 
     session = Session()
     client: MediaStoreClient = session.client("mediastore")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListContainersPaginator
 from .type_defs import (
+    CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     GetContainerPolicyOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyOutputTypeDef,
     ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -201,15 +203,18 @@
         Creates an access policy for the specified container to restrict the users and
         clients that can access it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_container_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_container_policy)
         """
     def put_cors_policy(
-        self, *, ContainerName: str, CorsPolicy: Sequence[CorsRuleTypeDef]
+        self,
+        *,
+        ContainerName: str,
+        CorsPolicy: Sequence[Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]]
     ) -> Dict[str, Any]:
         """
         Sets the cross-origin resource sharing (CORS) configuration on a container so
         that the container can service cross-origin requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_cors_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_cors_policy)
@@ -218,15 +223,18 @@
         """
         Writes an object lifecycle policy to a container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_lifecycle_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_lifecycle_policy)
         """
     def put_metric_policy(
-        self, *, ContainerName: str, MetricPolicy: MetricPolicyTypeDef
+        self,
+        *,
+        ContainerName: str,
+        MetricPolicy: Union[MetricPolicyTypeDef, MetricPolicyOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         The metric policy that you want to add to the container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_metric_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/client/#put_metric_policy)
         """
```

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/literals.py` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/literals.pyi` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/paginator.py` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/paginator.pyi` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/type_defs.py` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_mediastore.type_defs import ContainerTypeDef
 
     data: ContainerTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import ContainerLevelMetricsType, ContainerStatusType, MethodNameType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -295,15 +295,15 @@
     },
 )
 
 PutCorsPolicyInputRequestTypeDef = TypedDict(
     "PutCorsPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
-        "CorsPolicy": Sequence[CorsRuleTypeDef],
+        "CorsPolicy": Sequence[Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]],
     },
 )
 
 _RequiredCreateContainerInputRequestTypeDef = TypedDict(
     "_RequiredCreateContainerInputRequestTypeDef",
     {
         "ContainerName": str,
```

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/type_defs.pyi` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_mediastore.type_defs import ContainerTypeDef
 
     data: ContainerTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import ContainerLevelMetricsType, ContainerStatusType, MethodNameType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -288,15 +288,15 @@
     },
 )
 
 PutCorsPolicyInputRequestTypeDef = TypedDict(
     "PutCorsPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
-        "CorsPolicy": Sequence[CorsRuleTypeDef],
+        "CorsPolicy": Sequence[Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]],
     },
 )
 
 _RequiredCreateContainerInputRequestTypeDef = TypedDict(
     "_RequiredCreateContainerInputRequestTypeDef",
     {
         "ContainerName": str,
```

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/PKG-INFO` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore
-Version: 1.28.15
-Summary: Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/SOURCES.txt` & `mypy-boto3-mediastore-1.28.15.post1/mypy_boto3_mediastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.15/setup.py` & `mypy-boto3-mediastore-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediastore",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_mediastore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder"
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

