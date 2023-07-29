# Comparing `tmp/mypy-boto3-wafv2-1.28.15.tar.gz` & `tmp/mypy-boto3-wafv2-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wafv2-1.28.15.tar", last modified: Fri Jul 28 20:43:56 2023, max compression
+gzip compressed data, was "mypy-boto3-wafv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:25 2023, max compression
```

## Comparing `mypy-boto3-wafv2-1.28.15.tar` & `mypy-boto3-wafv2-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.314036 mypy-boto3-wafv2-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-07-28 20:43:56.314036 mypy-boto3-wafv2-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.306036 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-07-28 20:41:19.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-28 20:41:19.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-28 20:41:19.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-07-28 20:41:19.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    87748 2023-07-28 20:41:22.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    87645 2023-07-28 20:41:20.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.314036 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:56.314036 mypy-boto3-wafv2-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.709456 mypy-boto3-wafv2-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-07-29 10:04:25.709456 mypy-boto3-wafv2-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.701456 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37420 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37361 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-29 10:01:28.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    87884 2023-07-29 10:01:35.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87781 2023-07-29 10:01:33.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.709456 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:25.709456 mypy-boto3-wafv2-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-wafv2-1.28.15/LICENSE` & `mypy-boto3-wafv2-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.15/PKG-INFO` & `mypy-boto3-wafv2-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.28.15
-Summary: Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wafv2-1.28.15/README.md` & `mypy-boto3-wafv2-1.28.15.post1/README.md`

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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/__main__.py` & `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFV2 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.WAFV2 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
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

### Comparing `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/client.py` & `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import IPAddressVersionType, PlatformType, ResourceTypeType, ScopeType
 from .type_defs import (
+    AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     CreateWebACLResponseTypeDef,
     CustomResponseBodyTypeDef,
+    DefaultActionOutputTypeDef,
     DefaultActionTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
@@ -56,20 +58,23 @@
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     RegexTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     TagTypeDef,
+    TimeWindowOutputTypeDef,
     TimeWindowTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     VersionToPublishTypeDef,
@@ -141,15 +146,15 @@
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#can_paginate)
         """
 
     def check_capacity(
-        self, *, Scope: ScopeType, Rules: Sequence[RuleTypeDef]
+        self, *, Scope: ScopeType, Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]]
     ) -> CheckCapacityResponseTypeDef:
         """
         Returns the web ACL capacity unit (WCU) requirements for a specified scope and
         set of rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.check_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#check_capacity)
@@ -213,15 +218,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Capacity: int,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates a  RuleGroup per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_rule_group)
@@ -229,24 +234,24 @@
         """
 
     def create_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
-        DefaultAction: DefaultActionTypeDef,
+        DefaultAction: Union[DefaultActionTypeDef, DefaultActionOutputTypeDef],
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef] = ...
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#create_web_acl)
         """
