# Comparing `tmp/mypy-boto3-iottwinmaker-1.28.15.tar.gz` & `tmp/mypy-boto3-iottwinmaker-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iottwinmaker-1.28.15.tar", last modified: Fri Jul 28 20:43:02 2023, max compression
+gzip compressed data, was "mypy-boto3-iottwinmaker-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:23 2023, max compression
```

## Comparing `mypy-boto3-iottwinmaker-1.28.15.tar` & `mypy-boto3-iottwinmaker-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.505299 mypy-boto3-iottwinmaker-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16564 2023-07-28 20:43:02.505299 mypy-boto3-iottwinmaker-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.505299 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-28 20:28:44.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-07-28 20:28:43.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-28 20:28:44.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-07-28 20:28:44.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46171 2023-07-28 20:28:45.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46090 2023-07-28 20:28:44.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.505299 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16564 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:02.505299 mypy-boto3-iottwinmaker-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:28:41.000000 mypy-boto3-iottwinmaker-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.413197 mypy-boto3-iottwinmaker-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-07-29 10:03:23.413197 mypy-boto3-iottwinmaker-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.409197 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24868 2023-07-29 09:48:16.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24828 2023-07-29 09:48:16.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-29 09:48:16.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-07-29 09:48:16.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46211 2023-07-29 09:48:17.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46130 2023-07-29 09:48:17.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.413197 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:23.000000 mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:23.413197 mypy-boto3-iottwinmaker-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:48:15.000000 mypy-boto3-iottwinmaker-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15/LICENSE` & `mypy-boto3-iottwinmaker-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.15/PKG-INFO` & `mypy-boto3-iottwinmaker-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15/README.md` & `mypy-boto3-iottwinmaker-1.28.15.post1/README.md`

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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/__main__.py` & `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTTwinMaker 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.IoTTwinMaker 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker\nOther"
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

### Comparing `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/client.py` & `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     ListSyncResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyFilterTypeDef,
     PropertyGroupRequestTypeDef,
+    PropertyValueEntryOutputTypeDef,
     PropertyValueEntryTypeDef,
     SyncResourceFilterTypeDef,
     TabularConditionsTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     UpdateSceneResponseTypeDef,
@@ -105,15 +106,18 @@
         IoTTwinMakerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#exceptions)
         """
 
     def batch_put_property_values(
-        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryTypeDef]
+        self,
+        *,
+        workspaceId: str,
+        entries: Sequence[Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]]
     ) -> BatchPutPropertyValuesResponseTypeDef:
         """
         Sets values for multiple time series properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.batch_put_property_values)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#batch_put_property_values)
         """
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/client.pyi` & `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     ListSyncResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyFilterTypeDef,
     PropertyGroupRequestTypeDef,
+    PropertyValueEntryOutputTypeDef,
     PropertyValueEntryTypeDef,
     SyncResourceFilterTypeDef,
     TabularConditionsTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     UpdateSceneResponseTypeDef,
@@ -101,15 +102,18 @@
         """
         IoTTwinMakerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#exceptions)
         """
     def batch_put_property_values(
-        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryTypeDef]
+        self,
+        *,
+        workspaceId: str,
+        entries: Sequence[Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]]
     ) -> BatchPutPropertyValuesResponseTypeDef:
         """
         Sets values for multiple time series properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.batch_put_property_values)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#batch_put_property_values)
         """
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/literals.py` & `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/literals.pyi` & `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/type_defs.py` & `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1678,15 +1678,15 @@
     },
 )
 
 BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
     "BatchPutPropertyValuesRequestRequestTypeDef",
     {
         "workspaceId": str,
-        "entries": Sequence[PropertyValueEntryTypeDef],
+        "entries": Sequence[Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]],
     },
 )
 
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/type_defs.pyi` & `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1605,15 +1605,15 @@
     },
 )
 
 BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
     "BatchPutPropertyValuesRequestRequestTypeDef",
     {
         "workspaceId": str,
-        "entries": Sequence[PropertyValueEntryTypeDef],
+        "entries": Sequence[Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]],
     },
 )
 
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/PKG-INFO` & `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt` & `mypy-boto3-iottwinmaker-1.28.15.post1/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.15/setup.py` & `mypy-boto3-iottwinmaker-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iottwinmaker",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_iottwinmaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder"
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

