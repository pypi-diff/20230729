# Comparing `tmp/mypy-boto3-managedblockchain-1.28.12.tar.gz` & `tmp/mypy-boto3-managedblockchain-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-managedblockchain-1.28.12.tar", last modified: Thu Jul 27 05:34:59 2023, max compression
+gzip compressed data, was "mypy-boto3-managedblockchain-1.28.15.tar", last modified: Fri Jul 28 20:43:13 2023, max compression
```

## Comparing `mypy-boto3-managedblockchain-1.28.12.tar` & `mypy-boto3-managedblockchain-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16593 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20594 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29044 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-07-27 05:25:51.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16593 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:59.000000 mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:59.648446 mypy-boto3-managedblockchain-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-27 05:25:50.000000 mypy-boto3-managedblockchain-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:13.841454 mypy-boto3-managedblockchain-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-07-28 20:43:13.841454 mypy-boto3-managedblockchain-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:13.833454 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20594 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-07-28 20:30:53.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26645 2023-07-28 20:30:53.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:13.841454 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-07-28 20:43:13.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:43:13.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:13.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:13.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:13.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:43:13.000000 mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:13.841454 mypy-boto3-managedblockchain-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-28 20:30:52.000000 mypy-boto3-managedblockchain-1.28.15/setup.py
```

### Comparing `mypy-boto3-managedblockchain-1.28.12/LICENSE` & `mypy-boto3-managedblockchain-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.12/PKG-INFO` & `mypy-boto3-managedblockchain-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain
-Version: 1.28.12
-Summary: Type annotations for boto3.ManagedBlockchain 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ManagedBlockchain 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,108 +334,98 @@
 `mypy_boto3_managedblockchain.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
-    ApprovalThresholdPolicyOutputTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
-    CreateAccessorOutputTypeDef,
-    CreateMemberOutputTypeDef,
-    CreateNetworkOutputTypeDef,
-    CreateNodeOutputTypeDef,
-    CreateProposalOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteAccessorInputRequestTypeDef,
     DeleteMemberInputRequestTypeDef,
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
-    InviteActionOutputTypeDef,
     InviteActionTypeDef,
-    ListAccessorsInputListAccessorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
     ListNodesInputRequestTypeDef,
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
-    PaginatorConfigTypeDef,
-    RemoveActionOutputTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
-    ListAccessorsOutputTypeDef,
-    GetAccessorOutputTypeDef,
-    VotingPolicyOutputTypeDef,
     VotingPolicyTypeDef,
+    CreateAccessorOutputTypeDef,
+    CreateMemberOutputTypeDef,
+    CreateNetworkOutputTypeDef,
+    CreateNodeOutputTypeDef,
+    CreateProposalOutputTypeDef,
+    GetAccessorOutputTypeDef,
+    ListAccessorsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
+    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
-    LogConfigurationsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
     NetworkFrameworkAttributesTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeFrameworkAttributesTypeDef,
     ProposalActionsOutputTypeDef,
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
-    MemberFabricLogPublishingConfigurationOutputTypeDef,
-    NodeFabricLogPublishingConfigurationOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
     ProposalTypeDef,
     CreateProposalInputRequestTypeDef,
-    MemberLogPublishingConfigurationOutputTypeDef,
-    NodeLogPublishingConfigurationOutputTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
-    MemberTypeDef,
-    NodeTypeDef,
     MemberConfigurationTypeDef,
+    MemberTypeDef,
     UpdateMemberInputRequestTypeDef,
     NodeConfigurationTypeDef,
+    NodeTypeDef,
     UpdateNodeInputRequestTypeDef,
-    GetMemberOutputTypeDef,
-    GetNodeOutputTypeDef,
     CreateMemberInputRequestTypeDef,
     CreateNetworkInputRequestTypeDef,
+    GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
+    GetNodeOutputTypeDef,
 )
 
 
 def get_structure() -> AccessorSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-managedblockchain-1.28.12/README.md` & `mypy-boto3-managedblockchain-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,108 +302,98 @@
 `mypy_boto3_managedblockchain.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
-    ApprovalThresholdPolicyOutputTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
-    CreateAccessorOutputTypeDef,
-    CreateMemberOutputTypeDef,
-    CreateNetworkOutputTypeDef,
-    CreateNodeOutputTypeDef,
-    CreateProposalOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteAccessorInputRequestTypeDef,
     DeleteMemberInputRequestTypeDef,
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
-    InviteActionOutputTypeDef,
     InviteActionTypeDef,
-    ListAccessorsInputListAccessorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
     ListNodesInputRequestTypeDef,
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
-    PaginatorConfigTypeDef,
-    RemoveActionOutputTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
-    ListAccessorsOutputTypeDef,
-    GetAccessorOutputTypeDef,
-    VotingPolicyOutputTypeDef,
     VotingPolicyTypeDef,
+    CreateAccessorOutputTypeDef,
+    CreateMemberOutputTypeDef,
+    CreateNetworkOutputTypeDef,
+    CreateNodeOutputTypeDef,
+    CreateProposalOutputTypeDef,
+    GetAccessorOutputTypeDef,
+    ListAccessorsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
+    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
-    LogConfigurationsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
     NetworkFrameworkAttributesTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeFrameworkAttributesTypeDef,
     ProposalActionsOutputTypeDef,
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
-    MemberFabricLogPublishingConfigurationOutputTypeDef,
-    NodeFabricLogPublishingConfigurationOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
     ProposalTypeDef,
     CreateProposalInputRequestTypeDef,
