# Comparing `tmp/mypy-boto3-workmail-1.28.15.tar.gz` & `tmp/mypy-boto3-workmail-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workmail-1.28.15.tar", last modified: Fri Jul 28 20:43:57 2023, max compression
+gzip compressed data, was "mypy-boto3-workmail-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:26 2023, max compression
```

## Comparing `mypy-boto3-workmail-1.28.15.tar` & `mypy-boto3-workmail-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:57.930059 mypy-boto3-workmail-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21189 2023-07-28 20:43:57.930059 mypy-boto3-workmail-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19698 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:57.930059 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57101 2023-07-28 20:41:37.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57005 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-28 20:41:37.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-07-28 20:41:37.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-28 20:41:37.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-07-28 20:41:37.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60313 2023-07-28 20:41:39.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60232 2023-07-28 20:41:38.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:57.930059 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21189 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:57.930059 mypy-boto3-workmail-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.373459 mypy-boto3-workmail-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21195 2023-07-29 10:04:26.373459 mypy-boto3-workmail-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19698 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.369459 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57222 2023-07-29 10:01:50.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57126 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-29 10:01:50.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-07-29 10:01:50.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-29 10:01:50.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-07-29 10:01:50.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60398 2023-07-29 10:01:52.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60317 2023-07-29 10:01:51.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.373459 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21195 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:04:26.000000 mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:26.373459 mypy-boto3-workmail-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 10:01:45.000000 mypy-boto3-workmail-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-workmail-1.28.15/LICENSE` & `mypy-boto3-workmail-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15/PKG-INFO` & `mypy-boto3-workmail-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workmail
-Version: 1.28.15
-Summary: Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -378,14 +378,15 @@
     LambdaAvailabilityProviderTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
+    ImpersonationRuleOutputTypeDef,
     ImpersonationRuleTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
     DomainTypeDef,
     CreateResourceRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DelegateTypeDef,
     DeleteAccessControlRuleRequestRequestTypeDef,
@@ -415,15 +416,14 @@
     DnsRecordTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
-    ImpersonationRuleOutputTypeDef,
     GetMailDomainRequestRequestTypeDef,
     GetMailboxDetailsRequestRequestTypeDef,
     GetMobileDeviceAccessEffectRequestRequestTypeDef,
     MobileDeviceAccessMatchedRuleTypeDef,
     GetMobileDeviceAccessOverrideRequestRequestTypeDef,
     GroupTypeDef,
     ImpersonationRoleTypeDef,
@@ -491,23 +491,23 @@
     TestAvailabilityConfigurationResponseTypeDef,
     AvailabilityConfigurationTypeDef,
     DescribeResourceResponseTypeDef,
     UpdateResourceRequestRequestTypeDef,
     CreateAvailabilityConfigurationRequestRequestTypeDef,
     TestAvailabilityConfigurationRequestRequestTypeDef,
     UpdateAvailabilityConfigurationRequestRequestTypeDef,
+    GetImpersonationRoleResponseTypeDef,
     CreateImpersonationRoleRequestRequestTypeDef,
     UpdateImpersonationRoleRequestRequestTypeDef,
     CreateOrganizationRequestRequestTypeDef,
     ListResourceDelegatesResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetDefaultRetentionPolicyResponseTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
