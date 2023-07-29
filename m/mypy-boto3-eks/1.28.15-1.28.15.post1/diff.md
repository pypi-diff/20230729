# Comparing `tmp/mypy-boto3-eks-1.28.15.tar.gz` & `tmp/mypy-boto3-eks-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-eks-1.28.15.tar", last modified: Fri Jul 28 20:42:43 2023, max compression
+gzip compressed data, was "mypy-boto3-eks-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
```

## Comparing `mypy-boto3-eks-1.28.15.tar` & `mypy-boto3-eks-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.961043 mypy-boto3-eks-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-28 20:42:43.957043 mypy-boto3-eks-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19281 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.949043 mypy-boto3-eks-1.28.15/mypy_boto3_eks/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33061 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33004 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-28 20:25:00.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-07-28 20:25:00.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51661 2023-07-28 20:25:02.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51588 2023-07-28 20:25:02.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-28 20:25:00.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-28 20:25:00.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.957043 mypy-boto3-eks-1.28.15/mypy_boto3_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-28 20:42:43.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:43.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:43.000000 mypy-boto3-eks-1.28.15/mypy_boto3_eks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.961043 mypy-boto3-eks-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:24:59.000000 mypy-boto3-eks-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.669129 mypy-boto3-eks-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-07-29 10:03:02.669129 mypy-boto3-eks-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19281 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.669129 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33469 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33412 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51810 2023-07-29 09:44:32.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51737 2023-07-29 09:44:32.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-29 09:44:29.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.669129 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:02.000000 mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.669129 mypy-boto3-eks-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:44:28.000000 mypy-boto3-eks-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-eks-1.28.15/LICENSE` & `mypy-boto3-eks-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15/PKG-INFO` & `mypy-boto3-eks-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-eks
-Version: 1.28.15
-Summary: Type annotations for boto3.EKS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EKS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -428,14 +428,15 @@
     VpcConfigResponseTypeDef,
     ConnectorConfigRequestTypeDef,
     ControlPlanePlacementRequestTypeDef,
     ControlPlanePlacementResponseTypeDef,
     CreateAddonRequestRequestTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     VpcConfigRequestTypeDef,
+    FargateProfileSelectorOutputTypeDef,
     FargateProfileSelectorTypeDef,
     LaunchTemplateSpecificationTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
@@ -451,15 +452,14 @@
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
-    FargateProfileSelectorOutputTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
     ListAddonsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
@@ -486,14 +486,15 @@
     ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
+    FargateProfileTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
@@ -510,28 +511,27 @@
     ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
-    FargateProfileTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
     LoggingOutputTypeDef,
     LoggingTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
