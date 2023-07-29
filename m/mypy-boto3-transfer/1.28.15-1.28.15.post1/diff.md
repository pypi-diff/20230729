# Comparing `tmp/mypy-boto3-transfer-1.28.15.tar.gz` & `tmp/mypy-boto3-transfer-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transfer-1.28.15.tar", last modified: Fri Jul 28 20:43:53 2023, max compression
+gzip compressed data, was "mypy-boto3-transfer-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:22 2023, max compression
```

## Comparing `mypy-boto3-transfer-1.28.15.tar` & `mypy-boto3-transfer-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.898003 mypy-boto3-transfer-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-28 20:43:53.898003 mypy-boto3-transfer-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.890003 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47079 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47000 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62680 2023-07-28 20:40:51.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62587 2023-07-28 20:40:50.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.898003 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:53.898003 mypy-boto3-transfer-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.825446 mypy-boto3-transfer-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21979 2023-07-29 10:04:22.821445 mypy-boto3-transfer-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.813445 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47789 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47710 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62748 2023-07-29 10:01:03.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62655 2023-07-29 10:00:58.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.821445 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21979 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:22.825446 mypy-boto3-transfer-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-transfer-1.28.15/LICENSE` & `mypy-boto3-transfer-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15/PKG-INFO` & `mypy-boto3-transfer-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.28.15
-Summary: Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transfer-1.28.15/README.md` & `mypy-boto3-transfer-1.28.15.post1/README.md`

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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__init__.py` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__init__.pyi` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__main__.py` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Transfer 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Transfer 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
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

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/client.py` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeWorkflowResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     HomeDirectoryMapEntryTypeDef,
     IdentityProviderDetailsTypeDef,
     ImportCertificateResponseTypeDef,
     ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyResponseTypeDef,
     ListAccessesResponseTypeDef,
@@ -78,30 +79,35 @@
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
     ListServersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
+    PosixProfileOutputTypeDef,
     PosixProfileTypeDef,
+    ProtocolDetailsOutputTypeDef,
     ProtocolDetailsTypeDef,
+    SftpConnectorConfigOutputTypeDef,
     SftpConnectorConfigTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
     TestConnectionResponseTypeDef,
     TestIdentityProviderResponseTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
     UpdateCertificateResponseTypeDef,
     UpdateConnectorResponseTypeDef,
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
+    WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
+    WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
 )
 from .waiter import ServerOfflineWaiter, ServerOnlineWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -171,15 +177,15 @@
         Role: str,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...
+        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...
     ) -> CreateAccessResponseTypeDef:
         """
         Used by administrators to choose which groups in the directory should have
         access to upload and download files over the enabled protocols using Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_access)
@@ -209,15 +215,15 @@
         self,
         *,
         Url: str,
         AccessRole: str,
         As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SftpConfig: SftpConnectorConfigTypeDef = ...
+        SftpConfig: Union[SftpConnectorConfigTypeDef, SftpConnectorConfigOutputTypeDef] = ...
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for an outbound connection
         for the AS2 or SFTP protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_connector)
@@ -239,27 +245,27 @@
         """
 
     def create_server(
         self,
         *,
         Certificate: str = ...,
         Domain: DomainType = ...,
-        EndpointDetails: EndpointDetailsTypeDef = ...,
+        EndpointDetails: Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef] = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         IdentityProviderType: IdentityProviderTypeType = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
-        ProtocolDetails: ProtocolDetailsTypeDef = ...,
+        ProtocolDetails: Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef] = ...,
         SecurityPolicyName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        WorkflowDetails: WorkflowDetailsTypeDef = ...,
+        WorkflowDetails: Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef] = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> CreateServerResponseTypeDef:
         """
         Instantiates an auto-scaling virtual server based on the selected file transfer
         protocol in Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_server)
@@ -272,32 +278,32 @@
         Role: str,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
         SshPublicKeyBody: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user and associates them with an existing file transfer protocol-
         enabled server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_user)
         """
 
     def create_workflow(
         self,
         *,
-        Steps: Sequence[WorkflowStepTypeDef],
+        Steps: Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
         Description: str = ...,
-        OnExceptionSteps: Sequence[WorkflowStepTypeDef] = ...,
+        OnExceptionSteps: Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWorkflowResponseTypeDef:
         """
         Allows you to create a workflow with specified steps and step details the
         workflow invokes after file transfer completes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_workflow)
@@ -773,15 +779,15 @@
         *,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
         Role: str = ...
     ) -> UpdateAccessResponseTypeDef:
         """
         Allows you to update parameters for the access specified in the `ServerID` and
         `ExternalID` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_access)
@@ -826,15 +832,15 @@
         self,
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
         LoggingRole: str = ...,
-        SftpConfig: SftpConnectorConfigTypeDef = ...
+        SftpConfig: Union[SftpConnectorConfigTypeDef, SftpConnectorConfigOutputTypeDef] = ...
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_connector)
         """
@@ -861,25 +867,25 @@
         """
 
     def update_server(
         self,
         *,
         ServerId: str,
         Certificate: str = ...,
-        ProtocolDetails: ProtocolDetailsTypeDef = ...,
-        EndpointDetails: EndpointDetailsTypeDef = ...,
+        ProtocolDetails: Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef] = ...,
+        EndpointDetails: Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef] = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         SecurityPolicyName: str = ...,
-        WorkflowDetails: WorkflowDetailsTypeDef = ...,
+        WorkflowDetails: Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef] = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> UpdateServerResponseTypeDef:
         """
         Updates the file transfer protocol-enabled server's properties after that server
         has been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_server)
@@ -891,15 +897,15 @@
         *,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
         Role: str = ...
     ) -> UpdateUserResponseTypeDef:
         """
         Assigns new properties to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_user)
```

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/client.pyi` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeWorkflowResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     HomeDirectoryMapEntryTypeDef,
     IdentityProviderDetailsTypeDef,
     ImportCertificateResponseTypeDef,
     ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyResponseTypeDef,
     ListAccessesResponseTypeDef,
@@ -78,30 +79,35 @@
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
     ListServersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
+    PosixProfileOutputTypeDef,
     PosixProfileTypeDef,
+    ProtocolDetailsOutputTypeDef,
     ProtocolDetailsTypeDef,
+    SftpConnectorConfigOutputTypeDef,
     SftpConnectorConfigTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
     TestConnectionResponseTypeDef,
     TestIdentityProviderResponseTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
     UpdateCertificateResponseTypeDef,
     UpdateConnectorResponseTypeDef,
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
+    WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
+    WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
 )
 from .waiter import ServerOfflineWaiter, ServerOnlineWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -164,15 +170,15 @@
         Role: str,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...
+        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...
     ) -> CreateAccessResponseTypeDef:
         """
         Used by administrators to choose which groups in the directory should have
         access to upload and download files over the enabled protocols using Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_access)
@@ -200,15 +206,15 @@
         self,
         *,
         Url: str,
         AccessRole: str,
         As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SftpConfig: SftpConnectorConfigTypeDef = ...
+        SftpConfig: Union[SftpConnectorConfigTypeDef, SftpConnectorConfigOutputTypeDef] = ...
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for an outbound connection
         for the AS2 or SFTP protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_connector)
@@ -228,27 +234,27 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_profile)
         """
     def create_server(
         self,
         *,
         Certificate: str = ...,
         Domain: DomainType = ...,
-        EndpointDetails: EndpointDetailsTypeDef = ...,
+        EndpointDetails: Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef] = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         IdentityProviderType: IdentityProviderTypeType = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
-        ProtocolDetails: ProtocolDetailsTypeDef = ...,
+        ProtocolDetails: Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef] = ...,
         SecurityPolicyName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        WorkflowDetails: WorkflowDetailsTypeDef = ...,
+        WorkflowDetails: Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef] = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> CreateServerResponseTypeDef:
         """
         Instantiates an auto-scaling virtual server based on the selected file transfer
         protocol in Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_server)
@@ -260,31 +266,31 @@
         Role: str,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
         SshPublicKeyBody: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user and associates them with an existing file transfer protocol-
         enabled server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_user)
         """
     def create_workflow(
         self,
         *,
-        Steps: Sequence[WorkflowStepTypeDef],
+        Steps: Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
         Description: str = ...,
-        OnExceptionSteps: Sequence[WorkflowStepTypeDef] = ...,
+        OnExceptionSteps: Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWorkflowResponseTypeDef:
         """
         Allows you to create a workflow with specified steps and step details the
         workflow invokes after file transfer completes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_workflow)
@@ -714,15 +720,15 @@
         *,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
         Role: str = ...
     ) -> UpdateAccessResponseTypeDef:
         """
         Allows you to update parameters for the access specified in the `ServerID` and
         `ExternalID` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_access)
@@ -764,15 +770,15 @@
         self,
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
         LoggingRole: str = ...,
-        SftpConfig: SftpConnectorConfigTypeDef = ...
+        SftpConfig: Union[SftpConnectorConfigTypeDef, SftpConnectorConfigOutputTypeDef] = ...
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_connector)
         """
@@ -796,25 +802,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_profile)
         """
     def update_server(
         self,
         *,
         ServerId: str,
         Certificate: str = ...,
-        ProtocolDetails: ProtocolDetailsTypeDef = ...,
-        EndpointDetails: EndpointDetailsTypeDef = ...,
+        ProtocolDetails: Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef] = ...,
+        EndpointDetails: Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef] = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         SecurityPolicyName: str = ...,
-        WorkflowDetails: WorkflowDetailsTypeDef = ...,
+        WorkflowDetails: Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef] = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> UpdateServerResponseTypeDef:
         """
         Updates the file transfer protocol-enabled server's properties after that server
         has been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_server)
@@ -825,15 +831,15 @@
         *,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
         Role: str = ...
     ) -> UpdateUserResponseTypeDef:
         """
         Assigns new properties to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_user)
```

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/literals.py` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/literals.pyi` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/paginator.py` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/paginator.pyi` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/type_defs.py` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2531,22 +2531,22 @@
 ):
     pass
 
 
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
-        "Steps": Sequence[WorkflowStepTypeDef],
+        "Steps": Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWorkflowRequestRequestTypeDef",
     {
         "Description": str,
-        "OnExceptionSteps": Sequence[WorkflowStepTypeDef],
+        "OnExceptionSteps": Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class CreateWorkflowRequestRequestTypeDef(
```

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/type_defs.pyi` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2440,22 +2440,22 @@
     _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
 ):
     pass
 
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
-        "Steps": Sequence[WorkflowStepTypeDef],
+        "Steps": Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWorkflowRequestRequestTypeDef",
     {
         "Description": str,
-        "OnExceptionSteps": Sequence[WorkflowStepTypeDef],
+        "OnExceptionSteps": Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
```

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/waiter.py` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/waiter.pyi` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/PKG-INFO` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.28.15
-Summary: Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/SOURCES.txt` & `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15/setup.py` & `mypy-boto3-transfer-1.28.15.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transfer",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder"
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