-    MemberLogPublishingConfigurationOutputTypeDef,
-    NodeLogPublishingConfigurationOutputTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
-    MemberTypeDef,
-    NodeTypeDef,
     MemberConfigurationTypeDef,
+    MemberTypeDef,
     UpdateMemberInputRequestTypeDef,
     NodeConfigurationTypeDef,
+    NodeTypeDef,
     UpdateNodeInputRequestTypeDef,
-    GetMemberOutputTypeDef,
-    GetNodeOutputTypeDef,
     CreateMemberInputRequestTypeDef,
     CreateNetworkInputRequestTypeDef,
+    GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
+    GetNodeOutputTypeDef,
 )
 
 
 def get_structure() -> AccessorSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__init__.py` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__init__.pyi` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/__main__.py` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedBlockchain 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ManagedBlockchain 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\nOther"
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

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/client.py` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/client.pyi` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/literals.py` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/literals.pyi` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/paginator.py` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListAccessorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/paginator.pyi` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListAccessorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/paginators/#listaccessorspaginator)
         """
```

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/type_defs.py` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,108 +38,98 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
-    "ApprovalThresholdPolicyOutputTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
-    "CreateAccessorOutputTypeDef",
-    "CreateMemberOutputTypeDef",
-    "CreateNetworkOutputTypeDef",
-    "CreateNodeOutputTypeDef",
-    "CreateProposalOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteAccessorInputRequestTypeDef",
     "DeleteMemberInputRequestTypeDef",
     "DeleteNodeInputRequestTypeDef",
     "GetAccessorInputRequestTypeDef",
     "GetMemberInputRequestTypeDef",
     "GetNetworkInputRequestTypeDef",
     "GetNodeInputRequestTypeDef",
     "GetProposalInputRequestTypeDef",
     "NetworkSummaryTypeDef",
-    "InviteActionOutputTypeDef",
     "InviteActionTypeDef",
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessorsInputRequestTypeDef",
     "ListInvitationsInputRequestTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
     "ListNetworksInputRequestTypeDef",
     "ListNodesInputRequestTypeDef",
     "NodeSummaryTypeDef",
     "ListProposalVotesInputRequestTypeDef",
     "VoteSummaryTypeDef",
     "ListProposalsInputRequestTypeDef",
     "ProposalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "MemberFabricAttributesTypeDef",
     "MemberFabricConfigurationTypeDef",
     "NetworkEthereumAttributesTypeDef",
     "NetworkFabricAttributesTypeDef",
     "NetworkFabricConfigurationTypeDef",
     "NodeEthereumAttributesTypeDef",
     "NodeFabricAttributesTypeDef",
-    "PaginatorConfigTypeDef",
-    "RemoveActionOutputTypeDef",
     "RemoveActionTypeDef",
     "RejectInvitationInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VoteOnProposalInputRequestTypeDef",
-    "ListAccessorsOutputTypeDef",
-    "GetAccessorOutputTypeDef",
-    "VotingPolicyOutputTypeDef",
     "VotingPolicyTypeDef",
+    "CreateAccessorOutputTypeDef",
+    "CreateMemberOutputTypeDef",
+    "CreateNetworkOutputTypeDef",
+    "CreateNodeOutputTypeDef",
+    "CreateProposalOutputTypeDef",
+    "GetAccessorOutputTypeDef",
+    "ListAccessorsOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "InvitationTypeDef",
     "ListNetworksOutputTypeDef",
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListNodesOutputTypeDef",
     "ListProposalVotesOutputTypeDef",
     "ListProposalsOutputTypeDef",
-    "LogConfigurationsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
     "NetworkFrameworkAttributesTypeDef",
     "NetworkFrameworkConfigurationTypeDef",
     "NodeFrameworkAttributesTypeDef",
     "ProposalActionsOutputTypeDef",
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
-    "MemberFabricLogPublishingConfigurationOutputTypeDef",
-    "NodeFabricLogPublishingConfigurationOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
     "ProposalTypeDef",
     "CreateProposalInputRequestTypeDef",
-    "MemberLogPublishingConfigurationOutputTypeDef",
-    "NodeLogPublishingConfigurationOutputTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
-    "MemberTypeDef",
-    "NodeTypeDef",
     "MemberConfigurationTypeDef",
+    "MemberTypeDef",
     "UpdateMemberInputRequestTypeDef",
     "NodeConfigurationTypeDef",
+    "NodeTypeDef",
     "UpdateNodeInputRequestTypeDef",
-    "GetMemberOutputTypeDef",
-    "GetNodeOutputTypeDef",
     "CreateMemberInputRequestTypeDef",
     "CreateNetworkInputRequestTypeDef",
+    "GetMemberOutputTypeDef",
     "CreateNodeInputRequestTypeDef",
+    "GetNodeOutputTypeDef",
 )
 
 AccessorSummaryTypeDef = TypedDict(
     "AccessorSummaryTypeDef",
     {
         "Id": str,
         "Type": Literal["BILLING_TOKEN"],
@@ -160,24 +150,14 @@
         "CreationDate": datetime,
         "Arn": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-ApprovalThresholdPolicyOutputTypeDef = TypedDict(
-    "ApprovalThresholdPolicyOutputTypeDef",
-    {
-        "ThresholdPercentage": int,
-        "ProposalDurationInHours": int,
-        "ThresholdComparator": ThresholdComparatorType,
-    },
-    total=False,
-)
-
 ApprovalThresholdPolicyTypeDef = TypedDict(
     "ApprovalThresholdPolicyTypeDef",
     {
         "ThresholdPercentage": int,
         "ProposalDurationInHours": int,
         "ThresholdComparator": ThresholdComparatorType,
     },
@@ -202,53 +182,22 @@
 
 class CreateAccessorInputRequestTypeDef(
     _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
 ):
     pass
 
 
-CreateAccessorOutputTypeDef = TypedDict(
-    "CreateAccessorOutputTypeDef",
-    {
-        "AccessorId": str,
-        "BillingToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMemberOutputTypeDef = TypedDict(
-    "CreateMemberOutputTypeDef",
-    {
-        "MemberId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNetworkOutputTypeDef = TypedDict(
-    "CreateNetworkOutputTypeDef",
-    {
-        "NetworkId": str,
-        "MemberId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNodeOutputTypeDef = TypedDict(
-    "CreateNodeOutputTypeDef",
-    {
-        "NodeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProposalOutputTypeDef = TypedDict(
-    "CreateProposalOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ProposalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteAccessorInputRequestTypeDef = TypedDict(
     "DeleteAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
@@ -348,32 +297,27 @@
         "Status": NetworkStatusType,
         "CreationDate": datetime,
         "Arn": str,
     },
     total=False,
 )
 
-InviteActionOutputTypeDef = TypedDict(
-    "InviteActionOutputTypeDef",
-    {
-        "Principal": str,
-    },
-)
-
 InviteActionTypeDef = TypedDict(
     "InviteActionTypeDef",
     {
         "Principal": str,
     },
 )
 
-ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
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
 
 ListAccessorsInputRequestTypeDef = TypedDict(
     "ListAccessorsInputRequestTypeDef",
     {
@@ -553,30 +497,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
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
-LogConfigurationOutputTypeDef = TypedDict(
-    "LogConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 LogConfigurationTypeDef = TypedDict(
     "LogConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -636,56 +564,28 @@
     {
         "PeerEndpoint": str,
         "PeerEventEndpoint": str,
     },
     total=False,
 )
 
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
-RemoveActionOutputTypeDef = TypedDict(
-    "RemoveActionOutputTypeDef",
-    {
-        "MemberId": str,
-    },
-)
-
 RemoveActionTypeDef = TypedDict(
     "RemoveActionTypeDef",
     {
         "MemberId": str,
     },
 )
 
 RejectInvitationInputRequestTypeDef = TypedDict(
     "RejectInvitationInputRequestTypeDef",
     {
         "InvitationId": str,
     },
 )
 
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -704,45 +604,87 @@
         "NetworkId": str,
         "ProposalId": str,
         "VoterMemberId": str,
         "Vote": VoteValueType,
     },
 )
 
-ListAccessorsOutputTypeDef = TypedDict(
-    "ListAccessorsOutputTypeDef",
+VotingPolicyTypeDef = TypedDict(
+    "VotingPolicyTypeDef",
     {
-        "Accessors": List[AccessorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
+    },
+    total=False,
+)
+
+CreateAccessorOutputTypeDef = TypedDict(
+    "CreateAccessorOutputTypeDef",
+    {
+        "AccessorId": str,
+        "BillingToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMemberOutputTypeDef = TypedDict(
+    "CreateMemberOutputTypeDef",
+    {
+        "MemberId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkOutputTypeDef = TypedDict(
+    "CreateNetworkOutputTypeDef",
+    {
+        "NetworkId": str,
+        "MemberId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNodeOutputTypeDef = TypedDict(
+    "CreateNodeOutputTypeDef",
+    {
+        "NodeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProposalOutputTypeDef = TypedDict(
+    "CreateProposalOutputTypeDef",
+    {
+        "ProposalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccessorOutputTypeDef = TypedDict(
     "GetAccessorOutputTypeDef",
     {
         "Accessor": AccessorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VotingPolicyOutputTypeDef = TypedDict(
-    "VotingPolicyOutputTypeDef",
+ListAccessorsOutputTypeDef = TypedDict(
+    "ListAccessorsOutputTypeDef",
     {
-        "ApprovalThresholdPolicy": ApprovalThresholdPolicyOutputTypeDef,
+        "Accessors": List[AccessorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VotingPolicyTypeDef = TypedDict(
-    "VotingPolicyTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 InvitationTypeDef = TypedDict(
     "InvitationTypeDef",
     {
         "InvitationId": str,
         "CreationDate": datetime,
@@ -755,60 +697,60 @@
 )
 
 ListNetworksOutputTypeDef = TypedDict(
     "ListNetworksOutputTypeDef",
     {
         "Networks": List[NetworkSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "Members": List[MemberSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodesOutputTypeDef = TypedDict(
     "ListNodesOutputTypeDef",
     {
         "Nodes": List[NodeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProposalVotesOutputTypeDef = TypedDict(
     "ListProposalVotesOutputTypeDef",
     {
         "ProposalVotes": List[VoteSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProposalsOutputTypeDef = TypedDict(
     "ListProposalsOutputTypeDef",
     {
         "Proposals": List[ProposalSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LogConfigurationsOutputTypeDef = TypedDict(
-    "LogConfigurationsOutputTypeDef",
-    {
-        "Cloudwatch": LogConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 LogConfigurationsTypeDef = TypedDict(
     "LogConfigurationsTypeDef",
     {
         "Cloudwatch": LogConfigurationTypeDef,
     },
@@ -856,16 +798,16 @@
     },
     total=False,
 )
 
 ProposalActionsOutputTypeDef = TypedDict(
     "ProposalActionsOutputTypeDef",
     {
-        "Invitations": List[InviteActionOutputTypeDef],
-        "Removals": List[RemoveActionOutputTypeDef],
+        "Invitations": List[InviteActionTypeDef],
+        "Removals": List[RemoveActionTypeDef],
     },
     total=False,
 )
 
 ProposalActionsTypeDef = TypedDict(
     "ProposalActionsTypeDef",
     {
@@ -876,35 +818,18 @@
 )
 
 ListInvitationsOutputTypeDef = TypedDict(
     "ListInvitationsOutputTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MemberFabricLogPublishingConfigurationOutputTypeDef = TypedDict(
-    "MemberFabricLogPublishingConfigurationOutputTypeDef",
-    {
-        "CaLogs": LogConfigurationsOutputTypeDef,
-    },
-    total=False,
-)
-
-NodeFabricLogPublishingConfigurationOutputTypeDef = TypedDict(
-    "NodeFabricLogPublishingConfigurationOutputTypeDef",
-    {
-        "ChaincodeLogs": LogConfigurationsOutputTypeDef,
-        "PeerLogs": LogConfigurationsOutputTypeDef,
-    },
-    total=False,
-)
-
 MemberFabricLogPublishingConfigurationTypeDef = TypedDict(
     "MemberFabricLogPublishingConfigurationTypeDef",
     {
         "CaLogs": LogConfigurationsTypeDef,
     },
     total=False,
 )
@@ -924,15 +849,15 @@
         "Id": str,
         "Name": str,
         "Description": str,
         "Framework": FrameworkType,
         "FrameworkVersion": str,
         "FrameworkAttributes": NetworkFrameworkAttributesTypeDef,
         "VpcEndpointServiceName": str,
-        "VotingPolicy": VotingPolicyOutputTypeDef,
+        "VotingPolicy": VotingPolicyTypeDef,
         "Status": NetworkStatusType,
         "CreationDate": datetime,
         "Tags": Dict[str, str],
         "Arn": str,
     },
     total=False,
 )
@@ -979,30 +904,14 @@
 
 class CreateProposalInputRequestTypeDef(
     _RequiredCreateProposalInputRequestTypeDef, _OptionalCreateProposalInputRequestTypeDef
 ):
     pass
 
 
-MemberLogPublishingConfigurationOutputTypeDef = TypedDict(
-    "MemberLogPublishingConfigurationOutputTypeDef",
-    {
-        "Fabric": MemberFabricLogPublishingConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-NodeLogPublishingConfigurationOutputTypeDef = TypedDict(
-    "NodeLogPublishingConfigurationOutputTypeDef",
-    {
-        "Fabric": NodeFabricLogPublishingConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
         "Fabric": MemberFabricLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
@@ -1015,62 +924,24 @@
     total=False,
 )
 
 GetNetworkOutputTypeDef = TypedDict(
     "GetNetworkOutputTypeDef",
     {
         "Network": NetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProposalOutputTypeDef = TypedDict(
     "GetProposalOutputTypeDef",
     {
         "Proposal": ProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MemberTypeDef = TypedDict(
-    "MemberTypeDef",
-    {
-        "NetworkId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "FrameworkAttributes": MemberFrameworkAttributesTypeDef,
-        "LogPublishingConfiguration": MemberLogPublishingConfigurationOutputTypeDef,
-        "Status": MemberStatusType,
-        "CreationDate": datetime,
-        "Tags": Dict[str, str],
-        "Arn": str,
-        "KmsKeyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
-)
-
-NodeTypeDef = TypedDict(
-    "NodeTypeDef",
-    {
-        "NetworkId": str,
-        "MemberId": str,
-        "Id": str,
-        "InstanceType": str,
-        "AvailabilityZone": str,
-        "FrameworkAttributes": NodeFrameworkAttributesTypeDef,
-        "LogPublishingConfiguration": NodeLogPublishingConfigurationOutputTypeDef,
-        "StateDB": StateDBTypeType,
-        "Status": NodeStatusType,
-        "CreationDate": datetime,
-        "Tags": Dict[str, str],
-        "Arn": str,
-        "KmsKeyArn": str,
-    },
-    total=False,
 )
 
 _RequiredMemberConfigurationTypeDef = TypedDict(
     "_RequiredMemberConfigurationTypeDef",
     {
         "Name": str,
         "FrameworkConfiguration": MemberFrameworkConfigurationTypeDef,
@@ -1090,14 +961,32 @@
 
 class MemberConfigurationTypeDef(
     _RequiredMemberConfigurationTypeDef, _OptionalMemberConfigurationTypeDef
 ):
     pass
 
 
+MemberTypeDef = TypedDict(
+    "MemberTypeDef",
+    {
+        "NetworkId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "FrameworkAttributes": MemberFrameworkAttributesTypeDef,
+        "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
+        "Status": MemberStatusType,
+        "CreationDate": datetime,
+        "Tags": Dict[str, str],
+        "Arn": str,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateMemberInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMemberInputRequestTypeDef",
     {
         "NetworkId": str,
         "MemberId": str,
     },
 )
@@ -1135,14 +1024,34 @@
 
 class NodeConfigurationTypeDef(
     _RequiredNodeConfigurationTypeDef, _OptionalNodeConfigurationTypeDef
 ):
     pass
 
 
+NodeTypeDef = TypedDict(
+    "NodeTypeDef",
+    {
+        "NetworkId": str,
+        "MemberId": str,
+        "Id": str,
+        "InstanceType": str,
+        "AvailabilityZone": str,
+        "FrameworkAttributes": NodeFrameworkAttributesTypeDef,
+        "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
+        "StateDB": StateDBTypeType,
+        "Status": NodeStatusType,
+        "CreationDate": datetime,
+        "Tags": Dict[str, str],
+        "Arn": str,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateNodeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateNodeInputRequestTypeDef",
     {
         "NetworkId": str,
         "NodeId": str,
     },
 )
@@ -1158,30 +1067,14 @@
 
 class UpdateNodeInputRequestTypeDef(
     _RequiredUpdateNodeInputRequestTypeDef, _OptionalUpdateNodeInputRequestTypeDef
 ):
     pass
 
 
-GetMemberOutputTypeDef = TypedDict(
-    "GetMemberOutputTypeDef",
-    {
-        "Member": MemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetNodeOutputTypeDef = TypedDict(
-    "GetNodeOutputTypeDef",
-    {
-        "Node": NodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMemberInputRequestTypeDef = TypedDict(
     "CreateMemberInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "InvitationId": str,
         "NetworkId": str,
         "MemberConfiguration": MemberConfigurationTypeDef,
@@ -1212,14 +1105,22 @@
 
 class CreateNetworkInputRequestTypeDef(
     _RequiredCreateNetworkInputRequestTypeDef, _OptionalCreateNetworkInputRequestTypeDef
 ):
     pass
 
 
+GetMemberOutputTypeDef = TypedDict(
+    "GetMemberOutputTypeDef",
+    {
+        "Member": MemberTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateNodeInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "NetworkId": str,
         "NodeConfiguration": NodeConfigurationTypeDef,
     },
@@ -1234,7 +1135,16 @@
 )
 
 
 class CreateNodeInputRequestTypeDef(
     _RequiredCreateNodeInputRequestTypeDef, _OptionalCreateNodeInputRequestTypeDef
 ):
     pass
+
+
+GetNodeOutputTypeDef = TypedDict(
+    "GetNodeOutputTypeDef",
+    {
+        "Node": NodeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain/type_defs.pyi` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -37,108 +37,98 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
-    "ApprovalThresholdPolicyOutputTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
-    "CreateAccessorOutputTypeDef",
-    "CreateMemberOutputTypeDef",
-    "CreateNetworkOutputTypeDef",
-    "CreateNodeOutputTypeDef",
-    "CreateProposalOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteAccessorInputRequestTypeDef",
     "DeleteMemberInputRequestTypeDef",
     "DeleteNodeInputRequestTypeDef",
     "GetAccessorInputRequestTypeDef",
     "GetMemberInputRequestTypeDef",
     "GetNetworkInputRequestTypeDef",
     "GetNodeInputRequestTypeDef",
     "GetProposalInputRequestTypeDef",
     "NetworkSummaryTypeDef",
