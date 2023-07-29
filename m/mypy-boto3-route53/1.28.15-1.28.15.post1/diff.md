# Comparing `tmp/mypy-boto3-route53-1.28.15.tar.gz` & `tmp/mypy-boto3-route53-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-1.28.15.tar", last modified: Fri Jul 28 20:43:36 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:01 2023, max compression
```

## Comparing `mypy-boto3-route53-1.28.15.tar` & `mypy-boto3-route53-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.161760 mypy-boto3-route53-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22649 2023-07-28 20:43:36.161760 mypy-boto3-route53-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.161760 mypy-boto3-route53-1.28.15/mypy_boto3_route53/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55295 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55209 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63068 2023-07-28 20:37:13.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62997 2023-07-28 20:37:13.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.161760 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22649 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:36.161760 mypy-boto3-route53-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.969368 mypy-boto3-route53-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22655 2023-07-29 10:04:01.969368 mypy-boto3-route53-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.953368 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55401 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55315 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63068 2023-07-29 09:57:19.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62997 2023-07-29 09:57:18.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.969368 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22655 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:01.969368 mypy-boto3-route53-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-route53-1.28.15/LICENSE` & `mypy-boto3-route53-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/PKG-INFO` & `mypy-boto3-route53-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53
-Version: 1.28.15
-Summary: Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53-1.28.15/README.md` & `mypy-boto3-route53-1.28.15.post1/README.md`

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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/__init__.py` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/__init__.pyi` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/__main__.py` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Route53 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53\nOther"
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

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/client.py` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_route53.client import Route53Client
 
     session = Session()
     client: Route53Client = session.client("route53")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccountLimitTypeType,
     HealthCheckRegionType,
     HostedZoneLimitTypeType,
@@ -76,14 +76,15 @@
     GetHostedZoneResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyResponseTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     HostedZoneConfigTypeDef,
     ListCidrBlocksResponseTypeDef,
     ListCidrCollectionsResponseTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListGeoLocationsResponseTypeDef,
     ListHealthChecksResponseTypeDef,
@@ -301,15 +302,18 @@
         Creates a CIDR collection in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_cidr_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#create_cidr_collection)
         """
 
     def create_health_check(
-        self, *, CallerReference: str, HealthCheckConfig: HealthCheckConfigTypeDef
+        self,
+        *,
+        CallerReference: str,
+        HealthCheckConfig: Union[HealthCheckConfigTypeDef, HealthCheckConfigOutputTypeDef]
     ) -> CreateHealthCheckResponseTypeDef:
         """
         Creates a new health check.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_health_check)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#create_health_check)
         """
```

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/client.pyi` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_route53.client import Route53Client
 
     session = Session()
     client: Route53Client = session.client("route53")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccountLimitTypeType,
     HealthCheckRegionType,
     HostedZoneLimitTypeType,
@@ -76,14 +76,15 @@
     GetHostedZoneResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyResponseTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     HostedZoneConfigTypeDef,
     ListCidrBlocksResponseTypeDef,
     ListCidrCollectionsResponseTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListGeoLocationsResponseTypeDef,
     ListHealthChecksResponseTypeDef,
@@ -288,15 +289,18 @@
         """
         Creates a CIDR collection in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_cidr_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#create_cidr_collection)
         """
     def create_health_check(
-        self, *, CallerReference: str, HealthCheckConfig: HealthCheckConfigTypeDef
+        self,
+        *,
+        CallerReference: str,
+        HealthCheckConfig: Union[HealthCheckConfigTypeDef, HealthCheckConfigOutputTypeDef]
     ) -> CreateHealthCheckResponseTypeDef:
         """
         Creates a new health check.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_health_check)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#create_health_check)
         """
```

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/literals.py` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/literals.pyi` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/paginator.py` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/paginator.pyi` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/type_defs.py` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/type_defs.pyi` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/waiter.py` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53/waiter.pyi` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/PKG-INFO` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53
-Version: 1.28.15
-Summary: Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/SOURCES.txt` & `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15/setup.py` & `mypy-boto3-route53-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_route53"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder"
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

