# Comparing `tmp/mypy-boto3-pinpoint-email-1.28.15.tar.gz` & `tmp/mypy-boto3-pinpoint-email-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-email-1.28.15.tar", last modified: Fri Jul 28 20:43:27 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-email-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:52 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-email-1.28.15.tar` & `mypy-boto3-pinpoint-email-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.789646 mypy-boto3-pinpoint-email-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-07-28 20:43:27.773645 mypy-boto3-pinpoint-email-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.773645 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-07-28 20:33:25.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32917 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-28 20:33:26.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-28 20:33:26.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-28 20:33:25.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-28 20:33:25.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36033 2023-07-28 20:33:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35999 2023-07-28 20:33:26.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.773645 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:27.789646 mypy-boto3-pinpoint-email-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:52.829336 mypy-boto3-pinpoint-email-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-email-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-29 10:03:52.829336 mypy-boto3-pinpoint-email-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-email-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:52.829336 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33224 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33170 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:18.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36158 2023-07-29 09:53:19.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-07-29 09:53:19.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:52.829336 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:52.000000 mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:52.829336 mypy-boto3-pinpoint-email-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 09:53:17.000000 mypy-boto3-pinpoint-email-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15/LICENSE` & `mypy-boto3-pinpoint-email-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15/PKG-INFO` & `mypy-boto3-pinpoint-email-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-email
-Version: 1.28.15
-Summary: Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15/README.md` & `mypy-boto3-pinpoint-email-1.28.15.post1/README.md`

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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__init__.py` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__init__.pyi` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__main__.py` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PinpointEmail 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.PinpointEmail 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail\nOther"
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

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/client.py` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     ListEmailIdentitiesPaginator,
 )
 from .type_defs import (
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     EmailContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
@@ -49,14 +50,15 @@
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
+    ReputationOptionsOutputTypeDef,
     ReputationOptionsTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
 )
 
@@ -126,15 +128,15 @@
 
     def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsTypeDef = ...,
+        ReputationOptions: Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef] = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set)
@@ -509,15 +511,20 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#put_dedicated_ip_warmup_attributes)
         """
 
     def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
+        SubscribedDomains: Sequence[
+            Union[
+                DomainDeliverabilityTrackingOptionTypeDef,
+                DomainDeliverabilityTrackingOptionOutputTypeDef,
+            ]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard for your Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_deliverability_dashboard_option)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/client.pyi` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     ListEmailIdentitiesPaginator,
 )
 from .type_defs import (
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     EmailContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
@@ -49,14 +50,15 @@
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
+    ReputationOptionsOutputTypeDef,
     ReputationOptionsTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
 )
 
@@ -119,15 +121,15 @@
         """
     def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsTypeDef = ...,
+        ReputationOptions: Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef] = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set)
@@ -467,15 +469,20 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_dedicated_ip_warmup_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#put_dedicated_ip_warmup_attributes)
         """
     def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
+        SubscribedDomains: Sequence[
+            Union[
+                DomainDeliverabilityTrackingOptionTypeDef,
+                DomainDeliverabilityTrackingOptionOutputTypeDef,
+            ]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard for your Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_deliverability_dashboard_option)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/literals.py` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/literals.pyi` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/paginator.py` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/paginator.pyi` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/type_defs.py` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1233,15 +1233,20 @@
     {
         "DashboardEnabled": bool,
     },
 )
 _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
     "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
-        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
+        "SubscribedDomains": Sequence[
+            Union[
+                DomainDeliverabilityTrackingOptionTypeDef,
+                DomainDeliverabilityTrackingOptionOutputTypeDef,
+            ]
+        ],
     },
     total=False,
 )
 
 
 class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
     _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/type_defs.pyi` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1204,15 +1204,20 @@
     {
         "DashboardEnabled": bool,
     },
 )
 _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
     "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
-        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
+        "SubscribedDomains": Sequence[
+            Union[
+                DomainDeliverabilityTrackingOptionTypeDef,
+                DomainDeliverabilityTrackingOptionOutputTypeDef,
+            ]
+        ],
     },
     total=False,
 )
 
 class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
     _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
     _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-email
-Version: 1.28.15
-Summary: Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-email-1.28.15.post1/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.15/setup.py` & `mypy-boto3-pinpoint-email-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint-email",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_pinpoint_email"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder"
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

