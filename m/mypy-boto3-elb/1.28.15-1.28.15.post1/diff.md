# Comparing `tmp/mypy-boto3-elb-1.28.15.tar.gz` & `tmp/mypy-boto3-elb-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elb-1.28.15.tar", last modified: Fri Jul 28 20:42:46 2023, max compression
+gzip compressed data, was "mypy-boto3-elb-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:05 2023, max compression
```

## Comparing `mypy-boto3-elb-1.28.15.tar` & `mypy-boto3-elb-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.245075 mypy-boto3-elb-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-07-28 20:42:46.233075 mypy-boto3-elb-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.225075 mypy-boto3-elb-1.28.15/mypy_boto3_elb/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24944 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24903 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25023 2023-07-28 20:25:19.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25000 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.233075 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-07-28 20:42:45.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:46.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:45.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:45.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:45.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:45.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:46.245075 mypy-boto3-elb-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-28 20:25:17.000000 mypy-boto3-elb-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.653141 mypy-boto3-elb-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:47.000000 mypy-boto3-elb-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-07-29 10:03:05.645141 mypy-boto3-elb-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-07-29 09:44:47.000000 mypy-boto3-elb-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.633141 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-29 09:44:47.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-29 09:44:47.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 09:44:47.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25082 2023-07-29 09:44:49.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-07-29 09:44:49.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-29 09:44:49.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-29 09:44:49.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-29 09:44:49.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-29 09:44:49.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:47.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25023 2023-07-29 09:44:50.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25000 2023-07-29 09:44:50.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:47.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-29 09:44:49.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-29 09:44:49.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.645141 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-07-29 10:03:05.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:03:05.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:05.000000 mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:05.653141 mypy-boto3-elb-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-29 09:44:47.000000 mypy-boto3-elb-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-elb-1.28.15/LICENSE` & `mypy-boto3-elb-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/PKG-INFO` & `mypy-boto3-elb-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elb
-Version: 1.28.15
-Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elb-1.28.15/README.md` & `mypy-boto3-elb-1.28.15.post1/README.md`

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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/__init__.py` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/__init__.pyi` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/__main__.py` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticLoadBalancing 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.ElasticLoadBalancing 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing\nOther"
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

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/client.py` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_elb.client import ElasticLoadBalancingClient
 
     session = Session()
     client: ElasticLoadBalancingClient = session.client("elb")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeAccountLimitsPaginator, DescribeLoadBalancersPaginator
 from .type_defs import (
     AddAvailabilityZonesOutputTypeDef,
     ApplySecurityGroupsToLoadBalancerOutputTypeDef,
@@ -33,14 +33,15 @@
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
     DescribeTagsOutputTypeDef,
     DetachLoadBalancerFromSubnetsOutputTypeDef,
     HealthCheckTypeDef,
     InstanceTypeDef,
     ListenerTypeDef,
+    LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     PolicyAttributeTypeDef,
     RegisterEndPointsOutputTypeDef,
     RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
     TagTypeDef,
@@ -384,15 +385,20 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/client/#generate_presigned_url)
         """
 
     def modify_load_balancer_attributes(
-        self, *, LoadBalancerName: str, LoadBalancerAttributes: LoadBalancerAttributesTypeDef
+        self,
+        *,
+        LoadBalancerName: str,
+        LoadBalancerAttributes: Union[
+            LoadBalancerAttributesTypeDef, LoadBalancerAttributesOutputTypeDef
+        ]
     ) -> ModifyLoadBalancerAttributesOutputTypeDef:
         """
         Modifies the attributes of the specified load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.modify_load_balancer_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/client/#modify_load_balancer_attributes)
         """
```

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/client.pyi` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_elb.client import ElasticLoadBalancingClient
 
     session = Session()
     client: ElasticLoadBalancingClient = session.client("elb")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeAccountLimitsPaginator, DescribeLoadBalancersPaginator
 from .type_defs import (
     AddAvailabilityZonesOutputTypeDef,
     ApplySecurityGroupsToLoadBalancerOutputTypeDef,
@@ -33,14 +33,15 @@
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
     DescribeTagsOutputTypeDef,
     DetachLoadBalancerFromSubnetsOutputTypeDef,
     HealthCheckTypeDef,
     InstanceTypeDef,
     ListenerTypeDef,
+    LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     PolicyAttributeTypeDef,
     RegisterEndPointsOutputTypeDef,
     RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
     TagTypeDef,
@@ -353,15 +354,20 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/client/#generate_presigned_url)
         """
     def modify_load_balancer_attributes(
-        self, *, LoadBalancerName: str, LoadBalancerAttributes: LoadBalancerAttributesTypeDef
+        self,
+        *,
+        LoadBalancerName: str,
+        LoadBalancerAttributes: Union[
+            LoadBalancerAttributesTypeDef, LoadBalancerAttributesOutputTypeDef
+        ]
     ) -> ModifyLoadBalancerAttributesOutputTypeDef:
         """
         Modifies the attributes of the specified load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.modify_load_balancer_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/client/#modify_load_balancer_attributes)
         """
```

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/literals.py` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/literals.pyi` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/paginator.py` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/paginator.pyi` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/type_defs.py` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/type_defs.pyi` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/waiter.py` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb/waiter.pyi` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/PKG-INFO` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elb
-Version: 1.28.15
-Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/SOURCES.txt` & `mypy-boto3-elb-1.28.15.post1/mypy_boto3_elb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.15/setup.py` & `mypy-boto3-elb-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elb",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_elb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ElasticLoadBalancing 1.28.15 service generated with"
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
