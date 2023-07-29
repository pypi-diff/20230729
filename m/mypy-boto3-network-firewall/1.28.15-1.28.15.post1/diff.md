# Comparing `tmp/mypy-boto3-network-firewall-1.28.15.tar.gz` & `tmp/mypy-boto3-network-firewall-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-network-firewall-1.28.15.tar", last modified: Fri Jul 28 20:43:21 2023, max compression
+gzip compressed data, was "mypy-boto3-network-firewall-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:46 2023, max compression
```

## Comparing `mypy-boto3-network-firewall-1.28.15.tar` & `mypy-boto3-network-firewall-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.797563 mypy-boto3-network-firewall-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-07-28 20:43:21.793563 mypy-boto3-network-firewall-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18743 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.793563 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32089 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32041 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55242 2023-07-28 20:32:28.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55176 2023-07-28 20:32:27.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.793563 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:21.797563 mypy-boto3-network-firewall-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:46.249309 mypy-boto3-network-firewall-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-07-29 10:03:46.237309 mypy-boto3-network-firewall-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18743 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:46.229309 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32579 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55242 2023-07-29 09:52:07.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55176 2023-07-29 09:52:06.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:46.237309 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-07-29 10:03:45.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:03:46.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:45.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:45.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:45.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:03:45.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:46.249309 mypy-boto3-network-firewall-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 09:52:04.000000 mypy-boto3-network-firewall-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-network-firewall-1.28.15/LICENSE` & `mypy-boto3-network-firewall-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15/PKG-INFO` & `mypy-boto3-network-firewall-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.28.15
-Summary: Type annotations for boto3.NetworkFirewall 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.NetworkFirewall 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-network-firewall-1.28.15/README.md` & `mypy-boto3-network-firewall-1.28.15.post1/README.md`

 * *Files 1% similar despite different names*

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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__init__.py` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__init__.pyi` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__main__.py` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.NetworkFirewall 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.NetworkFirewall 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall\nOther"
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

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/client.py` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_network_firewall.client import NetworkFirewallClient
 
     session = Session()
     client: NetworkFirewallClient = session.client("network-firewall")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ResourceManagedStatusType, ResourceManagedTypeType, RuleGroupTypeType
 from .paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
@@ -42,25 +42,29 @@
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     DescribeRuleGroupResponseTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     EncryptionConfigurationTypeDef,
+    FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
+    RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
     SourceMetadataTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
+    TLSInspectionConfigurationOutputTypeDef,
     TLSInspectionConfigurationTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
@@ -187,15 +191,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_firewall)
         """
 
     def create_firewall_policy(
         self,
         *,
         FirewallPolicyName: str,
-        FirewallPolicy: FirewallPolicyTypeDef,
+        FirewallPolicy: Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef],
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
@@ -206,15 +210,15 @@
 
     def create_rule_group(
         self,
         *,
         RuleGroupName: str,
         Type: RuleGroupTypeType,
         Capacity: int,
-        RuleGroup: RuleGroupTypeDef = ...,
+        RuleGroup: Union[RuleGroupTypeDef, RuleGroupOutputTypeDef] = ...,
         Rules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> CreateRuleGroupResponseTypeDef:
@@ -226,15 +230,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_rule_group)
         """
 
     def create_tls_inspection_configuration(
         self,
         *,
         TLSInspectionConfigurationName: str,
-        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        TLSInspectionConfiguration: Union[
+            TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
+        ],
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateTLSInspectionConfigurationResponseTypeDef:
         """
         Creates an Network Firewall TLS inspection configuration.
 
@@ -517,15 +523,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_encryption_configuration)
         """
 
     def update_firewall_policy(
         self,
         *,
         UpdateToken: str,
-        FirewallPolicy: FirewallPolicyTypeDef,
+        FirewallPolicy: Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef],
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
@@ -552,30 +558,32 @@
         """
 
     def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        LoggingConfiguration: LoggingConfigurationTypeDef = ...
+        LoggingConfiguration: Union[
+            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+        ] = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_logging_configuration)
         """
 
     def update_rule_group(
         self,
         *,
         UpdateToken: str,
         RuleGroupArn: str = ...,
         RuleGroupName: str = ...,
-        RuleGroup: RuleGroupTypeDef = ...,
+        RuleGroup: Union[RuleGroupTypeDef, RuleGroupOutputTypeDef] = ...,
         Rules: str = ...,
         Type: RuleGroupTypeType = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> UpdateRuleGroupResponseTypeDef:
@@ -602,15 +610,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_subnet_change_protection)
         """
 
     def update_tls_inspection_configuration(
         self,
         *,
-        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        TLSInspectionConfiguration: Union[
+            TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
+        ],
         UpdateToken: str,
         TLSInspectionConfigurationArn: str = ...,
         TLSInspectionConfigurationName: str = ...,
         Description: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
         """
```

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/client.pyi` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_network_firewall.client import NetworkFirewallClient
 
     session = Session()
     client: NetworkFirewallClient = session.client("network-firewall")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ResourceManagedStatusType, ResourceManagedTypeType, RuleGroupTypeType
 from .paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
@@ -42,25 +42,29 @@
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     DescribeRuleGroupResponseTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     EncryptionConfigurationTypeDef,
+    FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
+    RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
     SourceMetadataTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
+    TLSInspectionConfigurationOutputTypeDef,
     TLSInspectionConfigurationTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
@@ -177,15 +181,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_firewall)
         """
     def create_firewall_policy(
         self,
         *,
         FirewallPolicyName: str,
-        FirewallPolicy: FirewallPolicyTypeDef,
+        FirewallPolicy: Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef],
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
@@ -195,15 +199,15 @@
         """
     def create_rule_group(
         self,
         *,
         RuleGroupName: str,
         Type: RuleGroupTypeType,
         Capacity: int,
-        RuleGroup: RuleGroupTypeDef = ...,
+        RuleGroup: Union[RuleGroupTypeDef, RuleGroupOutputTypeDef] = ...,
         Rules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> CreateRuleGroupResponseTypeDef:
@@ -214,15 +218,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_rule_group)
         """
     def create_tls_inspection_configuration(
         self,
         *,
         TLSInspectionConfigurationName: str,
-        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        TLSInspectionConfiguration: Union[
+            TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
+        ],
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateTLSInspectionConfigurationResponseTypeDef:
         """
         Creates an Network Firewall TLS inspection configuration.
 
@@ -479,15 +485,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_encryption_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_encryption_configuration)
         """
     def update_firewall_policy(
         self,
         *,
         UpdateToken: str,
-        FirewallPolicy: FirewallPolicyTypeDef,
+        FirewallPolicy: Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef],
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
@@ -512,29 +518,31 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_policy_change_protection)
         """
     def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        LoggingConfiguration: LoggingConfigurationTypeDef = ...
+        LoggingConfiguration: Union[
+            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+        ] = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_logging_configuration)
         """
     def update_rule_group(
         self,
         *,
         UpdateToken: str,
         RuleGroupArn: str = ...,
         RuleGroupName: str = ...,
-        RuleGroup: RuleGroupTypeDef = ...,
+        RuleGroup: Union[RuleGroupTypeDef, RuleGroupOutputTypeDef] = ...,
         Rules: str = ...,
         Type: RuleGroupTypeType = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> UpdateRuleGroupResponseTypeDef:
@@ -559,15 +567,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_subnet_change_protection)
         """
     def update_tls_inspection_configuration(
         self,
         *,
-        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        TLSInspectionConfiguration: Union[
+            TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
+        ],
         UpdateToken: str,
         TLSInspectionConfigurationArn: str = ...,
         TLSInspectionConfigurationName: str = ...,
         Description: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
         """
```

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/literals.py` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/literals.pyi` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/paginator.py` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/paginator.pyi` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/type_defs.py` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/type_defs.pyi` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/PKG-INFO` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.28.15
-Summary: Type annotations for boto3.NetworkFirewall 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.NetworkFirewall 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/SOURCES.txt` & `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15/setup.py` & `mypy-boto3-network-firewall-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-network-firewall",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_network_firewall"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.NetworkFirewall 1.28.15 service generated with"
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