-    "InviteActionOutputTypeDef",
     "InviteActionTypeDef",
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessorsInputRequestTypeDef",
     "ListInvitationsInputRequestTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
     "ListNetworksInputRequestTypeDef",
     "ListNodesInputRequestTypeDef",
     "NodeSummaryTypeDef",
     "ListProposalVotesInputRequestTypeDef",
     "VoteSummaryTypeDef",
     "ListProposalsInputRequestTypeDef",
     "ProposalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "MemberFabricAttributesTypeDef",
     "MemberFabricConfigurationTypeDef",
     "NetworkEthereumAttributesTypeDef",
     "NetworkFabricAttributesTypeDef",
     "NetworkFabricConfigurationTypeDef",
     "NodeEthereumAttributesTypeDef",
     "NodeFabricAttributesTypeDef",
-    "PaginatorConfigTypeDef",
-    "RemoveActionOutputTypeDef",
     "RemoveActionTypeDef",
     "RejectInvitationInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VoteOnProposalInputRequestTypeDef",
-    "ListAccessorsOutputTypeDef",
-    "GetAccessorOutputTypeDef",
-    "VotingPolicyOutputTypeDef",
     "VotingPolicyTypeDef",
+    "CreateAccessorOutputTypeDef",
+    "CreateMemberOutputTypeDef",
+    "CreateNetworkOutputTypeDef",
+    "CreateNodeOutputTypeDef",
+    "CreateProposalOutputTypeDef",
+    "GetAccessorOutputTypeDef",
+    "ListAccessorsOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "InvitationTypeDef",
     "ListNetworksOutputTypeDef",
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListNodesOutputTypeDef",
     "ListProposalVotesOutputTypeDef",
     "ListProposalsOutputTypeDef",
