# Comparing `tmp/mypy-boto3-customer-profiles-1.28.15.tar.gz` & `tmp/mypy-boto3-customer-profiles-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-customer-profiles-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
+gzip compressed data, was "mypy-boto3-customer-profiles-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:54 2023, max compression
```

## Comparing `mypy-boto3-customer-profiles-1.28.15.tar` & `mypy-boto3-customer-profiles-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.880915 mypy-boto3-customer-profiles-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-28 20:42:34.872915 mypy-boto3-customer-profiles-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18819 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.860915 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40360 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40301 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-28 20:22:25.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-28 20:22:25.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69309 2023-07-28 20:22:27.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69209 2023-07-28 20:22:26.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.872915 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.880915 mypy-boto3-customer-profiles-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.341096 mypy-boto3-customer-profiles-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20351 2023-07-29 10:02:54.329096 mypy-boto3-customer-profiles-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18819 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.317096 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40567 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40508 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-29 09:41:51.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-29 09:41:51.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-29 09:41:51.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69344 2023-07-29 09:41:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69244 2023-07-29 09:41:53.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.329096 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20351 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:54.341096 mypy-boto3-customer-profiles-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-customer-profiles-1.28.15/LICENSE` & `mypy-boto3-customer-profiles-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15/PKG-INFO` & `mypy-boto3-customer-profiles-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.28.15
-Summary: Type annotations for boto3.CustomerProfiles 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CustomerProfiles 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-customer-profiles-1.28.15/README.md` & `mypy-boto3-customer-profiles-1.28.15.post1/README.md`

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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__init__.py` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__init__.pyi` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__main__.py` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CustomerProfiles 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.CustomerProfiles 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
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

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/client.py` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,19 @@
     logicalOperatorType,
 )
 from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
+    AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
     ConditionsTypeDef,
     ConflictResolutionTypeDef,
+    ConsolidationOutputTypeDef,
     ConsolidationTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEventStreamResponseTypeDef,
     CreateIntegrationWorkflowResponseTypeDef,
     CreateProfileResponseTypeDef,
     DeleteDomainResponseTypeDef,
@@ -76,14 +78,15 @@
     ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     MatchingRequestTypeDef,
     MergeProfilesResponseTypeDef,
     ObjectFilterTypeDef,
     ObjectTypeFieldTypeDef,
+    ObjectTypeKeyOutputTypeDef,
     ObjectTypeKeyTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     RuleBasedMatchingRequestTypeDef,
     SearchProfilesResponseTypeDef,
     UpdateAddressTypeDef,
@@ -163,15 +166,15 @@
         """
 
     def create_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
-        AttributeDetails: AttributeDetailsTypeDef,
+        AttributeDetails: Union[AttributeDetailsTypeDef, AttributeDetailsOutputTypeDef],
         Statistic: StatisticType,
         DisplayName: str = ...,
         Description: str = ...,
         Conditions: ConditionsTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
         """
@@ -359,15 +362,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#generate_presigned_url)
         """
 
     def get_auto_merging_preview(
         self,
         *,
         DomainName: str,
-        Consolidation: ConsolidationTypeDef,
+        Consolidation: Union[ConsolidationTypeDef, ConsolidationOutputTypeDef],
         ConflictResolution: ConflictResolutionTypeDef,
         MinAllowedConfidenceScoreForMerging: float = ...
     ) -> GetAutoMergingPreviewResponseTypeDef:
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your data.
 
@@ -705,15 +708,15 @@
         Description: str,
         TemplateId: str = ...,
         ExpirationDays: int = ...,
         EncryptionKey: str = ...,
         AllowProfileCreation: bool = ...,
         SourceLastUpdatedTimestampFormat: str = ...,
         Fields: Mapping[str, ObjectTypeFieldTypeDef] = ...,
-        Keys: Mapping[str, Sequence[ObjectTypeKeyTypeDef]] = ...,
+        Keys: Mapping[str, Sequence[Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]]] = ...,
         Tags: Mapping[str, str] = ...
     ) -> PutProfileObjectTypeResponseTypeDef:
         """
         Defines a ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#put_profile_object_type)
```

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/client.pyi` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,19 @@
     logicalOperatorType,
 )
 from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
+    AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
     ConditionsTypeDef,
     ConflictResolutionTypeDef,
+    ConsolidationOutputTypeDef,
     ConsolidationTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEventStreamResponseTypeDef,
     CreateIntegrationWorkflowResponseTypeDef,
     CreateProfileResponseTypeDef,
     DeleteDomainResponseTypeDef,
@@ -76,14 +78,15 @@
     ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     MatchingRequestTypeDef,
     MergeProfilesResponseTypeDef,
     ObjectFilterTypeDef,
     ObjectTypeFieldTypeDef,
+    ObjectTypeKeyOutputTypeDef,
     ObjectTypeKeyTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     RuleBasedMatchingRequestTypeDef,
     SearchProfilesResponseTypeDef,
     UpdateAddressTypeDef,
@@ -155,15 +158,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#close)
         """
     def create_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
-        AttributeDetails: AttributeDetailsTypeDef,
+        AttributeDetails: Union[AttributeDetailsTypeDef, AttributeDetailsOutputTypeDef],
         Statistic: StatisticType,
         DisplayName: str = ...,
         Description: str = ...,
         Conditions: ConditionsTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
         """
@@ -336,15 +339,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#generate_presigned_url)
         """
     def get_auto_merging_preview(
         self,
         *,
         DomainName: str,
-        Consolidation: ConsolidationTypeDef,
+        Consolidation: Union[ConsolidationTypeDef, ConsolidationOutputTypeDef],
         ConflictResolution: ConflictResolutionTypeDef,
         MinAllowedConfidenceScoreForMerging: float = ...
     ) -> GetAutoMergingPreviewResponseTypeDef:
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your data.
 
@@ -653,15 +656,15 @@
         Description: str,
         TemplateId: str = ...,
         ExpirationDays: int = ...,
         EncryptionKey: str = ...,
         AllowProfileCreation: bool = ...,
         SourceLastUpdatedTimestampFormat: str = ...,
         Fields: Mapping[str, ObjectTypeFieldTypeDef] = ...,
-        Keys: Mapping[str, Sequence[ObjectTypeKeyTypeDef]] = ...,
+        Keys: Mapping[str, Sequence[Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]]] = ...,
         Tags: Mapping[str, str] = ...
     ) -> PutProfileObjectTypeResponseTypeDef:
         """
         Defines a ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#put_profile_object_type)
```

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/literals.py` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/literals.pyi` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/paginator.py` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/paginator.pyi` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/type_defs.py` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2117,15 +2117,15 @@
     {
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Mapping[str, ObjectTypeFieldTypeDef],
-        "Keys": Mapping[str, Sequence[ObjectTypeKeyTypeDef]],
+        "Keys": Mapping[str, Sequence[Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]]],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class PutProfileObjectTypeRequestRequestTypeDef(
```

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/type_defs.pyi` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2044,15 +2044,15 @@
     {
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Mapping[str, ObjectTypeFieldTypeDef],
-        "Keys": Mapping[str, Sequence[ObjectTypeKeyTypeDef]],
+        "Keys": Mapping[str, Sequence[Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]]],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 class PutProfileObjectTypeRequestRequestTypeDef(
     _RequiredPutProfileObjectTypeRequestRequestTypeDef,
```

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/PKG-INFO` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.28.15
-Summary: Type annotations for boto3.CustomerProfiles 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CustomerProfiles 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/SOURCES.txt` & `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15/setup.py` & `mypy-boto3-customer-profiles-1.28.15.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-customer-profiles",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CustomerProfiles 1.28.15 service generated with"
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

