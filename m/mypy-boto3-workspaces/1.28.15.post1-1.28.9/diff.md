# Comparing `tmp/mypy-boto3-workspaces-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-workspaces-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:27 2023, max compression
+gzip compressed data, was "mypy-boto3-workspaces-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-workspaces-1.28.15.post1.tar` & `mypy-boto3-workspaces-1.28.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.313463 mypy-boto3-workspaces-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:53.000000 mypy-boto3-workspaces-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22099 2023-07-29 10:04:27.313463 mypy-boto3-workspaces-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20594 2023-07-29 10:01:53.000000 mypy-boto3-workspaces-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.305462 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-29 10:01:53.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-29 10:01:53.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 10:01:53.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48335 2023-07-29 10:01:54.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48255 2023-07-29 10:01:53.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-07-29 10:01:54.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-07-29 10:01:54.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-07-29 10:01:54.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-29 10:01:54.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:53.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55688 2023-07-29 10:01:55.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55643 2023-07-29 10:01:55.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:53.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.313463 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22099 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:04:27.000000 mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:27.313463 mypy-boto3-workspaces-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 10:01:53.000000 mypy-boto3-workspaces-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.251903 mypy-boto3-workspaces-1.28.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48055 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47975 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57338 2023-07-21 20:32:48.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57297 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:32:58.251903 mypy-boto3-workspaces-1.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/setup.py
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/LICENSE` & `mypy-boto3-workspaces-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.15.post1/PKG-INFO` & `mypy-boto3-workspaces-1.28.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WorkSpaces 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.9
+Summary: Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces)](https://pepy.tech/project/mypy-boto3-workspaces)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,19 +393,23 @@
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
+    ClientPropertiesOutputTypeDef,
     ClientPropertiesTypeDef,
+    ComputeTypeOutputTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
+    ConnectionAliasPermissionOutputTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
@@ -426,28 +430,30 @@
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
     IosImportClientBrandingAttributesTypeDef,
+    IpRuleItemOutputTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
@@ -455,101 +461,106 @@
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
+    RootStorageOutputTypeDef,
+    SamlPropertiesOutputTypeDef,
+    SelfservicePermissionsOutputTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
+    UserStorageOutputTypeDef,
+    WorkspaceAccessPropertiesOutputTypeDef,
     WorkspacePropertiesOutputTypeDef,
     AssociateConnectionAliasResultTypeDef,
     CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInResultTypeDef,
     CreateConnectionAliasResultTypeDef,
     CreateIpGroupResultTypeDef,
     CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
     DescribeAccountResultTypeDef,
     ImportWorkspaceImageResultTypeDef,
     ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
-    WorkspacesIpGroupTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
     CreateConnectionAliasRequestRequestTypeDef,
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
-    DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
-    StandbyWorkspaceOutputTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
-    WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
     DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
+    DescribeTagsResultTypeDef,
+    StandbyWorkspaceOutputTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
     StartWorkspacesResultTypeDef,
     StopWorkspacesResultTypeDef,
     TerminateWorkspacesResultTypeDef,
     ImportClientBrandingRequestRequestTypeDef,
+    WorkspacesIpGroupTypeDef,
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
-    WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
+    WorkspaceBundleTypeDef,
+    WorkspaceDirectoryTypeDef,
     WorkspaceRequestOutputTypeDef,
     WorkspaceTypeDef,
-    DescribeIpGroupsResultTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
-    FailedCreateStandbyWorkspacesRequestTypeDef,
     CreateStandbyWorkspacesRequestRequestTypeDef,
+    FailedCreateStandbyWorkspacesRequestTypeDef,
+    DescribeIpGroupsResultTypeDef,
+    CreateWorkspacesRequestRequestTypeDef,
+    DescribeWorkspaceImagesResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
-    DescribeWorkspaceImagesResultTypeDef,
-    CreateWorkspacesRequestRequestTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
     DescribeWorkspacesResultTypeDef,
     CreateStandbyWorkspacesResultTypeDef,
     CreateWorkspacesResultTypeDef,
 )
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/README.md` & `mypy-boto3-workspaces-1.28.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces)](https://pepy.tech/project/mypy-boto3-workspaces)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,19 +361,23 @@
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
+    ClientPropertiesOutputTypeDef,
     ClientPropertiesTypeDef,
+    ComputeTypeOutputTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
+    ConnectionAliasPermissionOutputTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
@@ -394,28 +398,30 @@
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
     IosImportClientBrandingAttributesTypeDef,
+    IpRuleItemOutputTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
@@ -423,101 +429,106 @@
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
+    RootStorageOutputTypeDef,
+    SamlPropertiesOutputTypeDef,
+    SelfservicePermissionsOutputTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
+    UserStorageOutputTypeDef,
+    WorkspaceAccessPropertiesOutputTypeDef,
     WorkspacePropertiesOutputTypeDef,
     AssociateConnectionAliasResultTypeDef,
     CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInResultTypeDef,
     CreateConnectionAliasResultTypeDef,
     CreateIpGroupResultTypeDef,
     CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
     DescribeAccountResultTypeDef,
     ImportWorkspaceImageResultTypeDef,
     ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
-    WorkspacesIpGroupTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
     CreateConnectionAliasRequestRequestTypeDef,
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
-    DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
-    StandbyWorkspaceOutputTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
-    WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
     DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
+    DescribeTagsResultTypeDef,
+    StandbyWorkspaceOutputTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
     StartWorkspacesResultTypeDef,
     StopWorkspacesResultTypeDef,
     TerminateWorkspacesResultTypeDef,
     ImportClientBrandingRequestRequestTypeDef,
+    WorkspacesIpGroupTypeDef,
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
-    WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
+    WorkspaceBundleTypeDef,
+    WorkspaceDirectoryTypeDef,
     WorkspaceRequestOutputTypeDef,
     WorkspaceTypeDef,
-    DescribeIpGroupsResultTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
-    FailedCreateStandbyWorkspacesRequestTypeDef,
     CreateStandbyWorkspacesRequestRequestTypeDef,
+    FailedCreateStandbyWorkspacesRequestTypeDef,
+    DescribeIpGroupsResultTypeDef,
+    CreateWorkspacesRequestRequestTypeDef,
+    DescribeWorkspaceImagesResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
-    DescribeWorkspaceImagesResultTypeDef,
-    CreateWorkspacesRequestRequestTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
     DescribeWorkspacesResultTypeDef,
     CreateStandbyWorkspacesResultTypeDef,
     CreateWorkspacesResultTypeDef,
 )
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/__init__.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/__init__.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/__main__.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpaces 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.WorkSpaces 1.28.9\nVersion:         1.28.9\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/client.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_workspaces.client import WorkSpacesClient
 
     session = Session()
     client: WorkSpacesClient = session.client("workspaces")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApplicationType,
     ClientDeviceTypeType,
     DeletableSamlPropertyType,
@@ -78,29 +78,26 @@
     RebootRequestTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildRequestTypeDef,
     RebuildWorkspacesResultTypeDef,
     RootStorageTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
-    StandbyWorkspaceOutputTypeDef,
     StandbyWorkspaceTypeDef,
     StartRequestTypeDef,
     StartWorkspacesResultTypeDef,
     StopRequestTypeDef,
     StopWorkspacesResultTypeDef,
     TagTypeDef,
     TerminateRequestTypeDef,
     TerminateWorkspacesResultTypeDef,
     UserStorageTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
-    WorkspacePropertiesOutputTypeDef,
     WorkspacePropertiesTypeDef,
-    WorkspaceRequestOutputTypeDef,
     WorkspaceRequestTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -245,18 +242,15 @@
         Creates an IP access control group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_ip_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_ip_group)
         """
 
     def create_standby_workspaces(
-        self,
-        *,
-        PrimaryRegion: str,
-        StandbyWorkspaces: Sequence[Union[StandbyWorkspaceTypeDef, StandbyWorkspaceOutputTypeDef]]
+        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceTypeDef]
     ) -> CreateStandbyWorkspacesResultTypeDef:
         """
         Creates a standby WorkSpace in a secondary Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_standby_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_standby_workspaces)
         """
@@ -304,15 +298,15 @@
         Creates a new WorkSpace image from an existing WorkSpace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspace_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_workspace_image)
         """
 
     def create_workspaces(
-        self, *, Workspaces: Sequence[Union[WorkspaceRequestTypeDef, WorkspaceRequestOutputTypeDef]]
+        self, *, Workspaces: Sequence[WorkspaceRequestTypeDef]
     ) -> CreateWorkspacesResultTypeDef:
         """
         Creates one or more WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_workspaces)
         """