```

### Comparing `mypy-boto3-eks-1.28.15/README.md` & `mypy-boto3-eks-1.28.15.post1/README.md`

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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,14 +396,15 @@
     VpcConfigResponseTypeDef,
     ConnectorConfigRequestTypeDef,
     ControlPlanePlacementRequestTypeDef,
     ControlPlanePlacementResponseTypeDef,
     CreateAddonRequestRequestTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     VpcConfigRequestTypeDef,
+    FargateProfileSelectorOutputTypeDef,
     FargateProfileSelectorTypeDef,
     LaunchTemplateSpecificationTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
@@ -419,15 +420,14 @@
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
-    FargateProfileSelectorOutputTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
     ListAddonsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
@@ -454,14 +454,15 @@
     ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
+    FargateProfileTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
@@ -478,28 +479,27 @@
     ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
-    FargateProfileTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
     LoggingOutputTypeDef,
     LoggingTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
```

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/__init__.py` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/__init__.pyi` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/__main__.py` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EKS 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.EKS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS\nOther"
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

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/client.py` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_eks.client import EKSClient
 
     session = Session()
     client: EKSClient = session.client("eks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AMITypesType, CapacityTypesType, ResolveConflictsType
 from .paginator import (
     DescribeAddonVersionsPaginator,
     ListAddonsPaginator,
@@ -46,32 +46,36 @@
     DescribeAddonVersionsResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileSelectorOutputTypeDef,
     FargateProfileSelectorTypeDef,
     IdentityProviderConfigTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesResponseTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesResponseTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     OutpostConfigRequestTypeDef,
     RegisterClusterResponseTypeDef,
+    RemoteAccessConfigOutputTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
@@ -141,15 +145,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#exceptions)
         """
 
     def associate_encryption_config(
         self,
         *,
         clusterName: str,
-        encryptionConfig: Sequence[EncryptionConfigTypeDef],
+        encryptionConfig: Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
         clientRequestToken: str = ...
     ) -> AssociateEncryptionConfigResponseTypeDef:
         """
         Associate encryption configuration to an existing cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#associate_encryption_config)
@@ -209,18 +213,20 @@
         self,
         *,
         name: str,
         roleArn: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef,
         version: str = ...,
         kubernetesNetworkConfig: KubernetesNetworkConfigRequestTypeDef = ...,
-        logging: LoggingTypeDef = ...,
+        logging: Union[LoggingTypeDef, LoggingOutputTypeDef] = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        encryptionConfig: Sequence[EncryptionConfigTypeDef] = ...,
+        encryptionConfig: Sequence[
+            Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]
+        ] = ...,
         outpostConfig: OutpostConfigRequestTypeDef = ...
     ) -> CreateClusterResponseTypeDef:
         """
         Creates an Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#create_cluster)
@@ -229,15 +235,17 @@
     def create_fargate_profile(
         self,
         *,
         fargateProfileName: str,
         clusterName: str,
         podExecutionRoleArn: str,
         subnets: Sequence[str] = ...,
-        selectors: Sequence[FargateProfileSelectorTypeDef] = ...,
+        selectors: Sequence[
+            Union[FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef]
+        ] = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFargateProfileResponseTypeDef:
         """
         Creates an Fargate profile for your Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_fargate_profile)
@@ -251,15 +259,15 @@
         nodegroupName: str,
         subnets: Sequence[str],
         nodeRole: str,
         scalingConfig: NodegroupScalingConfigTypeDef = ...,
         diskSize: int = ...,
         instanceTypes: Sequence[str] = ...,
         amiType: AMITypesType = ...,
-        remoteAccess: RemoteAccessConfigTypeDef = ...,
+        remoteAccess: Union[RemoteAccessConfigTypeDef, RemoteAccessConfigOutputTypeDef] = ...,
         labels: Mapping[str, str] = ...,
         taints: Sequence[TaintTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientRequestToken: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
         capacityType: CapacityTypesType = ...,
@@ -560,15 +568,15 @@
         """
 
     def update_cluster_config(
         self,
         *,
         name: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef = ...,
-        logging: LoggingTypeDef = ...,
+        logging: Union[LoggingTypeDef, LoggingOutputTypeDef] = ...,
         clientRequestToken: str = ...
     ) -> UpdateClusterConfigResponseTypeDef:
         """
         Updates an Amazon EKS cluster configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_cluster_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#update_cluster_config)
```

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/client.pyi` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_eks.client import EKSClient
 
     session = Session()
     client: EKSClient = session.client("eks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AMITypesType, CapacityTypesType, ResolveConflictsType
 from .paginator import (
     DescribeAddonVersionsPaginator,
     ListAddonsPaginator,
@@ -46,32 +46,36 @@
     DescribeAddonVersionsResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileSelectorOutputTypeDef,
     FargateProfileSelectorTypeDef,
     IdentityProviderConfigTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesResponseTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesResponseTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     OutpostConfigRequestTypeDef,
     RegisterClusterResponseTypeDef,
+    RemoteAccessConfigOutputTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
@@ -136,15 +140,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#exceptions)
         """
     def associate_encryption_config(
         self,
         *,
         clusterName: str,
-        encryptionConfig: Sequence[EncryptionConfigTypeDef],
+        encryptionConfig: Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
         clientRequestToken: str = ...
     ) -> AssociateEncryptionConfigResponseTypeDef:
         """
         Associate encryption configuration to an existing cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#associate_encryption_config)
@@ -199,18 +203,20 @@
         self,
         *,
         name: str,
         roleArn: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef,
         version: str = ...,
         kubernetesNetworkConfig: KubernetesNetworkConfigRequestTypeDef = ...,
-        logging: LoggingTypeDef = ...,
+        logging: Union[LoggingTypeDef, LoggingOutputTypeDef] = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        encryptionConfig: Sequence[EncryptionConfigTypeDef] = ...,
+        encryptionConfig: Sequence[
+            Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]
+        ] = ...,
         outpostConfig: OutpostConfigRequestTypeDef = ...
     ) -> CreateClusterResponseTypeDef:
         """
         Creates an Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#create_cluster)
@@ -218,15 +224,17 @@
     def create_fargate_profile(
         self,
         *,
         fargateProfileName: str,
         clusterName: str,
         podExecutionRoleArn: str,
         subnets: Sequence[str] = ...,
-        selectors: Sequence[FargateProfileSelectorTypeDef] = ...,
+        selectors: Sequence[
+            Union[FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef]
+        ] = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFargateProfileResponseTypeDef:
         """
         Creates an Fargate profile for your Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_fargate_profile)
