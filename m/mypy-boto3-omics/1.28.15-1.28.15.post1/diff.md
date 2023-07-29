# Comparing `tmp/mypy-boto3-omics-1.28.15.tar.gz` & `tmp/mypy-boto3-omics-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-omics-1.28.15.tar", last modified: Fri Jul 28 20:43:23 2023, max compression
+gzip compressed data, was "mypy-boto3-omics-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:47 2023, max compression
```

## Comparing `mypy-boto3-omics-1.28.15.tar` & `mypy-boto3-omics-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:23.885592 mypy-boto3-omics-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-07-28 20:43:23.881592 mypy-boto3-omics-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27547 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:23.877592 mypy-boto3-omics-1.28.15/mypy_boto3_omics/
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61421 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61309 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-07-28 20:32:43.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21971 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97914 2023-07-28 20:32:48.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97758 2023-07-28 20:32:46.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:23.881592 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:23.885592 mypy-boto3-omics-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.697315 mypy-boto3-omics-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29032 2023-07-29 10:03:47.689315 mypy-boto3-omics-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27547 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.689315 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61486 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61374 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-07-29 09:52:22.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21971 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97914 2023-07-29 09:52:27.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97758 2023-07-29 09:52:26.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.689315 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29032 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:47.697315 mypy-boto3-omics-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-omics-1.28.15/LICENSE` & `mypy-boto3-omics-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/PKG-INFO` & `mypy-boto3-omics-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.28.15
-Summary: Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-omics-1.28.15/README.md` & `mypy-boto3-omics-1.28.15.post1/README.md`

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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/__init__.py` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/__init__.pyi` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/__main__.py` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Omics 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Omics 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
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

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/client.py` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
+    StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     VariantImportItemSourceTypeDef,
     WorkflowParameterTypeDef,
 )
@@ -282,15 +283,15 @@
         *,
         storeFormat: StoreFormatType,
         reference: ReferenceItemTypeDef = ...,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
         sseConfig: SseConfigTypeDef = ...,
-        storeOptions: StoreOptionsTypeDef = ...
+        storeOptions: Union[StoreOptionsTypeDef, StoreOptionsOutputTypeDef] = ...
     ) -> CreateAnnotationStoreResponseTypeDef:
         """
         Creates an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#create_annotation_store)
         """
```

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/client.pyi` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
+    StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     VariantImportItemSourceTypeDef,
     WorkflowParameterTypeDef,
 )
@@ -269,15 +270,15 @@
         *,
         storeFormat: StoreFormatType,
         reference: ReferenceItemTypeDef = ...,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
         sseConfig: SseConfigTypeDef = ...,
-        storeOptions: StoreOptionsTypeDef = ...
+        storeOptions: Union[StoreOptionsTypeDef, StoreOptionsOutputTypeDef] = ...
     ) -> CreateAnnotationStoreResponseTypeDef:
         """
         Creates an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#create_annotation_store)
         """
```

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/literals.py` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/literals.pyi` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/paginator.py` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/paginator.pyi` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/type_defs.py` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/type_defs.pyi` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/waiter.py` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics/waiter.pyi` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/PKG-INFO` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.28.15
-Summary: Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/SOURCES.txt` & `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15/setup.py` & `mypy-boto3-omics-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-omics",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

