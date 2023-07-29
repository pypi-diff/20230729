# Comparing `tmp/mypy-boto3-groundstation-1.28.15.tar.gz` & `tmp/mypy-boto3-groundstation-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-groundstation-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
+gzip compressed data, was "mypy-boto3-groundstation-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:13 2023, max compression
```

## Comparing `mypy-boto3-groundstation-1.28.15.tar` & `mypy-boto3-groundstation-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.345173 mypy-boto3-groundstation-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-07-28 20:42:53.345173 mypy-boto3-groundstation-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.329172 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26848 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26800 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40795 2023-07-28 20:27:10.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40746 2023-07-28 20:27:10.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.345173 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.345173 mypy-boto3-groundstation-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.561169 mypy-boto3-groundstation-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-29 10:03:13.561169 mypy-boto3-groundstation-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.553169 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26919 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40832 2023-07-29 09:46:44.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40783 2023-07-29 09:46:42.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-29 09:46:41.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.561169 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:13.000000 mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:13.561169 mypy-boto3-groundstation-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-29 09:46:40.000000 mypy-boto3-groundstation-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-groundstation-1.28.15/LICENSE` & `mypy-boto3-groundstation-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15/PKG-INFO` & `mypy-boto3-groundstation-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.28.15
-Summary: Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-groundstation-1.28.15/README.md` & `mypy-boto3-groundstation-1.28.15.post1/README.md`

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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__init__.py` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__init__.pyi` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__main__.py` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GroundStation 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.GroundStation 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
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

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/client.py` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     ConfigIdResponseTypeDef,
     ConfigTypeDataTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DescribeContactResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
     DiscoveryDataTypeDef,
+    EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     EphemerisDataTypeDef,
     EphemerisIdResponseTypeDef,
     GetAgentConfigurationResponseTypeDef,
     GetConfigResponseTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
@@ -139,15 +140,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_config)
         """
 
     def create_dataflow_endpoint_group(
         self,
         *,
-        endpointDetails: Sequence[EndpointDetailsTypeDef],
+        endpointDetails: Sequence[Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]],
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         tags: Mapping[str, str] = ...
     ) -> DataflowEndpointGroupIdResponseTypeDef:
         """
         Creates a `DataflowEndpoint` group containing the specified list of
         `DataflowEndpoint` objects.
```

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/client.pyi` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     ConfigIdResponseTypeDef,
     ConfigTypeDataTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DescribeContactResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
     DiscoveryDataTypeDef,
+    EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     EphemerisDataTypeDef,
     EphemerisIdResponseTypeDef,
     GetAgentConfigurationResponseTypeDef,
     GetConfigResponseTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
@@ -130,15 +131,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_config)
         """
     def create_dataflow_endpoint_group(
         self,
         *,
-        endpointDetails: Sequence[EndpointDetailsTypeDef],
+        endpointDetails: Sequence[Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]],
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         tags: Mapping[str, str] = ...
     ) -> DataflowEndpointGroupIdResponseTypeDef:
         """
         Creates a `DataflowEndpoint` group containing the specified list of
         `DataflowEndpoint` objects.
```

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/literals.py` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/literals.pyi` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/paginator.py` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/paginator.pyi` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/type_defs.py` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1577,15 +1577,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
     {
-        "endpointDetails": Sequence[EndpointDetailsTypeDef],
+        "endpointDetails": Sequence[Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]],
     },
 )
 _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
     {
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
```

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/type_defs.pyi` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1530,15 +1530,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
     {
-        "endpointDetails": Sequence[EndpointDetailsTypeDef],
+        "endpointDetails": Sequence[Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]],
     },
 )
 _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
     {
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
```

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/waiter.py` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/waiter.pyi` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/PKG-INFO` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.28.15
-Summary: Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/SOURCES.txt` & `mypy-boto3-groundstation-1.28.15.post1/mypy_boto3_groundstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.15/setup.py` & `mypy-boto3-groundstation-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-groundstation",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder"
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

