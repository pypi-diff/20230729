# Comparing `tmp/mypy-boto3-clouddirectory-1.28.15.tar.gz` & `tmp/mypy-boto3-clouddirectory-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-clouddirectory-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
+gzip compressed data, was "mypy-boto3-clouddirectory-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:41 2023, max compression
```

## Comparing `mypy-boto3-clouddirectory-1.28.15.tar` & `mypy-boto3-clouddirectory-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.424781 mypy-boto3-clouddirectory-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26158 2023-07-28 20:42:25.424781 mypy-boto3-clouddirectory-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24643 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.424781 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56752 2023-07-28 20:20:53.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56660 2023-07-28 20:20:53.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-28 20:20:54.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-28 20:20:53.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-07-28 20:20:53.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-07-28 20:20:53.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    89831 2023-07-28 20:20:57.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    89698 2023-07-28 20:20:55.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.424781 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26158 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.424781 mypy-boto3-clouddirectory-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.477050 mypy-boto3-clouddirectory-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26164 2023-07-29 10:02:41.469050 mypy-boto3-clouddirectory-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24643 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.465050 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57281 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57189 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    90060 2023-07-29 09:39:50.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89927 2023-07-29 09:39:48.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.469050 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26164 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:41.477050 mypy-boto3-clouddirectory-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-clouddirectory-1.28.15/LICENSE` & `mypy-boto3-clouddirectory-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15/PKG-INFO` & `mypy-boto3-clouddirectory-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-clouddirectory
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudDirectory 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudDirectory 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-clouddirectory-1.28.15/README.md` & `mypy-boto3-clouddirectory-1.28.15.post1/README.md`

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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__init__.py` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__init__.pyi` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__main__.py` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudDirectory 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.CloudDirectory 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory\nOther"
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

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/client.py` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_clouddirectory.client import CloudDirectoryClient
 
     session = Session()
     client: CloudDirectoryClient = session.client("clouddirectory")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConsistencyLevelType, DirectoryStateType, FacetStyleType, ObjectTypeType
 from .paginator import (
     ListAppliedSchemaArnsPaginator,
     ListAttachedIndicesPaginator,
@@ -41,16 +41,18 @@
     LookupPolicyPaginator,
 )
 from .type_defs import (
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeKeyTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     AttributeNameAndValueTypeDef,
     BatchReadOperationTypeDef,
     BatchReadResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchWriteResponseTypeDef,
     CreateDirectoryResponseTypeDef,
     CreateIndexResponseTypeDef,
@@ -59,14 +61,15 @@
     DeleteDirectoryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DetachFromIndexResponseTypeDef,
     DetachObjectResponseTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryResponseTypeDef,
+    FacetAttributeOutputTypeDef,
     FacetAttributeTypeDef,
     FacetAttributeUpdateTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryResponseTypeDef,
     GetFacetResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
@@ -102,14 +105,15 @@
     PutSchemaFromJsonResponseTypeDef,
     SchemaFacetTypeDef,
     TagTypeDef,
     TypedLinkAttributeRangeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
+    TypedLinkSpecifierOutputTypeDef,
     TypedLinkSpecifierTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
 )
 
@@ -188,15 +192,17 @@
 
     def add_facet_to_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
         ObjectReference: ObjectReferenceTypeDef,
-        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...
+        ObjectAttributeList: Sequence[
+            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Adds a new  Facet to an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.add_facet_to_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#add_facet_to_object)
         """
@@ -258,15 +264,17 @@
     def attach_typed_link(
         self,
         *,
         DirectoryArn: str,
         SourceObjectReference: ObjectReferenceTypeDef,
         TargetObjectReference: ObjectReferenceTypeDef,
         TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,
-        Attributes: Sequence[AttributeNameAndValueTypeDef]
+        Attributes: Sequence[
+            Union[AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef]
+        ]
     ) -> AttachTypedLinkResponseTypeDef:
         """
         Attaches a typed link to a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_typed_link)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#attach_typed_link)
         """
@@ -320,15 +328,15 @@
         """
 
     def create_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
-        Attributes: Sequence[FacetAttributeTypeDef] = ...,
+        Attributes: Sequence[Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]] = ...,
         ObjectType: ObjectTypeType = ...,
         FacetStyle: FacetStyleType = ...
     ) -> Dict[str, Any]:
         """
         Creates a new  Facet in a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_facet)
@@ -352,15 +360,17 @@
         """
 
     def create_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacets: Sequence[SchemaFacetTypeDef],
-        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...,
+        ObjectAttributeList: Sequence[
+            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
+        ] = ...,
         ParentReference: ObjectReferenceTypeDef = ...,
         LinkName: str = ...
     ) -> CreateObjectResponseTypeDef:
         """
         Creates an object in a  Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_object)
@@ -462,15 +472,18 @@
         Detaches a policy from an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#detach_policy)
         """
 
     def detach_typed_link(
-        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierTypeDef
+        self,
+        *,
+        DirectoryArn: str,
+        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Detaches a typed link from a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_typed_link)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#detach_typed_link)
         """
@@ -532,15 +545,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#get_facet)
         """
 
     def get_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
+        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef],
         AttributeNames: Sequence[str],
         ConsistencyLevel: ConsistencyLevelType = ...
     ) -> GetLinkAttributesResponseTypeDef:
         """
         Retrieves attributes that are associated with a typed link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_link_attributes)
@@ -953,15 +966,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#update_facet)
         """
 
     def update_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
+        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef],
         AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates a given typed link’s attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_link_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#update_link_attributes)
```

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/client.pyi` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_clouddirectory.client import CloudDirectoryClient
 
     session = Session()
     client: CloudDirectoryClient = session.client("clouddirectory")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConsistencyLevelType, DirectoryStateType, FacetStyleType, ObjectTypeType
 from .paginator import (
     ListAppliedSchemaArnsPaginator,
     ListAttachedIndicesPaginator,
@@ -41,16 +41,18 @@
     LookupPolicyPaginator,
 )
 from .type_defs import (
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeKeyTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     AttributeNameAndValueTypeDef,
     BatchReadOperationTypeDef,
     BatchReadResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchWriteResponseTypeDef,
     CreateDirectoryResponseTypeDef,
     CreateIndexResponseTypeDef,
@@ -59,14 +61,15 @@
     DeleteDirectoryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DetachFromIndexResponseTypeDef,
     DetachObjectResponseTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryResponseTypeDef,
+    FacetAttributeOutputTypeDef,
     FacetAttributeTypeDef,
     FacetAttributeUpdateTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryResponseTypeDef,
     GetFacetResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
@@ -102,14 +105,15 @@
     PutSchemaFromJsonResponseTypeDef,
     SchemaFacetTypeDef,
     TagTypeDef,
     TypedLinkAttributeRangeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
+    TypedLinkSpecifierOutputTypeDef,
     TypedLinkSpecifierTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
 )
 
@@ -183,15 +187,17 @@
         """
     def add_facet_to_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
         ObjectReference: ObjectReferenceTypeDef,
-        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...
+        ObjectAttributeList: Sequence[
+            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Adds a new  Facet to an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.add_facet_to_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#add_facet_to_object)
         """
@@ -248,15 +254,17 @@
     def attach_typed_link(
         self,
         *,
         DirectoryArn: str,
         SourceObjectReference: ObjectReferenceTypeDef,
         TargetObjectReference: ObjectReferenceTypeDef,
         TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,
-        Attributes: Sequence[AttributeNameAndValueTypeDef]
+        Attributes: Sequence[
+            Union[AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef]
+        ]
     ) -> AttachTypedLinkResponseTypeDef:
         """
         Attaches a typed link to a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_typed_link)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#attach_typed_link)
         """
@@ -304,15 +312,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#create_directory)
         """
     def create_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
-        Attributes: Sequence[FacetAttributeTypeDef] = ...,
+        Attributes: Sequence[Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]] = ...,
         ObjectType: ObjectTypeType = ...,
         FacetStyle: FacetStyleType = ...
     ) -> Dict[str, Any]:
         """
         Creates a new  Facet in a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_facet)
@@ -334,15 +342,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#create_index)
         """
     def create_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacets: Sequence[SchemaFacetTypeDef],
-        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...,
+        ObjectAttributeList: Sequence[
+            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
+        ] = ...,
         ParentReference: ObjectReferenceTypeDef = ...,
         LinkName: str = ...
     ) -> CreateObjectResponseTypeDef:
         """
         Creates an object in a  Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_object)
@@ -433,15 +443,18 @@
         """
         Detaches a policy from an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#detach_policy)
         """
     def detach_typed_link(
-        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierTypeDef
+        self,
+        *,
+        DirectoryArn: str,
+        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Detaches a typed link from a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_typed_link)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#detach_typed_link)
         """
@@ -496,15 +509,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_facet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#get_facet)
         """
     def get_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
+        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef],
         AttributeNames: Sequence[str],
         ConsistencyLevel: ConsistencyLevelType = ...
     ) -> GetLinkAttributesResponseTypeDef:
         """
         Retrieves attributes that are associated with a typed link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_link_attributes)
@@ -885,15 +898,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_facet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#update_facet)
         """
     def update_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
+        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef],
         AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates a given typed link’s attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_link_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#update_link_attributes)
```

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/literals.py` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/literals.pyi` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/paginator.py` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/paginator.pyi` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/type_defs.py` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2476,15 +2476,17 @@
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
     "_OptionalAddFacetToObjectRequestRequestTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ObjectAttributeList": Sequence[
+            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class AddFacetToObjectRequestRequestTypeDef(
     _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
@@ -2531,15 +2533,17 @@
         "DirectoryArn": str,
         "SchemaFacets": Sequence[SchemaFacetTypeDef],
     },
 )
 _OptionalCreateObjectRequestRequestTypeDef = TypedDict(
     "_OptionalCreateObjectRequestRequestTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ObjectAttributeList": Sequence[
+            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
+        ],
         "ParentReference": ObjectReferenceTypeDef,
         "LinkName": str,
     },
     total=False,
 )
 
 
@@ -2552,15 +2556,17 @@
 AttachTypedLinkRequestRequestTypeDef = TypedDict(
     "AttachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "Attributes": Sequence[AttributeNameAndValueTypeDef],
+        "Attributes": Sequence[
+            Union[AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef]
+        ],
     },
 )
 
 BatchAttachTypedLinkTypeDef = TypedDict(
     "BatchAttachTypedLinkTypeDef",
     {
         "SourceObjectReference": ObjectReferenceTypeDef,
@@ -3124,15 +3130,15 @@
         "SchemaArn": str,
         "Name": str,
     },
 )
 _OptionalCreateFacetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFacetRequestRequestTypeDef",
     {
-        "Attributes": Sequence[FacetAttributeTypeDef],
+        "Attributes": Sequence[Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]],
         "ObjectType": ObjectTypeType,
         "FacetStyle": FacetStyleType,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/type_defs.pyi` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2381,15 +2381,17 @@
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
     "_OptionalAddFacetToObjectRequestRequestTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ObjectAttributeList": Sequence[
+            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class AddFacetToObjectRequestRequestTypeDef(
     _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
 ):
@@ -2432,15 +2434,17 @@
         "DirectoryArn": str,
         "SchemaFacets": Sequence[SchemaFacetTypeDef],
     },
 )
 _OptionalCreateObjectRequestRequestTypeDef = TypedDict(
     "_OptionalCreateObjectRequestRequestTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ObjectAttributeList": Sequence[
+            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
+        ],
         "ParentReference": ObjectReferenceTypeDef,
         "LinkName": str,
     },
     total=False,
 )
 
 class CreateObjectRequestRequestTypeDef(
@@ -2451,15 +2455,17 @@
 AttachTypedLinkRequestRequestTypeDef = TypedDict(
     "AttachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "Attributes": Sequence[AttributeNameAndValueTypeDef],
+        "Attributes": Sequence[
+            Union[AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef]
+        ],
     },
 )
 
 BatchAttachTypedLinkTypeDef = TypedDict(
     "BatchAttachTypedLinkTypeDef",
     {
         "SourceObjectReference": ObjectReferenceTypeDef,
@@ -2997,15 +3003,15 @@
         "SchemaArn": str,
         "Name": str,
     },
 )
 _OptionalCreateFacetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFacetRequestRequestTypeDef",
     {
-        "Attributes": Sequence[FacetAttributeTypeDef],
+        "Attributes": Sequence[Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]],
         "ObjectType": ObjectTypeType,
         "FacetStyle": FacetStyleType,
     },
     total=False,
 )
 
 class CreateFacetRequestRequestTypeDef(
```

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/PKG-INFO` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-clouddirectory
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudDirectory 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudDirectory 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/SOURCES.txt` & `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15/setup.py` & `mypy-boto3-clouddirectory-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-clouddirectory",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_clouddirectory"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CloudDirectory 1.28.15 service generated with"
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

