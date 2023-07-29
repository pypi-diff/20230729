# Comparing `tmp/mypy-boto3-iot-1.28.15.tar.gz` & `tmp/mypy-boto3-iot-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
+gzip compressed data, was "mypy-boto3-iot-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:19 2023, max compression
```

## Comparing `mypy-boto3-iot-1.28.15.tar` & `mypy-boto3-iot-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.245254 mypy-boto3-iot-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    55452 2023-07-28 20:42:59.233254 mypy-boto3-iot-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    53981 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.221253 mypy-boto3-iot-1.28.15/mypy_boto3_iot/
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   181667 2023-07-28 20:27:57.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   181351 2023-07-28 20:27:56.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25037 2023-07-28 20:27:59.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-28 20:27:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    68966 2023-07-28 20:27:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    68905 2023-07-28 20:27:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   270064 2023-07-28 20:28:09.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   269715 2023-07-28 20:28:04.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.233254 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    55452 2023-07-28 20:42:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:42:59.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.245254 mypy-boto3-iot-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.933182 mypy-boto3-iot-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    55458 2023-07-29 10:03:19.925182 mypy-boto3-iot-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    53981 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.921182 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   183696 2023-07-29 09:47:30.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   183380 2023-07-29 09:47:29.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25037 2023-07-29 09:47:31.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-29 09:47:31.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    68966 2023-07-29 09:47:30.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68905 2023-07-29 09:47:30.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   270219 2023-07-29 09:47:42.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   269870 2023-07-29 09:47:36.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.925182 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    55458 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:19.000000 mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:19.933182 mypy-boto3-iot-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:47:28.000000 mypy-boto3-iot-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-iot-1.28.15/LICENSE` & `mypy-boto3-iot-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15/PKG-INFO` & `mypy-boto3-iot-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot
-Version: 1.28.15
-Summary: Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iot-1.28.15/README.md` & `mypy-boto3-iot-1.28.15.post1/README.md`

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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/__init__.py` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/__init__.pyi` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/__main__.py` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.IoT 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT\nOther"
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

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/client.py` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,28 +112,34 @@
     ListThingTypesPaginator,
     ListTopicRuleDestinationsPaginator,
     ListTopicRulesPaginator,
     ListV2LoggingLevelsPaginator,
     ListViolationEventsPaginator,
 )
 from .type_defs import (
+    AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
+    AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
     AlertTargetTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
+    AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
     AuditCheckConfigurationTypeDef,
+    AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
     AuditNotificationTargetTypeDef,
+    AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
     AuthorizerConfigTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
+    BehaviorOutputTypeDef,
     BehaviorTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketsAggregationTypeTypeDef,
     CancelJobResponseTypeDef,
     ConfigurationTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
@@ -192,14 +198,15 @@
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeThingGroupResponseTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
+    DetectMitigationActionsTaskTargetOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     GetBucketsAggregationResponseTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     GetIndexingConfigurationResponseTypeDef,
@@ -214,14 +221,15 @@
     GetPolicyVersionResponseTypeDef,
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     GetTopicRuleResponseTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     HttpContextTypeDef,
+    JobExecutionsRetryConfigOutputTypeDef,
     JobExecutionsRetryConfigTypeDef,
     JobExecutionsRolloutConfigTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
@@ -279,39 +287,46 @@
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     LoggingOptionsPayloadTypeDef,
     LogTargetTypeDef,
     MaintenanceWindowTypeDef,
     MetricToRetainTypeDef,
+    MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
     MqttContextTypeDef,
+    OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     PresignedUrlConfigTypeDef,
     ProvisioningHookTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingResponseTypeDef,
     RegistrationConfigTypeDef,
     ResourceIdentifierTypeDef,
+    SchedulingConfigOutputTypeDef,
     SchedulingConfigTypeDef,
     SearchIndexResponseTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StreamFileTypeDef,
     TagTypeDef,
     TestAuthorizationResponseTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
+    ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
+    ThingGroupPropertiesOutputTypeDef,
     ThingGroupPropertiesTypeDef,
+    ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
+    ThingTypePropertiesOutputTypeDef,
     ThingTypePropertiesTypeDef,
     TimeoutConfigTypeDef,
     TlsConfigTypeDef,
     TlsContextTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRulePayloadTypeDef,
     TransferCertificateResponseTypeDef,
@@ -325,14 +340,15 @@
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     VersionUpdateByJobsConfigTypeDef,
+    ViolationEventOccurrenceRangeOutputTypeDef,
     ViolationEventOccurrenceRangeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -697,15 +713,17 @@
         """
 
     def create_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
         queryString: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
+        thingGroupProperties: Union[
+            ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
+        ] = ...,
         indexName: str = ...,
         queryVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDynamicThingGroupResponseTypeDef:
         """
         Creates a dynamic thing group.
 
@@ -714,15 +732,15 @@
         """
 
     def create_fleet_metric(
         self,
         *,
         metricName: str,
         queryString: str,
-        aggregationType: AggregationTypeTypeDef,
+        aggregationType: Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef],
         period: int,
         aggregationField: str,
         description: str = ...,
         queryVersion: str = ...,
         indexName: str = ...,
         unit: FleetMetricUnitType = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -741,22 +759,24 @@
         targets: Sequence[str],
         documentSource: str = ...,
         document: str = ...,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         targetSelection: TargetSelectionType = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
+        jobExecutionsRetryConfig: Union[
+            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
+        ] = ...,
         documentParameters: Mapping[str, str] = ...,
-        schedulingConfig: SchedulingConfigTypeDef = ...,
+        schedulingConfig: Union[SchedulingConfigTypeDef, SchedulingConfigOutputTypeDef] = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_job)
@@ -768,18 +788,20 @@
         jobTemplateId: str,
         description: str,
         jobArn: str = ...,
         documentSource: str = ...,
         document: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
+        jobExecutionsRetryConfig: Union[
+            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
+        ] = ...,
         maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
@@ -798,15 +820,15 @@
         """
 
     def create_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str,
-        actionParams: MitigationActionParamsTypeDef,
+        actionParams: Union[MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef],
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateMitigationActionResponseTypeDef:
         """
         Defines an action that can be applied to audit findings by using
         StartAuditMitigationActionsTask.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_mitigation_action)
@@ -814,15 +836,15 @@
         """
 
     def create_ota_update(
         self,
         *,
         otaUpdateId: str,
         targets: Sequence[str],
-        files: Sequence[OTAUpdateFileTypeDef],
+        files: Sequence[Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]],
         roleArn: str,
         description: str = ...,
         protocols: Sequence[ProtocolType] = ...,
         targetSelection: TargetSelectionType = ...,
         awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,
         awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,
         awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,
@@ -961,15 +983,15 @@
         """
 
     def create_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorTypeDef] = ...,
+        behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a Device Defender security profile.
@@ -995,44 +1017,48 @@
         """
 
     def create_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadTypeDef = ...,
+        attributePayload: Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef] = ...,
         billingGroupName: str = ...
     ) -> CreateThingResponseTypeDef:
         """
         Creates a thing record in the registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing)
         """
 
     def create_thing_group(
         self,
         *,
         thingGroupName: str,
         parentGroupName: str = ...,
-        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
+        thingGroupProperties: Union[
+            ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
+        ] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingGroupResponseTypeDef:
         """
         Create a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing_group)
         """
 
     def create_thing_type(
         self,
         *,
         thingTypeName: str,
-        thingTypeProperties: ThingTypePropertiesTypeDef = ...,
+        thingTypeProperties: Union[
+            ThingTypePropertiesTypeDef, ThingTypePropertiesOutputTypeDef
+        ] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingTypeResponseTypeDef:
         """
         Creates a new thing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing_type)
@@ -2871,33 +2897,39 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#set_v2_logging_options)
         """
 
     def start_audit_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: AuditMitigationActionsTaskTargetTypeDef,
+        target: Union[
+            AuditMitigationActionsTaskTargetTypeDef, AuditMitigationActionsTaskTargetOutputTypeDef
+        ],
         auditCheckToActionsMapping: Mapping[str, Sequence[str]],
         clientRequestToken: str
     ) -> StartAuditMitigationActionsTaskResponseTypeDef:
         """
         Starts a task that applies a set of mitigation actions to the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_audit_mitigation_actions_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#start_audit_mitigation_actions_task)
         """
 
     def start_detect_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: DetectMitigationActionsTaskTargetTypeDef,
+        target: Union[
+            DetectMitigationActionsTaskTargetTypeDef, DetectMitigationActionsTaskTargetOutputTypeDef
+        ],
         actions: Sequence[str],
         clientRequestToken: str,
-        violationEventOccurrenceRange: ViolationEventOccurrenceRangeTypeDef = ...,
+        violationEventOccurrenceRange: Union[
+            ViolationEventOccurrenceRangeTypeDef, ViolationEventOccurrenceRangeOutputTypeDef
+        ] = ...,
         includeOnlyActiveViolations: bool = ...,
         includeSuppressedAlerts: bool = ...
     ) -> StartDetectMitigationActionsTaskResponseTypeDef:
         """
         Starts a Device Defender ML Detect mitigation actions task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_detect_mitigation_actions_task)
@@ -2939,15 +2971,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#tag_resource)
         """
 
     def test_authorization(
         self,
         *,
-        authInfos: Sequence[AuthInfoTypeDef],
+        authInfos: Sequence[Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]],
         principal: str = ...,
         cognitoIdentityPoolId: str = ...,
         clientId: str = ...,
         policyNamesToAdd: Sequence[str] = ...,
         policyNamesToSkip: Sequence[str] = ...
     ) -> TestAuthorizationResponseTypeDef:
         """
@@ -3119,15 +3151,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_domain_configuration)
         """
 
     def update_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef,
+        thingGroupProperties: Union[ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef],
         expectedVersion: int = ...,
         indexName: str = ...,
         queryString: str = ...,
         queryVersion: str = ...
     ) -> UpdateDynamicThingGroupResponseTypeDef:
         """
         Updates a dynamic thing group.
@@ -3148,15 +3180,15 @@
 
     def update_fleet_metric(
         self,
         *,
         metricName: str,
         indexName: str,
         queryString: str = ...,
-        aggregationType: AggregationTypeTypeDef = ...,
+        aggregationType: Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef] = ...,
         period: int = ...,
         aggregationField: str = ...,
         description: str = ...,
         queryVersion: str = ...,
         unit: FleetMetricUnitType = ...,
         expectedVersion: int = ...
     ) -> EmptyResponseMetadataTypeDef:
@@ -3166,16 +3198,20 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_fleet_metric)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_fleet_metric)
         """
 
     def update_indexing_configuration(
         self,
         *,
-        thingIndexingConfiguration: ThingIndexingConfigurationTypeDef = ...,
-        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...
+        thingIndexingConfiguration: Union[
+            ThingIndexingConfigurationTypeDef, ThingIndexingConfigurationOutputTypeDef
+        ] = ...,
+        thingGroupIndexingConfiguration: Union[
+            ThingGroupIndexingConfigurationTypeDef, ThingGroupIndexingConfigurationOutputTypeDef
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Updates the search configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_indexing_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_indexing_configuration)
         """
@@ -3183,32 +3219,36 @@
     def update_job(
         self,
         *,
         jobId: str,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         namespaceId: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...
+        jobExecutionsRetryConfig: Union[
+            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
+        ] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates supported fields of the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_job)
         """
 
     def update_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str = ...,
-        actionParams: MitigationActionParamsTypeDef = ...
+        actionParams: Union[
+            MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef
+        ] = ...
     ) -> UpdateMitigationActionResponseTypeDef:
         """
         Updates the definition for the specified mitigation action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_mitigation_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_mitigation_action)
         """
@@ -3305,15 +3345,15 @@
         """
 
     def update_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorTypeDef] = ...,
+        behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         deleteBehaviors: bool = ...,
         deleteAlertTargets: bool = ...,
         deleteAdditionalMetricsToRetain: bool = ...,
         expectedVersion: int = ...
@@ -3341,30 +3381,30 @@
         """
 
     def update_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadTypeDef = ...,
+        attributePayload: Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef] = ...,
         expectedVersion: int = ...,
         removeThingType: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the data for a thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_thing)
         """
 
     def update_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef,
+        thingGroupProperties: Union[ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef],
         expectedVersion: int = ...
     ) -> UpdateThingGroupResponseTypeDef:
         """
         Update a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_thing_group)
@@ -3392,15 +3432,15 @@
         Updates a topic rule destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_topic_rule_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_topic_rule_destination)
         """
 
     def validate_security_profile_behaviors(
-        self, *, behaviors: Sequence[BehaviorTypeDef]
+        self, *, behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]]
     ) -> ValidateSecurityProfileBehaviorsResponseTypeDef:
         """
         Validates a Device Defender security profile behaviors specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.validate_security_profile_behaviors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#validate_security_profile_behaviors)
         """
```

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/client.pyi` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -112,28 +112,34 @@
     ListThingTypesPaginator,
     ListTopicRuleDestinationsPaginator,
     ListTopicRulesPaginator,
     ListV2LoggingLevelsPaginator,
     ListViolationEventsPaginator,
 )
 from .type_defs import (
+    AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
+    AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
     AlertTargetTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
+    AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
     AuditCheckConfigurationTypeDef,
+    AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
     AuditNotificationTargetTypeDef,
+    AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
     AuthorizerConfigTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
+    BehaviorOutputTypeDef,
     BehaviorTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketsAggregationTypeTypeDef,
     CancelJobResponseTypeDef,
     ConfigurationTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
@@ -192,14 +198,15 @@
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeThingGroupResponseTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
+    DetectMitigationActionsTaskTargetOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     GetBucketsAggregationResponseTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     GetIndexingConfigurationResponseTypeDef,
@@ -214,14 +221,15 @@
     GetPolicyVersionResponseTypeDef,
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     GetTopicRuleResponseTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     HttpContextTypeDef,
+    JobExecutionsRetryConfigOutputTypeDef,
     JobExecutionsRetryConfigTypeDef,
     JobExecutionsRolloutConfigTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
@@ -279,39 +287,46 @@
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     LoggingOptionsPayloadTypeDef,
     LogTargetTypeDef,
     MaintenanceWindowTypeDef,
     MetricToRetainTypeDef,
+    MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
     MqttContextTypeDef,
+    OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     PresignedUrlConfigTypeDef,
     ProvisioningHookTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingResponseTypeDef,
     RegistrationConfigTypeDef,
     ResourceIdentifierTypeDef,
+    SchedulingConfigOutputTypeDef,
     SchedulingConfigTypeDef,
     SearchIndexResponseTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StreamFileTypeDef,
     TagTypeDef,
     TestAuthorizationResponseTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
+    ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
+    ThingGroupPropertiesOutputTypeDef,
     ThingGroupPropertiesTypeDef,
+    ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
+    ThingTypePropertiesOutputTypeDef,
     ThingTypePropertiesTypeDef,
     TimeoutConfigTypeDef,
     TlsConfigTypeDef,
     TlsContextTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRulePayloadTypeDef,
     TransferCertificateResponseTypeDef,
@@ -325,14 +340,15 @@
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     VersionUpdateByJobsConfigTypeDef,
+    ViolationEventOccurrenceRangeOutputTypeDef,
     ViolationEventOccurrenceRangeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -667,15 +683,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_domain_configuration)
         """
     def create_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
         queryString: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
+        thingGroupProperties: Union[
+            ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
+        ] = ...,
         indexName: str = ...,
         queryVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDynamicThingGroupResponseTypeDef:
         """
         Creates a dynamic thing group.
 
@@ -683,15 +701,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_dynamic_thing_group)
         """
     def create_fleet_metric(
         self,
         *,
         metricName: str,
         queryString: str,
-        aggregationType: AggregationTypeTypeDef,
+        aggregationType: Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef],
         period: int,
         aggregationField: str,
         description: str = ...,
         queryVersion: str = ...,
         indexName: str = ...,
         unit: FleetMetricUnitType = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -709,22 +727,24 @@
         targets: Sequence[str],
         documentSource: str = ...,
         document: str = ...,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         targetSelection: TargetSelectionType = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
+        jobExecutionsRetryConfig: Union[
+            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
+        ] = ...,
         documentParameters: Mapping[str, str] = ...,
-        schedulingConfig: SchedulingConfigTypeDef = ...,
+        schedulingConfig: Union[SchedulingConfigTypeDef, SchedulingConfigOutputTypeDef] = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_job)
@@ -735,18 +755,20 @@
         jobTemplateId: str,
         description: str,
         jobArn: str = ...,
         documentSource: str = ...,
         document: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
+        jobExecutionsRetryConfig: Union[
+            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
+        ] = ...,
         maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
@@ -763,30 +785,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_keys_and_certificate)
         """
     def create_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str,
-        actionParams: MitigationActionParamsTypeDef,
+        actionParams: Union[MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef],
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateMitigationActionResponseTypeDef:
         """
         Defines an action that can be applied to audit findings by using
         StartAuditMitigationActionsTask.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_mitigation_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_mitigation_action)
         """
     def create_ota_update(
         self,
         *,
         otaUpdateId: str,
         targets: Sequence[str],
-        files: Sequence[OTAUpdateFileTypeDef],
+        files: Sequence[Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]],
         roleArn: str,
         description: str = ...,
         protocols: Sequence[ProtocolType] = ...,
         targetSelection: TargetSelectionType = ...,
         awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,
         awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,
         awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,
@@ -915,15 +937,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_scheduled_audit)
         """
     def create_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorTypeDef] = ...,
+        behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a Device Defender security profile.
@@ -947,42 +969,46 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_stream)
         """
     def create_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadTypeDef = ...,
+        attributePayload: Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef] = ...,
         billingGroupName: str = ...
     ) -> CreateThingResponseTypeDef:
         """
         Creates a thing record in the registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing)
         """
     def create_thing_group(
         self,
         *,
         thingGroupName: str,
         parentGroupName: str = ...,
-        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
+        thingGroupProperties: Union[
+            ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
+        ] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingGroupResponseTypeDef:
         """
         Create a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing_group)
         """
     def create_thing_type(
         self,
         *,
         thingTypeName: str,
-        thingTypeProperties: ThingTypePropertiesTypeDef = ...,
+        thingTypeProperties: Union[
+            ThingTypePropertiesTypeDef, ThingTypePropertiesOutputTypeDef
+        ] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingTypeResponseTypeDef:
         """
         Creates a new thing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#create_thing_type)
@@ -2651,32 +2677,38 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.set_v2_logging_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#set_v2_logging_options)
         """
     def start_audit_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: AuditMitigationActionsTaskTargetTypeDef,
+        target: Union[
+            AuditMitigationActionsTaskTargetTypeDef, AuditMitigationActionsTaskTargetOutputTypeDef
+        ],
         auditCheckToActionsMapping: Mapping[str, Sequence[str]],
         clientRequestToken: str
     ) -> StartAuditMitigationActionsTaskResponseTypeDef:
         """
         Starts a task that applies a set of mitigation actions to the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_audit_mitigation_actions_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#start_audit_mitigation_actions_task)
         """
     def start_detect_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: DetectMitigationActionsTaskTargetTypeDef,
+        target: Union[
+            DetectMitigationActionsTaskTargetTypeDef, DetectMitigationActionsTaskTargetOutputTypeDef
+        ],
         actions: Sequence[str],
         clientRequestToken: str,
-        violationEventOccurrenceRange: ViolationEventOccurrenceRangeTypeDef = ...,
+        violationEventOccurrenceRange: Union[
+            ViolationEventOccurrenceRangeTypeDef, ViolationEventOccurrenceRangeOutputTypeDef
+        ] = ...,
         includeOnlyActiveViolations: bool = ...,
         includeSuppressedAlerts: bool = ...
     ) -> StartDetectMitigationActionsTaskResponseTypeDef:
         """
         Starts a Device Defender ML Detect mitigation actions task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_detect_mitigation_actions_task)
@@ -2713,15 +2745,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#tag_resource)
         """
     def test_authorization(
         self,
         *,
-        authInfos: Sequence[AuthInfoTypeDef],
+        authInfos: Sequence[Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]],
         principal: str = ...,
         cognitoIdentityPoolId: str = ...,
         clientId: str = ...,
         policyNamesToAdd: Sequence[str] = ...,
         policyNamesToSkip: Sequence[str] = ...
     ) -> TestAuthorizationResponseTypeDef:
         """
@@ -2880,15 +2912,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_domain_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_domain_configuration)
         """
     def update_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef,
+        thingGroupProperties: Union[ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef],
         expectedVersion: int = ...,
         indexName: str = ...,
         queryString: str = ...,
         queryVersion: str = ...
     ) -> UpdateDynamicThingGroupResponseTypeDef:
         """
         Updates a dynamic thing group.
@@ -2907,15 +2939,15 @@
         """
     def update_fleet_metric(
         self,
         *,
         metricName: str,
         indexName: str,
         queryString: str = ...,
-        aggregationType: AggregationTypeTypeDef = ...,
+        aggregationType: Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef] = ...,
         period: int = ...,
         aggregationField: str = ...,
         description: str = ...,
         queryVersion: str = ...,
         unit: FleetMetricUnitType = ...,
         expectedVersion: int = ...
     ) -> EmptyResponseMetadataTypeDef:
@@ -2924,47 +2956,55 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_fleet_metric)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_fleet_metric)
         """
     def update_indexing_configuration(
         self,
         *,
-        thingIndexingConfiguration: ThingIndexingConfigurationTypeDef = ...,
-        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...
+        thingIndexingConfiguration: Union[
+            ThingIndexingConfigurationTypeDef, ThingIndexingConfigurationOutputTypeDef
+        ] = ...,
+        thingGroupIndexingConfiguration: Union[
+            ThingGroupIndexingConfigurationTypeDef, ThingGroupIndexingConfigurationOutputTypeDef
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Updates the search configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_indexing_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_indexing_configuration)
         """
     def update_job(
         self,
         *,
         jobId: str,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: Union[AbortConfigTypeDef, AbortConfigOutputTypeDef] = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         namespaceId: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...
+        jobExecutionsRetryConfig: Union[
+            JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
+        ] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates supported fields of the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_job)
         """
     def update_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str = ...,
-        actionParams: MitigationActionParamsTypeDef = ...
+        actionParams: Union[
+            MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef
+        ] = ...
     ) -> UpdateMitigationActionResponseTypeDef:
         """
         Updates the definition for the specified mitigation action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_mitigation_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_mitigation_action)
         """
@@ -3054,15 +3094,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_scheduled_audit)
         """
     def update_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorTypeDef] = ...,
+        behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         deleteBehaviors: bool = ...,
         deleteAlertTargets: bool = ...,
         deleteAdditionalMetricsToRetain: bool = ...,
         expectedVersion: int = ...
@@ -3088,29 +3128,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_stream)
         """
     def update_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadTypeDef = ...,
+        attributePayload: Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef] = ...,
         expectedVersion: int = ...,
         removeThingType: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the data for a thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_thing)
         """
     def update_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef,
+        thingGroupProperties: Union[ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef],
         expectedVersion: int = ...
     ) -> UpdateThingGroupResponseTypeDef:
         """
         Update a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_thing_group)
@@ -3135,15 +3175,15 @@
         """
         Updates a topic rule destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_topic_rule_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#update_topic_rule_destination)
         """
     def validate_security_profile_behaviors(
-        self, *, behaviors: Sequence[BehaviorTypeDef]
+        self, *, behaviors: Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]]
     ) -> ValidateSecurityProfileBehaviorsResponseTypeDef:
         """
         Validates a Device Defender security profile behaviors specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.validate_security_profile_behaviors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/client/#validate_security_profile_behaviors)
         """
```

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/literals.py` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/literals.pyi` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/paginator.py` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/paginator.pyi` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/type_defs.py` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -6189,15 +6189,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredTestAuthorizationRequestRequestTypeDef",
     {
-        "authInfos": Sequence[AuthInfoTypeDef],
+        "authInfos": Sequence[Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]],
     },
 )
 _OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
     "_OptionalTestAuthorizationRequestRequestTypeDef",
     {
         "principal": str,
         "cognitoIdentityPoolId": str,
@@ -9545,15 +9545,15 @@
         "securityProfileName": str,
     },
 )
 _OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorTypeDef],
+        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
         "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": Sequence[str],
         "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
@@ -9572,15 +9572,15 @@
         "securityProfileName": str,
     },
 )
 _OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorTypeDef],
+        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
         "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": Sequence[str],
         "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
         "deleteBehaviors": bool,
         "deleteAlertTargets": bool,
         "deleteAdditionalMetricsToRetain": bool,
         "expectedVersion": int,
@@ -9595,15 +9595,15 @@
 ):
     pass
 
 
 ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
     "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     {
-        "behaviors": Sequence[BehaviorTypeDef],
+        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
     },
 )
 
 CodeSigningOutputTypeDef = TypedDict(
     "CodeSigningOutputTypeDef",
     {
         "awsSignerJobId": str,
@@ -10062,15 +10062,15 @@
 )
 
 _RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOTAUpdateRequestRequestTypeDef",
     {
         "otaUpdateId": str,
         "targets": Sequence[str],
-        "files": Sequence[OTAUpdateFileTypeDef],
+        "files": Sequence[Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]],
         "roleArn": str,
     },
 )
 _OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateOTAUpdateRequestRequestTypeDef",
     {
         "description": str,
```

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot/type_defs.pyi` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -6000,15 +6000,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredTestAuthorizationRequestRequestTypeDef",
     {
-        "authInfos": Sequence[AuthInfoTypeDef],
+        "authInfos": Sequence[Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]],
     },
 )
 _OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
     "_OptionalTestAuthorizationRequestRequestTypeDef",
     {
         "principal": str,
         "cognitoIdentityPoolId": str,
@@ -9212,15 +9212,15 @@
         "securityProfileName": str,
     },
 )
 _OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorTypeDef],
+        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
         "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": Sequence[str],
         "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
@@ -9237,15 +9237,15 @@
         "securityProfileName": str,
     },
 )
 _OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorTypeDef],
+        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
         "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": Sequence[str],
         "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
         "deleteBehaviors": bool,
         "deleteAlertTargets": bool,
         "deleteAdditionalMetricsToRetain": bool,
         "expectedVersion": int,
@@ -9258,15 +9258,15 @@
     _OptionalUpdateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
 ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
     "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     {
-        "behaviors": Sequence[BehaviorTypeDef],
+        "behaviors": Sequence[Union[BehaviorTypeDef, BehaviorOutputTypeDef]],
     },
 )
 
 CodeSigningOutputTypeDef = TypedDict(
     "CodeSigningOutputTypeDef",
     {
         "awsSignerJobId": str,
@@ -9717,15 +9717,15 @@
 )
 
 _RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOTAUpdateRequestRequestTypeDef",
     {
         "otaUpdateId": str,
         "targets": Sequence[str],
-        "files": Sequence[OTAUpdateFileTypeDef],
+        "files": Sequence[Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]],
         "roleArn": str,
     },
 )
 _OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateOTAUpdateRequestRequestTypeDef",
     {
         "description": str,
```

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/PKG-INFO` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot
-Version: 1.28.15
-Summary: Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/SOURCES.txt` & `mypy-boto3-iot-1.28.15.post1/mypy_boto3_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.15/setup.py` & `mypy-boto3-iot-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_iot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