-    "LogConfigurationsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
     "NetworkFrameworkAttributesTypeDef",
     "NetworkFrameworkConfigurationTypeDef",
     "NodeFrameworkAttributesTypeDef",
     "ProposalActionsOutputTypeDef",
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
-    "MemberFabricLogPublishingConfigurationOutputTypeDef",
-    "NodeFabricLogPublishingConfigurationOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
     "ProposalTypeDef",
     "CreateProposalInputRequestTypeDef",
-    "MemberLogPublishingConfigurationOutputTypeDef",
-    "NodeLogPublishingConfigurationOutputTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
-    "MemberTypeDef",
-    "NodeTypeDef",
     "MemberConfigurationTypeDef",
+    "MemberTypeDef",
     "UpdateMemberInputRequestTypeDef",
     "NodeConfigurationTypeDef",
+    "NodeTypeDef",
     "UpdateNodeInputRequestTypeDef",
-    "GetMemberOutputTypeDef",
-    "GetNodeOutputTypeDef",
     "CreateMemberInputRequestTypeDef",
     "CreateNetworkInputRequestTypeDef",
+    "GetMemberOutputTypeDef",
     "CreateNodeInputRequestTypeDef",
+    "GetNodeOutputTypeDef",
 )
 
 AccessorSummaryTypeDef = TypedDict(
     "AccessorSummaryTypeDef",
     {
         "Id": str,
         "Type": Literal["BILLING_TOKEN"],
@@ -159,24 +149,14 @@
         "CreationDate": datetime,
         "Arn": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-ApprovalThresholdPolicyOutputTypeDef = TypedDict(
-    "ApprovalThresholdPolicyOutputTypeDef",
-    {
-        "ThresholdPercentage": int,
-        "ProposalDurationInHours": int,
-        "ThresholdComparator": ThresholdComparatorType,
-    },
-    total=False,
-)
-
 ApprovalThresholdPolicyTypeDef = TypedDict(
     "ApprovalThresholdPolicyTypeDef",
     {
         "ThresholdPercentage": int,
         "ProposalDurationInHours": int,
         "ThresholdComparator": ThresholdComparatorType,
     },
@@ -199,53 +179,22 @@
 )
 
 class CreateAccessorInputRequestTypeDef(
     _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
 ):
     pass
 
-CreateAccessorOutputTypeDef = TypedDict(
-    "CreateAccessorOutputTypeDef",
-    {
-        "AccessorId": str,
-        "BillingToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMemberOutputTypeDef = TypedDict(
-    "CreateMemberOutputTypeDef",
-    {
-        "MemberId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNetworkOutputTypeDef = TypedDict(
-    "CreateNetworkOutputTypeDef",
-    {
-        "NetworkId": str,
-        "MemberId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNodeOutputTypeDef = TypedDict(
-    "CreateNodeOutputTypeDef",
-    {
-        "NodeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProposalOutputTypeDef = TypedDict(
-    "CreateProposalOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ProposalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteAccessorInputRequestTypeDef = TypedDict(
     "DeleteAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
@@ -341,32 +290,27 @@
         "Status": NetworkStatusType,
         "CreationDate": datetime,
         "Arn": str,
     },
     total=False,
 )
 
-InviteActionOutputTypeDef = TypedDict(
-    "InviteActionOutputTypeDef",
-    {
-        "Principal": str,
-    },
-)
-
 InviteActionTypeDef = TypedDict(
     "InviteActionTypeDef",
     {
         "Principal": str,
     },
 )
 
-ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
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
 
 ListAccessorsInputRequestTypeDef = TypedDict(
     "ListAccessorsInputRequestTypeDef",
     {
@@ -538,30 +482,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
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
-LogConfigurationOutputTypeDef = TypedDict(
-    "LogConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 LogConfigurationTypeDef = TypedDict(
     "LogConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -621,56 +549,28 @@
     {
         "PeerEndpoint": str,
         "PeerEventEndpoint": str,
     },
     total=False,
 )
 
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
-RemoveActionOutputTypeDef = TypedDict(
-    "RemoveActionOutputTypeDef",
-    {
-        "MemberId": str,
-    },
-)
-
 RemoveActionTypeDef = TypedDict(
     "RemoveActionTypeDef",
     {
         "MemberId": str,
     },
 )
 
 RejectInvitationInputRequestTypeDef = TypedDict(
     "RejectInvitationInputRequestTypeDef",
     {
         "InvitationId": str,
     },
 )
 
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -689,45 +589,87 @@
         "NetworkId": str,
         "ProposalId": str,
         "VoterMemberId": str,
         "Vote": VoteValueType,
     },
 )
 
-ListAccessorsOutputTypeDef = TypedDict(
-    "ListAccessorsOutputTypeDef",
+VotingPolicyTypeDef = TypedDict(
+    "VotingPolicyTypeDef",
     {
-        "Accessors": List[AccessorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
+    },
+    total=False,
+)
+
+CreateAccessorOutputTypeDef = TypedDict(
+    "CreateAccessorOutputTypeDef",
+    {
+        "AccessorId": str,
+        "BillingToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMemberOutputTypeDef = TypedDict(
+    "CreateMemberOutputTypeDef",
+    {
+        "MemberId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkOutputTypeDef = TypedDict(
+    "CreateNetworkOutputTypeDef",
+    {
+        "NetworkId": str,
+        "MemberId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNodeOutputTypeDef = TypedDict(
+    "CreateNodeOutputTypeDef",
+    {
+        "NodeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProposalOutputTypeDef = TypedDict(
+    "CreateProposalOutputTypeDef",
+    {
+        "ProposalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccessorOutputTypeDef = TypedDict(
     "GetAccessorOutputTypeDef",
     {
         "Accessor": AccessorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VotingPolicyOutputTypeDef = TypedDict(
-    "VotingPolicyOutputTypeDef",
+ListAccessorsOutputTypeDef = TypedDict(
+    "ListAccessorsOutputTypeDef",
     {
-        "ApprovalThresholdPolicy": ApprovalThresholdPolicyOutputTypeDef,
+        "Accessors": List[AccessorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VotingPolicyTypeDef = TypedDict(
-    "VotingPolicyTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 InvitationTypeDef = TypedDict(
     "InvitationTypeDef",
     {
         "InvitationId": str,
         "CreationDate": datetime,
@@ -740,60 +682,60 @@
 )
 
 ListNetworksOutputTypeDef = TypedDict(
     "ListNetworksOutputTypeDef",
     {
         "Networks": List[NetworkSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "Members": List[MemberSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodesOutputTypeDef = TypedDict(
     "ListNodesOutputTypeDef",
     {
         "Nodes": List[NodeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProposalVotesOutputTypeDef = TypedDict(
     "ListProposalVotesOutputTypeDef",
     {
         "ProposalVotes": List[VoteSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProposalsOutputTypeDef = TypedDict(
     "ListProposalsOutputTypeDef",
     {
         "Proposals": List[ProposalSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LogConfigurationsOutputTypeDef = TypedDict(
-    "LogConfigurationsOutputTypeDef",
-    {
-        "Cloudwatch": LogConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 LogConfigurationsTypeDef = TypedDict(
     "LogConfigurationsTypeDef",
     {
         "Cloudwatch": LogConfigurationTypeDef,
     },
@@ -841,16 +783,16 @@
     },
     total=False,
 )
 
 ProposalActionsOutputTypeDef = TypedDict(
     "ProposalActionsOutputTypeDef",
     {
-        "Invitations": List[InviteActionOutputTypeDef],
-        "Removals": List[RemoveActionOutputTypeDef],
+        "Invitations": List[InviteActionTypeDef],
+        "Removals": List[RemoveActionTypeDef],
     },
     total=False,
 )
 
 ProposalActionsTypeDef = TypedDict(
     "ProposalActionsTypeDef",
     {
@@ -861,33 +803,16 @@
 )
 
 ListInvitationsOutputTypeDef = TypedDict(
     "ListInvitationsOutputTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MemberFabricLogPublishingConfigurationOutputTypeDef = TypedDict(
-    "MemberFabricLogPublishingConfigurationOutputTypeDef",
-    {
-        "CaLogs": LogConfigurationsOutputTypeDef,
-    },
-    total=False,
-)
-
-NodeFabricLogPublishingConfigurationOutputTypeDef = TypedDict(
-    "NodeFabricLogPublishingConfigurationOutputTypeDef",
-    {
-        "ChaincodeLogs": LogConfigurationsOutputTypeDef,
-        "PeerLogs": LogConfigurationsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 MemberFabricLogPublishingConfigurationTypeDef = TypedDict(
     "MemberFabricLogPublishingConfigurationTypeDef",
     {
         "CaLogs": LogConfigurationsTypeDef,
     },
@@ -909,15 +834,15 @@
         "Id": str,
         "Name": str,
         "Description": str,
         "Framework": FrameworkType,
         "FrameworkVersion": str,
         "FrameworkAttributes": NetworkFrameworkAttributesTypeDef,
         "VpcEndpointServiceName": str,
-        "VotingPolicy": VotingPolicyOutputTypeDef,
+        "VotingPolicy": VotingPolicyTypeDef,
         "Status": NetworkStatusType,
         "CreationDate": datetime,
         "Tags": Dict[str, str],
         "Arn": str,
     },
     total=False,
 )
@@ -962,30 +887,14 @@
 )
 
 class CreateProposalInputRequestTypeDef(
     _RequiredCreateProposalInputRequestTypeDef, _OptionalCreateProposalInputRequestTypeDef
 ):
     pass
 
-MemberLogPublishingConfigurationOutputTypeDef = TypedDict(
-    "MemberLogPublishingConfigurationOutputTypeDef",
-    {
-        "Fabric": MemberFabricLogPublishingConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-NodeLogPublishingConfigurationOutputTypeDef = TypedDict(
-    "NodeLogPublishingConfigurationOutputTypeDef",
-    {
-        "Fabric": NodeFabricLogPublishingConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
         "Fabric": MemberFabricLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
@@ -998,62 +907,24 @@
     total=False,
 )
 
 GetNetworkOutputTypeDef = TypedDict(
     "GetNetworkOutputTypeDef",
     {
         "Network": NetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProposalOutputTypeDef = TypedDict(
     "GetProposalOutputTypeDef",
     {
         "Proposal": ProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MemberTypeDef = TypedDict(
-    "MemberTypeDef",
-    {
-        "NetworkId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "FrameworkAttributes": MemberFrameworkAttributesTypeDef,
-        "LogPublishingConfiguration": MemberLogPublishingConfigurationOutputTypeDef,
-        "Status": MemberStatusType,
-        "CreationDate": datetime,
-        "Tags": Dict[str, str],
-        "Arn": str,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
-NodeTypeDef = TypedDict(
-    "NodeTypeDef",
-    {
-        "NetworkId": str,
-        "MemberId": str,
-        "Id": str,
-        "InstanceType": str,
-        "AvailabilityZone": str,
-        "FrameworkAttributes": NodeFrameworkAttributesTypeDef,
-        "LogPublishingConfiguration": NodeLogPublishingConfigurationOutputTypeDef,
-        "StateDB": StateDBTypeType,
-        "Status": NodeStatusType,
-        "CreationDate": datetime,
-        "Tags": Dict[str, str],
-        "Arn": str,
-        "KmsKeyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredMemberConfigurationTypeDef = TypedDict(
     "_RequiredMemberConfigurationTypeDef",
     {
         "Name": str,
         "FrameworkConfiguration": MemberFrameworkConfigurationTypeDef,
@@ -1071,14 +942,32 @@
 )
 
 class MemberConfigurationTypeDef(
     _RequiredMemberConfigurationTypeDef, _OptionalMemberConfigurationTypeDef
 ):
     pass
 
+MemberTypeDef = TypedDict(
+    "MemberTypeDef",
+    {
+        "NetworkId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "FrameworkAttributes": MemberFrameworkAttributesTypeDef,
+        "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
+        "Status": MemberStatusType,
+        "CreationDate": datetime,
+        "Tags": Dict[str, str],
+        "Arn": str,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateMemberInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMemberInputRequestTypeDef",
     {
         "NetworkId": str,
         "MemberId": str,
     },
 )
@@ -1112,14 +1001,34 @@
 )
 
 class NodeConfigurationTypeDef(
     _RequiredNodeConfigurationTypeDef, _OptionalNodeConfigurationTypeDef
 ):
     pass
 
+NodeTypeDef = TypedDict(
+    "NodeTypeDef",
+    {
+        "NetworkId": str,
+        "MemberId": str,
+        "Id": str,
+        "InstanceType": str,
+        "AvailabilityZone": str,
+        "FrameworkAttributes": NodeFrameworkAttributesTypeDef,
+        "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
+        "StateDB": StateDBTypeType,
+        "Status": NodeStatusType,
+        "CreationDate": datetime,
+        "Tags": Dict[str, str],
+        "Arn": str,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateNodeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateNodeInputRequestTypeDef",
     {
         "NetworkId": str,
         "NodeId": str,
     },
 )
@@ -1133,30 +1042,14 @@
 )
 
 class UpdateNodeInputRequestTypeDef(
     _RequiredUpdateNodeInputRequestTypeDef, _OptionalUpdateNodeInputRequestTypeDef
 ):
     pass
 
-GetMemberOutputTypeDef = TypedDict(
-    "GetMemberOutputTypeDef",
-    {
-        "Member": MemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetNodeOutputTypeDef = TypedDict(
-    "GetNodeOutputTypeDef",
-    {
-        "Node": NodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMemberInputRequestTypeDef = TypedDict(
     "CreateMemberInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "InvitationId": str,
         "NetworkId": str,
         "MemberConfiguration": MemberConfigurationTypeDef,
@@ -1185,14 +1078,22 @@
 )
 
 class CreateNetworkInputRequestTypeDef(
     _RequiredCreateNetworkInputRequestTypeDef, _OptionalCreateNetworkInputRequestTypeDef
 ):
     pass
 
+GetMemberOutputTypeDef = TypedDict(
+    "GetMemberOutputTypeDef",
+    {
+        "Member": MemberTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateNodeInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "NetworkId": str,
         "NodeConfiguration": NodeConfigurationTypeDef,
     },
@@ -1206,7 +1107,15 @@
     total=False,
 )
 
 class CreateNodeInputRequestTypeDef(
     _RequiredCreateNodeInputRequestTypeDef, _OptionalCreateNodeInputRequestTypeDef
 ):
     pass
+
+GetNodeOutputTypeDef = TypedDict(
+    "GetNodeOutputTypeDef",
+    {
+        "Node": NodeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/PKG-INFO` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-managedblockchain
-Version: 1.28.12
-Summary: Type annotations for boto3.ManagedBlockchain 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ManagedBlockchain 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-managedblockchain.svg?color=blue)](https://pypi.org/project/mypy-boto3-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-managedblockchain)](https://pepy.tech/project/mypy-boto3-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedBlockchain 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[boto3.ManagedBlockchain 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [mypy-boto3-managedblockchain docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,108 +334,98 @@
 `mypy_boto3_managedblockchain.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
-    ApprovalThresholdPolicyOutputTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
-    CreateAccessorOutputTypeDef,
-    CreateMemberOutputTypeDef,
-    CreateNetworkOutputTypeDef,
-    CreateNodeOutputTypeDef,
-    CreateProposalOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteAccessorInputRequestTypeDef,
     DeleteMemberInputRequestTypeDef,
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
-    InviteActionOutputTypeDef,
     InviteActionTypeDef,
-    ListAccessorsInputListAccessorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
     ListNodesInputRequestTypeDef,
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
-    PaginatorConfigTypeDef,
-    RemoveActionOutputTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
-    ListAccessorsOutputTypeDef,
-    GetAccessorOutputTypeDef,
-    VotingPolicyOutputTypeDef,
     VotingPolicyTypeDef,
+    CreateAccessorOutputTypeDef,
+    CreateMemberOutputTypeDef,
+    CreateNetworkOutputTypeDef,
+    CreateNodeOutputTypeDef,
+    CreateProposalOutputTypeDef,
+    GetAccessorOutputTypeDef,
+    ListAccessorsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
+    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
-    LogConfigurationsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
     NetworkFrameworkAttributesTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeFrameworkAttributesTypeDef,
     ProposalActionsOutputTypeDef,
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
-    MemberFabricLogPublishingConfigurationOutputTypeDef,
-    NodeFabricLogPublishingConfigurationOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
     ProposalTypeDef,
     CreateProposalInputRequestTypeDef,
-    MemberLogPublishingConfigurationOutputTypeDef,
-    NodeLogPublishingConfigurationOutputTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
-    MemberTypeDef,
-    NodeTypeDef,
     MemberConfigurationTypeDef,
+    MemberTypeDef,
     UpdateMemberInputRequestTypeDef,
     NodeConfigurationTypeDef,
+    NodeTypeDef,
     UpdateNodeInputRequestTypeDef,
-    GetMemberOutputTypeDef,
-    GetNodeOutputTypeDef,
     CreateMemberInputRequestTypeDef,
     CreateNetworkInputRequestTypeDef,
+    GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
+    GetNodeOutputTypeDef,
 )
 
 
 def get_structure() -> AccessorSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-managedblockchain-1.28.12/mypy_boto3_managedblockchain.egg-info/SOURCES.txt` & `mypy-boto3-managedblockchain-1.28.15/mypy_boto3_managedblockchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-managedblockchain-1.28.12/setup.py` & `mypy-boto3-managedblockchain-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-managedblockchain",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_managedblockchain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedBlockchain 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ManagedBlockchain 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

