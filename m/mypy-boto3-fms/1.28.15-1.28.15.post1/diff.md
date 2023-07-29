# Comparing `tmp/mypy-boto3-fms-1.28.15.tar.gz` & `tmp/mypy-boto3-fms-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fms-1.28.15.tar", last modified: Fri Jul 28 20:42:49 2023, max compression
+gzip compressed data, was "mypy-boto3-fms-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:09 2023, max compression
```

## Comparing `mypy-boto3-fms-1.28.15.tar` & `mypy-boto3-fms-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.965126 mypy-boto3-fms-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-07-28 20:42:49.965126 mypy-boto3-fms-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19649 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.961126 mypy-boto3-fms-1.28.15/mypy_boto3_fms/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30820 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30763 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-28 20:25:58.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-07-28 20:25:58.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63794 2023-07-28 20:26:01.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63719 2023-07-28 20:26:00.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.961126 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:49.965126 mypy-boto3-fms-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.605155 mypy-boto3-fms-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-07-29 10:03:09.605155 mypy-boto3-fms-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19649 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.593155 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31257 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31200 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-29 09:45:30.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63794 2023-07-29 09:45:32.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63719 2023-07-29 09:45:31.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.605155 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21126 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:09.000000 mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:09.605155 mypy-boto3-fms-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:45:29.000000 mypy-boto3-fms-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-fms-1.28.15/LICENSE` & `mypy-boto3-fms-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15/PKG-INFO` & `mypy-boto3-fms-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.28.15
-Summary: Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-fms-1.28.15/README.md` & `mypy-boto3-fms-1.28.15.post1/README.md`

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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/__init__.py` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/__init__.pyi` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/__main__.py` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FMS 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.FMS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
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

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/client.py` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
+    AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
+    AppsListDataOutputTypeDef,
     AppsListDataTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
@@ -57,20 +59,23 @@
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
+    PolicyOutputTypeDef,
     PolicyTypeDef,
+    ProtocolsListDataOutputTypeDef,
     ProtocolsListDataTypeDef,
     PutAppsListResponseTypeDef,
     PutPolicyResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     PutResourceSetResponseTypeDef,
+    ResourceSetOutputTypeDef,
     ResourceSetTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -482,25 +487,31 @@
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_third_party_firewall_firewall_policies)
         """
 
     def put_admin_account(
-        self, *, AdminAccount: str, AdminScope: AdminScopeTypeDef = ...
+        self,
+        *,
+        AdminAccount: str,
+        AdminScope: Union[AdminScopeTypeDef, AdminScopeOutputTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_admin_account)
         """
 
     def put_apps_list(
-        self, *, AppsList: AppsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        AppsList: Union[AppsListDataTypeDef, AppsListDataOutputTypeDef],
+        TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_apps_list)
         """
@@ -513,35 +524,44 @@
         Firewall Manager uses to record SNS logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_notification_channel)
         """
 
     def put_policy(
-        self, *, Policy: PolicyTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        Policy: Union[PolicyTypeDef, PolicyOutputTypeDef],
+        TagList: Sequence[TagTypeDef] = ...
     ) -> PutPolicyResponseTypeDef:
         """
         Creates an Firewall Manager policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_policy)
         """
 
     def put_protocols_list(
-        self, *, ProtocolsList: ProtocolsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        ProtocolsList: Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef],
+        TagList: Sequence[TagTypeDef] = ...
     ) -> PutProtocolsListResponseTypeDef:
         """
         Creates an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_protocols_list)
         """
 
     def put_resource_set(
-        self, *, ResourceSet: ResourceSetTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        ResourceSet: Union[ResourceSetTypeDef, ResourceSetOutputTypeDef],
+        TagList: Sequence[TagTypeDef] = ...
     ) -> PutResourceSetResponseTypeDef:
         """
         Creates the resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_resource_set)
         """
```

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/client.pyi` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
+    AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
+    AppsListDataOutputTypeDef,
     AppsListDataTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
@@ -57,20 +59,23 @@
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
+    PolicyOutputTypeDef,
     PolicyTypeDef,
+    ProtocolsListDataOutputTypeDef,
     ProtocolsListDataTypeDef,
     PutAppsListResponseTypeDef,
     PutPolicyResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     PutResourceSetResponseTypeDef,
+    ResourceSetOutputTypeDef,
     ResourceSetTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -440,24 +445,30 @@
         Retrieves a list of all of the third-party firewall policies that are associated
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_third_party_firewall_firewall_policies)
         """
     def put_admin_account(
-        self, *, AdminAccount: str, AdminScope: AdminScopeTypeDef = ...
+        self,
+        *,
+        AdminAccount: str,
+        AdminScope: Union[AdminScopeTypeDef, AdminScopeOutputTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_admin_account)
         """
     def put_apps_list(
-        self, *, AppsList: AppsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        AppsList: Union[AppsListDataTypeDef, AppsListDataOutputTypeDef],
+        TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_apps_list)
         """
@@ -468,33 +479,42 @@
         Designates the IAM role and Amazon Simple Notification Service (SNS) topic that
         Firewall Manager uses to record SNS logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_notification_channel)
         """
     def put_policy(
-        self, *, Policy: PolicyTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        Policy: Union[PolicyTypeDef, PolicyOutputTypeDef],
+        TagList: Sequence[TagTypeDef] = ...
     ) -> PutPolicyResponseTypeDef:
         """
         Creates an Firewall Manager policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_policy)
         """
     def put_protocols_list(
-        self, *, ProtocolsList: ProtocolsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        ProtocolsList: Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef],
+        TagList: Sequence[TagTypeDef] = ...
     ) -> PutProtocolsListResponseTypeDef:
         """
         Creates an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_protocols_list)
         """
     def put_resource_set(
-        self, *, ResourceSet: ResourceSetTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        ResourceSet: Union[ResourceSetTypeDef, ResourceSetOutputTypeDef],
+        TagList: Sequence[TagTypeDef] = ...
     ) -> PutResourceSetResponseTypeDef:
         """
         Creates the resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_resource_set)
         """
```

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/literals.py` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/literals.pyi` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/paginator.py` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/paginator.pyi` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/type_defs.py` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms/type_defs.pyi` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/PKG-INFO` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.28.15
-Summary: Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/SOURCES.txt` & `mypy-boto3-fms-1.28.15.post1/mypy_boto3_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.15/setup.py` & `mypy-boto3-fms-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fms",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

