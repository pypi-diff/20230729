# Comparing `tmp/mypy-boto3-elbv2-1.28.15.tar.gz` & `tmp/mypy-boto3-elbv2-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elbv2-1.28.15.tar", last modified: Fri Jul 28 20:42:46 2023, max compression
+gzip compressed data, was "mypy-boto3-elbv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:05 2023, max compression
```

## Comparing `mypy-boto3-elbv2-1.28.15.tar` & `mypy-boto3-elbv2-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.469078 mypy-boto3-elbv2-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-07-28 20:42:46.469078 mypy-boto3-elbv2-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.453078 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33888 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33835 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-07-28 20:25:22.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43450 2023-07-28 20:25:23.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43403 2023-07-28 20:25:22.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.469078 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:46.469078 mypy-boto3-elbv2-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.713141 mypy-boto3-elbv2-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-07-29 10:03:05.705141 mypy-boto3-elbv2-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.705141 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34134 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34081 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-07-29 09:44:52.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-29 09:44:52.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43639 2023-07-29 09:44:53.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43592 2023-07-29 09:44:52.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.705141 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:05.000000 mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:05.713141 mypy-boto3-elbv2-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-29 09:44:51.000000 mypy-boto3-elbv2-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-elbv2-1.28.15/LICENSE` & `mypy-boto3-elbv2-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15/PKG-INFO` & `mypy-boto3-elbv2-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.28.15
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elbv2-1.28.15/README.md` & `mypy-boto3-elbv2-1.28.15.post1/README.md`

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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__init__.py` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__init__.pyi` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__main__.py` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.ElasticLoadBalancingv2 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2\nOther"
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

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/client.py` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_elbv2.client import ElasticLoadBalancingv2Client
 
     session = Session()
     client: ElasticLoadBalancingv2Client = session.client("elbv2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     IpAddressTypeType,
     LoadBalancerSchemeEnumType,
     LoadBalancerTypeEnumType,
@@ -32,14 +32,15 @@
     DescribeListenersPaginator,
     DescribeLoadBalancersPaginator,
     DescribeRulesPaginator,
     DescribeSSLPoliciesPaginator,
     DescribeTargetGroupsPaginator,
 )
 from .type_defs import (
+    ActionOutputTypeDef,
     ActionTypeDef,
     AddListenerCertificatesOutputTypeDef,
     CertificateTypeDef,
     CreateListenerOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     CreateRuleOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
@@ -57,14 +58,15 @@
     LoadBalancerAttributeTypeDef,
     MatcherTypeDef,
     ModifyListenerOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
+    RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
     SetSecurityGroupsOutputTypeDef,
     SetSubnetsOutputTypeDef,
     SubnetMappingTypeDef,
@@ -192,15 +194,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#close)
         """
 
     def create_listener(
         self,
         *,
         LoadBalancerArn: str,
-        DefaultActions: Sequence[ActionTypeDef],
+        DefaultActions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
         Protocol: ProtocolEnumType = ...,
         Port: int = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateListenerOutputTypeDef:
@@ -233,17 +235,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#create_load_balancer)
         """
 
     def create_rule(
         self,
         *,
         ListenerArn: str,
-        Conditions: Sequence[RuleConditionTypeDef],
+        Conditions: Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
         Priority: int,
-        Actions: Sequence[ActionTypeDef],
+        Actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateRuleOutputTypeDef:
         """
         Creates a rule for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#create_rule)
@@ -476,15 +478,15 @@
         self,
         *,
         ListenerArn: str,
         Port: int = ...,
         Protocol: ProtocolEnumType = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
-        DefaultActions: Sequence[ActionTypeDef] = ...,
+        DefaultActions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
         AlpnPolicy: Sequence[str] = ...
     ) -> ModifyListenerOutputTypeDef:
         """
         Replaces the specified properties of the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_listener)
@@ -501,16 +503,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_load_balancer_attributes)
         """
 
     def modify_rule(
         self,
         *,
         RuleArn: str,
-        Conditions: Sequence[RuleConditionTypeDef] = ...,
-        Actions: Sequence[ActionTypeDef] = ...
+        Conditions: Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]] = ...,
+        Actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...
     ) -> ModifyRuleOutputTypeDef:
         """
         Replaces the specified properties of the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_rule)
         """
```

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/client.pyi` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_elbv2.client import ElasticLoadBalancingv2Client
 
     session = Session()
     client: ElasticLoadBalancingv2Client = session.client("elbv2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     IpAddressTypeType,
     LoadBalancerSchemeEnumType,
     LoadBalancerTypeEnumType,
@@ -32,14 +32,15 @@
     DescribeListenersPaginator,
     DescribeLoadBalancersPaginator,
     DescribeRulesPaginator,
     DescribeSSLPoliciesPaginator,
     DescribeTargetGroupsPaginator,
 )
 from .type_defs import (
+    ActionOutputTypeDef,
     ActionTypeDef,
     AddListenerCertificatesOutputTypeDef,
     CertificateTypeDef,
     CreateListenerOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     CreateRuleOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
@@ -57,14 +58,15 @@
     LoadBalancerAttributeTypeDef,
     MatcherTypeDef,
     ModifyListenerOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
+    RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
     SetSecurityGroupsOutputTypeDef,
     SetSubnetsOutputTypeDef,
     SubnetMappingTypeDef,
@@ -183,15 +185,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#close)
         """
     def create_listener(
         self,
         *,
         LoadBalancerArn: str,
-        DefaultActions: Sequence[ActionTypeDef],
+        DefaultActions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
         Protocol: ProtocolEnumType = ...,
         Port: int = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateListenerOutputTypeDef:
@@ -222,17 +224,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_load_balancer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#create_load_balancer)
         """
     def create_rule(
         self,
         *,
         ListenerArn: str,
-        Conditions: Sequence[RuleConditionTypeDef],
+        Conditions: Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
         Priority: int,
-        Actions: Sequence[ActionTypeDef],
+        Actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateRuleOutputTypeDef:
         """
         Creates a rule for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#create_rule)
@@ -446,15 +448,15 @@
         self,
         *,
         ListenerArn: str,
         Port: int = ...,
         Protocol: ProtocolEnumType = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
-        DefaultActions: Sequence[ActionTypeDef] = ...,
+        DefaultActions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
         AlpnPolicy: Sequence[str] = ...
     ) -> ModifyListenerOutputTypeDef:
         """
         Replaces the specified properties of the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_listener)
@@ -469,16 +471,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_load_balancer_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_load_balancer_attributes)
         """
     def modify_rule(
         self,
         *,
         RuleArn: str,
-        Conditions: Sequence[RuleConditionTypeDef] = ...,
-        Actions: Sequence[ActionTypeDef] = ...
+        Conditions: Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]] = ...,
+        Actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...
     ) -> ModifyRuleOutputTypeDef:
         """
         Replaces the specified properties of the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/client/#modify_rule)
         """
```

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/literals.py` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/literals.pyi` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/paginator.py` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/paginator.pyi` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/type_defs.py` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_elbv2.type_defs import AuthenticateCognitoActionConfigOutputTypeDef
 
     data: AuthenticateCognitoActionConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ActionTypeEnumType,
     AuthenticateCognitoActionConditionalBehaviorEnumType,
     AuthenticateOidcActionConditionalBehaviorEnumType,
     IpAddressTypeType,
     LoadBalancerSchemeEnumType,
@@ -1501,15 +1501,15 @@
     total=False,
 )
 
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
-        "DefaultActions": Sequence[ActionTypeDef],
+        "DefaultActions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
     },
 )
 _OptionalCreateListenerInputRequestTypeDef = TypedDict(
     "_OptionalCreateListenerInputRequestTypeDef",
     {
         "Protocol": ProtocolEnumType,
         "Port": int,
@@ -1537,15 +1537,15 @@
 _OptionalModifyListenerInputRequestTypeDef = TypedDict(
     "_OptionalModifyListenerInputRequestTypeDef",
     {
         "Port": int,
         "Protocol": ProtocolEnumType,
         "SslPolicy": str,
         "Certificates": Sequence[CertificateTypeDef],
-        "DefaultActions": Sequence[ActionTypeDef],
+        "DefaultActions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
 
 class ModifyListenerInputRequestTypeDef(
@@ -1566,17 +1566,17 @@
     total=False,
 )
 
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
-        "Conditions": Sequence[RuleConditionTypeDef],
+        "Conditions": Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
         "Priority": int,
-        "Actions": Sequence[ActionTypeDef],
+        "Actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
     },
 )
 _OptionalCreateRuleInputRequestTypeDef = TypedDict(
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
@@ -1595,16 +1595,16 @@
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
     "_OptionalModifyRuleInputRequestTypeDef",
     {
-        "Conditions": Sequence[RuleConditionTypeDef],
-        "Actions": Sequence[ActionTypeDef],
+        "Conditions": Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
+        "Actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
     },
     total=False,
 )
 
 
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
```

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/type_defs.pyi` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_elbv2.type_defs import AuthenticateCognitoActionConfigOutputTypeDef
 
     data: AuthenticateCognitoActionConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ActionTypeEnumType,
     AuthenticateCognitoActionConditionalBehaviorEnumType,
     AuthenticateOidcActionConditionalBehaviorEnumType,
     IpAddressTypeType,
     LoadBalancerSchemeEnumType,
@@ -1462,15 +1462,15 @@
     total=False,
 )
 
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
-        "DefaultActions": Sequence[ActionTypeDef],
+        "DefaultActions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
     },
 )
 _OptionalCreateListenerInputRequestTypeDef = TypedDict(
     "_OptionalCreateListenerInputRequestTypeDef",
     {
         "Protocol": ProtocolEnumType,
         "Port": int,
@@ -1496,15 +1496,15 @@
 _OptionalModifyListenerInputRequestTypeDef = TypedDict(
     "_OptionalModifyListenerInputRequestTypeDef",
     {
         "Port": int,
         "Protocol": ProtocolEnumType,
         "SslPolicy": str,
         "Certificates": Sequence[CertificateTypeDef],
-        "DefaultActions": Sequence[ActionTypeDef],
+        "DefaultActions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
@@ -1523,17 +1523,17 @@
     total=False,
 )
 
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
-        "Conditions": Sequence[RuleConditionTypeDef],
+        "Conditions": Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
         "Priority": int,
-        "Actions": Sequence[ActionTypeDef],
+        "Actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
     },
 )
 _OptionalCreateRuleInputRequestTypeDef = TypedDict(
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
@@ -1550,16 +1550,16 @@
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
     "_OptionalModifyRuleInputRequestTypeDef",
     {
-        "Conditions": Sequence[RuleConditionTypeDef],
-        "Actions": Sequence[ActionTypeDef],
+        "Conditions": Sequence[Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]],
+        "Actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
     },
     total=False,
 )
 
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
```

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/waiter.py` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/waiter.pyi` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/PKG-INFO` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.28.15
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/SOURCES.txt` & `mypy-boto3-elbv2-1.28.15.post1/mypy_boto3_elbv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.15/setup.py` & `mypy-boto3-elbv2-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elbv2",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_elbv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with"
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