@@ -738,18 +732,15 @@
         Modify the default properties used to create WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_creation_properties)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_workspace_creation_properties)
         """
 
     def modify_workspace_properties(
-        self,
-        *,
-        WorkspaceId: str,
-        WorkspaceProperties: Union[WorkspacePropertiesTypeDef, WorkspacePropertiesOutputTypeDef]
+        self, *, WorkspaceId: str, WorkspaceProperties: WorkspacePropertiesTypeDef
     ) -> Dict[str, Any]:
         """
         Modifies the specified WorkSpace properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_properties)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_workspace_properties)
         """
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/client.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_workspaces.client import WorkSpacesClient
 
     session = Session()
     client: WorkSpacesClient = session.client("workspaces")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApplicationType,
     ClientDeviceTypeType,
     DeletableSamlPropertyType,
@@ -78,29 +78,26 @@
     RebootRequestTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildRequestTypeDef,
     RebuildWorkspacesResultTypeDef,
     RootStorageTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
-    StandbyWorkspaceOutputTypeDef,
     StandbyWorkspaceTypeDef,
     StartRequestTypeDef,
     StartWorkspacesResultTypeDef,
     StopRequestTypeDef,
     StopWorkspacesResultTypeDef,
     TagTypeDef,
     TerminateRequestTypeDef,
     TerminateWorkspacesResultTypeDef,
     UserStorageTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
-    WorkspacePropertiesOutputTypeDef,
     WorkspacePropertiesTypeDef,
-    WorkspaceRequestOutputTypeDef,
     WorkspaceRequestTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -231,18 +228,15 @@
         """
         Creates an IP access control group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_ip_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_ip_group)
         """
     def create_standby_workspaces(
-        self,
-        *,
-        PrimaryRegion: str,
-        StandbyWorkspaces: Sequence[Union[StandbyWorkspaceTypeDef, StandbyWorkspaceOutputTypeDef]]
+        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceTypeDef]
     ) -> CreateStandbyWorkspacesResultTypeDef:
         """
         Creates a standby WorkSpace in a secondary Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_standby_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_standby_workspaces)
         """
@@ -285,15 +279,15 @@
         """
         Creates a new WorkSpace image from an existing WorkSpace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspace_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_workspace_image)
         """
     def create_workspaces(
-        self, *, Workspaces: Sequence[Union[WorkspaceRequestTypeDef, WorkspaceRequestOutputTypeDef]]
+        self, *, Workspaces: Sequence[WorkspaceRequestTypeDef]
     ) -> CreateWorkspacesResultTypeDef:
         """
         Creates one or more WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#create_workspaces)
         """
@@ -680,18 +674,15 @@
         """
         Modify the default properties used to create WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_creation_properties)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_workspace_creation_properties)
         """
     def modify_workspace_properties(
-        self,
-        *,
-        WorkspaceId: str,
-        WorkspaceProperties: Union[WorkspacePropertiesTypeDef, WorkspacePropertiesOutputTypeDef]
+        self, *, WorkspaceId: str, WorkspaceProperties: WorkspacePropertiesTypeDef
     ) -> Dict[str, Any]:
         """
         Modifies the specified WorkSpace properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_properties)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/client/#modify_workspace_properties)
         """
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/literals.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -368,15 +367,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/literals.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -366,15 +365,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/paginator.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/paginator.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/type_defs.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,23 @@
 
 __all__ = (
     "AccountModificationTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "IpRuleItemTypeDef",
+    "CertificateBasedAuthPropertiesOutputTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
+    "ClientPropertiesOutputTypeDef",
     "ClientPropertiesTypeDef",
+    "ComputeTypeOutputTypeDef",
     "ComputeTypeTypeDef",
     "ConnectClientAddInTypeDef",
     "ConnectionAliasAssociationTypeDef",
+    "ConnectionAliasPermissionOutputTypeDef",
     "ConnectionAliasPermissionTypeDef",
     "TagTypeDef",
     "CreateConnectClientAddInRequestRequestTypeDef",
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     "RootStorageTypeDef",
     "UserStorageTypeDef",
     "OperatingSystemTypeDef",
@@ -96,28 +100,30 @@
     "IosClientBrandingAttributesTypeDef",
     "DescribeClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsRequestRequestTypeDef",
     "DescribeConnectionAliasPermissionsRequestRequestTypeDef",
     "DescribeConnectionAliasesRequestRequestTypeDef",
     "DescribeIpGroupsRequestRequestTypeDef",
     "DescribeTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     "DescribeWorkspaceImagePermissionsRequestRequestTypeDef",
     "ImagePermissionTypeDef",
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     "DescribeWorkspaceSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     "WorkspaceConnectionStatusTypeDef",
     "DescribeWorkspacesRequestRequestTypeDef",
     "DisassociateConnectionAliasRequestRequestTypeDef",
     "DisassociateIpGroupsRequestRequestTypeDef",
     "FailedWorkspaceChangeRequestTypeDef",
     "IosImportClientBrandingAttributesTypeDef",
+    "IpRuleItemOutputTypeDef",
     "ListAvailableManagementCidrRangesRequestRequestTypeDef",
     "MigrateWorkspaceRequestRequestTypeDef",
     "ModificationStateTypeDef",
     "ModifyAccountRequestRequestTypeDef",
     "SamlPropertiesTypeDef",
     "SelfservicePermissionsTypeDef",
     "WorkspaceAccessPropertiesTypeDef",
@@ -125,101 +131,106 @@
     "WorkspacePropertiesTypeDef",
     "ModifyWorkspaceStateRequestRequestTypeDef",
     "RebootRequestTypeDef",
     "RebuildRequestTypeDef",
     "RelatedWorkspacePropertiesTypeDef",
     "RestoreWorkspaceRequestRequestTypeDef",
     "RevokeIpRulesRequestRequestTypeDef",
+    "RootStorageOutputTypeDef",
+    "SamlPropertiesOutputTypeDef",
+    "SelfservicePermissionsOutputTypeDef",
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     "UpdateWorkspaceImagePermissionRequestRequestTypeDef",
+    "UserStorageOutputTypeDef",
+    "WorkspaceAccessPropertiesOutputTypeDef",
     "WorkspacePropertiesOutputTypeDef",
     "AssociateConnectionAliasResultTypeDef",
     "CopyWorkspaceImageResultTypeDef",
     "CreateConnectClientAddInResultTypeDef",
     "CreateConnectionAliasResultTypeDef",
     "CreateIpGroupResultTypeDef",
     "CreateUpdatedWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsResultTypeDef",
     "DescribeAccountResultTypeDef",
     "ImportWorkspaceImageResultTypeDef",
     "ListAvailableManagementCidrRangesResultTypeDef",
     "MigrateWorkspaceResultTypeDef",
     "AuthorizeIpRulesRequestRequestTypeDef",
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
-    "WorkspacesIpGroupTypeDef",
     "ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     "ClientPropertiesResultTypeDef",
     "ModifyClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsResultTypeDef",
     "ConnectionAliasTypeDef",
     "DescribeConnectionAliasPermissionsResultTypeDef",
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     "CopyWorkspaceImageRequestRequestTypeDef",
     "CreateConnectionAliasRequestRequestTypeDef",
     "CreateIpGroupRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUpdatedWorkspaceImageRequestRequestTypeDef",
     "CreateWorkspaceImageRequestRequestTypeDef",
-    "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
-    "StandbyWorkspaceOutputTypeDef",
     "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
-    "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
     "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
     "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
     "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
     "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
     "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
     "DescribeClientBrandingResultTypeDef",
     "ImportClientBrandingResultTypeDef",
+    "DescribeTagsResultTypeDef",
+    "StandbyWorkspaceOutputTypeDef",
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     "DescribeWorkspaceSnapshotsResultTypeDef",
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     "RebootWorkspacesResultTypeDef",
     "RebuildWorkspacesResultTypeDef",
     "StartWorkspacesResultTypeDef",
     "StopWorkspacesResultTypeDef",
     "TerminateWorkspacesResultTypeDef",
     "ImportClientBrandingRequestRequestTypeDef",
+    "WorkspacesIpGroupTypeDef",
     "ModifySamlPropertiesRequestRequestTypeDef",
     "ModifySelfservicePermissionsRequestRequestTypeDef",
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
-    "WorkspaceDirectoryTypeDef",
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     "ModifyWorkspacePropertiesRequestRequestTypeDef",
     "WorkspaceRequestTypeDef",
     "RebootWorkspacesRequestRequestTypeDef",
     "RebuildWorkspacesRequestRequestTypeDef",
     "StartWorkspacesRequestRequestTypeDef",
     "StopWorkspacesRequestRequestTypeDef",
     "TerminateWorkspacesRequestRequestTypeDef",
     "WorkspaceImageTypeDef",
+    "WorkspaceBundleTypeDef",
+    "WorkspaceDirectoryTypeDef",
     "WorkspaceRequestOutputTypeDef",
     "WorkspaceTypeDef",
-    "DescribeIpGroupsResultTypeDef",
     "DescribeClientPropertiesResultTypeDef",
     "DescribeConnectionAliasesResultTypeDef",
-    "FailedCreateStandbyWorkspacesRequestTypeDef",
     "CreateStandbyWorkspacesRequestRequestTypeDef",
+    "FailedCreateStandbyWorkspacesRequestTypeDef",
+    "DescribeIpGroupsResultTypeDef",
+    "CreateWorkspacesRequestRequestTypeDef",
+    "DescribeWorkspaceImagesResultTypeDef",
     "CreateWorkspaceBundleResultTypeDef",
     "DescribeWorkspaceBundlesResultTypeDef",
     "DescribeWorkspaceDirectoriesResultTypeDef",
-    "DescribeWorkspaceImagesResultTypeDef",
-    "CreateWorkspacesRequestRequestTypeDef",
     "FailedCreateWorkspaceRequestTypeDef",
     "DescribeWorkspacesResultTypeDef",
     "CreateStandbyWorkspacesResultTypeDef",
     "CreateWorkspacesResultTypeDef",
 )
 
 AccountModificationTypeDef = TypedDict(
@@ -228,15 +239,14 @@
         "ModificationState": DedicatedTenancyModificationStateEnumType,
         "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
         "DedicatedTenancyManagementCidrRange": str,
         "StartTime": datetime,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 AssociateConnectionAliasRequestRequestTypeDef = TypedDict(
     "AssociateConnectionAliasRequestRequestTypeDef",
     {
         "AliasId": str,
         "ResourceId": str,
@@ -267,32 +277,55 @@
     {
         "ipRule": str,
         "ruleDesc": str,
     },
     total=False,
 )
 
+CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
+    "CertificateBasedAuthPropertiesOutputTypeDef",
+    {
+        "Status": CertificateBasedAuthStatusEnumType,
+        "CertificateAuthorityArn": str,
+    },
+)
+
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusEnumType,
         "CertificateAuthorityArn": str,
     },
     total=False,
 )
 
+ClientPropertiesOutputTypeDef = TypedDict(
+    "ClientPropertiesOutputTypeDef",
+    {
+        "ReconnectEnabled": ReconnectEnumType,
+        "LogUploadEnabled": LogUploadEnumType,
+    },
+)
+
 ClientPropertiesTypeDef = TypedDict(
     "ClientPropertiesTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
     },
     total=False,
 )
 
+ComputeTypeOutputTypeDef = TypedDict(
+    "ComputeTypeOutputTypeDef",
+    {
+        "Name": ComputeType,
+    },
+)
+
 ComputeTypeTypeDef = TypedDict(
     "ComputeTypeTypeDef",
     {
         "Name": ComputeType,
     },
     total=False,
 )
@@ -301,26 +334,32 @@
     "ConnectClientAddInTypeDef",
     {
         "AddInId": str,
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
-    total=False,
 )
 
 ConnectionAliasAssociationTypeDef = TypedDict(
     "ConnectionAliasAssociationTypeDef",
     {
         "AssociationStatus": AssociationStatusType,
         "AssociatedAccountId": str,
         "ResourceId": str,
         "ConnectionIdentifier": str,
     },
-    total=False,
+)
+
+ConnectionAliasPermissionOutputTypeDef = TypedDict(
+    "ConnectionAliasPermissionOutputTypeDef",
+    {
+        "SharedAccountId": str,
+        "AllowAssociation": bool,
+    },
 )
 
 ConnectionAliasPermissionTypeDef = TypedDict(
     "ConnectionAliasPermissionTypeDef",
     {
         "SharedAccountId": str,
         "AllowAssociation": bool,
@@ -359,15 +398,14 @@
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     {
         "UserName": str,
         "DirectoryId": str,
         "State": WorkspaceStateType,
         "WorkspaceId": str,
     },
-    total=False,
 )
 
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
@@ -383,27 +421,25 @@
 )
 
 OperatingSystemTypeDef = TypedDict(
     "OperatingSystemTypeDef",
     {
         "Type": OperatingSystemTypeType,
     },
-    total=False,
 )
 
 DefaultClientBrandingAttributesTypeDef = TypedDict(
     "DefaultClientBrandingAttributesTypeDef",
     {
         "LogoUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DefaultImportClientBrandingAttributesTypeDef = TypedDict(
     "DefaultImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "SupportEmail": str,
@@ -420,15 +456,14 @@
         "EnableWorkDocs": bool,
         "EnableInternetAccess": bool,
         "DefaultOu": str,
         "CustomSecurityGroupId": str,
         "UserEnabledAsLocalAdministrator": bool,
         "EnableMaintenanceMode": bool,
     },
-    total=False,
 )
 
 DeleteClientBrandingRequestRequestTypeDef = TypedDict(
     "DeleteClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Platforms": Sequence[ClientDeviceTypeType],
@@ -519,15 +554,14 @@
         "Logo2xUrl": str,
         "Logo3xUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DescribeClientPropertiesRequestRequestTypeDef = TypedDict(
     "DescribeClientPropertiesRequestRequestTypeDef",
     {
         "ResourceIds": Sequence[str],
     },
@@ -603,14 +637,22 @@
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 DescribeWorkspaceBundlesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     {
         "BundleIds": Sequence[str],
         "Owner": str,
         "NextToken": str,
     },
@@ -651,15 +693,14 @@
 
 
 ImagePermissionTypeDef = TypedDict(
     "ImagePermissionTypeDef",
     {
         "SharedAccountId": str,
     },
-    total=False,
 )
 
 DescribeWorkspaceImagesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     {
         "ImageIds": Sequence[str],
         "ImageType": ImageTypeType,
@@ -677,15 +718,14 @@
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "SnapshotTime": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesConnectionStatusRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "NextToken": str,
@@ -697,15 +737,14 @@
     "WorkspaceConnectionStatusTypeDef",
     {
         "WorkspaceId": str,
         "ConnectionState": ConnectionStateType,
         "ConnectionStateCheckTimestamp": datetime,
         "LastKnownUserConnectionTimestamp": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "DirectoryId": str,
@@ -735,15 +774,14 @@
 FailedWorkspaceChangeRequestTypeDef = TypedDict(
     "FailedWorkspaceChangeRequestTypeDef",
     {
         "WorkspaceId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 IosImportClientBrandingAttributesTypeDef = TypedDict(
     "IosImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "Logo2x": Union[str, bytes, IO[Any], StreamingBody],
@@ -752,14 +790,22 @@
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Mapping[str, str],
     },
     total=False,
 )
 
+IpRuleItemOutputTypeDef = TypedDict(
+    "IpRuleItemOutputTypeDef",
+    {
+        "ipRule": str,
+        "ruleDesc": str,
+    },
+)
+
 _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagementCidrRangesRequestRequestTypeDef",
     {
         "ManagementCidrRangeConstraint": str,
     },
 )
 _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
@@ -789,15 +835,14 @@
 
 ModificationStateTypeDef = TypedDict(
     "ModificationStateTypeDef",
     {
         "Resource": ModificationResourceEnumType,
         "State": ModificationStateEnumType,
     },
-    total=False,
 )
 
 ModifyAccountRequestRequestTypeDef = TypedDict(
     "ModifyAccountRequestRequestTypeDef",
     {
         "DedicatedTenancySupport": Literal["ENABLED"],
         "DedicatedTenancyManagementCidrRange": str,
@@ -894,15 +939,14 @@
     "RelatedWorkspacePropertiesTypeDef",
     {
         "WorkspaceId": str,
         "Region": str,
         "State": WorkspaceStateType,
         "Type": StandbyWorkspaceRelationshipTypeType,
     },
-    total=False,
 )
 
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
@@ -912,14 +956,41 @@
     "RevokeIpRulesRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[str],
     },
 )
 
+RootStorageOutputTypeDef = TypedDict(
+    "RootStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+SamlPropertiesOutputTypeDef = TypedDict(
+    "SamlPropertiesOutputTypeDef",
+    {
+        "Status": SamlStatusEnumType,
+        "UserAccessUrl": str,
+        "RelayStateParameterName": str,
+    },
+)
+
+SelfservicePermissionsOutputTypeDef = TypedDict(
+    "SelfservicePermissionsOutputTypeDef",
+    {
+        "RestartWorkspace": ReconnectEnumType,
+        "IncreaseVolumeSize": ReconnectEnumType,
+        "ChangeComputeType": ReconnectEnumType,
+        "SwitchRunningMode": ReconnectEnumType,
+        "RebuildWorkspace": ReconnectEnumType,
+    },
+)
+
 StartRequestTypeDef = TypedDict(
     "StartRequestTypeDef",
     {
         "WorkspaceId": str,
     },
     total=False,
 )
@@ -965,15 +1036,14 @@
 
 UpdateResultTypeDef = TypedDict(
     "UpdateResultTypeDef",
     {
         "UpdateAvailable": bool,
         "Description": str,
     },
-    total=False,
 )
 
 UpdateWorkspaceBundleRequestRequestTypeDef = TypedDict(
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     {
         "BundleId": str,
         "ImageId": str,
@@ -986,25 +1056,45 @@
     {
         "ImageId": str,
         "AllowCopyImage": bool,
         "SharedAccountId": str,
     },
 )
 
+UserStorageOutputTypeDef = TypedDict(
+    "UserStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+WorkspaceAccessPropertiesOutputTypeDef = TypedDict(
+    "WorkspaceAccessPropertiesOutputTypeDef",
+    {
+        "DeviceTypeWindows": AccessPropertyValueType,
+        "DeviceTypeOsx": AccessPropertyValueType,
+        "DeviceTypeWeb": AccessPropertyValueType,
+        "DeviceTypeIos": AccessPropertyValueType,
+        "DeviceTypeAndroid": AccessPropertyValueType,
+        "DeviceTypeChromeOs": AccessPropertyValueType,
+        "DeviceTypeZeroClient": AccessPropertyValueType,
+        "DeviceTypeLinux": AccessPropertyValueType,
+    },
+)
+
 WorkspacePropertiesOutputTypeDef = TypedDict(
     "WorkspacePropertiesOutputTypeDef",
     {
         "RunningMode": RunningModeType,
         "RunningModeAutoStopTimeoutInMinutes": int,
         "RootVolumeSizeGib": int,
         "UserVolumeSizeGib": int,
         "ComputeTypeName": ComputeType,
         "Protocols": List[ProtocolType],
     },
-    total=False,
 )
 
 AssociateConnectionAliasResultTypeDef = TypedDict(
     "AssociateConnectionAliasResultTypeDef",
     {
         "ConnectionIdentifier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1107,25 +1197,14 @@
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[IpRuleItemTypeDef],
     },
 )
 
-WorkspacesIpGroupTypeDef = TypedDict(
-    "WorkspacesIpGroupTypeDef",
-    {
-        "groupId": str,
-        "groupName": str,
-        "groupDesc": str,
-        "userRules": List[IpRuleItemTypeDef],
-    },
-    total=False,
-)
-
 _RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
@@ -1147,17 +1226,16 @@
     pass
 
 
 ClientPropertiesResultTypeDef = TypedDict(
     "ClientPropertiesResultTypeDef",
     {
         "ResourceId": str,
-        "ClientProperties": ClientPropertiesTypeDef,
+        "ClientProperties": ClientPropertiesOutputTypeDef,
     },
-    total=False,
 )
 
 ModifyClientPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyClientPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesTypeDef,
@@ -1178,22 +1256,21 @@
     {
         "ConnectionString": str,
         "AliasId": str,
         "State": ConnectionAliasStateType,
         "OwnerAccountId": str,
         "Associations": List[ConnectionAliasAssociationTypeDef],
     },
-    total=False,
 )
 
 DescribeConnectionAliasPermissionsResultTypeDef = TypedDict(
     "DescribeConnectionAliasPermissionsResultTypeDef",
     {
         "AliasId": str,
-        "ConnectionAliasPermissions": List[ConnectionAliasPermissionTypeDef],
+        "ConnectionAliasPermissions": List[ConnectionAliasPermissionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectionAliasPermissionRequestRequestTypeDef = TypedDict(
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
@@ -1325,22 +1402,14 @@
 class CreateWorkspaceImageRequestRequestTypeDef(
     _RequiredCreateWorkspaceImageRequestRequestTypeDef,
     _OptionalCreateWorkspaceImageRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeTagsResultTypeDef = TypedDict(
-    "DescribeTagsResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredImportWorkspaceImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportWorkspaceImageRequestRequestTypeDef",
     {
         "Ec2ImageId": str,
         "IngestionProcess": WorkspaceImageIngestionProcessType,
         "ImageName": str,
         "ImageDescription": str,
@@ -1385,37 +1454,14 @@
 class RegisterWorkspaceDirectoryRequestRequestTypeDef(
     _RequiredRegisterWorkspaceDirectoryRequestRequestTypeDef,
     _OptionalRegisterWorkspaceDirectoryRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_RequiredStandbyWorkspaceOutputTypeDef",
-    {
-        "PrimaryWorkspaceId": str,
-        "DirectoryId": str,
-    },
-)
-_OptionalStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_OptionalStandbyWorkspaceOutputTypeDef",
-    {
-        "VolumeEncryptionKey": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class StandbyWorkspaceOutputTypeDef(
-    _RequiredStandbyWorkspaceOutputTypeDef, _OptionalStandbyWorkspaceOutputTypeDef
-):
-    pass
-
-
 _RequiredStandbyWorkspaceTypeDef = TypedDict(
     "_RequiredStandbyWorkspaceTypeDef",
     {
         "PrimaryWorkspaceId": str,
         "DirectoryId": str,
     },
 )
@@ -1456,33 +1502,14 @@
 class CreateWorkspaceBundleRequestRequestTypeDef(
     _RequiredCreateWorkspaceBundleRequestRequestTypeDef,
     _OptionalCreateWorkspaceBundleRequestRequestTypeDef,
 ):
     pass
 
 
-WorkspaceBundleTypeDef = TypedDict(
-    "WorkspaceBundleTypeDef",
-    {
-        "BundleId": str,
-        "Name": str,
-        "Owner": str,
-        "Description": str,
-        "ImageId": str,
-        "RootStorage": RootStorageTypeDef,
-        "UserStorage": UserStorageTypeDef,
-        "ComputeType": ComputeTypeTypeDef,
-        "LastUpdatedTime": datetime,
-        "CreationTime": datetime,
-        "State": WorkspaceBundleStateType,
-        "BundleType": BundleTypeType,
-    },
-    total=False,
-)
-
 CreateWorkspaceImageResultTypeDef = TypedDict(
     "CreateWorkspaceImageResultTypeDef",
     {
         "ImageId": str,
         "Name": str,
         "Description": str,
         "OperatingSystem": OperatingSystemTypeDef,
@@ -1606,14 +1633,32 @@
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeTagsResultTypeDef = TypedDict(
+    "DescribeTagsResultTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StandbyWorkspaceOutputTypeDef = TypedDict(
+    "StandbyWorkspaceOutputTypeDef",
+    {
+        "PrimaryWorkspaceId": str,
+        "VolumeEncryptionKey": str,
+        "DirectoryId": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
 DescribeWorkspaceImagePermissionsResultTypeDef = TypedDict(
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     {
         "ImageId": str,
         "ImagePermissions": List[ImagePermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1701,14 +1746,24 @@
 class ImportClientBrandingRequestRequestTypeDef(
     _RequiredImportClientBrandingRequestRequestTypeDef,
     _OptionalImportClientBrandingRequestRequestTypeDef,
 ):
     pass
 
 
+WorkspacesIpGroupTypeDef = TypedDict(
+    "WorkspacesIpGroupTypeDef",
+    {
+        "groupId": str,
+        "groupName": str,
+        "groupDesc": str,
+        "userRules": List[IpRuleItemOutputTypeDef],
+    },
+)
+
 _RequiredModifySamlPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifySamlPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifySamlPropertiesRequestRequestTypeDef = TypedDict(
@@ -1740,39 +1795,14 @@
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
     },
 )
 
-WorkspaceDirectoryTypeDef = TypedDict(
-    "WorkspaceDirectoryTypeDef",
-    {
-        "DirectoryId": str,
-        "Alias": str,
-        "DirectoryName": str,
-        "RegistrationCode": str,
-        "SubnetIds": List[str],
-        "DnsIpAddresses": List[str],
-        "CustomerUserName": str,
-        "IamRoleId": str,
-        "DirectoryType": WorkspaceDirectoryTypeType,
-        "WorkspaceSecurityGroupId": str,
-        "State": WorkspaceDirectoryStateType,
-        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
-        "ipGroupIds": List[str],
-        "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
-        "Tenancy": TenancyType,
-        "SelfservicePermissions": SelfservicePermissionsTypeDef,
-        "SamlProperties": SamlPropertiesTypeDef,
-        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
-    },
-    total=False,
-)
-
 ModifyWorkspaceCreationPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceCreationProperties": WorkspaceCreationPropertiesTypeDef,
     },
 )
@@ -1856,44 +1886,72 @@
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "ErrorCode": str,
         "ErrorMessage": str,
         "Created": datetime,
         "OwnerAccountId": str,
         "Updates": UpdateResultTypeDef,
     },
-    total=False,
 )
 
-_RequiredWorkspaceRequestOutputTypeDef = TypedDict(
-    "_RequiredWorkspaceRequestOutputTypeDef",
+WorkspaceBundleTypeDef = TypedDict(
+    "WorkspaceBundleTypeDef",
     {
-        "DirectoryId": str,
-        "UserName": str,
         "BundleId": str,
+        "Name": str,
+        "Owner": str,
+        "Description": str,
+        "ImageId": str,
+        "RootStorage": RootStorageOutputTypeDef,
+        "UserStorage": UserStorageOutputTypeDef,
+        "ComputeType": ComputeTypeOutputTypeDef,
+        "LastUpdatedTime": datetime,
+        "CreationTime": datetime,
+        "State": WorkspaceBundleStateType,
+        "BundleType": BundleTypeType,
+    },
+)
+
+WorkspaceDirectoryTypeDef = TypedDict(
+    "WorkspaceDirectoryTypeDef",
+    {
+        "DirectoryId": str,
+        "Alias": str,
+        "DirectoryName": str,
+        "RegistrationCode": str,
+        "SubnetIds": List[str],
+        "DnsIpAddresses": List[str],
+        "CustomerUserName": str,
+        "IamRoleId": str,
+        "DirectoryType": WorkspaceDirectoryTypeType,
+        "WorkspaceSecurityGroupId": str,
+        "State": WorkspaceDirectoryStateType,
+        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
+        "ipGroupIds": List[str],
+        "WorkspaceAccessProperties": WorkspaceAccessPropertiesOutputTypeDef,
+        "Tenancy": TenancyType,
+        "SelfservicePermissions": SelfservicePermissionsOutputTypeDef,
+        "SamlProperties": SamlPropertiesOutputTypeDef,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
     },
 )
-_OptionalWorkspaceRequestOutputTypeDef = TypedDict(
-    "_OptionalWorkspaceRequestOutputTypeDef",
+
+WorkspaceRequestOutputTypeDef = TypedDict(
+    "WorkspaceRequestOutputTypeDef",
     {
+        "DirectoryId": str,
+        "UserName": str,
+        "BundleId": str,
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
-
-class WorkspaceRequestOutputTypeDef(
-    _RequiredWorkspaceRequestOutputTypeDef, _OptionalWorkspaceRequestOutputTypeDef
-):
-    pass
-
-
 WorkspaceTypeDef = TypedDict(
     "WorkspaceTypeDef",
     {
         "WorkspaceId": str,
         "DirectoryId": str,
         "UserName": str,
         "IpAddress": str,
@@ -1906,24 +1964,14 @@
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
         "ModificationStates": List[ModificationStateTypeDef],
         "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
     },
-    total=False,
-)
-
-DescribeIpGroupsResultTypeDef = TypedDict(
-    "DescribeIpGroupsResultTypeDef",
-    {
-        "Result": List[WorkspacesIpGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
 )
 
 DescribeClientPropertiesResultTypeDef = TypedDict(
     "DescribeClientPropertiesResultTypeDef",
     {
         "ClientPropertiesList": List[ClientPropertiesResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1935,31 +1983,53 @@
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
+    {
+        "PrimaryRegion": str,
+        "StandbyWorkspaces": Sequence[StandbyWorkspaceTypeDef],
+    },
+)
+
 FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "FailedCreateStandbyWorkspacesRequestTypeDef",
     {
         "StandbyWorkspaceRequest": StandbyWorkspaceOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
-CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateStandbyWorkspacesRequestRequestTypeDef",
+DescribeIpGroupsResultTypeDef = TypedDict(
+    "DescribeIpGroupsResultTypeDef",
     {
-        "PrimaryRegion": str,
-        "StandbyWorkspaces": Sequence[
-            Union[StandbyWorkspaceTypeDef, StandbyWorkspaceOutputTypeDef]
-        ],
+        "Result": List[WorkspacesIpGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateWorkspacesRequestRequestTypeDef",
+    {
+        "Workspaces": Sequence[WorkspaceRequestTypeDef],
+    },
+)
+
+DescribeWorkspaceImagesResultTypeDef = TypedDict(
+    "DescribeWorkspaceImagesResultTypeDef",
+    {
+        "Images": List[WorkspaceImageTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
@@ -1981,38 +2051,21 @@
     {
         "Directories": List[WorkspaceDirectoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeWorkspaceImagesResultTypeDef = TypedDict(
-    "DescribeWorkspaceImagesResultTypeDef",
-    {
-        "Images": List[WorkspaceImageTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateWorkspacesRequestRequestTypeDef",
-    {
-        "Workspaces": Sequence[Union[WorkspaceRequestTypeDef, WorkspaceRequestOutputTypeDef]],
-    },
-)
-
 FailedCreateWorkspaceRequestTypeDef = TypedDict(
     "FailedCreateWorkspaceRequestTypeDef",
     {
         "WorkspaceRequest": WorkspaceRequestOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces/type_defs.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,23 @@
 
 __all__ = (
     "AccountModificationTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "IpRuleItemTypeDef",
+    "CertificateBasedAuthPropertiesOutputTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
+    "ClientPropertiesOutputTypeDef",
     "ClientPropertiesTypeDef",
+    "ComputeTypeOutputTypeDef",
     "ComputeTypeTypeDef",
     "ConnectClientAddInTypeDef",
     "ConnectionAliasAssociationTypeDef",
+    "ConnectionAliasPermissionOutputTypeDef",
     "ConnectionAliasPermissionTypeDef",
     "TagTypeDef",
     "CreateConnectClientAddInRequestRequestTypeDef",
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     "RootStorageTypeDef",
     "UserStorageTypeDef",
     "OperatingSystemTypeDef",
@@ -95,28 +99,30 @@
     "IosClientBrandingAttributesTypeDef",
     "DescribeClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsRequestRequestTypeDef",
     "DescribeConnectionAliasPermissionsRequestRequestTypeDef",
     "DescribeConnectionAliasesRequestRequestTypeDef",
     "DescribeIpGroupsRequestRequestTypeDef",
     "DescribeTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     "DescribeWorkspaceImagePermissionsRequestRequestTypeDef",
     "ImagePermissionTypeDef",
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     "DescribeWorkspaceSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     "WorkspaceConnectionStatusTypeDef",
     "DescribeWorkspacesRequestRequestTypeDef",
     "DisassociateConnectionAliasRequestRequestTypeDef",
     "DisassociateIpGroupsRequestRequestTypeDef",
     "FailedWorkspaceChangeRequestTypeDef",
     "IosImportClientBrandingAttributesTypeDef",
+    "IpRuleItemOutputTypeDef",
     "ListAvailableManagementCidrRangesRequestRequestTypeDef",
     "MigrateWorkspaceRequestRequestTypeDef",
     "ModificationStateTypeDef",
     "ModifyAccountRequestRequestTypeDef",
     "SamlPropertiesTypeDef",
     "SelfservicePermissionsTypeDef",
     "WorkspaceAccessPropertiesTypeDef",
@@ -124,101 +130,106 @@
     "WorkspacePropertiesTypeDef",
     "ModifyWorkspaceStateRequestRequestTypeDef",
     "RebootRequestTypeDef",
     "RebuildRequestTypeDef",
     "RelatedWorkspacePropertiesTypeDef",
     "RestoreWorkspaceRequestRequestTypeDef",
     "RevokeIpRulesRequestRequestTypeDef",
+    "RootStorageOutputTypeDef",
+    "SamlPropertiesOutputTypeDef",
+    "SelfservicePermissionsOutputTypeDef",
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     "UpdateWorkspaceImagePermissionRequestRequestTypeDef",
+    "UserStorageOutputTypeDef",
+    "WorkspaceAccessPropertiesOutputTypeDef",
     "WorkspacePropertiesOutputTypeDef",
     "AssociateConnectionAliasResultTypeDef",
     "CopyWorkspaceImageResultTypeDef",
     "CreateConnectClientAddInResultTypeDef",
     "CreateConnectionAliasResultTypeDef",
     "CreateIpGroupResultTypeDef",
     "CreateUpdatedWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsResultTypeDef",
     "DescribeAccountResultTypeDef",
     "ImportWorkspaceImageResultTypeDef",
     "ListAvailableManagementCidrRangesResultTypeDef",
     "MigrateWorkspaceResultTypeDef",
     "AuthorizeIpRulesRequestRequestTypeDef",
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
-    "WorkspacesIpGroupTypeDef",
     "ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     "ClientPropertiesResultTypeDef",
     "ModifyClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsResultTypeDef",
     "ConnectionAliasTypeDef",
     "DescribeConnectionAliasPermissionsResultTypeDef",
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     "CopyWorkspaceImageRequestRequestTypeDef",
     "CreateConnectionAliasRequestRequestTypeDef",
     "CreateIpGroupRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUpdatedWorkspaceImageRequestRequestTypeDef",
     "CreateWorkspaceImageRequestRequestTypeDef",
-    "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
-    "StandbyWorkspaceOutputTypeDef",
     "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
-    "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
     "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
     "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
     "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
     "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
     "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
     "DescribeClientBrandingResultTypeDef",
     "ImportClientBrandingResultTypeDef",
+    "DescribeTagsResultTypeDef",
+    "StandbyWorkspaceOutputTypeDef",
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     "DescribeWorkspaceSnapshotsResultTypeDef",
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     "RebootWorkspacesResultTypeDef",
     "RebuildWorkspacesResultTypeDef",
     "StartWorkspacesResultTypeDef",
     "StopWorkspacesResultTypeDef",
     "TerminateWorkspacesResultTypeDef",
     "ImportClientBrandingRequestRequestTypeDef",
+    "WorkspacesIpGroupTypeDef",
     "ModifySamlPropertiesRequestRequestTypeDef",
     "ModifySelfservicePermissionsRequestRequestTypeDef",
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
-    "WorkspaceDirectoryTypeDef",
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     "ModifyWorkspacePropertiesRequestRequestTypeDef",
     "WorkspaceRequestTypeDef",
     "RebootWorkspacesRequestRequestTypeDef",
     "RebuildWorkspacesRequestRequestTypeDef",
     "StartWorkspacesRequestRequestTypeDef",
     "StopWorkspacesRequestRequestTypeDef",
     "TerminateWorkspacesRequestRequestTypeDef",
     "WorkspaceImageTypeDef",
+    "WorkspaceBundleTypeDef",
+    "WorkspaceDirectoryTypeDef",
     "WorkspaceRequestOutputTypeDef",
     "WorkspaceTypeDef",
-    "DescribeIpGroupsResultTypeDef",
     "DescribeClientPropertiesResultTypeDef",
     "DescribeConnectionAliasesResultTypeDef",
-    "FailedCreateStandbyWorkspacesRequestTypeDef",
     "CreateStandbyWorkspacesRequestRequestTypeDef",
+    "FailedCreateStandbyWorkspacesRequestTypeDef",
+    "DescribeIpGroupsResultTypeDef",
+    "CreateWorkspacesRequestRequestTypeDef",
+    "DescribeWorkspaceImagesResultTypeDef",
     "CreateWorkspaceBundleResultTypeDef",
     "DescribeWorkspaceBundlesResultTypeDef",
     "DescribeWorkspaceDirectoriesResultTypeDef",
-    "DescribeWorkspaceImagesResultTypeDef",
-    "CreateWorkspacesRequestRequestTypeDef",
     "FailedCreateWorkspaceRequestTypeDef",
     "DescribeWorkspacesResultTypeDef",
     "CreateStandbyWorkspacesResultTypeDef",
     "CreateWorkspacesResultTypeDef",
 )
 
 AccountModificationTypeDef = TypedDict(
@@ -227,15 +238,14 @@
         "ModificationState": DedicatedTenancyModificationStateEnumType,
         "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
         "DedicatedTenancyManagementCidrRange": str,
         "StartTime": datetime,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 AssociateConnectionAliasRequestRequestTypeDef = TypedDict(
     "AssociateConnectionAliasRequestRequestTypeDef",
     {
         "AliasId": str,
         "ResourceId": str,
@@ -266,32 +276,55 @@
     {
         "ipRule": str,
         "ruleDesc": str,
     },
     total=False,
 )
 
+CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
+    "CertificateBasedAuthPropertiesOutputTypeDef",
+    {
+        "Status": CertificateBasedAuthStatusEnumType,
+        "CertificateAuthorityArn": str,
+    },
+)
+
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusEnumType,
         "CertificateAuthorityArn": str,
     },
     total=False,
 )
 
+ClientPropertiesOutputTypeDef = TypedDict(
+    "ClientPropertiesOutputTypeDef",
+    {
+        "ReconnectEnabled": ReconnectEnumType,
+        "LogUploadEnabled": LogUploadEnumType,
+    },
+)
+
 ClientPropertiesTypeDef = TypedDict(
     "ClientPropertiesTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
     },
     total=False,
 )
 
+ComputeTypeOutputTypeDef = TypedDict(
+    "ComputeTypeOutputTypeDef",
+    {
+        "Name": ComputeType,
+    },
+)
+
 ComputeTypeTypeDef = TypedDict(
     "ComputeTypeTypeDef",
     {
         "Name": ComputeType,
     },
     total=False,
 )
@@ -300,26 +333,32 @@
     "ConnectClientAddInTypeDef",
     {
         "AddInId": str,
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
-    total=False,
 )
 
 ConnectionAliasAssociationTypeDef = TypedDict(
     "ConnectionAliasAssociationTypeDef",
     {
         "AssociationStatus": AssociationStatusType,
         "AssociatedAccountId": str,
         "ResourceId": str,
         "ConnectionIdentifier": str,
     },
-    total=False,
+)
+
+ConnectionAliasPermissionOutputTypeDef = TypedDict(
+    "ConnectionAliasPermissionOutputTypeDef",
+    {
+        "SharedAccountId": str,
+        "AllowAssociation": bool,
+    },
 )
 
 ConnectionAliasPermissionTypeDef = TypedDict(
     "ConnectionAliasPermissionTypeDef",
     {
         "SharedAccountId": str,
         "AllowAssociation": bool,
@@ -356,15 +395,14 @@
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     {
         "UserName": str,
         "DirectoryId": str,
         "State": WorkspaceStateType,
         "WorkspaceId": str,
     },
-    total=False,
 )
 
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
@@ -380,27 +418,25 @@
 )
 
 OperatingSystemTypeDef = TypedDict(
     "OperatingSystemTypeDef",
     {
         "Type": OperatingSystemTypeType,
     },
-    total=False,
 )
 
 DefaultClientBrandingAttributesTypeDef = TypedDict(
     "DefaultClientBrandingAttributesTypeDef",
     {
         "LogoUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DefaultImportClientBrandingAttributesTypeDef = TypedDict(
     "DefaultImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "SupportEmail": str,
@@ -417,15 +453,14 @@
         "EnableWorkDocs": bool,
         "EnableInternetAccess": bool,
         "DefaultOu": str,
         "CustomSecurityGroupId": str,
         "UserEnabledAsLocalAdministrator": bool,
         "EnableMaintenanceMode": bool,
     },
-    total=False,
 )
 
 DeleteClientBrandingRequestRequestTypeDef = TypedDict(
     "DeleteClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Platforms": Sequence[ClientDeviceTypeType],
@@ -516,15 +551,14 @@
         "Logo2xUrl": str,
         "Logo3xUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DescribeClientPropertiesRequestRequestTypeDef = TypedDict(
     "DescribeClientPropertiesRequestRequestTypeDef",
     {
         "ResourceIds": Sequence[str],
     },
@@ -596,14 +630,22 @@
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 DescribeWorkspaceBundlesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     {
         "BundleIds": Sequence[str],
         "Owner": str,
         "NextToken": str,
     },
@@ -642,15 +684,14 @@
     pass
 
 ImagePermissionTypeDef = TypedDict(
     "ImagePermissionTypeDef",
     {
         "SharedAccountId": str,
     },
-    total=False,
 )
 
 DescribeWorkspaceImagesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     {
         "ImageIds": Sequence[str],
         "ImageType": ImageTypeType,
@@ -668,15 +709,14 @@
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "SnapshotTime": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesConnectionStatusRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "NextToken": str,
@@ -688,15 +728,14 @@
     "WorkspaceConnectionStatusTypeDef",
     {
         "WorkspaceId": str,
         "ConnectionState": ConnectionStateType,
         "ConnectionStateCheckTimestamp": datetime,
         "LastKnownUserConnectionTimestamp": datetime,
     },
-    total=False,
 )
 
 DescribeWorkspacesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "DirectoryId": str,
@@ -726,15 +765,14 @@
 FailedWorkspaceChangeRequestTypeDef = TypedDict(
     "FailedWorkspaceChangeRequestTypeDef",
     {
         "WorkspaceId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 IosImportClientBrandingAttributesTypeDef = TypedDict(
     "IosImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "Logo2x": Union[str, bytes, IO[Any], StreamingBody],
@@ -743,14 +781,22 @@
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Mapping[str, str],
     },
     total=False,
 )
 
+IpRuleItemOutputTypeDef = TypedDict(
+    "IpRuleItemOutputTypeDef",
+    {
+        "ipRule": str,
+        "ruleDesc": str,
+    },
+)
+
 _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagementCidrRangesRequestRequestTypeDef",
     {
         "ManagementCidrRangeConstraint": str,
     },
 )
 _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
@@ -778,15 +824,14 @@
 
 ModificationStateTypeDef = TypedDict(
     "ModificationStateTypeDef",
     {
         "Resource": ModificationResourceEnumType,
         "State": ModificationStateEnumType,
     },
-    total=False,
 )
 
 ModifyAccountRequestRequestTypeDef = TypedDict(
     "ModifyAccountRequestRequestTypeDef",
     {
         "DedicatedTenancySupport": Literal["ENABLED"],
         "DedicatedTenancyManagementCidrRange": str,
@@ -883,15 +928,14 @@
     "RelatedWorkspacePropertiesTypeDef",
     {
         "WorkspaceId": str,
         "Region": str,
         "State": WorkspaceStateType,
         "Type": StandbyWorkspaceRelationshipTypeType,
     },
-    total=False,
 )
 
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
@@ -901,14 +945,41 @@
     "RevokeIpRulesRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[str],
     },
 )
 
+RootStorageOutputTypeDef = TypedDict(
+    "RootStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+SamlPropertiesOutputTypeDef = TypedDict(
+    "SamlPropertiesOutputTypeDef",
+    {
+        "Status": SamlStatusEnumType,
+        "UserAccessUrl": str,
+        "RelayStateParameterName": str,
+    },
+)
+
+SelfservicePermissionsOutputTypeDef = TypedDict(
+    "SelfservicePermissionsOutputTypeDef",
+    {
+        "RestartWorkspace": ReconnectEnumType,
+        "IncreaseVolumeSize": ReconnectEnumType,
+        "ChangeComputeType": ReconnectEnumType,
+        "SwitchRunningMode": ReconnectEnumType,
+        "RebuildWorkspace": ReconnectEnumType,
+    },
+)
+
 StartRequestTypeDef = TypedDict(
     "StartRequestTypeDef",
     {
         "WorkspaceId": str,
     },
     total=False,
 )
@@ -952,15 +1023,14 @@
 
 UpdateResultTypeDef = TypedDict(
     "UpdateResultTypeDef",
     {
         "UpdateAvailable": bool,
         "Description": str,
     },
-    total=False,
 )
 
 UpdateWorkspaceBundleRequestRequestTypeDef = TypedDict(
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     {
         "BundleId": str,
         "ImageId": str,
@@ -973,25 +1043,45 @@
     {
         "ImageId": str,
         "AllowCopyImage": bool,
         "SharedAccountId": str,
     },
 )
 
+UserStorageOutputTypeDef = TypedDict(
+    "UserStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+WorkspaceAccessPropertiesOutputTypeDef = TypedDict(
+    "WorkspaceAccessPropertiesOutputTypeDef",
+    {
+        "DeviceTypeWindows": AccessPropertyValueType,
+        "DeviceTypeOsx": AccessPropertyValueType,
+        "DeviceTypeWeb": AccessPropertyValueType,
+        "DeviceTypeIos": AccessPropertyValueType,
+        "DeviceTypeAndroid": AccessPropertyValueType,
+        "DeviceTypeChromeOs": AccessPropertyValueType,
+        "DeviceTypeZeroClient": AccessPropertyValueType,
+        "DeviceTypeLinux": AccessPropertyValueType,
+    },
+)
+
 WorkspacePropertiesOutputTypeDef = TypedDict(
     "WorkspacePropertiesOutputTypeDef",
     {
         "RunningMode": RunningModeType,
         "RunningModeAutoStopTimeoutInMinutes": int,
         "RootVolumeSizeGib": int,
         "UserVolumeSizeGib": int,
         "ComputeTypeName": ComputeType,
         "Protocols": List[ProtocolType],
     },
-    total=False,
 )
 
 AssociateConnectionAliasResultTypeDef = TypedDict(
     "AssociateConnectionAliasResultTypeDef",
     {
         "ConnectionIdentifier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1094,25 +1184,14 @@
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[IpRuleItemTypeDef],
     },
 )
 
-WorkspacesIpGroupTypeDef = TypedDict(
-    "WorkspacesIpGroupTypeDef",
-    {
-        "groupId": str,
-        "groupName": str,
-        "groupDesc": str,
-        "userRules": List[IpRuleItemTypeDef],
-    },
-    total=False,
-)
-
 _RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
@@ -1132,17 +1211,16 @@
 ):
     pass
 
 ClientPropertiesResultTypeDef = TypedDict(
     "ClientPropertiesResultTypeDef",
     {
         "ResourceId": str,
-        "ClientProperties": ClientPropertiesTypeDef,
+        "ClientProperties": ClientPropertiesOutputTypeDef,
     },
-    total=False,
 )
 
 ModifyClientPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyClientPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesTypeDef,
@@ -1163,22 +1241,21 @@
     {
         "ConnectionString": str,
         "AliasId": str,
         "State": ConnectionAliasStateType,
         "OwnerAccountId": str,
         "Associations": List[ConnectionAliasAssociationTypeDef],
     },
-    total=False,
 )
 
 DescribeConnectionAliasPermissionsResultTypeDef = TypedDict(
     "DescribeConnectionAliasPermissionsResultTypeDef",
     {
         "AliasId": str,
-        "ConnectionAliasPermissions": List[ConnectionAliasPermissionTypeDef],
+        "ConnectionAliasPermissions": List[ConnectionAliasPermissionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectionAliasPermissionRequestRequestTypeDef = TypedDict(
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
@@ -1300,22 +1377,14 @@
 
 class CreateWorkspaceImageRequestRequestTypeDef(
     _RequiredCreateWorkspaceImageRequestRequestTypeDef,
     _OptionalCreateWorkspaceImageRequestRequestTypeDef,
 ):
     pass
 
-DescribeTagsResultTypeDef = TypedDict(
-    "DescribeTagsResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredImportWorkspaceImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportWorkspaceImageRequestRequestTypeDef",
     {
         "Ec2ImageId": str,
         "IngestionProcess": WorkspaceImageIngestionProcessType,
         "ImageName": str,
         "ImageDescription": str,
@@ -1356,35 +1425,14 @@
 
 class RegisterWorkspaceDirectoryRequestRequestTypeDef(
     _RequiredRegisterWorkspaceDirectoryRequestRequestTypeDef,
     _OptionalRegisterWorkspaceDirectoryRequestRequestTypeDef,
 ):
     pass
 
-_RequiredStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_RequiredStandbyWorkspaceOutputTypeDef",
-    {
-        "PrimaryWorkspaceId": str,
-        "DirectoryId": str,
-    },
-)
-_OptionalStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_OptionalStandbyWorkspaceOutputTypeDef",
-    {
-        "VolumeEncryptionKey": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class StandbyWorkspaceOutputTypeDef(
-    _RequiredStandbyWorkspaceOutputTypeDef, _OptionalStandbyWorkspaceOutputTypeDef
-):
-    pass
-
 _RequiredStandbyWorkspaceTypeDef = TypedDict(
     "_RequiredStandbyWorkspaceTypeDef",
     {
         "PrimaryWorkspaceId": str,
         "DirectoryId": str,
     },
 )
@@ -1421,33 +1469,14 @@
 
 class CreateWorkspaceBundleRequestRequestTypeDef(
     _RequiredCreateWorkspaceBundleRequestRequestTypeDef,
     _OptionalCreateWorkspaceBundleRequestRequestTypeDef,
 ):
     pass
 
-WorkspaceBundleTypeDef = TypedDict(
-    "WorkspaceBundleTypeDef",
-    {
-        "BundleId": str,
-        "Name": str,
-        "Owner": str,
-        "Description": str,
-        "ImageId": str,
-        "RootStorage": RootStorageTypeDef,
-        "UserStorage": UserStorageTypeDef,
-        "ComputeType": ComputeTypeTypeDef,
-        "LastUpdatedTime": datetime,
-        "CreationTime": datetime,
-        "State": WorkspaceBundleStateType,
-        "BundleType": BundleTypeType,
-    },
-    total=False,
-)
-
 CreateWorkspaceImageResultTypeDef = TypedDict(
     "CreateWorkspaceImageResultTypeDef",
     {
         "ImageId": str,
         "Name": str,
         "Description": str,
         "OperatingSystem": OperatingSystemTypeDef,
@@ -1569,14 +1598,32 @@
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeTagsResultTypeDef = TypedDict(
+    "DescribeTagsResultTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StandbyWorkspaceOutputTypeDef = TypedDict(
+    "StandbyWorkspaceOutputTypeDef",
+    {
+        "PrimaryWorkspaceId": str,
+        "VolumeEncryptionKey": str,
+        "DirectoryId": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
 DescribeWorkspaceImagePermissionsResultTypeDef = TypedDict(
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     {
         "ImageId": str,
         "ImagePermissions": List[ImagePermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1662,14 +1709,24 @@
 
 class ImportClientBrandingRequestRequestTypeDef(
     _RequiredImportClientBrandingRequestRequestTypeDef,
     _OptionalImportClientBrandingRequestRequestTypeDef,
 ):
     pass
 
+WorkspacesIpGroupTypeDef = TypedDict(
+    "WorkspacesIpGroupTypeDef",
+    {
+        "groupId": str,
+        "groupName": str,
+        "groupDesc": str,
+        "userRules": List[IpRuleItemOutputTypeDef],
+    },
+)
+
 _RequiredModifySamlPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifySamlPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifySamlPropertiesRequestRequestTypeDef = TypedDict(
@@ -1699,39 +1756,14 @@
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
     },
 )
 
-WorkspaceDirectoryTypeDef = TypedDict(
-    "WorkspaceDirectoryTypeDef",
-    {
-        "DirectoryId": str,
-        "Alias": str,
-        "DirectoryName": str,
-        "RegistrationCode": str,
-        "SubnetIds": List[str],
-        "DnsIpAddresses": List[str],
-        "CustomerUserName": str,
-        "IamRoleId": str,
-        "DirectoryType": WorkspaceDirectoryTypeType,
-        "WorkspaceSecurityGroupId": str,
-        "State": WorkspaceDirectoryStateType,
-        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
-        "ipGroupIds": List[str],
-        "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
-        "Tenancy": TenancyType,
-        "SelfservicePermissions": SelfservicePermissionsTypeDef,
-        "SamlProperties": SamlPropertiesTypeDef,
-        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
-    },
-    total=False,
-)
-
 ModifyWorkspaceCreationPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceCreationProperties": WorkspaceCreationPropertiesTypeDef,
     },
 )
@@ -1813,42 +1845,72 @@
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "ErrorCode": str,
         "ErrorMessage": str,
         "Created": datetime,
         "OwnerAccountId": str,
         "Updates": UpdateResultTypeDef,
     },
-    total=False,
 )
 
-_RequiredWorkspaceRequestOutputTypeDef = TypedDict(
-    "_RequiredWorkspaceRequestOutputTypeDef",
+WorkspaceBundleTypeDef = TypedDict(
+    "WorkspaceBundleTypeDef",
     {
-        "DirectoryId": str,
-        "UserName": str,
         "BundleId": str,
+        "Name": str,
+        "Owner": str,
+        "Description": str,
+        "ImageId": str,
+        "RootStorage": RootStorageOutputTypeDef,
+        "UserStorage": UserStorageOutputTypeDef,
+        "ComputeType": ComputeTypeOutputTypeDef,
+        "LastUpdatedTime": datetime,
+        "CreationTime": datetime,
+        "State": WorkspaceBundleStateType,
+        "BundleType": BundleTypeType,
+    },
+)
+
+WorkspaceDirectoryTypeDef = TypedDict(
+    "WorkspaceDirectoryTypeDef",
+    {
+        "DirectoryId": str,
+        "Alias": str,
+        "DirectoryName": str,
+        "RegistrationCode": str,
+        "SubnetIds": List[str],
+        "DnsIpAddresses": List[str],
+        "CustomerUserName": str,
+        "IamRoleId": str,
+        "DirectoryType": WorkspaceDirectoryTypeType,
+        "WorkspaceSecurityGroupId": str,
+        "State": WorkspaceDirectoryStateType,
+        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
+        "ipGroupIds": List[str],
+        "WorkspaceAccessProperties": WorkspaceAccessPropertiesOutputTypeDef,
+        "Tenancy": TenancyType,
+        "SelfservicePermissions": SelfservicePermissionsOutputTypeDef,
+        "SamlProperties": SamlPropertiesOutputTypeDef,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
     },
 )
-_OptionalWorkspaceRequestOutputTypeDef = TypedDict(
-    "_OptionalWorkspaceRequestOutputTypeDef",
+
+WorkspaceRequestOutputTypeDef = TypedDict(
+    "WorkspaceRequestOutputTypeDef",
     {
+        "DirectoryId": str,
+        "UserName": str,
+        "BundleId": str,
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
-class WorkspaceRequestOutputTypeDef(
-    _RequiredWorkspaceRequestOutputTypeDef, _OptionalWorkspaceRequestOutputTypeDef
-):
-    pass
-
 WorkspaceTypeDef = TypedDict(
     "WorkspaceTypeDef",
     {
         "WorkspaceId": str,
         "DirectoryId": str,
         "UserName": str,
         "IpAddress": str,
@@ -1861,24 +1923,14 @@
         "VolumeEncryptionKey": str,
         "UserVolumeEncryptionEnabled": bool,
         "RootVolumeEncryptionEnabled": bool,
         "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
         "ModificationStates": List[ModificationStateTypeDef],
         "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
     },
-    total=False,
-)
-
-DescribeIpGroupsResultTypeDef = TypedDict(
-    "DescribeIpGroupsResultTypeDef",
-    {
-        "Result": List[WorkspacesIpGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
 )
 
 DescribeClientPropertiesResultTypeDef = TypedDict(
     "DescribeClientPropertiesResultTypeDef",
     {
         "ClientPropertiesList": List[ClientPropertiesResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1890,31 +1942,53 @@
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
+    {
+        "PrimaryRegion": str,
+        "StandbyWorkspaces": Sequence[StandbyWorkspaceTypeDef],
+    },
+)
+
 FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "FailedCreateStandbyWorkspacesRequestTypeDef",
     {
         "StandbyWorkspaceRequest": StandbyWorkspaceOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
-CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateStandbyWorkspacesRequestRequestTypeDef",
+DescribeIpGroupsResultTypeDef = TypedDict(
+    "DescribeIpGroupsResultTypeDef",
     {
-        "PrimaryRegion": str,
-        "StandbyWorkspaces": Sequence[
-            Union[StandbyWorkspaceTypeDef, StandbyWorkspaceOutputTypeDef]
-        ],
+        "Result": List[WorkspacesIpGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateWorkspacesRequestRequestTypeDef",
+    {
+        "Workspaces": Sequence[WorkspaceRequestTypeDef],
+    },
+)
+
+DescribeWorkspaceImagesResultTypeDef = TypedDict(
+    "DescribeWorkspaceImagesResultTypeDef",
+    {
+        "Images": List[WorkspaceImageTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
@@ -1936,38 +2010,21 @@
     {
         "Directories": List[WorkspaceDirectoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeWorkspaceImagesResultTypeDef = TypedDict(
-    "DescribeWorkspaceImagesResultTypeDef",
-    {
-        "Images": List[WorkspaceImageTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateWorkspacesRequestRequestTypeDef",
-    {
-        "Workspaces": Sequence[Union[WorkspaceRequestTypeDef, WorkspaceRequestOutputTypeDef]],
-    },
-)
-
 FailedCreateWorkspaceRequestTypeDef = TypedDict(
     "FailedCreateWorkspaceRequestTypeDef",
     {
         "WorkspaceRequest": WorkspaceRequestOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces.egg-info/PKG-INFO` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WorkSpaces 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.9
+Summary: Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workspaces"></a>
 
 # mypy-boto3-workspaces
 
 [![PyPI - mypy-boto3-workspaces](https://img.shields.io/pypi/v/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces)](https://pepy.tech/project/mypy-boto3-workspaces)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,19 +393,23 @@
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
+    ClientPropertiesOutputTypeDef,
     ClientPropertiesTypeDef,
+    ComputeTypeOutputTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
+    ConnectionAliasPermissionOutputTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
@@ -426,28 +430,30 @@
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
     IosImportClientBrandingAttributesTypeDef,
+    IpRuleItemOutputTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
@@ -455,101 +461,106 @@
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
+    RootStorageOutputTypeDef,
+    SamlPropertiesOutputTypeDef,
+    SelfservicePermissionsOutputTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
+    UserStorageOutputTypeDef,
+    WorkspaceAccessPropertiesOutputTypeDef,
     WorkspacePropertiesOutputTypeDef,
     AssociateConnectionAliasResultTypeDef,
     CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInResultTypeDef,
     CreateConnectionAliasResultTypeDef,
     CreateIpGroupResultTypeDef,
     CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
     DescribeAccountResultTypeDef,
     ImportWorkspaceImageResultTypeDef,
     ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
-    WorkspacesIpGroupTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
     CreateConnectionAliasRequestRequestTypeDef,
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
-    DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
-    StandbyWorkspaceOutputTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
-    WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
     DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
     DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
+    DescribeTagsResultTypeDef,
+    StandbyWorkspaceOutputTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
     StartWorkspacesResultTypeDef,
     StopWorkspacesResultTypeDef,
     TerminateWorkspacesResultTypeDef,
     ImportClientBrandingRequestRequestTypeDef,
+    WorkspacesIpGroupTypeDef,
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
-    WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
+    WorkspaceBundleTypeDef,
+    WorkspaceDirectoryTypeDef,
     WorkspaceRequestOutputTypeDef,
     WorkspaceTypeDef,
-    DescribeIpGroupsResultTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
-    FailedCreateStandbyWorkspacesRequestTypeDef,
     CreateStandbyWorkspacesRequestRequestTypeDef,
+    FailedCreateStandbyWorkspacesRequestTypeDef,
+    DescribeIpGroupsResultTypeDef,
+    CreateWorkspacesRequestRequestTypeDef,
+    DescribeWorkspaceImagesResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
-    DescribeWorkspaceImagesResultTypeDef,
-    CreateWorkspacesRequestRequestTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
     DescribeWorkspacesResultTypeDef,
     CreateStandbyWorkspacesResultTypeDef,
     CreateWorkspacesResultTypeDef,
 )
```

### Comparing `mypy-boto3-workspaces-1.28.15.post1/mypy_boto3_workspaces.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.15.post1/setup.py` & `mypy-boto3-workspaces-1.28.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces",
-    version="1.28.15.post1",
+    version="1.28.9",
     packages=["mypy_boto3_workspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkSpaces 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