@@ -239,15 +247,15 @@
         nodegroupName: str,
         subnets: Sequence[str],
         nodeRole: str,
         scalingConfig: NodegroupScalingConfigTypeDef = ...,
         diskSize: int = ...,
         instanceTypes: Sequence[str] = ...,
         amiType: AMITypesType = ...,
-        remoteAccess: RemoteAccessConfigTypeDef = ...,
+        remoteAccess: Union[RemoteAccessConfigTypeDef, RemoteAccessConfigOutputTypeDef] = ...,
         labels: Mapping[str, str] = ...,
         taints: Sequence[TaintTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientRequestToken: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
         capacityType: CapacityTypesType = ...,
@@ -521,15 +529,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#update_addon)
         """
     def update_cluster_config(
         self,
         *,
         name: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef = ...,
-        logging: LoggingTypeDef = ...,
+        logging: Union[LoggingTypeDef, LoggingOutputTypeDef] = ...,
         clientRequestToken: str = ...
     ) -> UpdateClusterConfigResponseTypeDef:
         """
         Updates an Amazon EKS cluster configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_cluster_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/client/#update_cluster_config)
```

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/literals.py` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/literals.pyi` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/paginator.py` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/paginator.pyi` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/type_defs.py` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_eks.type_defs import AddonIssueTypeDef
 
     data: AddonIssueTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AddonIssueCodeType,
     AddonStatusType,
     AMITypesType,
     CapacityTypesType,
     ClusterIssueCodeType,
@@ -57,14 +57,15 @@
     "VpcConfigResponseTypeDef",
     "ConnectorConfigRequestTypeDef",
     "ControlPlanePlacementRequestTypeDef",
     "ControlPlanePlacementResponseTypeDef",
     "CreateAddonRequestRequestTypeDef",
     "KubernetesNetworkConfigRequestTypeDef",
     "VpcConfigRequestTypeDef",
+    "FargateProfileSelectorOutputTypeDef",
     "FargateProfileSelectorTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "NodegroupScalingConfigTypeDef",
     "NodegroupUpdateConfigTypeDef",
     "RemoteAccessConfigTypeDef",
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
@@ -80,15 +81,14 @@
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
-    "FargateProfileSelectorOutputTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
     "ListAddonsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
@@ -115,14 +115,15 @@
     "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
+    "FargateProfileTypeDef",
     "CreateFargateProfileRequestRequestTypeDef",
     "UpdateNodegroupVersionRequestRequestTypeDef",
     "CreateNodegroupRequestRequestTypeDef",
     "UpdateTaintsPayloadTypeDef",
     "DescribeAddonRequestAddonActiveWaitTypeDef",
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
@@ -139,28 +140,27 @@
     "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
     "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
-    "FargateProfileTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
     "LoggingOutputTypeDef",
     "LoggingTypeDef",
     "UpdateTypeDef",
     "AddonTypeDef",
     "AddonInfoTypeDef",
-    "UpdateNodegroupConfigRequestRequestTypeDef",
-    "AssociateEncryptionConfigRequestRequestTypeDef",
     "CreateFargateProfileResponseTypeDef",
     "DeleteFargateProfileResponseTypeDef",
     "DescribeFargateProfileResponseTypeDef",
+    "UpdateNodegroupConfigRequestRequestTypeDef",
+    "AssociateEncryptionConfigRequestRequestTypeDef",
     "DescribeIdentityProviderConfigResponseTypeDef",
     "NodegroupTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterConfigRequestRequestTypeDef",
     "AssociateEncryptionConfigResponseTypeDef",
     "AssociateIdentityProviderConfigResponseTypeDef",
@@ -383,14 +383,23 @@
         "endpointPublicAccess": bool,
         "endpointPrivateAccess": bool,
         "publicAccessCidrs": Sequence[str],
     },
     total=False,
 )
 
