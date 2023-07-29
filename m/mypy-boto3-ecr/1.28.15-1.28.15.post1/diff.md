# Comparing `tmp/mypy-boto3-ecr-1.28.15.tar.gz` & `tmp/mypy-boto3-ecr-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-1.28.15.tar", last modified: Fri Jul 28 20:42:43 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
```

## Comparing `mypy-boto3-ecr-1.28.15.tar` & `mypy-boto3-ecr-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.377035 mypy-boto3-ecr-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20107 2023-07-28 20:42:43.373035 mypy-boto3-ecr-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18636 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.361035 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33677 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33621 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52907 2023-07-28 20:24:45.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52832 2023-07-28 20:24:45.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.373035 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20107 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.377035 mypy-boto3-ecr-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.097126 mypy-boto3-ecr-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-07-29 10:03:02.097126 mypy-boto3-ecr-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18636 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.093126 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33909 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33853 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52949 2023-07-29 09:44:15.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52874 2023-07-29 09:44:14.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-29 09:44:13.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.097126 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:01.000000 mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.097126 mypy-boto3-ecr-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:44:12.000000 mypy-boto3-ecr-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-ecr-1.28.15/LICENSE` & `mypy-boto3-ecr-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15/PKG-INFO` & `mypy-boto3-ecr-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.28.15
-Summary: Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecr-1.28.15/README.md` & `mypy-boto3-ecr-1.28.15.post1/README.md`

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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__init__.py` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__init__.pyi` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__main__.py` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECR 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.ECR 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR\nOther"
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

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/client.py` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,17 @@
     PutImageResponseTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
+    RegistryScanningRuleOutputTypeDef,
     RegistryScanningRuleTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartImageScanResponseTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     TagTypeDef,
     UploadLayerPartResponseTypeDef,
 )
@@ -572,25 +574,32 @@
         Creates or updates the permissions policy for your registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_registry_policy)
         """
 
     def put_registry_scanning_configuration(
-        self, *, scanType: ScanTypeType = ..., rules: Sequence[RegistryScanningRuleTypeDef] = ...
+        self,
+        *,
+        scanType: ScanTypeType = ...,
+        rules: Sequence[Union[RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef]] = ...
     ) -> PutRegistryScanningConfigurationResponseTypeDef:
         """
         Creates or updates the scanning configuration for your private registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_scanning_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_registry_scanning_configuration)
         """
 
     def put_replication_configuration(
-        self, *, replicationConfiguration: ReplicationConfigurationTypeDef
+        self,
+        *,
+        replicationConfiguration: Union[
+            ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+        ]
     ) -> PutReplicationConfigurationResponseTypeDef:
         """
         Creates or updates the replication configuration for a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_replication_configuration)
         """
```

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/client.pyi` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,17 @@
     PutImageResponseTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
+    RegistryScanningRuleOutputTypeDef,
     RegistryScanningRuleTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartImageScanResponseTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     TagTypeDef,
     UploadLayerPartResponseTypeDef,
 )
@@ -531,24 +533,31 @@
         """
         Creates or updates the permissions policy for your registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_registry_policy)
         """
     def put_registry_scanning_configuration(
-        self, *, scanType: ScanTypeType = ..., rules: Sequence[RegistryScanningRuleTypeDef] = ...
+        self,
+        *,
+        scanType: ScanTypeType = ...,
+        rules: Sequence[Union[RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef]] = ...
     ) -> PutRegistryScanningConfigurationResponseTypeDef:
         """
         Creates or updates the scanning configuration for your private registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_scanning_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_registry_scanning_configuration)
         """
     def put_replication_configuration(
-        self, *, replicationConfiguration: ReplicationConfigurationTypeDef
+        self,
+        *,
+        replicationConfiguration: Union[
+            ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+        ]
     ) -> PutReplicationConfigurationResponseTypeDef:
         """
         Creates or updates the replication configuration for a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/client/#put_replication_configuration)
         """
```

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/literals.py` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/literals.pyi` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/paginator.py` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/paginator.pyi` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/type_defs.py` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1887,15 +1887,15 @@
     total=False,
 )
 
 PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
     "PutRegistryScanningConfigurationRequestRequestTypeDef",
     {
         "scanType": ScanTypeType,
-        "rules": Sequence[RegistryScanningRuleTypeDef],
+        "rules": Sequence[Union[RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef]],
     },
     total=False,
 )
 
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
```

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/type_defs.pyi` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1812,15 +1812,15 @@
     total=False,
 )
 
 PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
     "PutRegistryScanningConfigurationRequestRequestTypeDef",
     {
         "scanType": ScanTypeType,
-        "rules": Sequence[RegistryScanningRuleTypeDef],
+        "rules": Sequence[Union[RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef]],
     },
     total=False,
 )
 
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
```

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/waiter.py` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/waiter.pyi` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/PKG-INFO` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.28.15
-Summary: Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/SOURCES.txt` & `mypy-boto3-ecr-1.28.15.post1/mypy_boto3_ecr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.15/setup.py` & `mypy-boto3-ecr-1.28.15.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_ecr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

