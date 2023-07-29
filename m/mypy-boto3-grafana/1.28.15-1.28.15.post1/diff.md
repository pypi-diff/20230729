# Comparing `tmp/mypy-boto3-grafana-1.28.15.tar.gz` & `tmp/mypy-boto3-grafana-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-grafana-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
+gzip compressed data, was "mypy-boto3-grafana-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:13 2023, max compression
```

## Comparing `mypy-boto3-grafana-1.28.15.tar` & `mypy-boto3-grafana-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.089169 mypy-boto3-grafana-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-28 20:42:53.089169 mypy-boto3-grafana-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.085169 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22103 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22076 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.089169 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.089169 mypy-boto3-grafana-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.081167 mypy-boto3-grafana-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15523 2023-07-29 10:03:13.073167 mypy-boto3-grafana-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.073167 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-07-29 09:46:32.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22144 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:31.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.073167 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15523 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:03:12.000000 mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:13.081167 mypy-boto3-grafana-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:46:30.000000 mypy-boto3-grafana-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-grafana-1.28.15/LICENSE` & `mypy-boto3-grafana-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15/PKG-INFO` & `mypy-boto3-grafana-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.28.15
-Summary: Type annotations for boto3.ManagedGrafana 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ManagedGrafana 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-grafana-1.28.15/README.md` & `mypy-boto3-grafana-1.28.15.post1/README.md`

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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__init__.py` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__init__.pyi` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__main__.py` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedGrafana 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.ManagedGrafana 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana\nOther"
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

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/client.py` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_grafana.client import ManagedGrafanaClient
 
     session = Session()
     client: ManagedGrafanaClient = session.client("grafana")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
@@ -37,20 +37,24 @@
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
+    NetworkAccessConfigurationOutputTypeDef,
     NetworkAccessConfigurationTypeDef,
+    SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
+    UpdateInstructionOutputTypeDef,
     UpdateInstructionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -126,19 +130,21 @@
         *,
         accountAccessType: AccountAccessTypeType,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         permissionType: PermissionTypeType,
         clientToken: str = ...,
         configuration: str = ...,
         grafanaVersion: str = ...,
-        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
+        networkAccessControl: Union[
+            NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
+        ] = ...,
         organizationRoleName: str = ...,
         stackSetName: str = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfiguration: VpcConfigurationTypeDef = ...,
+        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> CreateWorkspaceResponseTypeDef:
@@ -293,35 +299,42 @@
         Managed Grafana resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#untag_resource)
         """
 
     def update_permissions(
-        self, *, updateInstructionBatch: Sequence[UpdateInstructionTypeDef], workspaceId: str
+        self,
+        *,
+        updateInstructionBatch: Sequence[
+            Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
+        ],
+        workspaceId: str
     ) -> UpdatePermissionsResponseTypeDef:
         """
         Updates which users in a workspace have the Grafana `Admin` or `Editor` roles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_permissions)
         """
 
     def update_workspace(
         self,
         *,
         workspaceId: str,
         accountAccessType: AccountAccessTypeType = ...,
-        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
+        networkAccessControl: Union[
+            NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
+        ] = ...,
         organizationRoleName: str = ...,
         permissionType: PermissionTypeType = ...,
         removeNetworkAccessConfiguration: bool = ...,
         removeVpcConfiguration: bool = ...,
         stackSetName: str = ...,
-        vpcConfiguration: VpcConfigurationTypeDef = ...,
+        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> UpdateWorkspaceResponseTypeDef:
@@ -333,15 +346,15 @@
         """
 
     def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
-        samlConfiguration: SamlConfigurationTypeDef = ...
+        samlConfiguration: Union[SamlConfigurationTypeDef, SamlConfigurationOutputTypeDef] = ...
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_workspace_authentication)
```

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/client.pyi` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_grafana.client import ManagedGrafanaClient
 
     session = Session()
     client: ManagedGrafanaClient = session.client("grafana")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
@@ -37,20 +37,24 @@
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
+    NetworkAccessConfigurationOutputTypeDef,
     NetworkAccessConfigurationTypeDef,
+    SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
+    UpdateInstructionOutputTypeDef,
     UpdateInstructionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -118,19 +122,21 @@
         *,
         accountAccessType: AccountAccessTypeType,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         permissionType: PermissionTypeType,
         clientToken: str = ...,
         configuration: str = ...,
         grafanaVersion: str = ...,
-        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
+        networkAccessControl: Union[
+            NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
+        ] = ...,
         organizationRoleName: str = ...,
         stackSetName: str = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfiguration: VpcConfigurationTypeDef = ...,
+        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> CreateWorkspaceResponseTypeDef:
@@ -270,34 +276,41 @@
         The `UntagResource` operation removes the association of the tag with the Amazon
         Managed Grafana resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#untag_resource)
         """
     def update_permissions(
-        self, *, updateInstructionBatch: Sequence[UpdateInstructionTypeDef], workspaceId: str
+        self,
+        *,
+        updateInstructionBatch: Sequence[
+            Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
+        ],
+        workspaceId: str
     ) -> UpdatePermissionsResponseTypeDef:
         """
         Updates which users in a workspace have the Grafana `Admin` or `Editor` roles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_permissions)
         """
     def update_workspace(
         self,
         *,
         workspaceId: str,
         accountAccessType: AccountAccessTypeType = ...,
-        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
+        networkAccessControl: Union[
+            NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
+        ] = ...,
         organizationRoleName: str = ...,
         permissionType: PermissionTypeType = ...,
         removeNetworkAccessConfiguration: bool = ...,
         removeVpcConfiguration: bool = ...,
         stackSetName: str = ...,
-        vpcConfiguration: VpcConfigurationTypeDef = ...,
+        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> UpdateWorkspaceResponseTypeDef:
@@ -308,15 +321,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_workspace)
         """
     def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
-        samlConfiguration: SamlConfigurationTypeDef = ...
+        samlConfiguration: Union[SamlConfigurationTypeDef, SamlConfigurationOutputTypeDef] = ...
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_workspace_authentication)
```

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/literals.py` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/literals.pyi` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/paginator.py` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/paginator.pyi` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/type_defs.py` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_grafana.type_defs import AssertionAttributesTypeDef
 
     data: AssertionAttributesTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
@@ -712,15 +712,17 @@
         "message": str,
     },
 )
 
 UpdatePermissionsRequestRequestTypeDef = TypedDict(
     "UpdatePermissionsRequestRequestTypeDef",
     {
-        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
+        "updateInstructionBatch": Sequence[
+            Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
+        ],
         "workspaceId": str,
     },
 )
 
 _RequiredSamlAuthenticationTypeDef = TypedDict(
     "_RequiredSamlAuthenticationTypeDef",
     {
```

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/type_defs.pyi` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_grafana.type_defs import AssertionAttributesTypeDef
 
     data: AssertionAttributesTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
@@ -691,15 +691,17 @@
         "message": str,
     },
 )
 
 UpdatePermissionsRequestRequestTypeDef = TypedDict(
     "UpdatePermissionsRequestRequestTypeDef",
     {
-        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
+        "updateInstructionBatch": Sequence[
+            Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
+        ],
         "workspaceId": str,
     },
 )
 
 _RequiredSamlAuthenticationTypeDef = TypedDict(
     "_RequiredSamlAuthenticationTypeDef",
     {
```

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/PKG-INFO` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.28.15
-Summary: Type annotations for boto3.ManagedGrafana 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ManagedGrafana 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/SOURCES.txt` & `mypy-boto3-grafana-1.28.15.post1/mypy_boto3_grafana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.15/setup.py` & `mypy-boto3-grafana-1.28.15.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-grafana",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_grafana"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ManagedGrafana 1.28.15 service generated with"
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

