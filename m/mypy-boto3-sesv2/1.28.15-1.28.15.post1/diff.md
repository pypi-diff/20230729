# Comparing `tmp/mypy-boto3-sesv2-1.28.15.tar.gz` & `tmp/mypy-boto3-sesv2-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sesv2-1.28.15.tar", last modified: Fri Jul 28 20:43:45 2023, max compression
+gzip compressed data, was "mypy-boto3-sesv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:12 2023, max compression
```

## Comparing `mypy-boto3-sesv2-1.28.15.tar` & `mypy-boto3-sesv2-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.241885 mypy-boto3-sesv2-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21181 2023-07-28 20:43:45.241885 mypy-boto3-sesv2-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.225885 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56738 2023-07-28 20:39:28.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56645 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-28 20:39:28.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-07-28 20:39:28.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70472 2023-07-28 20:39:30.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70402 2023-07-28 20:39:29.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.241885 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21181 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:45.241885 mypy-boto3-sesv2-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.469405 mypy-boto3-sesv2-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21187 2023-07-29 10:04:12.469405 mypy-boto3-sesv2-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.469405 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57068 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56975 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-29 09:59:34.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70597 2023-07-29 09:59:40.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70527 2023-07-29 09:59:34.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.469405 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21187 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:04:12.000000 mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:12.469405 mypy-boto3-sesv2-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:59:33.000000 mypy-boto3-sesv2-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-sesv2-1.28.15/LICENSE` & `mypy-boto3-sesv2-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.15/PKG-INFO` & `mypy-boto3-sesv2-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.28.15
-Summary: Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sesv2-1.28.15/README.md` & `mypy-boto3-sesv2-1.28.15.post1/README.md`

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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/__main__.py` & `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SESV2 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.SESV2 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\nOther"
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

### Comparing `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/client.py` & `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     BulkEmailEntryTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateImportJobResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
     DkimSigningAttributesTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     EmailContentTypeDef,
     EmailTemplateContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
@@ -78,19 +79,21 @@
     ListImportJobsResponseTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
+    ReputationOptionsOutputTypeDef,
     ReputationOptionsTypeDef,
     SendBulkEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
+    SuppressionOptionsOutputTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
     TopicPreferenceTypeDef,
     TopicTypeDef,
     TrackingOptionsTypeDef,
     VdmAttributesTypeDef,
@@ -170,18 +173,18 @@
 
     def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsTypeDef = ...,
+        ReputationOptions: Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef] = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SuppressionOptions: SuppressionOptionsTypeDef = ...,
+        SuppressionOptions: Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef] = ...,
         VdmOptions: VdmOptionsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#create_configuration_set)
@@ -927,15 +930,20 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_warmup_attributes)
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
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/client.pyi` & `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     BulkEmailEntryTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateImportJobResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
     DkimSigningAttributesTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     EmailContentTypeDef,
     EmailTemplateContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
@@ -78,19 +79,21 @@
     ListImportJobsResponseTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
+    ReputationOptionsOutputTypeDef,
     ReputationOptionsTypeDef,
     SendBulkEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
+    SuppressionOptionsOutputTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
     TopicPreferenceTypeDef,
     TopicTypeDef,
     TrackingOptionsTypeDef,
     VdmAttributesTypeDef,
@@ -163,18 +166,18 @@
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
         Tags: Sequence[TagTypeDef] = ...,
-        SuppressionOptions: SuppressionOptionsTypeDef = ...,
+        SuppressionOptions: Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef] = ...,
         VdmOptions: VdmOptionsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#create_configuration_set)
@@ -852,15 +855,20 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_warmup_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_dedicated_ip_warmup_attributes)
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
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/literals.py` & `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/literals.pyi` & `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/type_defs.py` & `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2326,15 +2326,20 @@
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

### Comparing `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/type_defs.pyi` & `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2271,15 +2271,20 @@
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

### Comparing `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/PKG-INFO` & `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.28.15
-Summary: Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/SOURCES.txt` & `mypy-boto3-sesv2-1.28.15.post1/mypy_boto3_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.15/setup.py` & `mypy-boto3-sesv2-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sesv2",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