@@ -480,15 +485,15 @@
 
     def get_sampled_requests(
         self,
         *,
         WebAclArn: str,
         RuleMetricName: str,
         Scope: ScopeType,
-        TimeWindow: TimeWindowTypeDef,
+        TimeWindow: Union[TimeWindowTypeDef, TimeWindowOutputTypeDef],
         MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         Gets detailed information about a specified number of requests--a sample--that
         WAF randomly selects from among the first 5,000 requests that your Amazon Web
         Services resource received during a time range that you choose.
 
@@ -639,15 +644,17 @@
         Retrieves an array of  WebACLSummary objects for the web ACLs that you manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_web_acls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#list_web_acls)
         """
 
     def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
+        self,
+        *,
+        LoggingConfiguration: Union[LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef]
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         Enables the specified  LoggingConfiguration, to start logging from a web ACL,
         according to the configuration provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.put_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#put_logging_configuration)
@@ -751,15 +758,15 @@
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_rule_group)
@@ -767,24 +774,24 @@
 
     def update_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
-        DefaultAction: DefaultActionTypeDef,
+        DefaultAction: Union[DefaultActionTypeDef, DefaultActionOutputTypeDef],
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef] = ...
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_web_acl)
         """
```

### Comparing `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/client.pyi` & `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import IPAddressVersionType, PlatformType, ResourceTypeType, ScopeType
 from .type_defs import (
+    AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     CreateWebACLResponseTypeDef,
     CustomResponseBodyTypeDef,
+    DefaultActionOutputTypeDef,
     DefaultActionTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
@@ -56,20 +58,23 @@
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     RegexTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     TagTypeDef,
+    TimeWindowOutputTypeDef,
     TimeWindowTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     VersionToPublishTypeDef,
@@ -135,15 +140,15 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#can_paginate)
         """
     def check_capacity(
-        self, *, Scope: ScopeType, Rules: Sequence[RuleTypeDef]
+        self, *, Scope: ScopeType, Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]]
     ) -> CheckCapacityResponseTypeDef:
         """
         Returns the web ACL capacity unit (WCU) requirements for a specified scope and
         set of rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.check_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#check_capacity)
@@ -202,39 +207,39 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Capacity: int,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates a  RuleGroup per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#create_rule_group)
         """
     def create_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
-        DefaultAction: DefaultActionTypeDef,
+        DefaultAction: Union[DefaultActionTypeDef, DefaultActionOutputTypeDef],
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef] = ...
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#create_web_acl)
         """
@@ -445,15 +450,15 @@
         """
     def get_sampled_requests(
         self,
         *,
         WebAclArn: str,
         RuleMetricName: str,
         Scope: ScopeType,
-        TimeWindow: TimeWindowTypeDef,
+        TimeWindow: Union[TimeWindowTypeDef, TimeWindowOutputTypeDef],
         MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         Gets detailed information about a specified number of requests--a sample--that
         WAF randomly selects from among the first 5,000 requests that your Amazon Web
         Services resource received during a time range that you choose.
 
@@ -589,15 +594,17 @@
         """
         Retrieves an array of  WebACLSummary objects for the web ACLs that you manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_web_acls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#list_web_acls)
         """
     def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
+        self,
+        *,
+        LoggingConfiguration: Union[LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef]
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         Enables the specified  LoggingConfiguration, to start logging from a web ACL,
         according to the configuration provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.put_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#put_logging_configuration)
@@ -693,39 +700,39 @@
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_rule_group)
         """
     def update_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
-        DefaultAction: DefaultActionTypeDef,
+        DefaultAction: Union[DefaultActionTypeDef, DefaultActionOutputTypeDef],
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef] = ...
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_web_acl)
         """
```

### Comparing `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/literals.py` & `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/literals.pyi` & `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/type_defs.py` & `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,22 +350,22 @@
         "Identifier": str,
     },
 )
 
 AndStatementOutputTypeDef = TypedDict(
     "AndStatementOutputTypeDef",
     {
-        "Statements": List["StatementOutputTypeDef"],
+        "Statements": List[Dict[str, Any]],
     },
 )
 
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
-        "Statements": Sequence[Dict[str, Any]],
+        "Statements": Sequence["StatementTypeDef"],
     },
 )
 
 AssociateWebACLRequestRequestTypeDef = TypedDict(
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLArn": str,
@@ -1310,15 +1310,15 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": "StatementTypeDef",
+        "Statement": "StatementOutputTypeDef",
     },
 )
 
 OrStatementOutputTypeDef = TypedDict(
     "OrStatementOutputTypeDef",
     {
         "Statements": List["StatementOutputTypeDef"],
@@ -3084,15 +3084,15 @@
     },
 )
 _OptionalManagedRuleGroupStatementOutputTypeDef = TypedDict(
     "_OptionalManagedRuleGroupStatementOutputTypeDef",
     {
         "Version": str,
         "ExcludedRules": List[ExcludedRuleTypeDef],
-        "ScopeDownStatement": Dict[str, Any],
+        "ScopeDownStatement": "StatementOutputTypeDef",
         "ManagedRuleGroupConfigs": List[ManagedRuleGroupConfigOutputTypeDef],
         "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
     },
     total=False,
 )
 
 
@@ -3175,15 +3175,15 @@
     },
 )
 _OptionalManagedRuleGroupStatementTypeDef = TypedDict(
     "_OptionalManagedRuleGroupStatementTypeDef",
     {
         "Version": str,
         "ExcludedRules": Sequence[ExcludedRuleTypeDef],
-        "ScopeDownStatement": "StatementTypeDef",
+        "ScopeDownStatement": Dict[str, Any],
         "ManagedRuleGroupConfigs": Sequence[ManagedRuleGroupConfigTypeDef],
         "RuleActionOverrides": Sequence[RuleActionOverrideTypeDef],
     },
     total=False,
 )
 
 
@@ -3215,15 +3215,15 @@
     pass
 
 
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
     },
 )
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
@@ -3232,15 +3232,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 
@@ -3259,15 +3259,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
@@ -3291,15 +3291,15 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 
 class UpdateRuleGroupRequestRequestTypeDef(
@@ -3319,15 +3319,15 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
@@ -3359,15 +3359,15 @@
         "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
         "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
         "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
         "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
         "RateBasedStatement": Dict[str, Any],
         "AndStatement": Dict[str, Any],
         "OrStatement": Dict[str, Any],
-        "NotStatement": NotStatementTypeDef,
+        "NotStatement": Dict[str, Any],
         "ManagedRuleGroupStatement": Dict[str, Any],
         "LabelMatchStatement": LabelMatchStatementTypeDef,
         "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
     },
     total=False,
 )
 
@@ -3390,15 +3390,15 @@
         "GeoMatchStatement": GeoMatchStatementTypeDef,
         "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
         "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
         "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
         "RateBasedStatement": Dict[str, Any],
         "AndStatement": Dict[str, Any],
         "OrStatement": Dict[str, Any],
-        "NotStatement": Dict[str, Any],
+        "NotStatement": NotStatementTypeDef,
         "ManagedRuleGroupStatement": Dict[str, Any],
         "LabelMatchStatement": LabelMatchStatementTypeDef,
         "RegexMatchStatement": RegexMatchStatementTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/type_defs.pyi` & `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -349,22 +349,22 @@
         "Identifier": str,
     },
 )
 
 AndStatementOutputTypeDef = TypedDict(
     "AndStatementOutputTypeDef",
     {
-        "Statements": List["StatementOutputTypeDef"],
+        "Statements": List[Dict[str, Any]],
     },
 )
 
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
-        "Statements": Sequence[Dict[str, Any]],
+        "Statements": Sequence["StatementTypeDef"],
     },
 )
 
 AssociateWebACLRequestRequestTypeDef = TypedDict(
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLArn": str,
@@ -1279,15 +1279,15 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": "StatementTypeDef",
+        "Statement": "StatementOutputTypeDef",
     },
 )
 
 OrStatementOutputTypeDef = TypedDict(
     "OrStatementOutputTypeDef",
     {
         "Statements": List["StatementOutputTypeDef"],
@@ -3001,15 +3001,15 @@
     },
 )
 _OptionalManagedRuleGroupStatementOutputTypeDef = TypedDict(
     "_OptionalManagedRuleGroupStatementOutputTypeDef",
     {
         "Version": str,
         "ExcludedRules": List[ExcludedRuleTypeDef],
-        "ScopeDownStatement": Dict[str, Any],
+        "ScopeDownStatement": "StatementOutputTypeDef",
         "ManagedRuleGroupConfigs": List[ManagedRuleGroupConfigOutputTypeDef],
         "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
     },
     total=False,
 )
 
 class ManagedRuleGroupStatementOutputTypeDef(
@@ -3086,15 +3086,15 @@
     },
 )
 _OptionalManagedRuleGroupStatementTypeDef = TypedDict(
     "_OptionalManagedRuleGroupStatementTypeDef",
     {
         "Version": str,
         "ExcludedRules": Sequence[ExcludedRuleTypeDef],
-        "ScopeDownStatement": "StatementTypeDef",
+        "ScopeDownStatement": Dict[str, Any],
         "ManagedRuleGroupConfigs": Sequence[ManagedRuleGroupConfigTypeDef],
         "RuleActionOverrides": Sequence[RuleActionOverrideTypeDef],
     },
     total=False,
 )
 
 class ManagedRuleGroupStatementTypeDef(
@@ -3122,15 +3122,15 @@
 ):
     pass
 
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
     },
 )
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
@@ -3139,15 +3139,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 class CreateRuleGroupRequestRequestTypeDef(
@@ -3164,15 +3164,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
@@ -3194,15 +3194,15 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 class UpdateRuleGroupRequestRequestTypeDef(
     _RequiredUpdateRuleGroupRequestRequestTypeDef, _OptionalUpdateRuleGroupRequestRequestTypeDef
@@ -3220,15 +3220,15 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
@@ -3258,15 +3258,15 @@
         "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
         "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
         "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
         "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
         "RateBasedStatement": Dict[str, Any],
         "AndStatement": Dict[str, Any],
         "OrStatement": Dict[str, Any],
-        "NotStatement": NotStatementTypeDef,
+        "NotStatement": Dict[str, Any],
         "ManagedRuleGroupStatement": Dict[str, Any],
         "LabelMatchStatement": LabelMatchStatementTypeDef,
         "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
     },
     total=False,
 )
 
@@ -3289,15 +3289,15 @@
         "GeoMatchStatement": GeoMatchStatementTypeDef,
         "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
         "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
         "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
         "RateBasedStatement": Dict[str, Any],
         "AndStatement": Dict[str, Any],
         "OrStatement": Dict[str, Any],
-        "NotStatement": Dict[str, Any],
+        "NotStatement": NotStatementTypeDef,
         "ManagedRuleGroupStatement": Dict[str, Any],
         "LabelMatchStatement": LabelMatchStatementTypeDef,
         "RegexMatchStatement": RegexMatchStatementTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/PKG-INFO` & `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.28.15
-Summary: Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/SOURCES.txt` & `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.15/setup.py` & `mypy-boto3-wafv2-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wafv2",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