-    GetImpersonationRoleResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     ListGroupMembersRequestListGroupMembersPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
```

### Comparing `mypy-boto3-workmail-1.28.15/README.md` & `mypy-boto3-workmail-1.28.15.post1/README.md`

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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,14 +346,15 @@
     LambdaAvailabilityProviderTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
+    ImpersonationRuleOutputTypeDef,
     ImpersonationRuleTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
     DomainTypeDef,
     CreateResourceRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DelegateTypeDef,
     DeleteAccessControlRuleRequestRequestTypeDef,
@@ -383,15 +384,14 @@
     DnsRecordTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
-    ImpersonationRuleOutputTypeDef,
     GetMailDomainRequestRequestTypeDef,
     GetMailboxDetailsRequestRequestTypeDef,
     GetMobileDeviceAccessEffectRequestRequestTypeDef,
     MobileDeviceAccessMatchedRuleTypeDef,
     GetMobileDeviceAccessOverrideRequestRequestTypeDef,
     GroupTypeDef,
     ImpersonationRoleTypeDef,
@@ -459,23 +459,23 @@
     TestAvailabilityConfigurationResponseTypeDef,
     AvailabilityConfigurationTypeDef,
     DescribeResourceResponseTypeDef,
     UpdateResourceRequestRequestTypeDef,
     CreateAvailabilityConfigurationRequestRequestTypeDef,
     TestAvailabilityConfigurationRequestRequestTypeDef,
     UpdateAvailabilityConfigurationRequestRequestTypeDef,
+    GetImpersonationRoleResponseTypeDef,
     CreateImpersonationRoleRequestRequestTypeDef,
     UpdateImpersonationRoleRequestRequestTypeDef,
     CreateOrganizationRequestRequestTypeDef,
     ListResourceDelegatesResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetDefaultRetentionPolicyResponseTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
-    GetImpersonationRoleResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     ListGroupMembersRequestListGroupMembersPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
```

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__init__.py` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__init__.pyi` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__main__.py` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkMail 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.WorkMail 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail\nOther"
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

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/client.py` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_workmail.client import WorkMailClient
 
     session = Session()
     client: WorkMailClient = session.client("workmail")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccessControlRuleEffectType,
     ImpersonationRoleTypeType,
     MobileDeviceAccessRuleEffectType,
@@ -60,14 +60,15 @@
     GetDefaultRetentionPolicyResponseTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
     GetImpersonationRoleResponseTypeDef,
     GetMailboxDetailsResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     GetMobileDeviceAccessOverrideResponseTypeDef,
+    ImpersonationRuleOutputTypeDef,
     ImpersonationRuleTypeDef,
     LambdaAvailabilityProviderTypeDef,
     ListAccessControlRulesResponseTypeDef,
     ListAliasesResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
     ListGroupMembersResponseTypeDef,
     ListGroupsResponseTypeDef,
