# Comparing `tmp/mypy-boto3-config-1.28.15.tar.gz` & `tmp/mypy-boto3-config-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-config-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
+gzip compressed data, was "mypy-boto3-config-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:51 2023, max compression
```

## Comparing `mypy-boto3-config-1.28.15.tar` & `mypy-boto3-config-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.600911 mypy-boto3-config-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37108 2023-07-28 20:42:34.596912 mypy-boto3-config-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35618 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.596912 mypy-boto3-config-1.28.15/mypy_boto3_config/
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88855 2023-07-28 20:22:10.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    88725 2023-07-28 20:22:10.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-07-28 20:22:11.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-07-28 20:22:11.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42907 2023-07-28 20:22:10.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    42874 2023-07-28 20:22:10.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   135358 2023-07-28 20:22:15.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   135191 2023-07-28 20:22:13.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.596912 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37108 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.600911 mypy-boto3-config-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.617087 mypy-boto3-config-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37114 2023-07-29 10:02:51.609087 mypy-boto3-config-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35618 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.605087 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-29 09:41:21.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89729 2023-07-29 09:41:21.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89599 2023-07-29 09:41:21.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-07-29 09:41:23.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-07-29 09:41:22.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42907 2023-07-29 09:41:22.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42874 2023-07-29 09:41:22.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:21.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   135526 2023-07-29 09:41:27.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135359 2023-07-29 09:41:25.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.609087 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37114 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:02:51.000000 mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:51.617087 mypy-boto3-config-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:41:20.000000 mypy-boto3-config-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-config-1.28.15/LICENSE` & `mypy-boto3-config-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15/PKG-INFO` & `mypy-boto3-config-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.28.15
-Summary: Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-config-1.28.15/README.md` & `mypy-boto3-config-1.28.15.post1/README.md`

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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/__init__.py` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/__init__.pyi` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/__main__.py` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConfigService 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.ConfigService 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService\nOther"
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

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/client.py` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,23 +60,26 @@
     ListDiscoveredResourcesPaginator,
     ListResourceEvaluationsPaginator,
     ListTagsForResourcePaginator,
     SelectAggregateResourceConfigPaginator,
     SelectResourceConfigPaginator,
 )
 from .type_defs import (
+    AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigResponseTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
+    ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
+    ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     DeliverConfigSnapshotResponseTypeDef,
@@ -105,14 +108,15 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
+    EvaluationOutputTypeDef,
     EvaluationTypeDef,
     ExternalEvaluationTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
@@ -132,29 +136,33 @@
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesResponseTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    OrganizationAggregationSourceOutputTypeDef,
     OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
+    OrganizationCustomRuleMetadataOutputTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
+    OrganizationManagedRuleMetadataOutputTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     PutConformancePackResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutStoredQueryResponseTypeDef,
+    RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     ResourceCountFiltersTypeDef,
     ResourceDetailsTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
@@ -1158,42 +1166,53 @@
         account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_aggregation_authorization)
         """
 
     def put_config_rule(
-        self, *, ConfigRule: ConfigRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        ConfigRule: Union[ConfigRuleTypeDef, ConfigRuleOutputTypeDef],
+        Tags: Sequence[TagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or updates an Config rule to evaluate if your Amazon Web Services resources
         comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_config_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_config_rule)
         """
 
     def put_configuration_aggregator(
         self,
         *,
         ConfigurationAggregatorName: str,
-        AccountAggregationSources: Sequence[AccountAggregationSourceTypeDef] = ...,
-        OrganizationAggregationSource: OrganizationAggregationSourceTypeDef = ...,
+        AccountAggregationSources: Sequence[
+            Union[AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef]
+        ] = ...,
+        OrganizationAggregationSource: Union[
+            OrganizationAggregationSourceTypeDef, OrganizationAggregationSourceOutputTypeDef
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> PutConfigurationAggregatorResponseTypeDef:
         """
         Creates and updates the configuration aggregator with the selected source
         accounts and regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_configuration_aggregator)
         """
 
     def put_configuration_recorder(
-        self, *, ConfigurationRecorder: ConfigurationRecorderTypeDef
+        self,
+        *,
+        ConfigurationRecorder: Union[
+            ConfigurationRecorderTypeDef, ConfigurationRecorderOutputTypeDef
+        ]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new configuration recorder to record configuration changes for
         specified resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_recorder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_configuration_recorder)
@@ -1228,15 +1247,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_delivery_channel)
         """
 
     def put_evaluations(
         self,
         *,
         ResultToken: str,
-        Evaluations: Sequence[EvaluationTypeDef] = ...,
+        Evaluations: Sequence[Union[EvaluationTypeDef, EvaluationOutputTypeDef]] = ...,
         TestMode: bool = ...
     ) -> PutEvaluationsResponseTypeDef:
         """
         Used by an Lambda function to deliver evaluation results to Config.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_evaluations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_evaluations)
@@ -1252,16 +1271,20 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_external_evaluation)
         """
 
     def put_organization_config_rule(
         self,
         *,
         OrganizationConfigRuleName: str,
-        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,
-        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,
+        OrganizationManagedRuleMetadata: Union[
+            OrganizationManagedRuleMetadataTypeDef, OrganizationManagedRuleMetadataOutputTypeDef
+        ] = ...,
+        OrganizationCustomRuleMetadata: Union[
+            OrganizationCustomRuleMetadataTypeDef, OrganizationCustomRuleMetadataOutputTypeDef
+        ] = ...,
         ExcludedAccounts: Sequence[str] = ...,
         OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
         Adds or updates an Config rule for your entire organization to evaluate if your
         Amazon Web Services resources comply with your desired configurations.
 
@@ -1285,15 +1308,19 @@
         Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_organization_conformance_pack)
         """
 
     def put_remediation_configurations(
-        self, *, RemediationConfigurations: Sequence[RemediationConfigurationTypeDef]
+        self,
+        *,
+        RemediationConfigurations: Sequence[
+            Union[RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef]
+        ]
     ) -> PutRemediationConfigurationsResponseTypeDef:
         """
         Adds or updates the remediation configuration with a specific Config rule with
         the selected target or action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_remediation_configurations)
```

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/client.pyi` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,23 +60,26 @@
     ListDiscoveredResourcesPaginator,
     ListResourceEvaluationsPaginator,
     ListTagsForResourcePaginator,
     SelectAggregateResourceConfigPaginator,
     SelectResourceConfigPaginator,
 )
 from .type_defs import (
+    AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigResponseTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
+    ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
+    ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     DeliverConfigSnapshotResponseTypeDef,
@@ -105,14 +108,15 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
+    EvaluationOutputTypeDef,
     EvaluationTypeDef,
     ExternalEvaluationTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
@@ -132,29 +136,33 @@
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesResponseTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    OrganizationAggregationSourceOutputTypeDef,
     OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
+    OrganizationCustomRuleMetadataOutputTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
+    OrganizationManagedRuleMetadataOutputTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     PutConformancePackResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutStoredQueryResponseTypeDef,
+    RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     ResourceCountFiltersTypeDef,
     ResourceDetailsTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
@@ -1081,40 +1089,51 @@
         Authorizes the aggregator account and region to collect data from the source
         account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_aggregation_authorization)
         """
     def put_config_rule(
-        self, *, ConfigRule: ConfigRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        ConfigRule: Union[ConfigRuleTypeDef, ConfigRuleOutputTypeDef],
+        Tags: Sequence[TagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or updates an Config rule to evaluate if your Amazon Web Services resources
         comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_config_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_config_rule)
         """
     def put_configuration_aggregator(
         self,
         *,
         ConfigurationAggregatorName: str,
-        AccountAggregationSources: Sequence[AccountAggregationSourceTypeDef] = ...,
-        OrganizationAggregationSource: OrganizationAggregationSourceTypeDef = ...,
+        AccountAggregationSources: Sequence[
+            Union[AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef]
+        ] = ...,
+        OrganizationAggregationSource: Union[
+            OrganizationAggregationSourceTypeDef, OrganizationAggregationSourceOutputTypeDef
+        ] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> PutConfigurationAggregatorResponseTypeDef:
         """
         Creates and updates the configuration aggregator with the selected source
         accounts and regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_configuration_aggregator)
         """
     def put_configuration_recorder(
-        self, *, ConfigurationRecorder: ConfigurationRecorderTypeDef
+        self,
+        *,
+        ConfigurationRecorder: Union[
+            ConfigurationRecorderTypeDef, ConfigurationRecorderOutputTypeDef
+        ]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new configuration recorder to record configuration changes for
         specified resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_recorder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_configuration_recorder)
@@ -1146,15 +1165,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_delivery_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_delivery_channel)
         """
     def put_evaluations(
         self,
         *,
         ResultToken: str,
-        Evaluations: Sequence[EvaluationTypeDef] = ...,
+        Evaluations: Sequence[Union[EvaluationTypeDef, EvaluationOutputTypeDef]] = ...,
         TestMode: bool = ...
     ) -> PutEvaluationsResponseTypeDef:
         """
         Used by an Lambda function to deliver evaluation results to Config.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_evaluations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_evaluations)
@@ -1168,16 +1187,20 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_external_evaluation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_external_evaluation)
         """
     def put_organization_config_rule(
         self,
         *,
         OrganizationConfigRuleName: str,
-        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,
-        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,
+        OrganizationManagedRuleMetadata: Union[
+            OrganizationManagedRuleMetadataTypeDef, OrganizationManagedRuleMetadataOutputTypeDef
+        ] = ...,
+        OrganizationCustomRuleMetadata: Union[
+            OrganizationCustomRuleMetadataTypeDef, OrganizationCustomRuleMetadataOutputTypeDef
+        ] = ...,
         ExcludedAccounts: Sequence[str] = ...,
         OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
         Adds or updates an Config rule for your entire organization to evaluate if your
         Amazon Web Services resources comply with your desired configurations.
 
@@ -1199,15 +1222,19 @@
         Deploys conformance packs across member accounts in an Amazon Web Services
         Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_organization_conformance_pack)
         """
     def put_remediation_configurations(
-        self, *, RemediationConfigurations: Sequence[RemediationConfigurationTypeDef]
+        self,
+        *,
+        RemediationConfigurations: Sequence[
+            Union[RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef]
+        ]
     ) -> PutRemediationConfigurationsResponseTypeDef:
         """
         Adds or updates the remediation configuration with a specific Config rule with
         the selected target or action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_remediation_configurations)
```

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/literals.py` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/literals.pyi` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/paginator.py` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/paginator.pyi` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/type_defs.py` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3381,15 +3381,15 @@
     {
         "ResultToken": str,
     },
 )
 _OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
     "_OptionalPutEvaluationsRequestRequestTypeDef",
     {
-        "Evaluations": Sequence[EvaluationTypeDef],
+        "Evaluations": Sequence[Union[EvaluationTypeDef, EvaluationOutputTypeDef]],
         "TestMode": bool,
     },
     total=False,
 )
 
 
 class PutEvaluationsRequestRequestTypeDef(
@@ -3771,15 +3771,17 @@
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
     {
-        "AccountAggregationSources": Sequence[AccountAggregationSourceTypeDef],
+        "AccountAggregationSources": Sequence[
+            Union[AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef]
+        ],
         "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
@@ -4474,15 +4476,17 @@
     },
     total=False,
 )
 
 PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
     "PutRemediationConfigurationsRequestRequestTypeDef",
     {
-        "RemediationConfigurations": Sequence[RemediationConfigurationTypeDef],
+        "RemediationConfigurations": Sequence[
+            Union[RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef]
+        ],
     },
 )
 
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
         "ConfigRules": List[ConfigRuleOutputTypeDef],
```

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config/type_defs.pyi` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3258,15 +3258,15 @@
     {
         "ResultToken": str,
     },
 )
 _OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
     "_OptionalPutEvaluationsRequestRequestTypeDef",
     {
-        "Evaluations": Sequence[EvaluationTypeDef],
+        "Evaluations": Sequence[Union[EvaluationTypeDef, EvaluationOutputTypeDef]],
         "TestMode": bool,
     },
     total=False,
 )
 
 class PutEvaluationsRequestRequestTypeDef(
     _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
@@ -3626,15 +3626,17 @@
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
     {
-        "AccountAggregationSources": Sequence[AccountAggregationSourceTypeDef],
+        "AccountAggregationSources": Sequence[
+            Union[AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef]
+        ],
         "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class PutConfigurationAggregatorRequestRequestTypeDef(
@@ -4309,15 +4311,17 @@
     },
     total=False,
 )
 
 PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
     "PutRemediationConfigurationsRequestRequestTypeDef",
     {
-        "RemediationConfigurations": Sequence[RemediationConfigurationTypeDef],
+        "RemediationConfigurations": Sequence[
+            Union[RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef]
+        ],
     },
 )
 
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
         "ConfigRules": List[ConfigRuleOutputTypeDef],
```

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/PKG-INFO` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.28.15
-Summary: Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/SOURCES.txt` & `mypy-boto3-config-1.28.15.post1/mypy_boto3_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.15/setup.py` & `mypy-boto3-config-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-config",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder"
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

