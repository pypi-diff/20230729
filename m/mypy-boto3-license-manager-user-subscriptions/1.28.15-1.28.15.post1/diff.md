# Comparing `tmp/mypy-boto3-license-manager-user-subscriptions-1.28.15.tar.gz` & `tmp/mypy-boto3-license-manager-user-subscriptions-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-user-subscriptions-1.28.15.tar", last modified: Fri Jul 28 20:43:09 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-user-subscriptions-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:33 2023, max compression
```

## Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15.tar` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:09.037388 mypy-boto3-license-manager-user-subscriptions-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-07-28 20:43:09.033388 mypy-boto3-license-manager-user-subscriptions-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:09.033388 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-07-28 20:30:12.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-07-28 20:30:12.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:09.033388 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:09.037388 mypy-boto3-license-manager-user-subscriptions-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.409249 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-29 10:03:33.409249 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.409249 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14566 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-07-29 09:49:49.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-07-29 09:49:49.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.409249 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-29 10:03:33.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:33.409249 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-29 09:49:48.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/LICENSE` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/PKG-INFO` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-user-subscriptions
-Version: 1.28.15
-Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/README.md` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/README.md`

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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__init__.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__init__.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__main__.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions\nOther"
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/client.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_license_manager_user_subscriptions.client import LicenseManagerUserSubscriptionsClient
 
     session = Session()
     client: LicenseManagerUserSubscriptionsClient = session.client("license-manager-user-subscriptions")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListIdentityProvidersPaginator,
     ListInstancesPaginator,
     ListProductSubscriptionsPaginator,
@@ -31,14 +31,15 @@
     FilterTypeDef,
     IdentityProviderTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     ListUserAssociationsResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
     UpdateIdentityProviderSettingsResponseTypeDef,
     UpdateSettingsTypeDef,
 )
 
@@ -210,15 +211,15 @@
         """
 
     def register_identity_provider(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        Settings: SettingsTypeDef = ...
+        Settings: Union[SettingsTypeDef, SettingsOutputTypeDef] = ...
     ) -> RegisterIdentityProviderResponseTypeDef:
         """
         Registers an identity provider for user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.register_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/client/#register_identity_provider)
         """
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/client.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_license_manager_user_subscriptions.client import LicenseManagerUserSubscriptionsClient
 
     session = Session()
     client: LicenseManagerUserSubscriptionsClient = session.client("license-manager-user-subscriptions")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListIdentityProvidersPaginator,
     ListInstancesPaginator,
     ListProductSubscriptionsPaginator,
@@ -31,14 +31,15 @@
     FilterTypeDef,
     IdentityProviderTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     ListUserAssociationsResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
     UpdateIdentityProviderSettingsResponseTypeDef,
     UpdateSettingsTypeDef,
 )
 
@@ -195,15 +196,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/client/#list_user_associations)
         """
     def register_identity_provider(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        Settings: SettingsTypeDef = ...
+        Settings: Union[SettingsTypeDef, SettingsOutputTypeDef] = ...
     ) -> RegisterIdentityProviderResponseTypeDef:
         """
         Registers an identity provider for user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.register_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/client/#register_identity_provider)
         """
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/literals.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/literals.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/paginator.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/paginator.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/type_defs.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-user-subscriptions
-Version: 1.28.15
-Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.15/setup.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager-user-subscriptions",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_license_manager_user_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with"
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

