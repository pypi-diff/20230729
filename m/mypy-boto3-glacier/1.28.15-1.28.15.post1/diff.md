# Comparing `tmp/mypy-boto3-glacier-1.28.15.tar.gz` & `tmp/mypy-boto3-glacier-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glacier-1.28.15.tar", last modified: Fri Jul 28 20:42:52 2023, max compression
+gzip compressed data, was "mypy-boto3-glacier-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:12 2023, max compression
```

## Comparing `mypy-boto3-glacier-1.28.15.tar` & `mypy-boto3-glacier-1.28.15.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:52.365159 mypy-boto3-glacier-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-07-28 20:42:52.361159 mypy-boto3-glacier-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:52.361159 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26579 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-28 20:26:31.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-28 20:26:31.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-28 20:26:30.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-28 20:26:30.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-07-28 20:26:30.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    39087 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39382 2023-07-28 20:26:32.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39310 2023-07-28 20:26:32.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-28 20:26:30.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-28 20:26:30.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:52.361159 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:52.365159 mypy-boto3-glacier-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:12.445165 mypy-boto3-glacier-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19841 2023-07-29 10:03:12.445165 mypy-boto3-glacier-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:12.433165 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26791 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26745 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-29 09:46:03.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39087 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39382 2023-07-29 09:46:04.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39310 2023-07-29 09:46:03.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-29 09:46:02.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:12.445165 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19841 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:03:12.000000 mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:12.445165 mypy-boto3-glacier-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:46:01.000000 mypy-boto3-glacier-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-glacier-1.28.15/LICENSE` & `mypy-boto3-glacier-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/PKG-INFO` & `mypy-boto3-glacier-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glacier
-Version: 1.28.15
-Summary: Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-glacier-1.28.15/README.md` & `mypy-boto3-glacier-1.28.15.post1/README.md`

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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__init__.py` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__init__.pyi` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__main__.py` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glacier 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Glacier 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier\nOther"
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

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/client.py` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     ListMultipartUploadsPaginator,
     ListPartsPaginator,
     ListVaultsPaginator,
 )
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
+    DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     GetVaultLockOutputTypeDef,
@@ -47,14 +48,15 @@
     ListProvisionedCapacityOutputTypeDef,
     ListTagsForVaultOutputTypeDef,
     ListVaultsOutputTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
     VaultAccessPolicyTypeDef,
     VaultLockPolicyTypeDef,
+    VaultNotificationConfigOutputTypeDef,
     VaultNotificationConfigTypeDef,
 )
 from .waiter import VaultExistsWaiter, VaultNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -449,15 +451,18 @@
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.remove_tags_from_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#remove_tags_from_vault)
         """
 
     def set_data_retrieval_policy(
-        self, *, accountId: str = "-", Policy: DataRetrievalPolicyTypeDef = ...
+        self,
+        *,
+        accountId: str = "-",
+        Policy: Union[DataRetrievalPolicyTypeDef, DataRetrievalPolicyOutputTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation sets and then enacts a data retrieval policy in the region
         specified in the PUT request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_data_retrieval_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#set_data_retrieval_policy)
@@ -475,15 +480,17 @@
         """
 
     def set_vault_notifications(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
-        vaultNotificationConfig: VaultNotificationConfigTypeDef = ...
+        vaultNotificationConfig: Union[
+            VaultNotificationConfigTypeDef, VaultNotificationConfigOutputTypeDef
+        ] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation configures notifications that will be sent when specific events
         happen to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#set_vault_notifications)
```

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/client.pyi` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     ListMultipartUploadsPaginator,
     ListPartsPaginator,
     ListVaultsPaginator,
 )
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
+    DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     GetVaultLockOutputTypeDef,
@@ -47,14 +48,15 @@
     ListProvisionedCapacityOutputTypeDef,
     ListTagsForVaultOutputTypeDef,
     ListVaultsOutputTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
     VaultAccessPolicyTypeDef,
     VaultLockPolicyTypeDef,
+    VaultNotificationConfigOutputTypeDef,
     VaultNotificationConfigTypeDef,
 )
 from .waiter import VaultExistsWaiter, VaultNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -413,15 +415,18 @@
         This operation removes one or more tags from the set of tags attached to a
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.remove_tags_from_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#remove_tags_from_vault)
         """
     def set_data_retrieval_policy(
-        self, *, accountId: str = "-", Policy: DataRetrievalPolicyTypeDef = ...
+        self,
+        *,
+        accountId: str = "-",
+        Policy: Union[DataRetrievalPolicyTypeDef, DataRetrievalPolicyOutputTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation sets and then enacts a data retrieval policy in the region
         specified in the PUT request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_data_retrieval_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#set_data_retrieval_policy)
@@ -437,15 +442,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#set_vault_access_policy)
         """
     def set_vault_notifications(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
-        vaultNotificationConfig: VaultNotificationConfigTypeDef = ...
+        vaultNotificationConfig: Union[
+            VaultNotificationConfigTypeDef, VaultNotificationConfigOutputTypeDef
+        ] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation configures notifications that will be sent when specific events
         happen to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#set_vault_notifications)
```

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/literals.py` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/literals.pyi` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/paginator.py` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/paginator.pyi` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/service_resource.py` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/service_resource.pyi` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/type_defs.py` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/type_defs.pyi` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/waiter.py` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/waiter.pyi` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/PKG-INFO` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glacier
-Version: 1.28.15
-Summary: Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/SOURCES.txt` & `mypy-boto3-glacier-1.28.15.post1/mypy_boto3_glacier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.15/setup.py` & `mypy-boto3-glacier-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glacier",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_glacier"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder"
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

