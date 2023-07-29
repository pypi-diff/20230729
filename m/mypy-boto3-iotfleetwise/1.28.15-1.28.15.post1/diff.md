# Comparing `tmp/mypy-boto3-iotfleetwise-1.28.15.tar.gz` & `tmp/mypy-boto3-iotfleetwise-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotfleetwise-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
+gzip compressed data, was "mypy-boto3-iotfleetwise-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:21 2023, max compression
```

## Comparing `mypy-boto3-iotfleetwise-1.28.15.tar` & `mypy-boto3-iotfleetwise-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.549258 mypy-boto3-iotfleetwise-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-07-28 20:42:59.541258 mypy-boto3-iotfleetwise-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.529258 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40870 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40800 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-28 20:28:29.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60272 2023-07-28 20:28:31.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60166 2023-07-28 20:28:30.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.541258 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:59.000000 mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.549258 mypy-boto3-iotfleetwise-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:28:27.000000 mypy-boto3-iotfleetwise-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.805189 mypy-boto3-iotfleetwise-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21522 2023-07-29 10:03:21.793189 mypy-boto3-iotfleetwise-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.789189 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40971 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40901 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-07-29 09:48:01.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60350 2023-07-29 09:48:03.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60244 2023-07-29 09:48:02.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:21.793189 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21522 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:21.000000 mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:21.805189 mypy-boto3-iotfleetwise-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:48:00.000000 mypy-boto3-iotfleetwise-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15/LICENSE` & `mypy-boto3-iotfleetwise-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15/PKG-INFO` & `mypy-boto3-iotfleetwise-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15/README.md` & `mypy-boto3-iotfleetwise-1.28.15.post1/README.md`

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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__init__.py` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__init__.pyi` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/__main__.py` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTFleetWise 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.IoTFleetWise 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise\nOther"
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

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/client.py` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     ListSignalCatalogNodesResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     NetworkInterfaceTypeDef,
+    NodeOutputTypeDef,
     NodeTypeDef,
     RegisterAccountResponseTypeDef,
     SignalDecoderTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
     TimestreamResourcesTypeDef,
     UpdateCampaignResponseTypeDef,
@@ -274,15 +275,15 @@
         """
 
     def create_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodes: Sequence[NodeTypeDef] = ...,
+        nodes: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSignalCatalogResponseTypeDef:
         """
         Creates a collection of standardized signals that can be reused to create
         vehicle models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_signal_catalog)
@@ -707,16 +708,16 @@
         """
 
     def update_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodesToAdd: Sequence[NodeTypeDef] = ...,
-        nodesToUpdate: Sequence[NodeTypeDef] = ...,
+        nodesToAdd: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
+        nodesToUpdate: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
         nodesToRemove: Sequence[str] = ...
     ) -> UpdateSignalCatalogResponseTypeDef:
         """
         Updates a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_signal_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#update_signal_catalog)
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/client.pyi` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     ListSignalCatalogNodesResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     NetworkInterfaceTypeDef,
+    NodeOutputTypeDef,
     NodeTypeDef,
     RegisterAccountResponseTypeDef,
     SignalDecoderTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
     TimestreamResourcesTypeDef,
     UpdateCampaignResponseTypeDef,
@@ -260,15 +261,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#create_model_manifest)
         """
     def create_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodes: Sequence[NodeTypeDef] = ...,
+        nodes: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSignalCatalogResponseTypeDef:
         """
         Creates a collection of standardized signals that can be reused to create
         vehicle models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_signal_catalog)
@@ -651,16 +652,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#update_model_manifest)
         """
     def update_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodesToAdd: Sequence[NodeTypeDef] = ...,
-        nodesToUpdate: Sequence[NodeTypeDef] = ...,
+        nodesToAdd: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
+        nodesToUpdate: Sequence[Union[NodeTypeDef, NodeOutputTypeDef]] = ...,
         nodesToRemove: Sequence[str] = ...
     ) -> UpdateSignalCatalogResponseTypeDef:
         """
         Updates a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_signal_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#update_signal_catalog)
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/literals.py` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/literals.pyi` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/paginator.py` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/paginator.pyi` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/type_defs.py` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2281,15 +2281,15 @@
         "name": str,
     },
 )
 _OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSignalCatalogRequestRequestTypeDef",
     {
         "description": str,
-        "nodes": Sequence[NodeTypeDef],
+        "nodes": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class CreateSignalCatalogRequestRequestTypeDef(
@@ -2305,16 +2305,16 @@
         "name": str,
     },
 )
 _OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
     {
         "description": str,
-        "nodesToAdd": Sequence[NodeTypeDef],
-        "nodesToUpdate": Sequence[NodeTypeDef],
+        "nodesToAdd": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
+        "nodesToUpdate": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
         "nodesToRemove": Sequence[str],
     },
     total=False,
 )
 
 
 class UpdateSignalCatalogRequestRequestTypeDef(
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise/type_defs.pyi` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2182,15 +2182,15 @@
         "name": str,
     },
 )
 _OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSignalCatalogRequestRequestTypeDef",
     {
         "description": str,
-        "nodes": Sequence[NodeTypeDef],
+        "nodes": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateSignalCatalogRequestRequestTypeDef(
     _RequiredCreateSignalCatalogRequestRequestTypeDef,
@@ -2204,16 +2204,16 @@
         "name": str,
     },
 )
 _OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
     {
         "description": str,
-        "nodesToAdd": Sequence[NodeTypeDef],
-        "nodesToUpdate": Sequence[NodeTypeDef],
+        "nodesToAdd": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
+        "nodesToUpdate": Sequence[Union[NodeTypeDef, NodeOutputTypeDef]],
         "nodesToRemove": Sequence[str],
     },
     total=False,
 )
 
 class UpdateSignalCatalogRequestRequestTypeDef(
     _RequiredUpdateSignalCatalogRequestRequestTypeDef,
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/PKG-INFO` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
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
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleetwise-1.28.15/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt` & `mypy-boto3-iotfleetwise-1.28.15.post1/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.28.15/setup.py` & `mypy-boto3-iotfleetwise-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotfleetwise",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_iotfleetwise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.IoTFleetWise 1.28.15 service generated with mypy-boto3-builder"
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

