# Comparing `tmp/mypy-boto3-amplify-1.28.15.tar.gz` & `tmp/mypy-boto3-amplify-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplify-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
+gzip compressed data, was "mypy-boto3-amplify-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:23 2023, max compression
```

## Comparing `mypy-boto3-amplify-1.28.15.tar` & `mypy-boto3-amplify-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.632608 mypy-boto3-amplify-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-07-28 20:42:12.632608 mypy-boto3-amplify-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.616608 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27948 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27900 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-28 20:18:50.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-28 20:18:50.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35813 2023-07-28 20:18:51.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35754 2023-07-28 20:18:50.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.632608 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.632608 mypy-boto3-amplify-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.892978 mypy-boto3-amplify-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-29 10:02:23.892978 mypy-boto3-amplify-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.868978 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28127 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35813 2023-07-29 09:37:41.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35754 2023-07-29 09:37:40.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.892978 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:23.000000 mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:23.892978 mypy-boto3-amplify-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:37:39.000000 mypy-boto3-amplify-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-amplify-1.28.15/LICENSE` & `mypy-boto3-amplify-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15/PKG-INFO` & `mypy-boto3-amplify-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.28.15
-Summary: Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-amplify-1.28.15/README.md` & `mypy-boto3-amplify-1.28.15.post1/README.md`

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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__init__.py` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__init__.pyi` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__main__.py` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Amplify 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Amplify 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify\nOther"
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

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/client.py` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .paginator import (
     ListAppsPaginator,
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 from .type_defs import (
+    AutoBranchCreationConfigOutputTypeDef,
     AutoBranchCreationConfigTypeDef,
     CreateAppResultTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     CreateWebhookResultTypeDef,
@@ -145,15 +146,17 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...
+        autoBranchCreationConfig: Union[
+            AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
+        ] = ...
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#create_app)
         """
@@ -529,15 +532,17 @@
         enableBasicAuth: bool = ...,
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
+        autoBranchCreationConfig: Union[
+            AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
+        ] = ...,
         repository: str = ...,
         oauthToken: str = ...,
         accessToken: str = ...
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
```

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/client.pyi` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .paginator import (
     ListAppsPaginator,
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 from .type_defs import (
+    AutoBranchCreationConfigOutputTypeDef,
     AutoBranchCreationConfigTypeDef,
     CreateAppResultTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     CreateWebhookResultTypeDef,
@@ -138,15 +139,17 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...
+        autoBranchCreationConfig: Union[
+            AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
+        ] = ...
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#create_app)
         """
@@ -488,15 +491,17 @@
         enableBasicAuth: bool = ...,
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
+        autoBranchCreationConfig: Union[
+            AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
+        ] = ...,
         repository: str = ...,
         oauthToken: str = ...,
         accessToken: str = ...
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
```

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/literals.py` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/literals.pyi` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/paginator.py` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/paginator.pyi` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/type_defs.py` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/type_defs.pyi` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/PKG-INFO` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.28.15
-Summary: Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/SOURCES.txt` & `mypy-boto3-amplify-1.28.15.post1/mypy_boto3_amplify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.15/setup.py` & `mypy-boto3-amplify-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplify",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_amplify"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder"
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