+FargateProfileSelectorOutputTypeDef = TypedDict(
+    "FargateProfileSelectorOutputTypeDef",
+    {
+        "namespace": str,
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
 FargateProfileSelectorTypeDef = TypedDict(
     "FargateProfileSelectorTypeDef",
     {
         "namespace": str,
         "labels": Mapping[str, str],
     },
     total=False,
@@ -613,23 +622,14 @@
         "errorCode": ErrorCodeType,
         "errorMessage": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
-FargateProfileSelectorOutputTypeDef = TypedDict(
-    "FargateProfileSelectorOutputTypeDef",
-    {
-        "namespace": str,
-        "labels": Dict[str, str],
-    },
-    total=False,
-)
-
 OidcIdentityProviderConfigTypeDef = TypedDict(
     "OidcIdentityProviderConfigTypeDef",
     {
         "identityProviderConfigName": str,
         "identityProviderConfigArn": str,
         "clusterName": str,
         "issuerUrl": str,
@@ -1090,27 +1090,45 @@
 
 class OutpostConfigResponseTypeDef(
     _RequiredOutpostConfigResponseTypeDef, _OptionalOutpostConfigResponseTypeDef
 ):
     pass
 
 
+FargateProfileTypeDef = TypedDict(
+    "FargateProfileTypeDef",
+    {
+        "fargateProfileName": str,
+        "fargateProfileArn": str,
+        "clusterName": str,
+        "createdAt": datetime,
+        "podExecutionRoleArn": str,
+        "subnets": List[str],
+        "selectors": List[FargateProfileSelectorOutputTypeDef],
+        "status": FargateProfileStatusType,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFargateProfileRequestRequestTypeDef",
     {
         "fargateProfileName": str,
         "clusterName": str,
         "podExecutionRoleArn": str,
     },
 )
 _OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFargateProfileRequestRequestTypeDef",
     {
         "subnets": Sequence[str],
-        "selectors": Sequence[FargateProfileSelectorTypeDef],
+        "selectors": Sequence[
+            Union[FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef]
+        ],
         "clientRequestToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
@@ -1564,30 +1582,14 @@
     {
         "resources": Sequence[str],
         "provider": ProviderTypeDef,
     },
     total=False,
 )
 
-FargateProfileTypeDef = TypedDict(
-    "FargateProfileTypeDef",
-    {
-        "fargateProfileName": str,
-        "fargateProfileArn": str,
-        "clusterName": str,
-        "createdAt": datetime,
-        "podExecutionRoleArn": str,
-        "subnets": List[str],
-        "selectors": List[FargateProfileSelectorOutputTypeDef],
-        "status": FargateProfileStatusType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
     },
     total=False,
 )
@@ -1667,14 +1669,38 @@
         "publisher": str,
         "owner": str,
         "marketplaceInformation": MarketplaceInformationTypeDef,
     },
     total=False,
 )
 
+CreateFargateProfileResponseTypeDef = TypedDict(
+    "CreateFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFargateProfileResponseTypeDef = TypedDict(
+    "DeleteFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFargateProfileResponseTypeDef = TypedDict(
+    "DescribeFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1698,15 +1724,15 @@
     pass
 
 
 _RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
     {
         "clusterName": str,
-        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
+        "encryptionConfig": Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
     },
 )
 _OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
@@ -1717,38 +1743,14 @@
 class AssociateEncryptionConfigRequestRequestTypeDef(
     _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
     _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
 
-CreateFargateProfileResponseTypeDef = TypedDict(
-    "CreateFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFargateProfileResponseTypeDef = TypedDict(
-    "DeleteFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFargateProfileResponseTypeDef = TypedDict(
-    "DescribeFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1822,15 +1824,15 @@
     "_OptionalCreateClusterRequestRequestTypeDef",
     {
         "version": str,
         "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
         "logging": LoggingTypeDef,
         "clientRequestToken": str,
         "tags": Mapping[str, str],
-        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
+        "encryptionConfig": Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
         "outpostConfig": OutpostConfigRequestTypeDef,
     },
     total=False,
 )
 
 
 class CreateClusterRequestRequestTypeDef(
```

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/type_defs.pyi` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_eks.type_defs import AddonIssueTypeDef
 
     data: AddonIssueTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AddonIssueCodeType,
     AddonStatusType,
     AMITypesType,
     CapacityTypesType,
     ClusterIssueCodeType,
@@ -56,14 +56,15 @@
     "VpcConfigResponseTypeDef",
     "ConnectorConfigRequestTypeDef",
     "ControlPlanePlacementRequestTypeDef",
     "ControlPlanePlacementResponseTypeDef",
     "CreateAddonRequestRequestTypeDef",
     "KubernetesNetworkConfigRequestTypeDef",
     "VpcConfigRequestTypeDef",
+    "FargateProfileSelectorOutputTypeDef",
     "FargateProfileSelectorTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "NodegroupScalingConfigTypeDef",
     "NodegroupUpdateConfigTypeDef",
     "RemoteAccessConfigTypeDef",
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
@@ -79,15 +80,14 @@
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
-    "FargateProfileSelectorOutputTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
     "ListAddonsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
@@ -114,14 +114,15 @@
     "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
+    "FargateProfileTypeDef",
     "CreateFargateProfileRequestRequestTypeDef",
     "UpdateNodegroupVersionRequestRequestTypeDef",
     "CreateNodegroupRequestRequestTypeDef",
     "UpdateTaintsPayloadTypeDef",
     "DescribeAddonRequestAddonActiveWaitTypeDef",
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
@@ -138,28 +139,27 @@
     "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
     "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
-    "FargateProfileTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
     "LoggingOutputTypeDef",
     "LoggingTypeDef",
     "UpdateTypeDef",
     "AddonTypeDef",
     "AddonInfoTypeDef",
-    "UpdateNodegroupConfigRequestRequestTypeDef",
-    "AssociateEncryptionConfigRequestRequestTypeDef",
     "CreateFargateProfileResponseTypeDef",
     "DeleteFargateProfileResponseTypeDef",
     "DescribeFargateProfileResponseTypeDef",
+    "UpdateNodegroupConfigRequestRequestTypeDef",
+    "AssociateEncryptionConfigRequestRequestTypeDef",
     "DescribeIdentityProviderConfigResponseTypeDef",
     "NodegroupTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterConfigRequestRequestTypeDef",
     "AssociateEncryptionConfigResponseTypeDef",
     "AssociateIdentityProviderConfigResponseTypeDef",
@@ -378,14 +378,23 @@
         "endpointPublicAccess": bool,
         "endpointPrivateAccess": bool,
         "publicAccessCidrs": Sequence[str],
     },
     total=False,
 )
 
+FargateProfileSelectorOutputTypeDef = TypedDict(
+    "FargateProfileSelectorOutputTypeDef",
+    {
+        "namespace": str,
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
 FargateProfileSelectorTypeDef = TypedDict(
     "FargateProfileSelectorTypeDef",
     {
         "namespace": str,
         "labels": Mapping[str, str],
     },
     total=False,
@@ -604,23 +613,14 @@
         "errorCode": ErrorCodeType,
         "errorMessage": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
-FargateProfileSelectorOutputTypeDef = TypedDict(
-    "FargateProfileSelectorOutputTypeDef",
-    {
-        "namespace": str,
-        "labels": Dict[str, str],
-    },
-    total=False,
-)
-
 OidcIdentityProviderConfigTypeDef = TypedDict(
     "OidcIdentityProviderConfigTypeDef",
     {
         "identityProviderConfigName": str,
         "identityProviderConfigArn": str,
         "clusterName": str,
         "issuerUrl": str,
@@ -1059,27 +1059,45 @@
 )
 
 class OutpostConfigResponseTypeDef(
     _RequiredOutpostConfigResponseTypeDef, _OptionalOutpostConfigResponseTypeDef
 ):
     pass
 
+FargateProfileTypeDef = TypedDict(
+    "FargateProfileTypeDef",
+    {
+        "fargateProfileName": str,
+        "fargateProfileArn": str,
+        "clusterName": str,
+        "createdAt": datetime,
+        "podExecutionRoleArn": str,
+        "subnets": List[str],
+        "selectors": List[FargateProfileSelectorOutputTypeDef],
+        "status": FargateProfileStatusType,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFargateProfileRequestRequestTypeDef",
     {
         "fargateProfileName": str,
         "clusterName": str,
         "podExecutionRoleArn": str,
     },
 )
 _OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFargateProfileRequestRequestTypeDef",
     {
         "subnets": Sequence[str],
-        "selectors": Sequence[FargateProfileSelectorTypeDef],
+        "selectors": Sequence[
+            Union[FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef]
+        ],
         "clientRequestToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateFargateProfileRequestRequestTypeDef(
@@ -1499,30 +1517,14 @@
     {
         "resources": Sequence[str],
         "provider": ProviderTypeDef,
     },
     total=False,
 )
 
-FargateProfileTypeDef = TypedDict(
-    "FargateProfileTypeDef",
-    {
-        "fargateProfileName": str,
-        "fargateProfileArn": str,
-        "clusterName": str,
-        "createdAt": datetime,
-        "podExecutionRoleArn": str,
-        "subnets": List[str],
-        "selectors": List[FargateProfileSelectorOutputTypeDef],
-        "status": FargateProfileStatusType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
     },
     total=False,
 )
@@ -1602,14 +1604,38 @@
         "publisher": str,
         "owner": str,
         "marketplaceInformation": MarketplaceInformationTypeDef,
     },
     total=False,
 )
 
+CreateFargateProfileResponseTypeDef = TypedDict(
+    "CreateFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFargateProfileResponseTypeDef = TypedDict(
+    "DeleteFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFargateProfileResponseTypeDef = TypedDict(
+    "DescribeFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1631,15 +1657,15 @@
 ):
     pass
 
 _RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
     {
         "clusterName": str,
-        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
+        "encryptionConfig": Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
     },
 )
 _OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
@@ -1648,38 +1674,14 @@
 
 class AssociateEncryptionConfigRequestRequestTypeDef(
     _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
     _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
-CreateFargateProfileResponseTypeDef = TypedDict(
-    "CreateFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFargateProfileResponseTypeDef = TypedDict(
-    "DeleteFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFargateProfileResponseTypeDef = TypedDict(
-    "DescribeFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1753,15 +1755,15 @@
     "_OptionalCreateClusterRequestRequestTypeDef",
     {
         "version": str,
         "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
         "logging": LoggingTypeDef,
         "clientRequestToken": str,
         "tags": Mapping[str, str],
-        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
+        "encryptionConfig": Sequence[Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]],
         "outpostConfig": OutpostConfigRequestTypeDef,
     },
     total=False,
 )
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
```

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/waiter.py` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks/waiter.pyi` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks.egg-info/PKG-INFO` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-eks
-Version: 1.28.15
-Summary: Type annotations for boto3.EKS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EKS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -428,14 +428,15 @@
     VpcConfigResponseTypeDef,
     ConnectorConfigRequestTypeDef,
     ControlPlanePlacementRequestTypeDef,
     ControlPlanePlacementResponseTypeDef,
     CreateAddonRequestRequestTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     VpcConfigRequestTypeDef,
+    FargateProfileSelectorOutputTypeDef,
     FargateProfileSelectorTypeDef,
     LaunchTemplateSpecificationTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
@@ -451,15 +452,14 @@
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
-    FargateProfileSelectorOutputTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
     ListAddonsRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
@@ -486,14 +486,15 @@
     ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
+    FargateProfileTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
@@ -510,28 +511,27 @@
     ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
-    FargateProfileTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
     LoggingOutputTypeDef,
     LoggingTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
```

### Comparing `mypy-boto3-eks-1.28.15/mypy_boto3_eks.egg-info/SOURCES.txt` & `mypy-boto3-eks-1.28.15.post1/mypy_boto3_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.15/setup.py` & `mypy-boto3-eks-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-eks",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_eks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EKS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.EKS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

