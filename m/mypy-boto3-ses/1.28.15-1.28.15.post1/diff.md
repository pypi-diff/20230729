# Comparing `tmp/mypy-boto3-ses-1.28.15.tar.gz` & `tmp/mypy-boto3-ses-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ses-1.28.15.tar", last modified: Fri Jul 28 20:43:44 2023, max compression
+gzip compressed data, was "mypy-boto3-ses-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:12 2023, max compression
```

## Comparing `mypy-boto3-ses-1.28.15.tar` & `mypy-boto3-ses-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.829879 mypy-boto3-ses-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-07-28 20:43:44.829879 mypy-boto3-ses-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.829879 mypy-boto3-ses-1.28.15/mypy_boto3_ses/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49195 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49111 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49427 2023-07-28 20:39:23.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49360 2023-07-28 20:39:22.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.829879 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:44.829879 mypy-boto3-ses-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.373404 mypy-boto3-ses-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20529 2023-07-29 10:04:12.365404 mypy-boto3-ses-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.365404 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49503 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49419 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-07-29 09:59:31.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-29 09:59:31.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49427 2023-07-29 09:59:32.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49360 2023-07-29 09:59:31.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.365404 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20529 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:12.373404 mypy-boto3-ses-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-ses-1.28.15/LICENSE` & `mypy-boto3-ses-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/PKG-INFO` & `mypy-boto3-ses-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ses
-Version: 1.28.15
-Summary: Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ses-1.28.15/README.md` & `mypy-boto3-ses-1.28.15.post1/README.md`

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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/__init__.py` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/__init__.pyi` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/__main__.py` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SES 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.SES 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES\nOther"
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

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/client.py` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ses.client import SESClient
 
     session = Session()
     client: SESClient = session.client("ses")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BehaviorOnMXFailureType,
     ConfigurationSetAttributeType,
     IdentityTypeType,
@@ -38,14 +38,15 @@
     DeliveryOptionsTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
+    EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
@@ -62,14 +63,15 @@
     ListTemplatesResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     MessageDsnTypeDef,
     MessageTagTypeDef,
     MessageTypeDef,
     RawMessageTypeDef,
     ReceiptFilterTypeDef,
+    ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
     SendBounceResponseTypeDef,
     SendBulkTemplatedEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
@@ -186,15 +188,18 @@
         Creates a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_configuration_set)
         """
 
     def create_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
+        self,
+        *,
+        ConfigurationSetName: str,
+        EventDestination: Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Creates a configuration set event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_configuration_set_event_destination)
         """
@@ -232,15 +237,19 @@
         Creates a new IP address filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_receipt_filter)
         """
 
     def create_receipt_rule(
-        self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef, After: str = ...
+        self,
+        *,
+        RuleSetName: str,
+        Rule: Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef],
+        After: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_receipt_rule)
         """
@@ -830,15 +839,18 @@
         current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_account_sending_enabled)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_account_sending_enabled)
         """
 
     def update_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
+        self,
+        *,
+        ConfigurationSetName: str,
+        EventDestination: Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates the event destination of a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_configuration_set_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_configuration_set_event_destination)
         """
@@ -889,15 +901,17 @@
         """
         Updates an existing custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_custom_verification_email_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_custom_verification_email_template)
         """
 
-    def update_receipt_rule(self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef) -> Dict[str, Any]:
+    def update_receipt_rule(
+        self, *, RuleSetName: str, Rule: Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef]
+    ) -> Dict[str, Any]:
         """
         Updates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_receipt_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_receipt_rule)
         """
```

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/client.pyi` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ses.client import SESClient
 
     session = Session()
     client: SESClient = session.client("ses")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BehaviorOnMXFailureType,
     ConfigurationSetAttributeType,
     IdentityTypeType,
@@ -38,14 +38,15 @@
     DeliveryOptionsTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
+    EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
@@ -62,14 +63,15 @@
     ListTemplatesResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     MessageDsnTypeDef,
     MessageTagTypeDef,
     MessageTypeDef,
     RawMessageTypeDef,
     ReceiptFilterTypeDef,
+    ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
     SendBounceResponseTypeDef,
     SendBulkTemplatedEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
@@ -177,15 +179,18 @@
         """
         Creates a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_configuration_set)
         """
     def create_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
+        self,
+        *,
+        ConfigurationSetName: str,
+        EventDestination: Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Creates a configuration set event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_configuration_set_event_destination)
         """
@@ -219,15 +224,19 @@
         """
         Creates a new IP address filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_receipt_filter)
         """
     def create_receipt_rule(
-        self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef, After: str = ...
+        self,
+        *,
+        RuleSetName: str,
+        Rule: Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef],
+        After: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_receipt_rule)
         """
@@ -762,15 +771,18 @@
         Enables or disables email sending across your entire Amazon SES account in the
         current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_account_sending_enabled)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_account_sending_enabled)
         """
     def update_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
+        self,
+        *,
+        ConfigurationSetName: str,
+        EventDestination: Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates the event destination of a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_configuration_set_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_configuration_set_event_destination)
         """
@@ -816,15 +828,17 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_custom_verification_email_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_custom_verification_email_template)
         """
-    def update_receipt_rule(self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef) -> Dict[str, Any]:
+    def update_receipt_rule(
+        self, *, RuleSetName: str, Rule: Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef]
+    ) -> Dict[str, Any]:
         """
         Updates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_receipt_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_receipt_rule)
         """
     def update_template(self, *, Template: TemplateTypeDef) -> Dict[str, Any]:
```

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/literals.py` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/literals.pyi` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/paginator.py` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/paginator.pyi` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/type_defs.py` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/type_defs.pyi` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/waiter.py` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses/waiter.pyi` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/PKG-INFO` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ses
-Version: 1.28.15
-Summary: Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/SOURCES.txt` & `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15/setup.py` & `mypy-boto3-ses-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ses",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_ses"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

