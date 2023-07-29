# Comparing `tmp/mypy-boto3-sso-admin-1.28.15.tar.gz` & `tmp/mypy-boto3-sso-admin-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sso-admin-1.28.15.tar", last modified: Fri Jul 28 20:43:49 2023, max compression
+gzip compressed data, was "mypy-boto3-sso-admin-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:16 2023, max compression
```

## Comparing `mypy-boto3-sso-admin-1.28.15.tar` & `mypy-boto3-sso-admin-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.305940 mypy-boto3-sso-admin-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-07-28 20:43:49.305940 mypy-boto3-sso-admin-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19011 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.293940 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34786 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-28 20:40:14.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40501 2023-07-28 20:40:14.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40452 2023-07-28 20:40:14.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.305940 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:49.305940 mypy-boto3-sso-admin-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.961423 mypy-boto3-sso-admin-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-07-29 10:04:16.953423 mypy-boto3-sso-admin-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19011 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.949423 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35055 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40501 2023-07-29 10:00:22.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40452 2023-07-29 10:00:22.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:21.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.953423 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-07-29 10:04:16.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:04:16.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:16.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:16.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:16.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:04:16.000000 mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:16.961423 mypy-boto3-sso-admin-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-29 10:00:20.000000 mypy-boto3-sso-admin-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-sso-admin-1.28.15/LICENSE` & `mypy-boto3-sso-admin-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.15/PKG-INFO` & `mypy-boto3-sso-admin-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-admin
-Version: 1.28.15
-Summary: Type annotations for boto3.SSOAdmin 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SSOAdmin 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sso-admin-1.28.15/README.md` & `mypy-boto3-sso-admin-1.28.15.post1/README.md`

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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__init__.py` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__init__.pyi` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__main__.py` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSOAdmin 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.SSOAdmin 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin\nOther"
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

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/client.py` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_sso_admin.client import SSOAdminClient
 
     session = Session()
     client: SSOAdminClient = session.client("sso-admin")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PrincipalTypeType, ProvisioningStatusType, ProvisionTargetTypeType
 from .paginator import (
     ListAccountAssignmentCreationStatusPaginator,
     ListAccountAssignmentDeletionStatusPaginator,
@@ -40,14 +40,15 @@
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
     GetInlinePolicyForPermissionSetResponseTypeDef,
     GetPermissionsBoundaryForPermissionSetResponseTypeDef,
+    InstanceAccessControlAttributeConfigurationOutputTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
     ListAccountAssignmentCreationStatusResponseTypeDef,
     ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
     ListAccountsForProvisionedPermissionSetResponseTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
@@ -165,15 +166,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#create_account_assignment)
         """
 
     def create_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceArn: str,
-        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef
+        InstanceAccessControlAttributeConfiguration: Union[
+            InstanceAccessControlAttributeConfigurationTypeDef,
+            InstanceAccessControlAttributeConfigurationOutputTypeDef,
+        ]
     ) -> Dict[str, Any]:
         """
         Enables the attributes-based access control (ABAC) feature for the specified IAM
         Identity Center instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_instance_access_control_attribute_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#create_instance_access_control_attribute_configuration)
@@ -583,15 +587,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#untag_resource)
         """
 
     def update_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceArn: str,
-        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef
+        InstanceAccessControlAttributeConfiguration: Union[
+            InstanceAccessControlAttributeConfigurationTypeDef,
+            InstanceAccessControlAttributeConfigurationOutputTypeDef,
+        ]
     ) -> Dict[str, Any]:
         """
         Updates the IAM Identity Center identity store attributes that you can use with
         the IAM Identity Center instance for attributes-based access control (ABAC).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_instance_access_control_attribute_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#update_instance_access_control_attribute_configuration)
```

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/client.pyi` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_sso_admin.client import SSOAdminClient
 
     session = Session()
     client: SSOAdminClient = session.client("sso-admin")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PrincipalTypeType, ProvisioningStatusType, ProvisionTargetTypeType
 from .paginator import (
     ListAccountAssignmentCreationStatusPaginator,
     ListAccountAssignmentDeletionStatusPaginator,
@@ -40,14 +40,15 @@
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
     GetInlinePolicyForPermissionSetResponseTypeDef,
     GetPermissionsBoundaryForPermissionSetResponseTypeDef,
+    InstanceAccessControlAttributeConfigurationOutputTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
     ListAccountAssignmentCreationStatusResponseTypeDef,
     ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
     ListAccountsForProvisionedPermissionSetResponseTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
@@ -155,15 +156,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_account_assignment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#create_account_assignment)
         """
     def create_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceArn: str,
-        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef
+        InstanceAccessControlAttributeConfiguration: Union[
+            InstanceAccessControlAttributeConfigurationTypeDef,
+            InstanceAccessControlAttributeConfigurationOutputTypeDef,
+        ]
     ) -> Dict[str, Any]:
         """
         Enables the attributes-based access control (ABAC) feature for the specified IAM
         Identity Center instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_instance_access_control_attribute_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#create_instance_access_control_attribute_configuration)
@@ -540,15 +544,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#untag_resource)
         """
     def update_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceArn: str,
-        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef
+        InstanceAccessControlAttributeConfiguration: Union[
+            InstanceAccessControlAttributeConfigurationTypeDef,
+            InstanceAccessControlAttributeConfigurationOutputTypeDef,
+        ]
     ) -> Dict[str, Any]:
         """
         Updates the IAM Identity Center identity store attributes that you can use with
         the IAM Identity Center instance for attributes-based access control (ABAC).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_instance_access_control_attribute_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/client/#update_instance_access_control_attribute_configuration)
```

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/literals.py` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/literals.pyi` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/paginator.py` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/paginator.pyi` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/type_defs.py` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/type_defs.pyi` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/PKG-INFO` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-admin
-Version: 1.28.15
-Summary: Type annotations for boto3.SSOAdmin 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SSOAdmin 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/SOURCES.txt` & `mypy-boto3-sso-admin-1.28.15.post1/mypy_boto3_sso_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.15/setup.py` & `mypy-boto3-sso-admin-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sso-admin",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_sso_admin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.SSOAdmin 1.28.15 service generated with mypy-boto3-builder"
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