@@ -239,15 +240,15 @@
 
     def create_impersonation_role(
         self,
         *,
         OrganizationId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[ImpersonationRuleTypeDef],
+        Rules: Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
         ClientToken: str = ...,
         Description: str = ...
     ) -> CreateImpersonationRoleResponseTypeDef:
         """
         Creates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_impersonation_role)
@@ -1015,15 +1016,15 @@
     def update_impersonation_role(
         self,
         *,
         OrganizationId: str,
         ImpersonationRoleId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[ImpersonationRuleTypeDef],
+        Rules: Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_impersonation_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/client/#update_impersonation_role)
```

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/client.pyi` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_workmail.client import WorkMailClient
 
     session = Session()
     client: WorkMailClient = session.client("workmail")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccessControlRuleEffectType,
     ImpersonationRoleTypeType,
     MobileDeviceAccessRuleEffectType,
@@ -60,14 +60,15 @@
     GetDefaultRetentionPolicyResponseTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
     GetImpersonationRoleResponseTypeDef,
     GetMailboxDetailsResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     GetMobileDeviceAccessOverrideResponseTypeDef,
+    ImpersonationRuleOutputTypeDef,
     ImpersonationRuleTypeDef,
     LambdaAvailabilityProviderTypeDef,
     ListAccessControlRulesResponseTypeDef,
     ListAliasesResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
     ListGroupMembersResponseTypeDef,
     ListGroupsResponseTypeDef,
@@ -225,15 +226,15 @@
         """
     def create_impersonation_role(
         self,
         *,
         OrganizationId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[ImpersonationRuleTypeDef],
+        Rules: Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
         ClientToken: str = ...,
         Description: str = ...
     ) -> CreateImpersonationRoleResponseTypeDef:
         """
         Creates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_impersonation_role)
@@ -932,15 +933,15 @@
     def update_impersonation_role(
         self,
         *,
         OrganizationId: str,
         ImpersonationRoleId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[ImpersonationRuleTypeDef],
+        Rules: Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_impersonation_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/client/#update_impersonation_role)
```

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/literals.py` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/literals.pyi` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/paginator.py` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/paginator.pyi` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/type_defs.py` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_workmail.type_defs import AccessControlRuleTypeDef
 
     data: AccessControlRuleTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AccessControlRuleEffectType,
     AccessEffectType,
     AvailabilityProviderTypeType,
     DnsRecordVerificationStatusType,
     EntityStateType,
@@ -47,14 +47,15 @@
     "LambdaAvailabilityProviderTypeDef",
     "RedactedEwsAvailabilityProviderTypeDef",
     "BookingOptionsTypeDef",
     "CancelMailboxExportJobRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "EwsAvailabilityProviderTypeDef",
     "CreateGroupRequestRequestTypeDef",
+    "ImpersonationRuleOutputTypeDef",
     "ImpersonationRuleTypeDef",
     "CreateMobileDeviceAccessRuleRequestRequestTypeDef",
     "DomainTypeDef",
     "CreateResourceRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DelegateTypeDef",
     "DeleteAccessControlRuleRequestRequestTypeDef",
@@ -84,15 +85,14 @@
     "DnsRecordTypeDef",
     "FolderConfigurationTypeDef",
     "GetAccessControlEffectRequestRequestTypeDef",
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectRequestRequestTypeDef",
     "ImpersonationMatchedRuleTypeDef",
     "GetImpersonationRoleRequestRequestTypeDef",
-    "ImpersonationRuleOutputTypeDef",
     "GetMailDomainRequestRequestTypeDef",
     "GetMailboxDetailsRequestRequestTypeDef",
     "GetMobileDeviceAccessEffectRequestRequestTypeDef",
     "MobileDeviceAccessMatchedRuleTypeDef",
     "GetMobileDeviceAccessOverrideRequestRequestTypeDef",
     "GroupTypeDef",
     "ImpersonationRoleTypeDef",
@@ -160,23 +160,23 @@
     "TestAvailabilityConfigurationResponseTypeDef",
     "AvailabilityConfigurationTypeDef",
     "DescribeResourceResponseTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "CreateAvailabilityConfigurationRequestRequestTypeDef",
     "TestAvailabilityConfigurationRequestRequestTypeDef",
     "UpdateAvailabilityConfigurationRequestRequestTypeDef",
+    "GetImpersonationRoleResponseTypeDef",
     "CreateImpersonationRoleRequestRequestTypeDef",
     "UpdateImpersonationRoleRequestRequestTypeDef",
     "CreateOrganizationRequestRequestTypeDef",
     "ListResourceDelegatesResponseTypeDef",
     "GetMailDomainResponseTypeDef",
     "GetDefaultRetentionPolicyResponseTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectResponseTypeDef",
-    "GetImpersonationRoleResponseTypeDef",
     "GetMobileDeviceAccessEffectResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "ListImpersonationRolesResponseTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     "ListGroupMembersRequestListGroupMembersPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
@@ -313,14 +313,39 @@
     "CreateGroupRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
     },
 )
 
+_RequiredImpersonationRuleOutputTypeDef = TypedDict(
+    "_RequiredImpersonationRuleOutputTypeDef",
+    {
+        "ImpersonationRuleId": str,
+        "Effect": AccessEffectType,
+    },
+)
+_OptionalImpersonationRuleOutputTypeDef = TypedDict(
+    "_OptionalImpersonationRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetUsers": List[str],
+        "NotTargetUsers": List[str],
+    },
+    total=False,
+)
+
+
+class ImpersonationRuleOutputTypeDef(
+    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredImpersonationRuleTypeDef = TypedDict(
     "_RequiredImpersonationRuleTypeDef",
     {
         "ImpersonationRuleId": str,
         "Effect": AccessEffectType,
     },
 )
@@ -705,39 +730,14 @@
     "GetImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
     },
 )
 
-_RequiredImpersonationRuleOutputTypeDef = TypedDict(
-    "_RequiredImpersonationRuleOutputTypeDef",
-    {
-        "ImpersonationRuleId": str,
-        "Effect": AccessEffectType,
-    },
-)
-_OptionalImpersonationRuleOutputTypeDef = TypedDict(
-    "_OptionalImpersonationRuleOutputTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetUsers": List[str],
-        "NotTargetUsers": List[str],
-    },
-    total=False,
-)
-
-
-class ImpersonationRuleOutputTypeDef(
-    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
-):
-    pass
-
-
 GetMailDomainRequestRequestTypeDef = TypedDict(
     "GetMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1815,21 +1815,35 @@
 class UpdateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalUpdateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+GetImpersonationRoleResponseTypeDef = TypedDict(
+    "GetImpersonationRoleResponseTypeDef",
+    {
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Description": str,
+        "Rules": List[ImpersonationRuleOutputTypeDef],
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[ImpersonationRuleTypeDef],
+        "Rules": Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
     },
 )
 _OptionalCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_OptionalCreateImpersonationRoleRequestRequestTypeDef",
     {
         "ClientToken": str,
         "Description": str,
@@ -1848,15 +1862,15 @@
 _RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
         "Name": str,
         "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[ImpersonationRuleTypeDef],
+        "Rules": Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
     },
 )
 _OptionalUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
     {
         "Description": str,
     },
@@ -1960,28 +1974,14 @@
         "Type": ImpersonationRoleTypeType,
         "Effect": AccessEffectType,
         "MatchedRules": List[ImpersonationMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetImpersonationRoleResponseTypeDef = TypedDict(
-    "GetImpersonationRoleResponseTypeDef",
-    {
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Description": str,
-        "Rules": List[ImpersonationRuleOutputTypeDef],
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetMobileDeviceAccessEffectResponseTypeDef = TypedDict(
     "GetMobileDeviceAccessEffectResponseTypeDef",
     {
         "Effect": MobileDeviceAccessRuleEffectType,
         "MatchedRules": List[MobileDeviceAccessMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/type_defs.pyi` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_workmail.type_defs import AccessControlRuleTypeDef
 
     data: AccessControlRuleTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AccessControlRuleEffectType,
     AccessEffectType,
     AvailabilityProviderTypeType,
     DnsRecordVerificationStatusType,
     EntityStateType,
@@ -46,14 +46,15 @@
     "LambdaAvailabilityProviderTypeDef",
     "RedactedEwsAvailabilityProviderTypeDef",
     "BookingOptionsTypeDef",
     "CancelMailboxExportJobRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "EwsAvailabilityProviderTypeDef",
     "CreateGroupRequestRequestTypeDef",
+    "ImpersonationRuleOutputTypeDef",
     "ImpersonationRuleTypeDef",
     "CreateMobileDeviceAccessRuleRequestRequestTypeDef",
     "DomainTypeDef",
     "CreateResourceRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DelegateTypeDef",
     "DeleteAccessControlRuleRequestRequestTypeDef",
@@ -83,15 +84,14 @@
     "DnsRecordTypeDef",
     "FolderConfigurationTypeDef",
     "GetAccessControlEffectRequestRequestTypeDef",
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectRequestRequestTypeDef",
     "ImpersonationMatchedRuleTypeDef",
     "GetImpersonationRoleRequestRequestTypeDef",
-    "ImpersonationRuleOutputTypeDef",
     "GetMailDomainRequestRequestTypeDef",
     "GetMailboxDetailsRequestRequestTypeDef",
     "GetMobileDeviceAccessEffectRequestRequestTypeDef",
     "MobileDeviceAccessMatchedRuleTypeDef",
     "GetMobileDeviceAccessOverrideRequestRequestTypeDef",
     "GroupTypeDef",
     "ImpersonationRoleTypeDef",
@@ -159,23 +159,23 @@
     "TestAvailabilityConfigurationResponseTypeDef",
     "AvailabilityConfigurationTypeDef",
     "DescribeResourceResponseTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "CreateAvailabilityConfigurationRequestRequestTypeDef",
     "TestAvailabilityConfigurationRequestRequestTypeDef",
     "UpdateAvailabilityConfigurationRequestRequestTypeDef",
+    "GetImpersonationRoleResponseTypeDef",
     "CreateImpersonationRoleRequestRequestTypeDef",
     "UpdateImpersonationRoleRequestRequestTypeDef",
     "CreateOrganizationRequestRequestTypeDef",
     "ListResourceDelegatesResponseTypeDef",
     "GetMailDomainResponseTypeDef",
     "GetDefaultRetentionPolicyResponseTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectResponseTypeDef",
-    "GetImpersonationRoleResponseTypeDef",
     "GetMobileDeviceAccessEffectResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "ListImpersonationRolesResponseTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     "ListGroupMembersRequestListGroupMembersPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
@@ -312,14 +312,37 @@
     "CreateGroupRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
     },
 )
 
+_RequiredImpersonationRuleOutputTypeDef = TypedDict(
+    "_RequiredImpersonationRuleOutputTypeDef",
+    {
+        "ImpersonationRuleId": str,
+        "Effect": AccessEffectType,
+    },
+)
+_OptionalImpersonationRuleOutputTypeDef = TypedDict(
+    "_OptionalImpersonationRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetUsers": List[str],
+        "NotTargetUsers": List[str],
+    },
+    total=False,
+)
+
+class ImpersonationRuleOutputTypeDef(
+    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
+):
+    pass
+
 _RequiredImpersonationRuleTypeDef = TypedDict(
     "_RequiredImpersonationRuleTypeDef",
     {
         "ImpersonationRuleId": str,
         "Effect": AccessEffectType,
     },
 )
@@ -694,37 +717,14 @@
     "GetImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
     },
 )
 
-_RequiredImpersonationRuleOutputTypeDef = TypedDict(
-    "_RequiredImpersonationRuleOutputTypeDef",
-    {
-        "ImpersonationRuleId": str,
-        "Effect": AccessEffectType,
-    },
-)
-_OptionalImpersonationRuleOutputTypeDef = TypedDict(
-    "_OptionalImpersonationRuleOutputTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetUsers": List[str],
-        "NotTargetUsers": List[str],
-    },
-    total=False,
-)
-
-class ImpersonationRuleOutputTypeDef(
-    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
-):
-    pass
-
 GetMailDomainRequestRequestTypeDef = TypedDict(
     "GetMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1758,21 +1758,35 @@
 
 class UpdateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalUpdateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
+GetImpersonationRoleResponseTypeDef = TypedDict(
+    "GetImpersonationRoleResponseTypeDef",
+    {
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Description": str,
+        "Rules": List[ImpersonationRuleOutputTypeDef],
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[ImpersonationRuleTypeDef],
+        "Rules": Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
     },
 )
 _OptionalCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_OptionalCreateImpersonationRoleRequestRequestTypeDef",
     {
         "ClientToken": str,
         "Description": str,
@@ -1789,15 +1803,15 @@
 _RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
         "Name": str,
         "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[ImpersonationRuleTypeDef],
+        "Rules": Sequence[Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]],
     },
 )
 _OptionalUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
     {
         "Description": str,
     },
@@ -1895,28 +1909,14 @@
         "Type": ImpersonationRoleTypeType,
         "Effect": AccessEffectType,
         "MatchedRules": List[ImpersonationMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetImpersonationRoleResponseTypeDef = TypedDict(
-    "GetImpersonationRoleResponseTypeDef",
-    {
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Description": str,
-        "Rules": List[ImpersonationRuleOutputTypeDef],
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetMobileDeviceAccessEffectResponseTypeDef = TypedDict(
     "GetMobileDeviceAccessEffectResponseTypeDef",
     {
         "Effect": MobileDeviceAccessRuleEffectType,
         "MatchedRules": List[MobileDeviceAccessMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/PKG-INFO` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workmail
-Version: 1.28.15
-Summary: Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -378,14 +378,15 @@
     LambdaAvailabilityProviderTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
+    ImpersonationRuleOutputTypeDef,
     ImpersonationRuleTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
     DomainTypeDef,
     CreateResourceRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DelegateTypeDef,
     DeleteAccessControlRuleRequestRequestTypeDef,
@@ -415,15 +416,14 @@
     DnsRecordTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
-    ImpersonationRuleOutputTypeDef,
     GetMailDomainRequestRequestTypeDef,
     GetMailboxDetailsRequestRequestTypeDef,
     GetMobileDeviceAccessEffectRequestRequestTypeDef,
     MobileDeviceAccessMatchedRuleTypeDef,
     GetMobileDeviceAccessOverrideRequestRequestTypeDef,
     GroupTypeDef,
     ImpersonationRoleTypeDef,
@@ -491,23 +491,23 @@
     TestAvailabilityConfigurationResponseTypeDef,
     AvailabilityConfigurationTypeDef,
     DescribeResourceResponseTypeDef,
     UpdateResourceRequestRequestTypeDef,
     CreateAvailabilityConfigurationRequestRequestTypeDef,
     TestAvailabilityConfigurationRequestRequestTypeDef,
     UpdateAvailabilityConfigurationRequestRequestTypeDef,
+    GetImpersonationRoleResponseTypeDef,
     CreateImpersonationRoleRequestRequestTypeDef,
     UpdateImpersonationRoleRequestRequestTypeDef,
     CreateOrganizationRequestRequestTypeDef,
     ListResourceDelegatesResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetDefaultRetentionPolicyResponseTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
-    GetImpersonationRoleResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     ListGroupMembersRequestListGroupMembersPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
```

### Comparing `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/SOURCES.txt` & `mypy-boto3-workmail-1.28.15.post1/mypy_boto3_workmail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.15/setup.py` & `mypy-boto3-workmail-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workmail",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_workmail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder"
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

