# Comparing `tmp/mypy-boto3-cognito-identity-1.28.12.tar.gz` & `tmp/mypy-boto3-cognito-identity-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-identity-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
+gzip compressed data, was "mypy-boto3-cognito-identity-1.28.15.tar", last modified: Fri Jul 28 20:42:31 2023, max compression
```

## Comparing `mypy-boto3-cognito-identity-1.28.12.tar` & `mypy-boto3-cognito-identity-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.460549 mypy-boto3-cognito-identity-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-27 05:34:29.460549 mypy-boto3-cognito-identity-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.456549 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-07-27 05:19:17.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19545 2023-07-27 05:19:17.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.456549 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.460549 mypy-boto3-cognito-identity-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.668869 mypy-boto3-cognito-identity-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-28 20:42:31.668869 mypy-boto3-cognito-identity-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.660869 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-07-28 20:21:48.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.668869 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-28 20:42:31.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:42:31.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:31.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:42:31.000000 mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:31.668869 mypy-boto3-cognito-identity-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 20:21:47.000000 mypy-boto3-cognito-identity-1.28.15/setup.py
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/LICENSE` & `mypy-boto3-cognito-identity-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.12/PKG-INFO` & `mypy-boto3-cognito-identity-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-identity
-Version: 1.28.12
-Summary: Type annotations for boto3.CognitoIdentity 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CognitoIdentity 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-identity)](https://pepy.tech/project/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,72 +326,70 @@
 ### Typed dictionaries
 
 `mypy_boto3_cognito_identity.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
-    CognitoIdentityProviderOutputTypeDef,
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityInputRequestTypeDef,
     GetIdInputRequestTypeDef,
-    GetIdResponseTypeDef,
     GetIdentityPoolRolesInputRequestTypeDef,
     GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenInputRequestTypeDef,
-    GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapInputRequestTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
     IdentityDescriptionTypeDef,
     IdentityPoolShortDescriptionTypeDef,
     ListIdentitiesInputRequestTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
-    MappingRuleOutputTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    IdentityPoolTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
+    GetIdResponseTypeDef,
+    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
+    GetOpenIdTokenResponseTypeDef,
+    GetPrincipalTagAttributeMapResponseTypeDef,
+    IdentityDescriptionResponseTypeDef,
+    IdentityPoolTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    LookupDeveloperIdentityResponseTypeDef,
+    MergeDeveloperIdentitiesResponseTypeDef,
+    SetPrincipalTagAttributeMapResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
+    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
     RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderOutputTypeDef:
+def get_structure() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/README.md` & `mypy-boto3-cognito-identity-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-identity)](https://pepy.tech/project/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,72 +294,70 @@
 ### Typed dictionaries
 
 `mypy_boto3_cognito_identity.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
-    CognitoIdentityProviderOutputTypeDef,
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityInputRequestTypeDef,
     GetIdInputRequestTypeDef,
-    GetIdResponseTypeDef,
     GetIdentityPoolRolesInputRequestTypeDef,
     GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenInputRequestTypeDef,
-    GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapInputRequestTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
     IdentityDescriptionTypeDef,
     IdentityPoolShortDescriptionTypeDef,
     ListIdentitiesInputRequestTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
-    MappingRuleOutputTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    IdentityPoolTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
+    GetIdResponseTypeDef,
+    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
+    GetOpenIdTokenResponseTypeDef,
+    GetPrincipalTagAttributeMapResponseTypeDef,
+    IdentityDescriptionResponseTypeDef,
+    IdentityPoolTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    LookupDeveloperIdentityResponseTypeDef,
+    MergeDeveloperIdentitiesResponseTypeDef,
+    SetPrincipalTagAttributeMapResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
+    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
     RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderOutputTypeDef:
+def get_structure() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__init__.py` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__init__.pyi` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__main__.py` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoIdentity 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CognitoIdentity 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/client.py` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     GetIdResponseTypeDef,
     GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
+    IdentityDescriptionResponseTypeDef,
     IdentityPoolTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
     RoleMappingTypeDef,
@@ -139,15 +139,15 @@
         """
         Deletes an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.delete_identity_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/client/#delete_identity_pool)
         """
 
-    def describe_identity(self, *, IdentityId: str) -> IdentityDescriptionResponseMetadataTypeDef:
+    def describe_identity(self, *, IdentityId: str) -> IdentityDescriptionResponseTypeDef:
         """
         Returns metadata related to the given identity, including when the identity was
         created and any associated linked logins.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.describe_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/client/#describe_identity)
         """
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/client.pyi` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     GetIdResponseTypeDef,
     GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
+    IdentityDescriptionResponseTypeDef,
     IdentityPoolTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
     RoleMappingTypeDef,
@@ -129,15 +129,15 @@
     def delete_identity_pool(self, *, IdentityPoolId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.delete_identity_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/client/#delete_identity_pool)
         """
-    def describe_identity(self, *, IdentityId: str) -> IdentityDescriptionResponseMetadataTypeDef:
+    def describe_identity(self, *, IdentityId: str) -> IdentityDescriptionResponseTypeDef:
         """
         Returns metadata related to the given identity, including when the identity was
         created and any associated linked logins.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.describe_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/client/#describe_identity)
         """
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/literals.py` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/literals.pyi` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/paginator.py` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListIdentityPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/paginators/#listidentitypoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentityPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/paginators/#listidentitypoolspaginator)
         """
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/paginator.pyi` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListIdentityPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/paginators/#listidentitypoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentityPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/paginators/#listidentitypoolspaginator)
         """
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/type_defs.py` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cognito-identity service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cognito_identity.type_defs import CognitoIdentityProviderOutputTypeDef
+    from mypy_boto3_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
 
-    data: CognitoIdentityProviderOutputTypeDef = {...}
+    data: CognitoIdentityProviderTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -25,80 +25,68 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "CognitoIdentityProviderOutputTypeDef",
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
     "DescribeIdentityInputRequestTypeDef",
     "DescribeIdentityPoolInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCredentialsForIdentityInputRequestTypeDef",
     "GetIdInputRequestTypeDef",
-    "GetIdResponseTypeDef",
     "GetIdentityPoolRolesInputRequestTypeDef",
     "GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef",
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
     "GetOpenIdTokenInputRequestTypeDef",
-    "GetOpenIdTokenResponseTypeDef",
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    "IdentityDescriptionResponseMetadataTypeDef",
     "IdentityDescriptionTypeDef",
     "IdentityPoolShortDescriptionTypeDef",
     "ListIdentitiesInputRequestTypeDef",
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListIdentityPoolsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "LookupDeveloperIdentityInputRequestTypeDef",
-    "LookupDeveloperIdentityResponseTypeDef",
-    "MappingRuleOutputTypeDef",
     "MappingRuleTypeDef",
     "MergeDeveloperIdentitiesInputRequestTypeDef",
-    "MergeDeveloperIdentitiesResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SetPrincipalTagAttributeMapInputRequestTypeDef",
-    "SetPrincipalTagAttributeMapResponseTypeDef",
     "TagResourceInputRequestTypeDef",
     "UnlinkDeveloperIdentityInputRequestTypeDef",
     "UnlinkIdentityInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "IdentityPoolTypeDef",
     "CreateIdentityPoolInputRequestTypeDef",
     "IdentityPoolRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCredentialsForIdentityResponseTypeDef",
+    "GetIdResponseTypeDef",
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
+    "GetOpenIdTokenResponseTypeDef",
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    "IdentityDescriptionResponseTypeDef",
+    "IdentityPoolTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "LookupDeveloperIdentityResponseTypeDef",
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    "SetPrincipalTagAttributeMapResponseTypeDef",
     "DeleteIdentitiesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoolsResponseTypeDef",
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     "RulesConfigurationTypeOutputTypeDef",
     "RulesConfigurationTypeTypeDef",
     "RoleMappingOutputTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
-CognitoIdentityProviderOutputTypeDef = TypedDict(
-    "CognitoIdentityProviderOutputTypeDef",
-    {
-        "ProviderName": str,
-        "ClientId": str,
-        "ServerSideTokenCheck": bool,
-    },
-    total=False,
-)
-
 CognitoIdentityProviderTypeDef = TypedDict(
     "CognitoIdentityProviderTypeDef",
     {
         "ProviderName": str,
         "ClientId": str,
         "ServerSideTokenCheck": bool,
     },
@@ -119,14 +107,25 @@
 DeleteIdentitiesInputRequestTypeDef = TypedDict(
     "DeleteIdentitiesInputRequestTypeDef",
     {
         "IdentityIdsToDelete": Sequence[str],
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 UnprocessedIdentityIdTypeDef = TypedDict(
     "UnprocessedIdentityIdTypeDef",
     {
         "IdentityId": str,
         "ErrorCode": ErrorCodeType,
     },
     total=False,
@@ -149,21 +148,14 @@
 DescribeIdentityPoolInputRequestTypeDef = TypedDict(
     "DescribeIdentityPoolInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
     "_RequiredGetCredentialsForIdentityInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
@@ -201,22 +193,14 @@
 
 class GetIdInputRequestTypeDef(
     _RequiredGetIdInputRequestTypeDef, _OptionalGetIdInputRequestTypeDef
 ):
     pass
 
 
-GetIdResponseTypeDef = TypedDict(
-    "GetIdResponseTypeDef",
-    {
-        "IdentityId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "GetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -241,23 +225,14 @@
 class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(
     _RequiredGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
     _OptionalGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
 
-GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_RequiredGetOpenIdTokenInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetOpenIdTokenInputRequestTypeDef = TypedDict(
@@ -271,53 +246,22 @@
 
 class GetOpenIdTokenInputRequestTypeDef(
     _RequiredGetOpenIdTokenInputRequestTypeDef, _OptionalGetOpenIdTokenInputRequestTypeDef
 ):
     pass
 
 
-GetOpenIdTokenResponseTypeDef = TypedDict(
-    "GetOpenIdTokenResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
 
-GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IdentityDescriptionResponseMetadataTypeDef = TypedDict(
-    "IdentityDescriptionResponseMetadataTypeDef",
-    {
-        "IdentityId": str,
-        "Logins": List[str],
-        "CreationDate": datetime,
-        "LastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentityDescriptionTypeDef = TypedDict(
     "IdentityDescriptionTypeDef",
     {
         "IdentityId": str,
         "Logins": List[str],
         "CreationDate": datetime,
         "LastModifiedDate": datetime,
@@ -353,18 +297,20 @@
 
 class ListIdentitiesInputRequestTypeDef(
     _RequiredListIdentitiesInputRequestTypeDef, _OptionalListIdentitiesInputRequestTypeDef
 ):
     pass
 
 
-ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 _RequiredListIdentityPoolsInputRequestTypeDef = TypedDict(
     "_RequiredListIdentityPoolsInputRequestTypeDef",
     {
@@ -389,22 +335,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
     "_RequiredLookupDeveloperIdentityInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
@@ -422,34 +360,14 @@
 class LookupDeveloperIdentityInputRequestTypeDef(
     _RequiredLookupDeveloperIdentityInputRequestTypeDef,
     _OptionalLookupDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
 
-LookupDeveloperIdentityResponseTypeDef = TypedDict(
-    "LookupDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "DeveloperUserIdentifierList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MappingRuleOutputTypeDef = TypedDict(
-    "MappingRuleOutputTypeDef",
-    {
-        "Claim": str,
-        "MatchType": MappingRuleMatchTypeType,
-        "Value": str,
-        "RoleARN": str,
-    },
-)
-
 MappingRuleTypeDef = TypedDict(
     "MappingRuleTypeDef",
     {
         "Claim": str,
         "MatchType": MappingRuleMatchTypeType,
         "Value": str,
         "RoleARN": str,
@@ -462,43 +380,14 @@
         "SourceUserIdentifier": str,
         "DestinationUserIdentifier": str,
         "DeveloperProviderName": str,
         "IdentityPoolId": str,
     },
 )
 
-MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
-    "MergeDeveloperIdentitiesResponseTypeDef",
-    {
-        "IdentityId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "_RequiredSetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
@@ -515,25 +404,14 @@
 class SetPrincipalTagAttributeMapInputRequestTypeDef(
     _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef,
     _OptionalSetPrincipalTagAttributeMapInputRequestTypeDef,
 ):
     pass
 
 
-SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "SetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -561,31 +439,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-IdentityPoolTypeDef = TypedDict(
-    "IdentityPoolTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityPoolName": str,
-        "AllowUnauthenticatedIdentities": bool,
-        "AllowClassicFlow": bool,
-        "SupportedLoginProviders": Dict[str, str],
-        "DeveloperProviderName": str,
-        "OpenIdConnectProviderARNs": List[str],
-        "CognitoIdentityProviders": List[CognitoIdentityProviderOutputTypeDef],
-        "SamlProviderARNs": List[str],
-        "IdentityPoolTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateIdentityPoolInputRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityPoolInputRequestTypeDef",
     {
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
     },
 )
@@ -635,54 +496,171 @@
 
 class IdentityPoolRequestTypeDef(
     _RequiredIdentityPoolRequestTypeDef, _OptionalIdentityPoolRequestTypeDef
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetCredentialsForIdentityResponseTypeDef = TypedDict(
     "GetCredentialsForIdentityResponseTypeDef",
     {
         "IdentityId": str,
         "Credentials": CredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIdResponseTypeDef = TypedDict(
+    "GetIdResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpenIdTokenResponseTypeDef = TypedDict(
+    "GetOpenIdTokenResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IdentityDescriptionResponseTypeDef = TypedDict(
+    "IdentityDescriptionResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Logins": List[str],
+        "CreationDate": datetime,
+        "LastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IdentityPoolTypeDef = TypedDict(
+    "IdentityPoolTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityPoolName": str,
+        "AllowUnauthenticatedIdentities": bool,
+        "AllowClassicFlow": bool,
+        "SupportedLoginProviders": Dict[str, str],
+        "DeveloperProviderName": str,
+        "OpenIdConnectProviderARNs": List[str],
+        "CognitoIdentityProviders": List[CognitoIdentityProviderTypeDef],
+        "SamlProviderARNs": List[str],
+        "IdentityPoolTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LookupDeveloperIdentityResponseTypeDef = TypedDict(
+    "LookupDeveloperIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "DeveloperUserIdentifierList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "SetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteIdentitiesResponseTypeDef = TypedDict(
     "DeleteIdentitiesResponseTypeDef",
     {
         "UnprocessedIdentityIds": List[UnprocessedIdentityIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentitiesResponseTypeDef = TypedDict(
     "ListIdentitiesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Identities": List[IdentityDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityPoolsResponseTypeDef = TypedDict(
     "ListIdentityPoolsResponseTypeDef",
     {
         "IdentityPools": List[IdentityPoolShortDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 RulesConfigurationTypeOutputTypeDef = TypedDict(
     "RulesConfigurationTypeOutputTypeDef",
     {
-        "Rules": List[MappingRuleOutputTypeDef],
+        "Rules": List[MappingRuleTypeDef],
     },
 )
 
 RulesConfigurationTypeTypeDef = TypedDict(
     "RulesConfigurationTypeTypeDef",
     {
         "Rules": Sequence[MappingRuleTypeDef],
@@ -733,15 +711,15 @@
 
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
         "RoleMappings": Dict[str, RoleMappingOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/type_defs.pyi` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cognito-identity service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cognito_identity.type_defs import CognitoIdentityProviderOutputTypeDef
+    from mypy_boto3_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
 
-    data: CognitoIdentityProviderOutputTypeDef = {...}
+    data: CognitoIdentityProviderTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -24,80 +24,68 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "CognitoIdentityProviderOutputTypeDef",
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
     "DescribeIdentityInputRequestTypeDef",
     "DescribeIdentityPoolInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCredentialsForIdentityInputRequestTypeDef",
     "GetIdInputRequestTypeDef",
-    "GetIdResponseTypeDef",
     "GetIdentityPoolRolesInputRequestTypeDef",
     "GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef",
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
     "GetOpenIdTokenInputRequestTypeDef",
-    "GetOpenIdTokenResponseTypeDef",
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    "IdentityDescriptionResponseMetadataTypeDef",
     "IdentityDescriptionTypeDef",
     "IdentityPoolShortDescriptionTypeDef",
     "ListIdentitiesInputRequestTypeDef",
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListIdentityPoolsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "LookupDeveloperIdentityInputRequestTypeDef",
-    "LookupDeveloperIdentityResponseTypeDef",
-    "MappingRuleOutputTypeDef",
     "MappingRuleTypeDef",
     "MergeDeveloperIdentitiesInputRequestTypeDef",
-    "MergeDeveloperIdentitiesResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SetPrincipalTagAttributeMapInputRequestTypeDef",
-    "SetPrincipalTagAttributeMapResponseTypeDef",
     "TagResourceInputRequestTypeDef",
     "UnlinkDeveloperIdentityInputRequestTypeDef",
     "UnlinkIdentityInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "IdentityPoolTypeDef",
     "CreateIdentityPoolInputRequestTypeDef",
     "IdentityPoolRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCredentialsForIdentityResponseTypeDef",
+    "GetIdResponseTypeDef",
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
+    "GetOpenIdTokenResponseTypeDef",
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    "IdentityDescriptionResponseTypeDef",
+    "IdentityPoolTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "LookupDeveloperIdentityResponseTypeDef",
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    "SetPrincipalTagAttributeMapResponseTypeDef",
     "DeleteIdentitiesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoolsResponseTypeDef",
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     "RulesConfigurationTypeOutputTypeDef",
     "RulesConfigurationTypeTypeDef",
     "RoleMappingOutputTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
-CognitoIdentityProviderOutputTypeDef = TypedDict(
-    "CognitoIdentityProviderOutputTypeDef",
-    {
-        "ProviderName": str,
-        "ClientId": str,
-        "ServerSideTokenCheck": bool,
-    },
-    total=False,
-)
-
 CognitoIdentityProviderTypeDef = TypedDict(
     "CognitoIdentityProviderTypeDef",
     {
         "ProviderName": str,
         "ClientId": str,
         "ServerSideTokenCheck": bool,
     },
@@ -118,14 +106,25 @@
 DeleteIdentitiesInputRequestTypeDef = TypedDict(
     "DeleteIdentitiesInputRequestTypeDef",
     {
         "IdentityIdsToDelete": Sequence[str],
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 UnprocessedIdentityIdTypeDef = TypedDict(
     "UnprocessedIdentityIdTypeDef",
     {
         "IdentityId": str,
         "ErrorCode": ErrorCodeType,
     },
     total=False,
@@ -148,21 +147,14 @@
 DescribeIdentityPoolInputRequestTypeDef = TypedDict(
     "DescribeIdentityPoolInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
     "_RequiredGetCredentialsForIdentityInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
@@ -196,22 +188,14 @@
 )
 
 class GetIdInputRequestTypeDef(
     _RequiredGetIdInputRequestTypeDef, _OptionalGetIdInputRequestTypeDef
 ):
     pass
 
-GetIdResponseTypeDef = TypedDict(
-    "GetIdResponseTypeDef",
-    {
-        "IdentityId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "GetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -234,23 +218,14 @@
 
 class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(
     _RequiredGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
     _OptionalGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
-GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_RequiredGetOpenIdTokenInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetOpenIdTokenInputRequestTypeDef = TypedDict(
@@ -262,53 +237,22 @@
 )
 
 class GetOpenIdTokenInputRequestTypeDef(
     _RequiredGetOpenIdTokenInputRequestTypeDef, _OptionalGetOpenIdTokenInputRequestTypeDef
 ):
     pass
 
-GetOpenIdTokenResponseTypeDef = TypedDict(
-    "GetOpenIdTokenResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
 
-GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IdentityDescriptionResponseMetadataTypeDef = TypedDict(
-    "IdentityDescriptionResponseMetadataTypeDef",
-    {
-        "IdentityId": str,
-        "Logins": List[str],
-        "CreationDate": datetime,
-        "LastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentityDescriptionTypeDef = TypedDict(
     "IdentityDescriptionTypeDef",
     {
         "IdentityId": str,
         "Logins": List[str],
         "CreationDate": datetime,
         "LastModifiedDate": datetime,
@@ -342,18 +286,20 @@
 )
 
 class ListIdentitiesInputRequestTypeDef(
     _RequiredListIdentitiesInputRequestTypeDef, _OptionalListIdentitiesInputRequestTypeDef
 ):
     pass
 
-ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 _RequiredListIdentityPoolsInputRequestTypeDef = TypedDict(
     "_RequiredListIdentityPoolsInputRequestTypeDef",
     {
@@ -376,22 +322,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
     "_RequiredLookupDeveloperIdentityInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
@@ -407,34 +345,14 @@
 
 class LookupDeveloperIdentityInputRequestTypeDef(
     _RequiredLookupDeveloperIdentityInputRequestTypeDef,
     _OptionalLookupDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
-LookupDeveloperIdentityResponseTypeDef = TypedDict(
-    "LookupDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "DeveloperUserIdentifierList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MappingRuleOutputTypeDef = TypedDict(
-    "MappingRuleOutputTypeDef",
-    {
-        "Claim": str,
-        "MatchType": MappingRuleMatchTypeType,
-        "Value": str,
-        "RoleARN": str,
-    },
-)
-
 MappingRuleTypeDef = TypedDict(
     "MappingRuleTypeDef",
     {
         "Claim": str,
         "MatchType": MappingRuleMatchTypeType,
         "Value": str,
         "RoleARN": str,
@@ -447,43 +365,14 @@
         "SourceUserIdentifier": str,
         "DestinationUserIdentifier": str,
         "DeveloperProviderName": str,
         "IdentityPoolId": str,
     },
 )
 
-MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
-    "MergeDeveloperIdentitiesResponseTypeDef",
-    {
-        "IdentityId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "_RequiredSetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
@@ -498,25 +387,14 @@
 
 class SetPrincipalTagAttributeMapInputRequestTypeDef(
     _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef,
     _OptionalSetPrincipalTagAttributeMapInputRequestTypeDef,
 ):
     pass
 
-SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "SetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -544,31 +422,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-IdentityPoolTypeDef = TypedDict(
-    "IdentityPoolTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityPoolName": str,
-        "AllowUnauthenticatedIdentities": bool,
-        "AllowClassicFlow": bool,
-        "SupportedLoginProviders": Dict[str, str],
-        "DeveloperProviderName": str,
-        "OpenIdConnectProviderARNs": List[str],
-        "CognitoIdentityProviders": List[CognitoIdentityProviderOutputTypeDef],
-        "SamlProviderARNs": List[str],
-        "IdentityPoolTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateIdentityPoolInputRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityPoolInputRequestTypeDef",
     {
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
     },
 )
@@ -614,54 +475,171 @@
 )
 
 class IdentityPoolRequestTypeDef(
     _RequiredIdentityPoolRequestTypeDef, _OptionalIdentityPoolRequestTypeDef
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetCredentialsForIdentityResponseTypeDef = TypedDict(
     "GetCredentialsForIdentityResponseTypeDef",
     {
         "IdentityId": str,
         "Credentials": CredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIdResponseTypeDef = TypedDict(
+    "GetIdResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpenIdTokenResponseTypeDef = TypedDict(
+    "GetOpenIdTokenResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IdentityDescriptionResponseTypeDef = TypedDict(
+    "IdentityDescriptionResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Logins": List[str],
+        "CreationDate": datetime,
+        "LastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IdentityPoolTypeDef = TypedDict(
+    "IdentityPoolTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityPoolName": str,
+        "AllowUnauthenticatedIdentities": bool,
+        "AllowClassicFlow": bool,
+        "SupportedLoginProviders": Dict[str, str],
+        "DeveloperProviderName": str,
+        "OpenIdConnectProviderARNs": List[str],
+        "CognitoIdentityProviders": List[CognitoIdentityProviderTypeDef],
+        "SamlProviderARNs": List[str],
+        "IdentityPoolTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LookupDeveloperIdentityResponseTypeDef = TypedDict(
+    "LookupDeveloperIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "DeveloperUserIdentifierList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "SetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteIdentitiesResponseTypeDef = TypedDict(
     "DeleteIdentitiesResponseTypeDef",
     {
         "UnprocessedIdentityIds": List[UnprocessedIdentityIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentitiesResponseTypeDef = TypedDict(
     "ListIdentitiesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Identities": List[IdentityDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityPoolsResponseTypeDef = TypedDict(
     "ListIdentityPoolsResponseTypeDef",
     {
         "IdentityPools": List[IdentityPoolShortDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 RulesConfigurationTypeOutputTypeDef = TypedDict(
     "RulesConfigurationTypeOutputTypeDef",
     {
-        "Rules": List[MappingRuleOutputTypeDef],
+        "Rules": List[MappingRuleTypeDef],
     },
 )
 
 RulesConfigurationTypeTypeDef = TypedDict(
     "RulesConfigurationTypeTypeDef",
     {
         "Rules": Sequence[MappingRuleTypeDef],
@@ -708,15 +686,15 @@
 
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
         "RoleMappings": Dict[str, RoleMappingOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/PKG-INFO` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-identity
-Version: 1.28.12
-Summary: Type annotations for boto3.CognitoIdentity 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CognitoIdentity 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-identity)](https://pepy.tech/project/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,72 +326,70 @@
 ### Typed dictionaries
 
 `mypy_boto3_cognito_identity.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
-    CognitoIdentityProviderOutputTypeDef,
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityInputRequestTypeDef,
     GetIdInputRequestTypeDef,
-    GetIdResponseTypeDef,
     GetIdentityPoolRolesInputRequestTypeDef,
     GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenInputRequestTypeDef,
-    GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapInputRequestTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
     IdentityDescriptionTypeDef,
     IdentityPoolShortDescriptionTypeDef,
     ListIdentitiesInputRequestTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
-    MappingRuleOutputTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    IdentityPoolTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
+    GetIdResponseTypeDef,
+    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
+    GetOpenIdTokenResponseTypeDef,
+    GetPrincipalTagAttributeMapResponseTypeDef,
+    IdentityDescriptionResponseTypeDef,
+    IdentityPoolTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    LookupDeveloperIdentityResponseTypeDef,
+    MergeDeveloperIdentitiesResponseTypeDef,
+    SetPrincipalTagAttributeMapResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
+    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
     RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderOutputTypeDef:
+def get_structure() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/SOURCES.txt` & `mypy-boto3-cognito-identity-1.28.15/mypy_boto3_cognito_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.12/setup.py` & `mypy-boto3-cognito-identity-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-identity",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cognito_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoIdentity 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CognitoIdentity 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

