# Comparing `tmp/mypy-boto3-appmesh-1.28.15.tar.gz` & `tmp/mypy-boto3-appmesh-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appmesh-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
+gzip compressed data, was "mypy-boto3-appmesh-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:31 2023, max compression
```

## Comparing `mypy-boto3-appmesh-1.28.15.tar` & `mypy-boto3-appmesh-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.272655 mypy-boto3-appmesh-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-07-28 20:42:16.268655 mypy-boto3-appmesh-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22845 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.256654 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30176 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-28 20:19:29.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-28 20:19:29.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   100348 2023-07-28 20:19:32.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   100157 2023-07-28 20:19:31.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.268655 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.272655 mypy-boto3-appmesh-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.145007 mypy-boto3-appmesh-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-07-29 10:02:31.141008 mypy-boto3-appmesh-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22845 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.133007 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30776 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30723 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   100348 2023-07-29 09:38:25.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100157 2023-07-29 09:38:22.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.141008 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:31.145007 mypy-boto3-appmesh-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-appmesh-1.28.15/LICENSE` & `mypy-boto3-appmesh-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15/PKG-INFO` & `mypy-boto3-appmesh-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appmesh
-Version: 1.28.15
-Summary: Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appmesh-1.28.15/README.md` & `mypy-boto3-appmesh-1.28.15.post1/README.md`

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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__init__.py` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__init__.pyi` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__main__.py` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppMesh 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.AppMesh 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh\nOther"
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

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/client.py` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appmesh.client import AppMeshClient
 
     session = Session()
     client: AppMeshClient = session.client("appmesh")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListGatewayRoutesPaginator,
     ListMeshesPaginator,
     ListRoutesPaginator,
@@ -46,35 +46,40 @@
     DescribeGatewayRouteOutputTypeDef,
     DescribeMeshOutputTypeDef,
     DescribeRouteOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
+    GatewayRouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
     ListGatewayRoutesOutputTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     MeshSpecTypeDef,
+    RouteSpecOutputTypeDef,
     RouteSpecTypeDef,
     TagRefTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     UpdateMeshOutputTypeDef,
     UpdateRouteOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
+    VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
+    VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
+    VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
     VirtualServiceSpecTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -140,15 +145,15 @@
         """
 
     def create_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecTypeDef,
+        spec: Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef],
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateGatewayRouteOutputTypeDef:
         """
         Creates a gateway route.
@@ -173,15 +178,15 @@
         """
 
     def create_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecTypeDef,
+        spec: Union[RouteSpecTypeDef, RouteSpecOutputTypeDef],
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateRouteOutputTypeDef:
         """
         Creates a route that is associated with a virtual router.
@@ -190,15 +195,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_route)
         """
 
     def create_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecTypeDef,
+        spec: Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef],
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualGatewayOutputTypeDef:
         """
         Creates a virtual gateway.
@@ -207,15 +212,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_gateway)
         """
 
     def create_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecTypeDef,
+        spec: Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef],
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualNodeOutputTypeDef:
         """
         Creates a virtual node within a service mesh.
@@ -224,15 +229,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_node)
         """
 
     def create_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecTypeDef,
+        spec: Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef],
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualRouterOutputTypeDef:
         """
         Creates a virtual router within a service mesh.
@@ -516,15 +521,15 @@
         """
 
     def update_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecTypeDef,
+        spec: Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef],
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateGatewayRouteOutputTypeDef:
         """
         Updates an existing gateway route that is associated to a specified virtual
         gateway in a service mesh.
@@ -544,15 +549,15 @@
         """
 
     def update_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecTypeDef,
+        spec: Union[RouteSpecTypeDef, RouteSpecOutputTypeDef],
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateRouteOutputTypeDef:
         """
         Updates an existing route for a specified service mesh and virtual router.
 
@@ -560,15 +565,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_route)
         """
 
     def update_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecTypeDef,
+        spec: Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef],
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualGatewayOutputTypeDef:
         """
         Updates an existing virtual gateway in a specified service mesh.
 
@@ -576,15 +581,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_gateway)
         """
 
     def update_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecTypeDef,
+        spec: Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef],
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualNodeOutputTypeDef:
         """
         Updates an existing virtual node in a specified service mesh.
 
@@ -592,15 +597,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_node)
         """
 
     def update_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecTypeDef,
+        spec: Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef],
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualRouterOutputTypeDef:
         """
         Updates an existing virtual router in a specified service mesh.
```

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/client.pyi` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appmesh.client import AppMeshClient
 
     session = Session()
     client: AppMeshClient = session.client("appmesh")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListGatewayRoutesPaginator,
     ListMeshesPaginator,
     ListRoutesPaginator,
@@ -46,35 +46,40 @@
     DescribeGatewayRouteOutputTypeDef,
     DescribeMeshOutputTypeDef,
     DescribeRouteOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
+    GatewayRouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
     ListGatewayRoutesOutputTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     MeshSpecTypeDef,
+    RouteSpecOutputTypeDef,
     RouteSpecTypeDef,
     TagRefTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     UpdateMeshOutputTypeDef,
     UpdateRouteOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
+    VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
+    VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
+    VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
     VirtualServiceSpecTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -133,15 +138,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#close)
         """
     def create_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecTypeDef,
+        spec: Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef],
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateGatewayRouteOutputTypeDef:
         """
         Creates a gateway route.
@@ -164,15 +169,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_mesh)
         """
     def create_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecTypeDef,
+        spec: Union[RouteSpecTypeDef, RouteSpecOutputTypeDef],
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateRouteOutputTypeDef:
         """
         Creates a route that is associated with a virtual router.
@@ -180,15 +185,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_route)
         """
     def create_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecTypeDef,
+        spec: Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef],
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualGatewayOutputTypeDef:
         """
         Creates a virtual gateway.
@@ -196,15 +201,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_gateway)
         """
     def create_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecTypeDef,
+        spec: Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef],
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualNodeOutputTypeDef:
         """
         Creates a virtual node within a service mesh.
@@ -212,15 +217,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_node)
         """
     def create_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecTypeDef,
+        spec: Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef],
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualRouterOutputTypeDef:
         """
         Creates a virtual router within a service mesh.
@@ -477,15 +482,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#untag_resource)
         """
     def update_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecTypeDef,
+        spec: Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef],
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateGatewayRouteOutputTypeDef:
         """
         Updates an existing gateway route that is associated to a specified virtual
         gateway in a service mesh.
@@ -503,60 +508,60 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_mesh)
         """
     def update_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecTypeDef,
+        spec: Union[RouteSpecTypeDef, RouteSpecOutputTypeDef],
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateRouteOutputTypeDef:
         """
         Updates an existing route for a specified service mesh and virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_route)
         """
     def update_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecTypeDef,
+        spec: Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef],
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualGatewayOutputTypeDef:
         """
         Updates an existing virtual gateway in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_gateway)
         """
     def update_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecTypeDef,
+        spec: Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef],
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualNodeOutputTypeDef:
         """
         Updates an existing virtual node in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_node)
         """
     def update_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecTypeDef,
+        spec: Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef],
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualRouterOutputTypeDef:
         """
         Updates an existing virtual router in a specified service mesh.
```

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/literals.py` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/literals.pyi` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/paginator.py` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/paginator.pyi` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/type_defs.py` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/type_defs.pyi` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/PKG-INFO` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appmesh
-Version: 1.28.15
-Summary: Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/SOURCES.txt` & `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15/setup.py` & `mypy-boto3-appmesh-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appmesh",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_appmesh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder"
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

