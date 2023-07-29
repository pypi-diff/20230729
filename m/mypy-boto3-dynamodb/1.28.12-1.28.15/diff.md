# Comparing `tmp/mypy-boto3-dynamodb-1.28.12.tar.gz` & `tmp/mypy-boto3-dynamodb-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodb-1.28.12.tar", last modified: Thu Jul 27 05:34:36 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodb-1.28.15.tar", last modified: Fri Jul 28 20:42:40 2023, max compression
```

## Comparing `mypy-boto3-dynamodb-1.28.12.tar` & `mypy-boto3-dynamodb-1.28.15.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.200528 mypy-boto3-dynamodb-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29424 2023-07-27 05:34:36.200528 mypy-boto3-dynamodb-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27933 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.200528 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54381 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-27 05:20:38.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-27 05:20:38.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-27 05:20:38.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    27558 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   158324 2023-07-27 05:20:41.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   158157 2023-07-27 05:20:40.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-27 05:20:38.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-27 05:20:38.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.200528 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29424 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:36.000000 mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:36.200528 mypy-boto3-dynamodb-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:20:37.000000 mypy-boto3-dynamodb-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.760999 mypy-boto3-dynamodb-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:23:29.000000 mypy-boto3-dynamodb-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25978 2023-07-28 20:42:40.760999 mypy-boto3-dynamodb-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24487 2023-07-28 20:23:29.000000 mypy-boto3-dynamodb-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.740999 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-28 20:23:29.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-28 20:23:29.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:23:29.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53205 2023-07-28 20:23:29.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53138 2023-07-28 20:23:29.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-28 20:23:31.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-28 20:23:31.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-28 20:23:31.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-28 20:23:31.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:23:29.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26601 2023-07-28 20:23:30.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26574 2023-07-28 20:23:30.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   121636 2023-07-28 20:23:35.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121497 2023-07-28 20:23:33.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:23:29.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-28 20:23:31.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-28 20:23:31.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.760999 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25978 2023-07-28 20:42:40.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-28 20:42:40.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:40.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:40.000000 mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:40.760999 mypy-boto3-dynamodb-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:23:28.000000 mypy-boto3-dynamodb-1.28.15/setup.py
```

### Comparing `mypy-boto3-dynamodb-1.28.12/LICENSE` & `mypy-boto3-dynamodb-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.12/PKG-INFO` & `mypy-boto3-dynamodb-1.28.15/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-dynamodb
-Version: 1.28.12
-Summary: Type annotations for boto3.DynamoDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 dynamodb type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-dynamodb"></a>
 
 # mypy-boto3-dynamodb
 
 [![PyPI - mypy-boto3-dynamodb](https://img.shields.io/pypi/v/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -481,152 +449,94 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    ArchivalSummaryTableTypeDef,
+    ResponseMetadataTypeDef,
     ArchivalSummaryTypeDef,
-    AttributeDefinitionOutputTypeDef,
-    AttributeDefinitionServiceResourceTypeDef,
-    AttributeDefinitionTableOutputTypeDef,
-    AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
-    AttributeValueServiceResourceTypeDef,
-    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
-    AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
-    BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
-    KeysAndAttributesServiceResourceTypeDef,
-    KeysAndAttributesServiceResourceOutputTypeDef,
-    ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
-    BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
-    CapacityServiceResourceTypeDef,
-    CapacityTableTypeDef,
     CapacityTypeDef,
-    ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
     ContributorInsightsSummaryTypeDef,
     CreateBackupInputRequestTypeDef,
-    KeySchemaElementTableTypeDef,
-    ProjectionTableTypeDef,
-    ProvisionedThroughputTableTypeDef,
     KeySchemaElementTypeDef,
     ProjectionTypeDef,
     ProvisionedThroughputTypeDef,
     ReplicaTypeDef,
     CreateReplicaActionTypeDef,
-    ProvisionedThroughputOverrideTableTypeDef,
     ProvisionedThroughputOverrideTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
     TagTypeDef,
-    KeySchemaElementServiceResourceTypeDef,
-    ProvisionedThroughputServiceResourceTypeDef,
-    SSESpecificationServiceResourceTypeDef,
-    StreamSpecificationServiceResourceTypeDef,
-    TagServiceResourceTypeDef,
     CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
-    DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
-    ExpectedAttributeValueTableTypeDef,
-    ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
-    DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
-    DeleteRequestServiceResourceOutputTypeDef,
-    DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
-    KeySchemaElementTableOutputTypeDef,
-    ProjectionTableOutputTypeDef,
-    ProvisionedThroughputDescriptionTableTypeDef,
-    KeySchemaElementOutputTypeDef,
     ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
-    ProvisionedThroughputOutputTypeDef,
-    ProjectionServiceResourceTypeDef,
-    ReplicaOutputTypeDef,
-    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
-    TagTableTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    ProvisionedThroughputOverrideOutputTypeDef,
-    ProvisionedThroughputOverrideTableOutputTypeDef,
-    PutRequestServiceResourceOutputTypeDef,
-    PutRequestServiceResourceTypeDef,
-    TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
-    SSESpecificationOutputTypeDef,
-    SSESpecificationTableTypeDef,
-    StreamSpecificationOutputTypeDef,
-    StreamSpecificationTableOutputTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
-    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
+    ArchivalSummaryResponseTypeDef,
+    BillingModeSummaryResponseTypeDef,
+    DescribeLimitsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListTablesOutputTypeDef,
+    ProvisionedThroughputDescriptionResponseTypeDef,
+    RestoreSummaryResponseTypeDef,
+    SSEDescriptionResponseTypeDef,
+    StreamSpecificationResponseTypeDef,
+    TableClassSummaryResponseTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
     DeleteRequestOutputTypeDef,
@@ -644,177 +554,151 @@
     PutRequestOutputTypeDef,
     PutRequestTypeDef,
     PutTypeDef,
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
-    ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
-    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    ConsumedCapacityServiceResourceTypeDef,
-    ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    QueryInputTableQueryTypeDef,
-    ScanInputScanPaginateTypeDef,
-    ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    CreateGlobalSecondaryIndexActionTableTypeDef,
-    UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
     GlobalSecondaryIndexTypeDef,
+    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    ReplicaGlobalSecondaryIndexTableTypeDef,
+    GlobalTableTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
-    DeleteItemInputTableDeleteItemTypeDef,
-    PutItemInputTablePutItemTypeDef,
-    UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
-    GlobalSecondaryIndexDescriptionTableTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
     LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
-    GlobalSecondaryIndexOutputTypeDef,
-    SourceTableDetailsTypeDef,
-    GlobalSecondaryIndexServiceResourceTypeDef,
-    LocalSecondaryIndexServiceResourceTypeDef,
-    GlobalTableTypeDef,
     ImportSummaryTypeDef,
-    ListTagsOfResourceOutputTableTypeDef,
-    ListTagsOfResourceOutputTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
-    WriteRequestServiceResourceOutputTypeDef,
-    WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveOutputTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
+    UpdateTimeToLiveOutputTypeDef,
     BatchStatementResponseTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
+    QueryInputQueryPaginateTypeDef,
     QueryInputRequestTypeDef,
+    QueryInputTableQueryTypeDef,
     ScanInputRequestTypeDef,
+    ScanInputScanPaginateTypeDef,
+    ScanInputTableScanTypeDef,
     DeleteItemInputRequestTypeDef,
+    DeleteItemInputTableDeleteItemTypeDef,
     PutItemInputRequestTypeDef,
+    PutItemInputTablePutItemTypeDef,
     UpdateItemInputRequestTypeDef,
+    UpdateItemInputTableUpdateItemTypeDef,
     TransactGetItemTypeDef,
     BatchGetItemInputRequestTypeDef,
+    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     ExecuteTransactionInputRequestTypeDef,
     WriteRequestOutputTypeDef,
     WriteRequestTypeDef,
     TransactWriteItemTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
-    BatchGetItemOutputServiceResourceTypeDef,
-    DeleteItemOutputTableTypeDef,
-    GetItemOutputTableTypeDef,
-    PutItemOutputTableTypeDef,
-    QueryOutputTableTypeDef,
-    ScanOutputTableTypeDef,
-    UpdateItemOutputTableTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
-    GlobalSecondaryIndexUpdateTableTypeDef,
     CreateTableInputRequestTypeDef,
+    CreateTableInputServiceResourceCreateTableTypeDef,
     RestoreTableFromBackupInputRequestTypeDef,
     RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    CreateReplicationGroupMemberActionTableTypeDef,
-    UpdateReplicationGroupMemberActionTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
+    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
-    SourceTableFeatureDetailsTypeDef,
     TableCreationParametersOutputTypeDef,
-    CreateTableInputServiceResourceCreateTableTypeDef,
-    ListGlobalTablesOutputTypeDef,
+    SourceTableFeatureDetailsTypeDef,
     ListImportsOutputTypeDef,
-    ReplicaDescriptionTypeDef,
-    ReplicaDescriptionTableTypeDef,
-    BatchWriteItemOutputServiceResourceTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     BatchExecuteStatementOutputTypeDef,
     TransactGetItemsInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
     BatchWriteItemInputRequestTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     ImportTableInputRequestTypeDef,
-    ReplicationGroupUpdateTableTypeDef,
-    ReplicationGroupUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    TableDescriptionTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    ImportTableDescriptionTypeDef,
+    BackupDescriptionTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
-    UpdateTableInputRequestTypeDef,
-    DeleteBackupOutputTypeDef,
-    DescribeBackupOutputTypeDef,
-    DescribeImportOutputTypeDef,
-    ImportTableOutputTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
+    UpdateTableInputRequestTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    DescribeImportOutputTypeDef,
+    ImportTableOutputTypeDef,
+    DeleteBackupOutputTypeDef,
+    DescribeBackupOutputTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ArchivalSummaryTableResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__init__.py` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__init__.pyi` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/__main__.py` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDB 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.DynamoDB 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/client.py` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,59 +311,55 @@
         self,
         *,
         TableName: str,
         Key: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
@@ -522,30 +518,28 @@
     def execute_statement(
         self,
         *,
         Statement: str,
         Parameters: Sequence[
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ]
         ] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         Limit: int = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
@@ -611,30 +605,28 @@
         self,
         *,
         TableName: str,
         Key: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
@@ -747,59 +739,55 @@
         self,
         *,
         TableName: str,
         Item: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
@@ -820,57 +808,53 @@
         QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ExclusiveStartKey: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...
     ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
@@ -928,58 +912,54 @@
         Select: SelectType = ...,
         ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ExclusiveStartKey: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ConsistentRead: bool = ...
     ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
@@ -1100,30 +1080,28 @@
         self,
         *,
         TableName: str,
         Key: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
@@ -1131,30 +1109,28 @@
         UpdateExpression: str = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
```

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/client.pyi` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -297,59 +297,55 @@
         self,
         *,
         TableName: str,
         Key: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
@@ -491,30 +487,28 @@
     def execute_statement(
         self,
         *,
         Statement: str,
         Parameters: Sequence[
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ]
         ] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         Limit: int = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
@@ -576,30 +570,28 @@
         self,
         *,
         TableName: str,
         Key: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
@@ -703,59 +695,55 @@
         self,
         *,
         TableName: str,
         Item: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
@@ -775,57 +763,53 @@
         QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ExclusiveStartKey: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...
     ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
@@ -880,58 +864,54 @@
         Select: SelectType = ...,
         ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ExclusiveStartKey: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ConsistentRead: bool = ...
     ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
@@ -1043,30 +1023,28 @@
         self,
         *,
         TableName: str,
         Key: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
@@ -1074,30 +1052,28 @@
         UpdateExpression: str = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
```

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/literals.py` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/literals.pyi` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/paginator.py` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -36,109 +36,103 @@
 from .literals import (
     BackupTypeFilterType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     SelectType,
 )
 from .type_defs import (
-    ConditionTableTypeDef,
-    ListBackupsOutputTableTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTagsOfResourceOutputTableTypeDef,
+    ConditionTypeDef,
+    ListBackupsOutputTypeDef,
+    ListTablesOutputTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     PaginatorConfigTypeDef,
-    QueryOutputTableTypeDef,
-    ScanOutputTableTypeDef,
+    QueryOutputTypeDef,
+    ScanOutputTypeDef,
 )
 
 __all__ = (
     "ListBackupsPaginator",
     "ListTablesPaginator",
     "ListTagsOfResourcePaginator",
     "QueryPaginator",
     "ScanPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListBackupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
     """
 
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: Union[datetime, str] = ...,
         TimeRangeUpperBound: Union[datetime, str] = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListBackupsOutputTableTypeDef]:
+        PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListBackupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
         """
 
-
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTablesOutputTableTypeDef]:
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
         """
 
-
 class ListTagsOfResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsOfResourceOutputTableTypeDef]:
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListTagsOfResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
-
 class QueryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
     """
 
     def paginate(
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
@@ -157,36 +151,35 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[QueryOutputTableTypeDef]:
+        PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[QueryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
-
 class ScanPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
     """
 
     def paginate(
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
@@ -206,13 +199,13 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ScanOutputTableTypeDef]:
+        PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ScanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/service_resource.py` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/service_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,54 +35,48 @@
     ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    AttributeDefinitionServiceResourceTypeDef,
-    AttributeDefinitionTableOutputTypeDef,
-    AttributeDefinitionTableTypeDef,
-    AttributeValueUpdateTableTypeDef,
-    BatchGetItemOutputServiceResourceTypeDef,
-    BatchWriteItemOutputServiceResourceTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
-    ConditionTableTypeDef,
-    DeleteItemOutputTableTypeDef,
-    DeleteTableOutputTableTypeDef,
-    ExpectedAttributeValueTableTypeDef,
-    GetItemOutputTableTypeDef,
-    GlobalSecondaryIndexDescriptionTableTypeDef,
-    GlobalSecondaryIndexServiceResourceTypeDef,
-    GlobalSecondaryIndexUpdateTableTypeDef,
-    KeysAndAttributesServiceResourceTypeDef,
-    KeySchemaElementServiceResourceTypeDef,
-    KeySchemaElementTableOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
-    LocalSecondaryIndexServiceResourceTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    ProvisionedThroughputServiceResourceTypeDef,
-    ProvisionedThroughputTableTypeDef,
-    PutItemOutputTableTypeDef,
-    QueryOutputTableTypeDef,
-    ReplicaDescriptionTableTypeDef,
-    ReplicationGroupUpdateTableTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    ScanOutputTableTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    SSESpecificationServiceResourceTypeDef,
-    SSESpecificationTableTypeDef,
-    StreamSpecificationServiceResourceTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    StreamSpecificationTableTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
-    TagServiceResourceTypeDef,
-    UpdateItemOutputTableTypeDef,
-    WriteRequestServiceResourceTypeDef,
+    ArchivalSummaryResponseTypeDef,
+    AttributeDefinitionTypeDef,
+    AttributeValueUpdateTypeDef,
+    BatchGetItemOutputTypeDef,
+    BatchWriteItemOutputTypeDef,
+    BillingModeSummaryResponseTypeDef,
+    ConditionTypeDef,
+    DeleteItemOutputTypeDef,
+    DeleteTableOutputTypeDef,
+    ExpectedAttributeValueTypeDef,
+    GetItemOutputTypeDef,
+    GlobalSecondaryIndexDescriptionTypeDef,
+    GlobalSecondaryIndexTypeDef,
+    GlobalSecondaryIndexUpdateTypeDef,
+    KeysAndAttributesTypeDef,
+    KeySchemaElementTypeDef,
+    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexTypeDef,
+    ProvisionedThroughputDescriptionResponseTypeDef,
+    ProvisionedThroughputTypeDef,
+    PutItemOutputTypeDef,
+    QueryOutputTypeDef,
+    ReplicaDescriptionTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    RestoreSummaryResponseTypeDef,
+    ScanOutputTypeDef,
+    SSEDescriptionResponseTypeDef,
+    SSESpecificationTypeDef,
+    StreamSpecificationResponseTypeDef,
+    StreamSpecificationTypeDef,
+    TableClassSummaryResponseTypeDef,
+    TagTypeDef,
+    UpdateItemOutputTypeDef,
+    WriteRequestTypeDef,
 )
 
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
 
 class ServiceResourceTablesCollection(ResourceCollection):
     """
@@ -143,48 +137,48 @@
 
 class Table(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#table)
     """
 
-    attribute_definitions: List[AttributeDefinitionTableOutputTypeDef]
+    attribute_definitions: List[AttributeDefinitionTypeDef]
     table_name: str
-    key_schema: List[KeySchemaElementTableOutputTypeDef]
+    key_schema: List[KeySchemaElementTypeDef]
     table_status: TableStatusType
     creation_date_time: datetime
-    provisioned_throughput: ProvisionedThroughputDescriptionTableResponseMetadataTypeDef
+    provisioned_throughput: ProvisionedThroughputDescriptionResponseTypeDef
     table_size_bytes: int
     item_count: int
     table_arn: str
     table_id: str
-    billing_mode_summary: BillingModeSummaryTableResponseMetadataTypeDef
-    local_secondary_indexes: List[LocalSecondaryIndexDescriptionTableTypeDef]
-    global_secondary_indexes: List[GlobalSecondaryIndexDescriptionTableTypeDef]
-    stream_specification: StreamSpecificationTableResponseMetadataTypeDef
+    billing_mode_summary: BillingModeSummaryResponseTypeDef
+    local_secondary_indexes: List[LocalSecondaryIndexDescriptionTypeDef]
+    global_secondary_indexes: List[GlobalSecondaryIndexDescriptionTypeDef]
+    stream_specification: StreamSpecificationResponseTypeDef
     latest_stream_label: str
     latest_stream_arn: str
     global_table_version: str
-    replicas: List[ReplicaDescriptionTableTypeDef]
-    restore_summary: RestoreSummaryTableResponseMetadataTypeDef
-    sse_description: SSEDescriptionTableResponseMetadataTypeDef
-    archival_summary: ArchivalSummaryTableResponseMetadataTypeDef
-    table_class_summary: TableClassSummaryTableResponseMetadataTypeDef
+    replicas: List[ReplicaDescriptionTypeDef]
+    restore_summary: RestoreSummaryResponseTypeDef
+    sse_description: SSEDescriptionResponseTypeDef
+    archival_summary: ArchivalSummaryResponseTypeDef
+    table_class_summary: TableClassSummaryResponseTypeDef
     deletion_protection_enabled: bool
     name: str
 
     def batch_writer(self, overwrite_by_pkeys: List[str] = ...) -> BatchWriter:
         """
         Create a batch writer object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablebatch_writer-method)
         """
 
-    def delete(self) -> DeleteTableOutputTableTypeDef:
+    def delete(self) -> DeleteTableOutputTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tabledelete-method)
         """
 
@@ -206,15 +200,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: Union[str, ConditionBase] = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
@@ -233,15 +227,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> DeleteItemOutputTableTypeDef:
+    ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tabledelete_item-method)
         """
 
@@ -276,15 +270,15 @@
             ],
         ],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
-    ) -> GetItemOutputTableTypeDef:
+    ) -> GetItemOutputTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableget_item-method)
         """
@@ -316,15 +310,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: Union[str, ConditionBase] = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
@@ -343,15 +337,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> PutItemOutputTableTypeDef:
+    ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableput_item-method)
         """
 
@@ -359,16 +353,16 @@
         self,
         *,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ExclusiveStartKey: Mapping[
             str,
             Union[
                 bytes,
                 bytearray,
@@ -406,15 +400,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...
-    ) -> QueryOutputTableTypeDef:
+    ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablequery-method)
         """
@@ -431,15 +425,15 @@
     def scan(
         self,
         *,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ExclusiveStartKey: Mapping[
             str,
             Union[
                 bytes,
                 bytearray,
                 str,
@@ -478,33 +472,33 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...
-    ) -> ScanOutputTableTypeDef:
+    ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablescan-method)
         """
 
     def update(
         self,
         *,
-        AttributeDefinitions: Sequence[AttributeDefinitionTableTypeDef] = ...,
+        AttributeDefinitions: Sequence[AttributeDefinitionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
-        ProvisionedThroughput: ProvisionedThroughputTableTypeDef = ...,
-        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTableTypeDef] = ...,
-        StreamSpecification: StreamSpecificationTableTypeDef = ...,
-        SSESpecification: SSESpecificationTableTypeDef = ...,
-        ReplicaUpdates: Sequence[ReplicationGroupUpdateTableTypeDef] = ...,
+        ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
+        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
+        StreamSpecification: StreamSpecificationTypeDef = ...,
+        SSESpecification: SSESpecificationTypeDef = ...,
+        ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> "_Table":
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given table.
 
@@ -530,16 +524,16 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
-        AttributeUpdates: Mapping[str, AttributeValueUpdateTableTypeDef] = ...,
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: Union[str, ConditionBase] = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
@@ -559,15 +553,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> UpdateItemOutputTableTypeDef:
+    ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableupdate_item-method)
         """
@@ -612,53 +606,53 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcetable-method)
         """
 
     def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, KeysAndAttributesServiceResourceTypeDef],
+        RequestItems: Mapping[str, KeysAndAttributesTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
-    ) -> BatchGetItemOutputServiceResourceTypeDef:
+    ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_get_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcebatch_get_item-method)
         """
 
     def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
+        RequestItems: Mapping[str, Sequence[WriteRequestTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
-    ) -> BatchWriteItemOutputServiceResourceTypeDef:
+    ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_write_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcebatch_write_item-method)
         """
 
     def create_table(
         self,
         *,
-        AttributeDefinitions: Sequence[AttributeDefinitionServiceResourceTypeDef],
+        AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
-        KeySchema: Sequence[KeySchemaElementServiceResourceTypeDef],
-        LocalSecondaryIndexes: Sequence[LocalSecondaryIndexServiceResourceTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexServiceResourceTypeDef] = ...,
+        KeySchema: Sequence[KeySchemaElementTypeDef],
+        LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         BillingMode: BillingModeType = ...,
-        ProvisionedThroughput: ProvisionedThroughputServiceResourceTypeDef = ...,
-        StreamSpecification: StreamSpecificationServiceResourceTypeDef = ...,
-        SSESpecification: SSESpecificationServiceResourceTypeDef = ...,
-        Tags: Sequence[TagServiceResourceTypeDef] = ...,
+        ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
+        StreamSpecification: StreamSpecificationTypeDef = ...,
+        SSESpecification: SSESpecificationTypeDef = ...,
+        Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> _Table:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)
```

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/service_resource.pyi` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/service_resource.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -35,54 +35,48 @@
     ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    AttributeDefinitionServiceResourceTypeDef,
-    AttributeDefinitionTableOutputTypeDef,
-    AttributeDefinitionTableTypeDef,
-    AttributeValueUpdateTableTypeDef,
-    BatchGetItemOutputServiceResourceTypeDef,
-    BatchWriteItemOutputServiceResourceTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
-    ConditionTableTypeDef,
-    DeleteItemOutputTableTypeDef,
-    DeleteTableOutputTableTypeDef,
-    ExpectedAttributeValueTableTypeDef,
-    GetItemOutputTableTypeDef,
-    GlobalSecondaryIndexDescriptionTableTypeDef,
-    GlobalSecondaryIndexServiceResourceTypeDef,
-    GlobalSecondaryIndexUpdateTableTypeDef,
-    KeysAndAttributesServiceResourceTypeDef,
-    KeySchemaElementServiceResourceTypeDef,
-    KeySchemaElementTableOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
-    LocalSecondaryIndexServiceResourceTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    ProvisionedThroughputServiceResourceTypeDef,
-    ProvisionedThroughputTableTypeDef,
-    PutItemOutputTableTypeDef,
-    QueryOutputTableTypeDef,
-    ReplicaDescriptionTableTypeDef,
-    ReplicationGroupUpdateTableTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    ScanOutputTableTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    SSESpecificationServiceResourceTypeDef,
-    SSESpecificationTableTypeDef,
-    StreamSpecificationServiceResourceTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    StreamSpecificationTableTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
-    TagServiceResourceTypeDef,
-    UpdateItemOutputTableTypeDef,
-    WriteRequestServiceResourceTypeDef,
+    ArchivalSummaryResponseTypeDef,
+    AttributeDefinitionTypeDef,
+    AttributeValueUpdateTypeDef,
+    BatchGetItemOutputTypeDef,
+    BatchWriteItemOutputTypeDef,
+    BillingModeSummaryResponseTypeDef,
+    ConditionTypeDef,
+    DeleteItemOutputTypeDef,
+    DeleteTableOutputTypeDef,
+    ExpectedAttributeValueTypeDef,
+    GetItemOutputTypeDef,
+    GlobalSecondaryIndexDescriptionTypeDef,
+    GlobalSecondaryIndexTypeDef,
+    GlobalSecondaryIndexUpdateTypeDef,
+    KeysAndAttributesTypeDef,
+    KeySchemaElementTypeDef,
+    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexTypeDef,
+    ProvisionedThroughputDescriptionResponseTypeDef,
+    ProvisionedThroughputTypeDef,
+    PutItemOutputTypeDef,
+    QueryOutputTypeDef,
+    ReplicaDescriptionTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    RestoreSummaryResponseTypeDef,
+    ScanOutputTypeDef,
+    SSEDescriptionResponseTypeDef,
+    SSESpecificationTypeDef,
+    StreamSpecificationResponseTypeDef,
+    StreamSpecificationTypeDef,
+    TableClassSummaryResponseTypeDef,
+    TagTypeDef,
+    UpdateItemOutputTypeDef,
+    WriteRequestTypeDef,
 )
 
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
 class ServiceResourceTablesCollection(ResourceCollection):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
@@ -136,47 +130,47 @@
 
 class Table(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#table)
     """
 
-    attribute_definitions: List[AttributeDefinitionTableOutputTypeDef]
+    attribute_definitions: List[AttributeDefinitionTypeDef]
     table_name: str
-    key_schema: List[KeySchemaElementTableOutputTypeDef]
+    key_schema: List[KeySchemaElementTypeDef]
     table_status: TableStatusType
     creation_date_time: datetime
-    provisioned_throughput: ProvisionedThroughputDescriptionTableResponseMetadataTypeDef
+    provisioned_throughput: ProvisionedThroughputDescriptionResponseTypeDef
     table_size_bytes: int
     item_count: int
     table_arn: str
     table_id: str
-    billing_mode_summary: BillingModeSummaryTableResponseMetadataTypeDef
-    local_secondary_indexes: List[LocalSecondaryIndexDescriptionTableTypeDef]
-    global_secondary_indexes: List[GlobalSecondaryIndexDescriptionTableTypeDef]
-    stream_specification: StreamSpecificationTableResponseMetadataTypeDef
+    billing_mode_summary: BillingModeSummaryResponseTypeDef
+    local_secondary_indexes: List[LocalSecondaryIndexDescriptionTypeDef]
+    global_secondary_indexes: List[GlobalSecondaryIndexDescriptionTypeDef]
+    stream_specification: StreamSpecificationResponseTypeDef
     latest_stream_label: str
     latest_stream_arn: str
     global_table_version: str
-    replicas: List[ReplicaDescriptionTableTypeDef]
-    restore_summary: RestoreSummaryTableResponseMetadataTypeDef
-    sse_description: SSEDescriptionTableResponseMetadataTypeDef
-    archival_summary: ArchivalSummaryTableResponseMetadataTypeDef
-    table_class_summary: TableClassSummaryTableResponseMetadataTypeDef
+    replicas: List[ReplicaDescriptionTypeDef]
+    restore_summary: RestoreSummaryResponseTypeDef
+    sse_description: SSEDescriptionResponseTypeDef
+    archival_summary: ArchivalSummaryResponseTypeDef
+    table_class_summary: TableClassSummaryResponseTypeDef
     deletion_protection_enabled: bool
     name: str
 
     def batch_writer(self, overwrite_by_pkeys: List[str] = ...) -> BatchWriter:
         """
         Create a batch writer object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablebatch_writer-method)
         """
-    def delete(self) -> DeleteTableOutputTableTypeDef:
+    def delete(self) -> DeleteTableOutputTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tabledelete-method)
         """
     def delete_item(
@@ -197,15 +191,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: Union[str, ConditionBase] = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
@@ -224,15 +218,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> DeleteItemOutputTableTypeDef:
+    ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tabledelete_item-method)
         """
     def get_available_subresources(self) -> Sequence[str]:
@@ -265,15 +259,15 @@
             ],
         ],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
-    ) -> GetItemOutputTableTypeDef:
+    ) -> GetItemOutputTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableget_item-method)
         """
@@ -303,15 +297,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: Union[str, ConditionBase] = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[
@@ -330,31 +324,31 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> PutItemOutputTableTypeDef:
+    ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableput_item-method)
         """
     def query(
         self,
         *,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ExclusiveStartKey: Mapping[
             str,
             Union[
                 bytes,
                 bytearray,
@@ -392,15 +386,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...
-    ) -> QueryOutputTableTypeDef:
+    ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablequery-method)
         """
@@ -415,15 +409,15 @@
     def scan(
         self,
         *,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ExclusiveStartKey: Mapping[
             str,
             Union[
                 bytes,
                 bytearray,
                 str,
@@ -462,32 +456,32 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...
-    ) -> ScanOutputTableTypeDef:
+    ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablescan-method)
         """
     def update(
         self,
         *,
-        AttributeDefinitions: Sequence[AttributeDefinitionTableTypeDef] = ...,
+        AttributeDefinitions: Sequence[AttributeDefinitionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
-        ProvisionedThroughput: ProvisionedThroughputTableTypeDef = ...,
-        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTableTypeDef] = ...,
-        StreamSpecification: StreamSpecificationTableTypeDef = ...,
-        SSESpecification: SSESpecificationTableTypeDef = ...,
-        ReplicaUpdates: Sequence[ReplicationGroupUpdateTableTypeDef] = ...,
+        ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
+        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
+        StreamSpecification: StreamSpecificationTypeDef = ...,
+        SSESpecification: SSESpecificationTypeDef = ...,
+        ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> "_Table":
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given table.
 
@@ -512,16 +506,16 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
-        AttributeUpdates: Mapping[str, AttributeValueUpdateTableTypeDef] = ...,
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: Union[str, ConditionBase] = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
@@ -541,15 +535,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> UpdateItemOutputTableTypeDef:
+    ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableupdate_item-method)
         """
@@ -588,51 +582,51 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcetable-method)
         """
     def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, KeysAndAttributesServiceResourceTypeDef],
+        RequestItems: Mapping[str, KeysAndAttributesTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
-    ) -> BatchGetItemOutputServiceResourceTypeDef:
+    ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_get_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcebatch_get_item-method)
         """
     def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
+        RequestItems: Mapping[str, Sequence[WriteRequestTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
-    ) -> BatchWriteItemOutputServiceResourceTypeDef:
+    ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_write_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcebatch_write_item-method)
         """
     def create_table(
         self,
         *,
-        AttributeDefinitions: Sequence[AttributeDefinitionServiceResourceTypeDef],
+        AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
-        KeySchema: Sequence[KeySchemaElementServiceResourceTypeDef],
-        LocalSecondaryIndexes: Sequence[LocalSecondaryIndexServiceResourceTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexServiceResourceTypeDef] = ...,
+        KeySchema: Sequence[KeySchemaElementTypeDef],
+        LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         BillingMode: BillingModeType = ...,
-        ProvisionedThroughput: ProvisionedThroughputServiceResourceTypeDef = ...,
-        StreamSpecification: StreamSpecificationServiceResourceTypeDef = ...,
-        SSESpecification: SSESpecificationServiceResourceTypeDef = ...,
-        Tags: Sequence[TagServiceResourceTypeDef] = ...,
+        ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
+        StreamSpecification: StreamSpecificationTypeDef = ...,
+        SSESpecification: SSESpecificationTypeDef = ...,
+        Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> _Table:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)
```

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/type_defs.py` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/type_defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dynamodb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dynamodb.type_defs import ArchivalSummaryTableResponseMetadataTypeDef
+    from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef
 
-    data: ArchivalSummaryTableResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -60,152 +60,94 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ArchivalSummaryTableResponseMetadataTypeDef",
-    "ArchivalSummaryTableTypeDef",
+    "ResponseMetadataTypeDef",
     "ArchivalSummaryTypeDef",
-    "AttributeDefinitionOutputTypeDef",
-    "AttributeDefinitionServiceResourceTypeDef",
-    "AttributeDefinitionTableOutputTypeDef",
-    "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
-    "AttributeValueServiceResourceTypeDef",
-    "AttributeValueTableTypeDef",
     "AttributeValueTypeDef",
-    "AttributeValueUpdateTableTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
-    "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
-    "KeysAndAttributesServiceResourceTypeDef",
-    "KeysAndAttributesServiceResourceOutputTypeDef",
-    "ItemCollectionMetricsServiceResourceTypeDef",
-    "BillingModeSummaryTableResponseMetadataTypeDef",
-    "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
-    "CapacityServiceResourceTypeDef",
-    "CapacityTableTypeDef",
     "CapacityTypeDef",
-    "ConditionTableTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
     "ContributorInsightsSummaryTypeDef",
     "CreateBackupInputRequestTypeDef",
-    "KeySchemaElementTableTypeDef",
-    "ProjectionTableTypeDef",
-    "ProvisionedThroughputTableTypeDef",
     "KeySchemaElementTypeDef",
     "ProjectionTypeDef",
     "ProvisionedThroughputTypeDef",
     "ReplicaTypeDef",
     "CreateReplicaActionTypeDef",
-    "ProvisionedThroughputOverrideTableTypeDef",
     "ProvisionedThroughputOverrideTypeDef",
     "SSESpecificationTypeDef",
     "StreamSpecificationTypeDef",
     "TagTypeDef",
-    "KeySchemaElementServiceResourceTypeDef",
-    "ProvisionedThroughputServiceResourceTypeDef",
-    "SSESpecificationServiceResourceTypeDef",
-    "StreamSpecificationServiceResourceTypeDef",
-    "TagServiceResourceTypeDef",
     "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
-    "DeleteGlobalSecondaryIndexActionTableTypeDef",
     "DeleteGlobalSecondaryIndexActionTypeDef",
-    "ExpectedAttributeValueTableTypeDef",
-    "ItemCollectionMetricsTableTypeDef",
     "DeleteReplicaActionTypeDef",
-    "DeleteReplicationGroupMemberActionTableTypeDef",
     "DeleteReplicationGroupMemberActionTypeDef",
-    "DeleteRequestServiceResourceOutputTypeDef",
-    "DeleteRequestServiceResourceTypeDef",
     "DeleteTableInputRequestTypeDef",
     "DescribeBackupInputRequestTypeDef",
     "DescribeContinuousBackupsInputRequestTypeDef",
     "DescribeContributorInsightsInputRequestTypeDef",
     "FailureExceptionTypeDef",
     "EndpointTypeDef",
     "DescribeExportInputRequestTypeDef",
     "ExportDescriptionTypeDef",
     "DescribeGlobalTableInputRequestTypeDef",
     "DescribeGlobalTableSettingsInputRequestTypeDef",
     "DescribeImportInputRequestTypeDef",
     "DescribeKinesisStreamingDestinationInputRequestTypeDef",
     "KinesisDataStreamDestinationTypeDef",
-    "DescribeLimitsOutputTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportSummaryTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "GetItemInputTableGetItemTypeDef",
-    "KeySchemaElementTableOutputTypeDef",
-    "ProjectionTableOutputTypeDef",
-    "ProvisionedThroughputDescriptionTableTypeDef",
-    "KeySchemaElementOutputTypeDef",
     "ProjectionOutputTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
-    "ProvisionedThroughputOutputTypeDef",
-    "ProjectionServiceResourceTypeDef",
-    "ReplicaOutputTypeDef",
-    "S3BucketSourceOutputTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
-    "KinesisStreamingDestinationOutputTypeDef",
-    "ListBackupsInputListBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListTablesInputListTablesPaginateTypeDef",
     "ListTablesInputRequestTypeDef",
-    "ListTablesOutputTableTypeDef",
-    "ListTablesOutputTypeDef",
-    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
-    "TagTableTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
-    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
-    "ProvisionedThroughputOverrideOutputTypeDef",
-    "ProvisionedThroughputOverrideTableOutputTypeDef",
-    "PutRequestServiceResourceOutputTypeDef",
-    "PutRequestServiceResourceTypeDef",
-    "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreSummaryTableResponseMetadataTypeDef",
-    "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
-    "SSEDescriptionTableResponseMetadataTypeDef",
-    "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
-    "SSESpecificationOutputTypeDef",
-    "SSESpecificationTableTypeDef",
-    "StreamSpecificationOutputTypeDef",
-    "StreamSpecificationTableOutputTypeDef",
-    "StreamSpecificationTableResponseMetadataTypeDef",
-    "StreamSpecificationTableTypeDef",
     "TableBatchWriterRequestTypeDef",
-    "TableClassSummaryTableResponseMetadataTypeDef",
-    "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
+    "ArchivalSummaryResponseTypeDef",
+    "BillingModeSummaryResponseTypeDef",
+    "DescribeLimitsOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "KinesisStreamingDestinationOutputTypeDef",
+    "ListTablesOutputTypeDef",
+    "ProvisionedThroughputDescriptionResponseTypeDef",
+    "RestoreSummaryResponseTypeDef",
+    "SSEDescriptionResponseTypeDef",
+    "StreamSpecificationResponseTypeDef",
+    "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementErrorTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
     "DeleteRequestOutputTypeDef",
@@ -223,279 +165,178 @@
     "PutRequestOutputTypeDef",
     "PutRequestTypeDef",
     "PutTypeDef",
     "UpdateTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
-    "ListBackupsOutputTableTypeDef",
     "ListBackupsOutputTypeDef",
-    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    "ConsumedCapacityServiceResourceTypeDef",
-    "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
-    "QueryInputQueryPaginateTypeDef",
-    "QueryInputTableQueryTypeDef",
-    "ScanInputScanPaginateTypeDef",
-    "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
-    "CreateGlobalSecondaryIndexActionTableTypeDef",
-    "UpdateGlobalSecondaryIndexActionTableTypeDef",
     "LocalSecondaryIndexTypeDef",
     "CreateGlobalSecondaryIndexActionTypeDef",
     "GlobalSecondaryIndexTypeDef",
+    "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
     "CreateGlobalTableInputRequestTypeDef",
-    "ReplicaGlobalSecondaryIndexTableTypeDef",
+    "GlobalTableTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexTypeDef",
+    "ListTagsOfResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "InputFormatOptionsOutputTypeDef",
     "InputFormatOptionsTypeDef",
-    "DeleteItemInputTableDeleteItemTypeDef",
-    "PutItemInputTablePutItemTypeDef",
-    "UpdateItemInputTableUpdateItemTypeDef",
     "ReplicaUpdateTypeDef",
     "DescribeContributorInsightsOutputTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DescribeExportOutputTypeDef",
     "ExportTableToPointInTimeOutputTypeDef",
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     "DescribeTableInputTableExistsWaitTypeDef",
     "DescribeTableInputTableNotExistsWaitTypeDef",
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
-    "LocalSecondaryIndexDescriptionTableTypeDef",
-    "GlobalSecondaryIndexDescriptionTableTypeDef",
+    "GlobalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexOutputTypeDef",
     "LocalSecondaryIndexDescriptionTypeDef",
     "LocalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
-    "GlobalSecondaryIndexInfoTypeDef",
-    "GlobalSecondaryIndexOutputTypeDef",
-    "SourceTableDetailsTypeDef",
-    "GlobalSecondaryIndexServiceResourceTypeDef",
-    "LocalSecondaryIndexServiceResourceTypeDef",
-    "GlobalTableTypeDef",
     "ImportSummaryTypeDef",
-    "ListTagsOfResourceOutputTableTypeDef",
-    "ListTagsOfResourceOutputTypeDef",
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    "ListTablesInputListTablesPaginateTypeDef",
+    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
-    "WriteRequestServiceResourceOutputTypeDef",
-    "WriteRequestServiceResourceTypeDef",
-    "UpdateTimeToLiveOutputTypeDef",
     "UpdateTimeToLiveInputRequestTypeDef",
+    "UpdateTimeToLiveOutputTypeDef",
     "BatchStatementResponseTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
+    "QueryInputQueryPaginateTypeDef",
     "QueryInputRequestTypeDef",
+    "QueryInputTableQueryTypeDef",
     "ScanInputRequestTypeDef",
+    "ScanInputScanPaginateTypeDef",
+    "ScanInputTableScanTypeDef",
     "DeleteItemInputRequestTypeDef",
+    "DeleteItemInputTableDeleteItemTypeDef",
     "PutItemInputRequestTypeDef",
+    "PutItemInputTablePutItemTypeDef",
     "UpdateItemInputRequestTypeDef",
+    "UpdateItemInputTableUpdateItemTypeDef",
     "TransactGetItemTypeDef",
     "BatchGetItemInputRequestTypeDef",
+    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "ExecuteTransactionInputRequestTypeDef",
     "WriteRequestOutputTypeDef",
     "WriteRequestTypeDef",
     "TransactWriteItemTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
-    "BatchGetItemOutputServiceResourceTypeDef",
-    "DeleteItemOutputTableTypeDef",
-    "GetItemOutputTableTypeDef",
-    "PutItemOutputTableTypeDef",
-    "QueryOutputTableTypeDef",
-    "ScanOutputTableTypeDef",
-    "UpdateItemOutputTableTypeDef",
     "BatchGetItemOutputTypeDef",
     "DeleteItemOutputTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ExecuteTransactionOutputTypeDef",
     "GetItemOutputTypeDef",
     "PutItemOutputTypeDef",
     "QueryOutputTypeDef",
     "ScanOutputTypeDef",
     "TransactGetItemsOutputTypeDef",
     "TransactWriteItemsOutputTypeDef",
     "UpdateItemOutputTypeDef",
     "DescribeContinuousBackupsOutputTypeDef",
     "UpdateContinuousBackupsOutputTypeDef",
-    "GlobalSecondaryIndexUpdateTableTypeDef",
     "CreateTableInputRequestTypeDef",
+    "CreateTableInputServiceResourceCreateTableTypeDef",
     "RestoreTableFromBackupInputRequestTypeDef",
     "RestoreTableToPointInTimeInputRequestTypeDef",
     "TableCreationParametersTypeDef",
     "GlobalSecondaryIndexUpdateTypeDef",
-    "CreateReplicationGroupMemberActionTableTypeDef",
-    "UpdateReplicationGroupMemberActionTableTypeDef",
+    "ListGlobalTablesOutputTypeDef",
+    "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
-    "SourceTableFeatureDetailsTypeDef",
     "TableCreationParametersOutputTypeDef",
-    "CreateTableInputServiceResourceCreateTableTypeDef",
-    "ListGlobalTablesOutputTypeDef",
+    "SourceTableFeatureDetailsTypeDef",
     "ListImportsOutputTypeDef",
-    "ReplicaDescriptionTypeDef",
-    "ReplicaDescriptionTableTypeDef",
-    "BatchWriteItemOutputServiceResourceTypeDef",
-    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "BatchExecuteStatementOutputTypeDef",
     "TransactGetItemsInputRequestTypeDef",
     "BatchWriteItemOutputTypeDef",
     "BatchWriteItemInputRequestTypeDef",
+    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "TransactWriteItemsInputRequestTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ImportTableInputRequestTypeDef",
-    "ReplicationGroupUpdateTableTypeDef",
-    "ReplicationGroupUpdateTypeDef",
-    "BackupDescriptionTypeDef",
-    "ImportTableDescriptionTypeDef",
     "GlobalTableDescriptionTypeDef",
     "TableDescriptionTypeDef",
-    "TableDescriptionTableTypeDef",
+    "ReplicationGroupUpdateTypeDef",
+    "ImportTableDescriptionTypeDef",
+    "BackupDescriptionTypeDef",
     "ReplicaAutoScalingDescriptionTypeDef",
     "ReplicaSettingsDescriptionTypeDef",
     "ReplicaAutoScalingUpdateTypeDef",
     "ReplicaSettingsUpdateTypeDef",
-    "UpdateTableInputTableUpdateTypeDef",
-    "UpdateTableInputRequestTypeDef",
-    "DeleteBackupOutputTypeDef",
-    "DescribeBackupOutputTypeDef",
-    "DescribeImportOutputTypeDef",
-    "ImportTableOutputTypeDef",
     "CreateGlobalTableOutputTypeDef",
     "DescribeGlobalTableOutputTypeDef",
     "UpdateGlobalTableOutputTypeDef",
     "CreateTableOutputTypeDef",
     "DeleteTableOutputTypeDef",
     "DescribeTableOutputTypeDef",
     "RestoreTableFromBackupOutputTypeDef",
     "RestoreTableToPointInTimeOutputTypeDef",
     "UpdateTableOutputTypeDef",
-    "DeleteTableOutputTableTypeDef",
+    "UpdateTableInputRequestTypeDef",
+    "UpdateTableInputTableUpdateTypeDef",
+    "DescribeImportOutputTypeDef",
+    "ImportTableOutputTypeDef",
+    "DeleteBackupOutputTypeDef",
+    "DescribeBackupOutputTypeDef",
     "TableAutoScalingDescriptionTypeDef",
     "DescribeGlobalTableSettingsOutputTypeDef",
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
 )
 
-ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryTableResponseMetadataTypeDef",
-    {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ArchivalSummaryTableTypeDef = TypedDict(
-    "ArchivalSummaryTableTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 ArchivalSummaryTypeDef = TypedDict(
     "ArchivalSummaryTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
     total=False,
 )
 
-AttributeDefinitionOutputTypeDef = TypedDict(
-    "AttributeDefinitionOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
-)
-
-AttributeDefinitionServiceResourceTypeDef = TypedDict(
-    "AttributeDefinitionServiceResourceTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
-)
-
-AttributeDefinitionTableOutputTypeDef = TypedDict(
-    "AttributeDefinitionTableOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
-)
-
-AttributeDefinitionTableTypeDef = TypedDict(
-    "AttributeDefinitionTableTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
-)
-
 AttributeDefinitionTypeDef = TypedDict(
     "AttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
-AttributeValueServiceResourceTypeDef = TypedDict(
-    "AttributeValueServiceResourceTypeDef",
-    {
-        "S": str,
-        "N": str,
-        "B": bytes,
-        "SS": List[str],
-        "NS": List[str],
-        "BS": List[bytes],
-        "M": Dict[str, Dict[str, Any]],
-        "L": List[Dict[str, Any]],
-        "NULL": bool,
-        "BOOL": bool,
-    },
-    total=False,
-)
-
-AttributeValueTableTypeDef = TypedDict(
-    "AttributeValueTableTypeDef",
-    {
-        "S": str,
-        "N": str,
-        "B": bytes,
-        "SS": List[str],
-        "NS": List[str],
-        "BS": List[bytes],
-        "M": Dict[str, Dict[str, Any]],
-        "L": List[Dict[str, Any]],
-        "NULL": bool,
-        "BOOL": bool,
-    },
-    total=False,
-)
-
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": str,
         "B": bytes,
         "SS": Sequence[str],
@@ -505,38 +346,14 @@
         "L": Sequence[Any],
         "NULL": bool,
         "BOOL": bool,
     },
     total=False,
 )
 
-AttributeValueUpdateTableTypeDef = TypedDict(
-    "AttributeValueUpdateTableTypeDef",
-    {
-        "Value": Union[
-            bytes,
-            bytearray,
-            str,
-            int,
-            Decimal,
-            bool,
-            Set[int],
-            Set[Decimal],
-            Set[str],
-            Set[bytes],
-            Set[bytearray],
-            Sequence[Any],
-            Mapping[str, Any],
-            None,
-        ],
-        "Action": AttributeActionType,
-    },
-    total=False,
-)
-
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
@@ -601,31 +418,14 @@
 )
 
 
 class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
     pass
 
 
-BackupSummaryTableTypeDef = TypedDict(
-    "BackupSummaryTableTypeDef",
-    {
-        "TableName": str,
-        "TableId": str,
-        "TableArn": str,
-        "BackupArn": str,
-        "BackupName": str,
-        "BackupCreationDateTime": datetime,
-        "BackupExpiryDateTime": datetime,
-        "BackupStatus": BackupStatusType,
-        "BackupType": BackupTypeType,
-        "BackupSizeBytes": int,
-    },
-    total=False,
-)
-
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
@@ -635,186 +435,33 @@
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
     total=False,
 )
 
-_RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
-    "_RequiredKeysAndAttributesServiceResourceTypeDef",
-    {
-        "Keys": Sequence[
-            Mapping[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
-    },
-)
-_OptionalKeysAndAttributesServiceResourceTypeDef = TypedDict(
-    "_OptionalKeysAndAttributesServiceResourceTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class KeysAndAttributesServiceResourceTypeDef(
-    _RequiredKeysAndAttributesServiceResourceTypeDef,
-    _OptionalKeysAndAttributesServiceResourceTypeDef,
-):
-    pass
-
-
-_RequiredKeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
-    "_RequiredKeysAndAttributesServiceResourceOutputTypeDef",
-    {
-        "Keys": List[Dict[str, "AttributeValueServiceResourceTypeDef"]],
-    },
-)
-_OptionalKeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
-    "_OptionalKeysAndAttributesServiceResourceOutputTypeDef",
-    {
-        "AttributesToGet": List[str],
-        "ConsistentRead": bool,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class KeysAndAttributesServiceResourceOutputTypeDef(
-    _RequiredKeysAndAttributesServiceResourceOutputTypeDef,
-    _OptionalKeysAndAttributesServiceResourceOutputTypeDef,
-):
-    pass
-
-
-ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
-    "ItemCollectionMetricsServiceResourceTypeDef",
-    {
-        "ItemCollectionKey": Dict[str, "AttributeValueServiceResourceTypeDef"],
-        "SizeEstimateRangeGB": List[float],
-    },
-    total=False,
-)
-
-BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryTableResponseMetadataTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BillingModeSummaryTableTypeDef = TypedDict(
-    "BillingModeSummaryTableTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-    },
-    total=False,
-)
-
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
     total=False,
 )
 
-CapacityServiceResourceTypeDef = TypedDict(
-    "CapacityServiceResourceTypeDef",
-    {
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "CapacityUnits": float,
-    },
-    total=False,
-)
-
-CapacityTableTypeDef = TypedDict(
-    "CapacityTableTypeDef",
-    {
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "CapacityUnits": float,
-    },
-    total=False,
-)
-
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
     total=False,
 )
 
-_RequiredConditionTableTypeDef = TypedDict(
-    "_RequiredConditionTableTypeDef",
-    {
-        "ComparisonOperator": ComparisonOperatorType,
-    },
-)
-_OptionalConditionTableTypeDef = TypedDict(
-    "_OptionalConditionTableTypeDef",
-    {
-        "AttributeValueList": Sequence[
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
-    },
-    total=False,
-)
-
-
-class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
-    pass
-
-
 PointInTimeRecoveryDescriptionTypeDef = TypedDict(
     "PointInTimeRecoveryDescriptionTypeDef",
     {
         "PointInTimeRecoveryStatus": PointInTimeRecoveryStatusType,
         "EarliestRestorableDateTime": datetime,
         "LatestRestorableDateTime": datetime,
     },
@@ -835,39 +482,14 @@
     "CreateBackupInputRequestTypeDef",
     {
         "TableName": str,
         "BackupName": str,
     },
 )
 
-KeySchemaElementTableTypeDef = TypedDict(
-    "KeySchemaElementTableTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
-ProjectionTableTypeDef = TypedDict(
-    "ProjectionTableTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": Sequence[str],
-    },
-    total=False,
-)
-
-ProvisionedThroughputTableTypeDef = TypedDict(
-    "ProvisionedThroughputTableTypeDef",
-    {
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
 KeySchemaElementTypeDef = TypedDict(
     "KeySchemaElementTypeDef",
     {
         "AttributeName": str,
         "KeyType": KeyTypeType,
     },
 )
@@ -900,22 +522,14 @@
 CreateReplicaActionTypeDef = TypedDict(
     "CreateReplicaActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
-ProvisionedThroughputOverrideTableTypeDef = TypedDict(
-    "ProvisionedThroughputOverrideTableTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-    total=False,
-)
-
 ProvisionedThroughputOverrideTypeDef = TypedDict(
     "ProvisionedThroughputOverrideTypeDef",
     {
         "ReadCapacityUnits": int,
     },
     total=False,
 )
@@ -955,70 +569,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-KeySchemaElementServiceResourceTypeDef = TypedDict(
-    "KeySchemaElementServiceResourceTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
-ProvisionedThroughputServiceResourceTypeDef = TypedDict(
-    "ProvisionedThroughputServiceResourceTypeDef",
-    {
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
-SSESpecificationServiceResourceTypeDef = TypedDict(
-    "SSESpecificationServiceResourceTypeDef",
-    {
-        "Enabled": bool,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyId": str,
-    },
-    total=False,
-)
-
-_RequiredStreamSpecificationServiceResourceTypeDef = TypedDict(
-    "_RequiredStreamSpecificationServiceResourceTypeDef",
-    {
-        "StreamEnabled": bool,
-    },
-)
-_OptionalStreamSpecificationServiceResourceTypeDef = TypedDict(
-    "_OptionalStreamSpecificationServiceResourceTypeDef",
-    {
-        "StreamViewType": StreamViewTypeType,
-    },
-    total=False,
-)
-
-
-class StreamSpecificationServiceResourceTypeDef(
-    _RequiredStreamSpecificationServiceResourceTypeDef,
-    _OptionalStreamSpecificationServiceResourceTypeDef,
-):
-    pass
-
-
-TagServiceResourceTypeDef = TypedDict(
-    "TagServiceResourceTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 CsvOptionsOutputTypeDef = TypedDict(
     "CsvOptionsOutputTypeDef",
     {
         "Delimiter": str,
         "HeaderList": List[str],
     },
     total=False,
@@ -1036,133 +594,35 @@
 DeleteBackupInputRequestTypeDef = TypedDict(
     "DeleteBackupInputRequestTypeDef",
     {
         "BackupArn": str,
     },
 )
 
-DeleteGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "DeleteGlobalSecondaryIndexActionTableTypeDef",
-    {
-        "IndexName": str,
-    },
-)
-
 DeleteGlobalSecondaryIndexActionTypeDef = TypedDict(
     "DeleteGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
     },
 )
 
-ExpectedAttributeValueTableTypeDef = TypedDict(
-    "ExpectedAttributeValueTableTypeDef",
-    {
-        "Value": Union[
-            bytes,
-            bytearray,
-            str,
-            int,
-            Decimal,
-            bool,
-            Set[int],
-            Set[Decimal],
-            Set[str],
-            Set[bytes],
-            Set[bytearray],
-            Sequence[Any],
-            Mapping[str, Any],
-            None,
-        ],
-        "Exists": bool,
-        "ComparisonOperator": ComparisonOperatorType,
-        "AttributeValueList": Sequence[
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
-    },
-    total=False,
-)
-
-ItemCollectionMetricsTableTypeDef = TypedDict(
-    "ItemCollectionMetricsTableTypeDef",
-    {
-        "ItemCollectionKey": Dict[str, "AttributeValueTableTypeDef"],
-        "SizeEstimateRangeGB": List[float],
-    },
-    total=False,
-)
-
 DeleteReplicaActionTypeDef = TypedDict(
     "DeleteReplicaActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
-DeleteReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "DeleteReplicationGroupMemberActionTableTypeDef",
-    {
-        "RegionName": str,
-    },
-)
-
 DeleteReplicationGroupMemberActionTypeDef = TypedDict(
     "DeleteReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
-DeleteRequestServiceResourceOutputTypeDef = TypedDict(
-    "DeleteRequestServiceResourceOutputTypeDef",
-    {
-        "Key": Dict[str, "AttributeValueServiceResourceTypeDef"],
-    },
-)
-
-DeleteRequestServiceResourceTypeDef = TypedDict(
-    "DeleteRequestServiceResourceTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-
 DeleteTableInputRequestTypeDef = TypedDict(
     "DeleteTableInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 
@@ -1286,25 +746,14 @@
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
     total=False,
 )
 
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "AccountMaxReadCapacityUnits": int,
-        "AccountMaxWriteCapacityUnits": int,
-        "TableMaxReadCapacityUnits": int,
-        "TableMaxWriteCapacityUnits": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 
@@ -1336,21 +785,14 @@
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
     total=False,
@@ -1424,51 +866,14 @@
 
 class GetItemInputTableGetItemTypeDef(
     _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
 
-KeySchemaElementTableOutputTypeDef = TypedDict(
-    "KeySchemaElementTableOutputTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
-ProjectionTableOutputTypeDef = TypedDict(
-    "ProjectionTableOutputTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": List[str],
-    },
-    total=False,
-)
-
-ProvisionedThroughputDescriptionTableTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionTableTypeDef",
-    {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-    total=False,
-)
-
-KeySchemaElementOutputTypeDef = TypedDict(
-    "KeySchemaElementOutputTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
 ProjectionOutputTypeDef = TypedDict(
     "ProjectionOutputTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": List[str],
     },
     total=False,
@@ -1482,61 +887,14 @@
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
     total=False,
 )
 
-ProvisionedThroughputOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
-ProjectionServiceResourceTypeDef = TypedDict(
-    "ProjectionServiceResourceTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": Sequence[str],
-    },
-    total=False,
-)
-
-ReplicaOutputTypeDef = TypedDict(
-    "ReplicaOutputTypeDef",
-    {
-        "RegionName": str,
-    },
-    total=False,
-)
-
-_RequiredS3BucketSourceOutputTypeDef = TypedDict(
-    "_RequiredS3BucketSourceOutputTypeDef",
-    {
-        "S3Bucket": str,
-    },
-)
-_OptionalS3BucketSourceOutputTypeDef = TypedDict(
-    "_OptionalS3BucketSourceOutputTypeDef",
-    {
-        "S3BucketOwner": str,
-        "S3KeyPrefix": str,
-    },
-    total=False,
-)
-
-
-class S3BucketSourceOutputTypeDef(
-    _RequiredS3BucketSourceOutputTypeDef, _OptionalS3BucketSourceOutputTypeDef
-):
-    pass
-
-
 _RequiredS3BucketSourceTypeDef = TypedDict(
     "_RequiredS3BucketSourceTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalS3BucketSourceTypeDef = TypedDict(
@@ -1557,32 +915,20 @@
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
 
-KinesisStreamingDestinationOutputTypeDef = TypedDict(
-    "KinesisStreamingDestinationOutputTypeDef",
-    {
-        "TableName": str,
-        "StreamArn": str,
-        "DestinationStatus": DestinationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
-    "ListBackupsInputListBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "BackupType": BackupTypeFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
@@ -1632,71 +978,23 @@
         "TableArn": str,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTablesInputListTablesPaginateTypeDef = TypedDict(
-    "ListTablesInputListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTablesInputRequestTypeDef = TypedDict(
     "ListTablesInputRequestTypeDef",
     {
         "ExclusiveStartTableName": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTablesOutputTypeDef = TypedDict(
-    "ListTablesOutputTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
-    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsOfResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsOfResourceInputRequestTypeDef = TypedDict(
@@ -1710,170 +1008,30 @@
 
 class ListTagsOfResourceInputRequestTypeDef(
     _RequiredListTagsOfResourceInputRequestTypeDef, _OptionalListTagsOfResourceInputRequestTypeDef
 ):
     pass
 
 
-TagTableTypeDef = TypedDict(
-    "TagTableTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
-ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
-    {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ProvisionedThroughputOverrideOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOverrideOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-    total=False,
-)
-
-ProvisionedThroughputOverrideTableOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOverrideTableOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-    total=False,
-)
-
-PutRequestServiceResourceOutputTypeDef = TypedDict(
-    "PutRequestServiceResourceOutputTypeDef",
-    {
-        "Item": Dict[str, "AttributeValueServiceResourceTypeDef"],
-    },
-)
-
-PutRequestServiceResourceTypeDef = TypedDict(
-    "PutRequestServiceResourceTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-
-TableClassSummaryTableTypeDef = TypedDict(
-    "TableClassSummaryTableTypeDef",
-    {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-    },
-    total=False,
-)
-
 TableClassSummaryTypeDef = TypedDict(
     "TableClassSummaryTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryTableResponseMetadataTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredRestoreSummaryTableTypeDef = TypedDict(
-    "_RequiredRestoreSummaryTableTypeDef",
-    {
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
-    },
-)
-_OptionalRestoreSummaryTableTypeDef = TypedDict(
-    "_OptionalRestoreSummaryTableTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-    },
-    total=False,
-)
-
-
-class RestoreSummaryTableTypeDef(
-    _RequiredRestoreSummaryTableTypeDef, _OptionalRestoreSummaryTableTypeDef
-):
-    pass
-
-
 _RequiredRestoreSummaryTypeDef = TypedDict(
     "_RequiredRestoreSummaryTypeDef",
     {
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
@@ -1887,234 +1045,209 @@
 )
 
 
 class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
     pass
 
 
-SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionTableResponseMetadataTypeDef",
-    {
-        "Status": SSEStatusType,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SSEDescriptionTableTypeDef = TypedDict(
-    "SSEDescriptionTableTypeDef",
+SSEDescriptionTypeDef = TypedDict(
+    "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
     total=False,
 )
 
-SSEDescriptionTypeDef = TypedDict(
-    "SSEDescriptionTypeDef",
+TableBatchWriterRequestTypeDef = TypedDict(
+    "TableBatchWriterRequestTypeDef",
     {
-        "Status": SSEStatusType,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
+        "overwrite_by_pkeys": List[str],
     },
     total=False,
 )
 
-SSESpecificationOutputTypeDef = TypedDict(
-    "SSESpecificationOutputTypeDef",
+TimeToLiveSpecificationTypeDef = TypedDict(
+    "TimeToLiveSpecificationTypeDef",
     {
         "Enabled": bool,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyId": str,
+        "AttributeName": str,
     },
-    total=False,
 )
 
-SSESpecificationTableTypeDef = TypedDict(
-    "SSESpecificationTableTypeDef",
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
     {
-        "Enabled": bool,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyId": str,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
-    total=False,
 )
 
-_RequiredStreamSpecificationOutputTypeDef = TypedDict(
-    "_RequiredStreamSpecificationOutputTypeDef",
+_RequiredUpdateContributorInsightsInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateContributorInsightsInputRequestTypeDef",
     {
-        "StreamEnabled": bool,
+        "TableName": str,
+        "ContributorInsightsAction": ContributorInsightsActionType,
     },
 )
-_OptionalStreamSpecificationOutputTypeDef = TypedDict(
-    "_OptionalStreamSpecificationOutputTypeDef",
+_OptionalUpdateContributorInsightsInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateContributorInsightsInputRequestTypeDef",
     {
-        "StreamViewType": StreamViewTypeType,
+        "IndexName": str,
     },
     total=False,
 )
 
 
-class StreamSpecificationOutputTypeDef(
-    _RequiredStreamSpecificationOutputTypeDef, _OptionalStreamSpecificationOutputTypeDef
+class UpdateContributorInsightsInputRequestTypeDef(
+    _RequiredUpdateContributorInsightsInputRequestTypeDef,
+    _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredStreamSpecificationTableOutputTypeDef = TypedDict(
-    "_RequiredStreamSpecificationTableOutputTypeDef",
+ArchivalSummaryResponseTypeDef = TypedDict(
+    "ArchivalSummaryResponseTypeDef",
     {
-        "StreamEnabled": bool,
+        "ArchivalDateTime": datetime,
+        "ArchivalReason": str,
+        "ArchivalBackupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStreamSpecificationTableOutputTypeDef = TypedDict(
-    "_OptionalStreamSpecificationTableOutputTypeDef",
-    {
-        "StreamViewType": StreamViewTypeType,
-    },
-    total=False,
-)
-
-
-class StreamSpecificationTableOutputTypeDef(
-    _RequiredStreamSpecificationTableOutputTypeDef, _OptionalStreamSpecificationTableOutputTypeDef
-):
-    pass
-
 
-StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationTableResponseMetadataTypeDef",
+BillingModeSummaryResponseTypeDef = TypedDict(
+    "BillingModeSummaryResponseTypeDef",
     {
-        "StreamEnabled": bool,
-        "StreamViewType": StreamViewTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BillingMode": BillingModeType,
+        "LastUpdateToPayPerRequestDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStreamSpecificationTableTypeDef = TypedDict(
-    "_RequiredStreamSpecificationTableTypeDef",
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
     {
-        "StreamEnabled": bool,
+        "AccountMaxReadCapacityUnits": int,
+        "AccountMaxWriteCapacityUnits": int,
+        "TableMaxReadCapacityUnits": int,
+        "TableMaxWriteCapacityUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStreamSpecificationTableTypeDef = TypedDict(
-    "_OptionalStreamSpecificationTableTypeDef",
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "StreamViewType": StreamViewTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class StreamSpecificationTableTypeDef(
-    _RequiredStreamSpecificationTableTypeDef, _OptionalStreamSpecificationTableTypeDef
-):
-    pass
-
-
-TableBatchWriterRequestTypeDef = TypedDict(
-    "TableBatchWriterRequestTypeDef",
+KinesisStreamingDestinationOutputTypeDef = TypedDict(
+    "KinesisStreamingDestinationOutputTypeDef",
     {
-        "overwrite_by_pkeys": List[str],
+        "TableName": str,
+        "StreamArn": str,
+        "DestinationStatus": DestinationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryTableResponseMetadataTypeDef",
+ListTablesOutputTypeDef = TypedDict(
+    "ListTablesOutputTypeDef",
     {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TimeToLiveSpecificationOutputTypeDef = TypedDict(
-    "TimeToLiveSpecificationOutputTypeDef",
+ProvisionedThroughputDescriptionResponseTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionResponseTypeDef",
     {
-        "Enabled": bool,
-        "AttributeName": str,
+        "LastIncreaseDateTime": datetime,
+        "LastDecreaseDateTime": datetime,
+        "NumberOfDecreasesToday": int,
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TimeToLiveSpecificationTypeDef = TypedDict(
-    "TimeToLiveSpecificationTypeDef",
+RestoreSummaryResponseTypeDef = TypedDict(
+    "RestoreSummaryResponseTypeDef",
     {
-        "Enabled": bool,
-        "AttributeName": str,
+        "SourceBackupArn": str,
+        "SourceTableArn": str,
+        "RestoreDateTime": datetime,
+        "RestoreInProgress": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceInputRequestTypeDef = TypedDict(
-    "UntagResourceInputRequestTypeDef",
+SSEDescriptionResponseTypeDef = TypedDict(
+    "SSEDescriptionResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "Status": SSEStatusType,
+        "SSEType": SSETypeType,
+        "KMSMasterKeyArn": str,
+        "InaccessibleEncryptionDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateContributorInsightsInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateContributorInsightsInputRequestTypeDef",
+StreamSpecificationResponseTypeDef = TypedDict(
+    "StreamSpecificationResponseTypeDef",
     {
-        "TableName": str,
-        "ContributorInsightsAction": ContributorInsightsActionType,
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateContributorInsightsInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateContributorInsightsInputRequestTypeDef",
+
+TableClassSummaryResponseTypeDef = TypedDict(
+    "TableClassSummaryResponseTypeDef",
     {
-        "IndexName": str,
+        "TableClass": TableClassType,
+        "LastUpdateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateContributorInsightsInputRequestTypeDef(
-    _RequiredUpdateContributorInsightsInputRequestTypeDef,
-    _OptionalUpdateContributorInsightsInputRequestTypeDef,
-):
-    pass
-
-
 UpdateContributorInsightsOutputTypeDef = TypedDict(
     "UpdateContributorInsightsOutputTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": Union[
             AttributeValueTypeDef,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
+            bytes,
+            bytearray,
+            str,
+            int,
+            Decimal,
+            bool,
+            Set[int],
+            Set[Decimal],
+            Set[str],
+            Set[bytes],
+            Set[bytearray],
+            Sequence[Any],
+            Mapping[str, Any],
+            None,
         ],
         "Action": AttributeActionType,
     },
     total=False,
 )
 
 BatchStatementErrorTypeDef = TypedDict(
@@ -2135,30 +1268,28 @@
 )
 _OptionalBatchStatementRequestTypeDef = TypedDict(
     "_OptionalBatchStatementRequestTypeDef",
     {
         "Parameters": Sequence[
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ]
         ],
         "ConsistentRead": bool,
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
@@ -2173,60 +1304,56 @@
 _RequiredConditionCheckTypeDef = TypedDict(
     "_RequiredConditionCheckTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "TableName": str,
         "ConditionExpression": str,
     },
 )
 _OptionalConditionCheckTypeDef = TypedDict(
     "_OptionalConditionCheckTypeDef",
     {
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
@@ -2243,30 +1370,28 @@
 )
 _OptionalConditionTypeDef = TypedDict(
     "_OptionalConditionTypeDef",
     {
         "AttributeValueList": Sequence[
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ]
         ],
     },
     total=False,
 )
 
 
@@ -2284,88 +1409,82 @@
 DeleteRequestTypeDef = TypedDict(
     "DeleteRequestTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
     },
 )
 
 _RequiredDeleteTypeDef = TypedDict(
     "_RequiredDeleteTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "TableName": str,
     },
 )
 _OptionalDeleteTypeDef = TypedDict(
     "_OptionalDeleteTypeDef",
     {
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
@@ -2382,30 +1501,28 @@
 )
 _OptionalExecuteStatementInputRequestTypeDef = TypedDict(
     "_OptionalExecuteStatementInputRequestTypeDef",
     {
         "Parameters": Sequence[
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ]
         ],
         "ConsistentRead": bool,
         "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
@@ -2421,82 +1538,76 @@
 
 
 ExpectedAttributeValueTypeDef = TypedDict(
     "ExpectedAttributeValueTypeDef",
     {
         "Value": Union[
             AttributeValueTypeDef,
+            bytes,
+            bytearray,
+            str,
+            int,
+            Decimal,
+            bool,
+            Set[int],
+            Set[Decimal],
+            Set[str],
+            Set[bytes],
+            Set[bytearray],
+            Sequence[Any],
+            Mapping[str, Any],
+            None,
+        ],
+        "Exists": bool,
+        "ComparisonOperator": ComparisonOperatorType,
+        "AttributeValueList": Sequence[
             Union[
+                AttributeValueTypeDef,
                 bytes,
                 bytearray,
                 str,
                 int,
                 Decimal,
                 bool,
                 Set[int],
                 Set[Decimal],
                 Set[str],
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
-            ],
-        ],
-        "Exists": bool,
-        "ComparisonOperator": ComparisonOperatorType,
-        "AttributeValueList": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
             ]
         ],
     },
     total=False,
 )
 
 _RequiredGetItemInputRequestTypeDef = TypedDict(
     "_RequiredGetItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
     },
 )
 _OptionalGetItemInputRequestTypeDef = TypedDict(
     "_OptionalGetItemInputRequestTypeDef",
     {
@@ -2519,30 +1630,28 @@
 _RequiredGetTypeDef = TypedDict(
     "_RequiredGetTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "TableName": str,
     },
 )
 _OptionalGetTypeDef = TypedDict(
     "_OptionalGetTypeDef",
@@ -2603,30 +1712,28 @@
     "_RequiredKeysAndAttributesTypeDef",
     {
         "Keys": Sequence[
             Mapping[
                 str,
                 Union[
                     AttributeValueTypeDef,
-                    Union[
-                        bytes,
-                        bytearray,
-                        str,
-                        int,
-                        Decimal,
-                        bool,
-                        Set[int],
-                        Set[Decimal],
-                        Set[str],
-                        Set[bytes],
-                        Set[bytearray],
-                        Sequence[Any],
-                        Mapping[str, Any],
-                        None,
-                    ],
+                    bytes,
+                    bytearray,
+                    str,
+                    int,
+                    Decimal,
+                    bool,
+                    Set[int],
+                    Set[Decimal],
+                    Set[str],
+                    Set[bytes],
+                    Set[bytearray],
+                    Sequence[Any],
+                    Mapping[str, Any],
+                    None,
                 ],
             ]
         ],
     },
 )
 _OptionalKeysAndAttributesTypeDef = TypedDict(
     "_OptionalKeysAndAttributesTypeDef",
@@ -2654,30 +1761,28 @@
 )
 _OptionalParameterizedStatementTypeDef = TypedDict(
     "_OptionalParameterizedStatementTypeDef",
     {
         "Parameters": Sequence[
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ]
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
@@ -2698,88 +1803,82 @@
 PutRequestTypeDef = TypedDict(
     "PutRequestTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
     },
 )
 
 _RequiredPutTypeDef = TypedDict(
     "_RequiredPutTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "TableName": str,
     },
 )
 _OptionalPutTypeDef = TypedDict(
     "_OptionalPutTypeDef",
     {
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
@@ -2791,30 +1890,28 @@
 _RequiredUpdateTypeDef = TypedDict(
     "_RequiredUpdateTypeDef",
     {
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "UpdateExpression": str,
         "TableName": str,
     },
 )
 _OptionalUpdateTypeDef = TypedDict(
@@ -2822,30 +1919,28 @@
     {
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
@@ -2888,322 +1983,41 @@
     pass
 
 
 CreateBackupOutputTypeDef = TypedDict(
     "CreateBackupOutputTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupsOutputTableTypeDef = TypedDict(
-    "ListBackupsOutputTableTypeDef",
-    {
-        "BackupSummaries": List[BackupSummaryTableTypeDef],
-        "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupsOutputTypeDef = TypedDict(
     "ListBackupsOutputTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    {
-        "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
-    },
-)
-_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-    },
-    total=False,
-)
-
-
-class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
-    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-):
-    pass
-
-
-ConsumedCapacityServiceResourceTypeDef = TypedDict(
-    "ConsumedCapacityServiceResourceTypeDef",
-    {
-        "TableName": str,
-        "CapacityUnits": float,
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "Table": CapacityServiceResourceTypeDef,
-        "LocalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
-        "GlobalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
-    },
-    total=False,
-)
-
-ConsumedCapacityTableTypeDef = TypedDict(
-    "ConsumedCapacityTableTypeDef",
-    {
-        "TableName": str,
-        "CapacityUnits": float,
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "Table": CapacityTableTypeDef,
-        "LocalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
-        "GlobalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
-    },
-    total=False,
-)
-
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
     total=False,
 )
 
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
-
-QueryInputTableQueryTypeDef = TypedDict(
-    "QueryInputTableQueryTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": Union[str, ConditionBase],
-        "KeyConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-    total=False,
-)
-
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
-
-ScanInputTableScanTypeDef = TypedDict(
-    "ScanInputTableScanTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-    },
-    total=False,
-)
-
 _RequiredContinuousBackupsDescriptionTypeDef = TypedDict(
     "_RequiredContinuousBackupsDescriptionTypeDef",
     {
         "ContinuousBackupsStatus": ContinuousBackupsStatusType,
     },
 )
 _OptionalContinuousBackupsDescriptionTypeDef = TypedDict(
@@ -3222,47 +2036,15 @@
 
 
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": Sequence[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
-    },
-)
-_OptionalCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "_OptionalCreateGlobalSecondaryIndexActionTableTypeDef",
-    {
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateGlobalSecondaryIndexActionTableTypeDef(
-    _RequiredCreateGlobalSecondaryIndexActionTableTypeDef,
-    _OptionalCreateGlobalSecondaryIndexActionTableTypeDef,
-):
-    pass
-
-
-UpdateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "UpdateGlobalSecondaryIndexActionTableTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LocalSecondaryIndexTypeDef = TypedDict(
     "LocalSecondaryIndexTypeDef",
     {
         "IndexName": str,
@@ -3314,14 +2096,42 @@
 
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
 
+_RequiredSourceTableDetailsTypeDef = TypedDict(
+    "_RequiredSourceTableDetailsTypeDef",
+    {
+        "TableName": str,
+        "TableId": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "TableCreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+    },
+)
+_OptionalSourceTableDetailsTypeDef = TypedDict(
+    "_OptionalSourceTableDetailsTypeDef",
+    {
+        "TableArn": str,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "BillingMode": BillingModeType,
+    },
+    total=False,
+)
+
+
+class SourceTableDetailsTypeDef(
+    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
+):
+    pass
+
+
 UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
 )
@@ -3330,36 +2140,32 @@
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": Sequence[ReplicaTypeDef],
     },
 )
 
-_RequiredReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
-    "_RequiredReplicaGlobalSecondaryIndexTableTypeDef",
+GlobalTableTypeDef = TypedDict(
+    "GlobalTableTypeDef",
     {
-        "IndexName": str,
+        "GlobalTableName": str,
+        "ReplicationGroup": List[ReplicaTypeDef],
     },
+    total=False,
 )
-_OptionalReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
-    "_OptionalReplicaGlobalSecondaryIndexTableTypeDef",
+
+ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     {
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
-
-class ReplicaGlobalSecondaryIndexTableTypeDef(
-    _RequiredReplicaGlobalSecondaryIndexTableTypeDef,
-    _OptionalReplicaGlobalSecondaryIndexTableTypeDef,
-):
-    pass
-
-
 _RequiredReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalReplicaGlobalSecondaryIndexTypeDef = TypedDict(
@@ -3373,14 +2179,23 @@
 
 class ReplicaGlobalSecondaryIndexTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTypeDef, _OptionalReplicaGlobalSecondaryIndexTypeDef
 ):
     pass
 
 
+ListTagsOfResourceOutputTypeDef = TypedDict(
+    "ListTagsOfResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -3397,211 +2212,14 @@
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class DeleteItemInputTableDeleteItemTypeDef(
-    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
-):
-    pass
-
-
-_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
-    "_RequiredPutItemInputTablePutItemTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
-    "_OptionalPutItemInputTablePutItemTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionalOperator": ConditionalOperatorType,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class PutItemInputTablePutItemTypeDef(
-    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
-):
-    pass
-
-
-_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
-    {
-        "AttributeUpdates": Mapping[str, AttributeValueUpdateTableTypeDef],
-        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "UpdateExpression": str,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class UpdateItemInputTableUpdateItemTypeDef(
-    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
-):
-    pass
-
-
 ReplicaUpdateTypeDef = TypedDict(
     "ReplicaUpdateTypeDef",
     {
         "Create": CreateReplicaActionTypeDef,
         "Delete": DeleteReplicaActionTypeDef,
     },
     total=False,
@@ -3612,48 +2230,48 @@
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsRuleList": List[str],
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "LastUpdateDateTime": datetime,
         "FailureException": FailureExceptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportOutputTypeDef = TypedDict(
     "DescribeExportOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportTableToPointInTimeOutputTypeDef = TypedDict(
     "ExportTableToPointInTimeOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKinesisStreamingDestinationOutputTypeDef = TypedDict(
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     {
         "TableName": str,
         "KinesisDataStreamDestinations": List[KinesisDataStreamDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeTableInputTableExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableExistsWaitTypeDef",
     {
         "TableName": str,
@@ -3697,289 +2315,178 @@
     pass
 
 
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTableTypeDef",
+GlobalSecondaryIndexInfoTypeDef = TypedDict(
+    "GlobalSecondaryIndexInfoTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
-        "Projection": ProjectionTableOutputTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
-GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "GlobalSecondaryIndexDescriptionTableTypeDef",
+_RequiredGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "_RequiredGlobalSecondaryIndexOutputTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
-        "Projection": ProjectionTableOutputTypeDef,
-        "IndexStatus": IndexStatusType,
-        "Backfilling": bool,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+    },
+)
+_OptionalGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "_OptionalGlobalSecondaryIndexOutputTypeDef",
+    {
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
+
+class GlobalSecondaryIndexOutputTypeDef(
+    _RequiredGlobalSecondaryIndexOutputTypeDef, _OptionalGlobalSecondaryIndexOutputTypeDef
+):
+    pass
+
+
 LocalSecondaryIndexDescriptionTypeDef = TypedDict(
     "LocalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
         "Projection": ProjectionOutputTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
     total=False,
 )
 
 LocalSecondaryIndexInfoTypeDef = TypedDict(
     "LocalSecondaryIndexInfoTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
         "Projection": ProjectionOutputTypeDef,
     },
     total=False,
 )
 
 GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
         "Projection": ProjectionOutputTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
     total=False,
 )
 
-GlobalSecondaryIndexInfoTypeDef = TypedDict(
-    "GlobalSecondaryIndexInfoTypeDef",
+ImportSummaryTypeDef = TypedDict(
+    "ImportSummaryTypeDef",
     {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "ImportArn": str,
+        "ImportStatus": ImportStatusType,
+        "TableArn": str,
+        "S3BucketSource": S3BucketSourceTypeDef,
+        "CloudWatchLogGroupArn": str,
+        "InputFormat": InputFormatType,
+        "StartTime": datetime,
+        "EndTime": datetime,
     },
     total=False,
 )
 
-_RequiredGlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "_RequiredGlobalSecondaryIndexOutputTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-    },
-)
-_OptionalGlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "_OptionalGlobalSecondaryIndexOutputTypeDef",
+ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
+    "ListBackupsInputListBackupsPaginateTypeDef",
     {
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "TableName": str,
+        "TimeRangeLowerBound": Union[datetime, str],
+        "TimeRangeUpperBound": Union[datetime, str],
+        "BackupType": BackupTypeFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class GlobalSecondaryIndexOutputTypeDef(
-    _RequiredGlobalSecondaryIndexOutputTypeDef, _OptionalGlobalSecondaryIndexOutputTypeDef
-):
-    pass
-
-
-_RequiredSourceTableDetailsTypeDef = TypedDict(
-    "_RequiredSourceTableDetailsTypeDef",
-    {
-        "TableName": str,
-        "TableId": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "TableCreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-    },
-)
-_OptionalSourceTableDetailsTypeDef = TypedDict(
-    "_OptionalSourceTableDetailsTypeDef",
+ListTablesInputListTablesPaginateTypeDef = TypedDict(
+    "ListTablesInputListTablesPaginateTypeDef",
     {
-        "TableArn": str,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "BillingMode": BillingModeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class SourceTableDetailsTypeDef(
-    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
-):
-    pass
-
-
-_RequiredGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
-    "_RequiredGlobalSecondaryIndexServiceResourceTypeDef",
+_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     {
-        "IndexName": str,
-        "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
-        "Projection": ProjectionServiceResourceTypeDef,
+        "ResourceArn": str,
     },
 )
-_OptionalGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
-    "_OptionalGlobalSecondaryIndexServiceResourceTypeDef",
+_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     {
-        "ProvisionedThroughput": ProvisionedThroughputServiceResourceTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class GlobalSecondaryIndexServiceResourceTypeDef(
-    _RequiredGlobalSecondaryIndexServiceResourceTypeDef,
-    _OptionalGlobalSecondaryIndexServiceResourceTypeDef,
+class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
+    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
 ):
     pass
 
 
-LocalSecondaryIndexServiceResourceTypeDef = TypedDict(
-    "LocalSecondaryIndexServiceResourceTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
-        "Projection": ProjectionServiceResourceTypeDef,
-    },
-)
-
-GlobalTableTypeDef = TypedDict(
-    "GlobalTableTypeDef",
-    {
-        "GlobalTableName": str,
-        "ReplicationGroup": List[ReplicaOutputTypeDef],
-    },
-    total=False,
-)
-
-ImportSummaryTypeDef = TypedDict(
-    "ImportSummaryTypeDef",
-    {
-        "ImportArn": str,
-        "ImportStatus": ImportStatusType,
-        "TableArn": str,
-        "S3BucketSource": S3BucketSourceOutputTypeDef,
-        "CloudWatchLogGroupArn": str,
-        "InputFormat": InputFormatType,
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
-
-ListTagsOfResourceOutputTableTypeDef = TypedDict(
-    "ListTagsOfResourceOutputTableTypeDef",
-    {
-        "Tags": List[TagTableTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsOfResourceOutputTypeDef = TypedDict(
-    "ListTagsOfResourceOutputTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
         "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
     },
 )
 
-ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
-    },
-    total=False,
-)
-
-ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
-    },
-    total=False,
-)
-
-WriteRequestServiceResourceOutputTypeDef = TypedDict(
-    "WriteRequestServiceResourceOutputTypeDef",
-    {
-        "PutRequest": PutRequestServiceResourceOutputTypeDef,
-        "DeleteRequest": DeleteRequestServiceResourceOutputTypeDef,
-    },
-    total=False,
-)
-
-WriteRequestServiceResourceTypeDef = TypedDict(
-    "WriteRequestServiceResourceTypeDef",
+UpdateTimeToLiveInputRequestTypeDef = TypedDict(
+    "UpdateTimeToLiveInputRequestTypeDef",
     {
-        "PutRequest": PutRequestServiceResourceTypeDef,
-        "DeleteRequest": DeleteRequestServiceResourceTypeDef,
+        "TableName": str,
+        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
     },
-    total=False,
 )
 
 UpdateTimeToLiveOutputTypeDef = TypedDict(
     "UpdateTimeToLiveOutputTypeDef",
     {
-        "TimeToLiveSpecification": TimeToLiveSpecificationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateTimeToLiveInputRequestTypeDef = TypedDict(
-    "UpdateTimeToLiveInputRequestTypeDef",
-    {
-        "TableName": str,
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
@@ -4007,14 +2514,67 @@
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
 
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+
 _RequiredQueryInputRequestTypeDef = TypedDict(
     "_RequiredQueryInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalQueryInputRequestTypeDef = TypedDict(
@@ -4029,70 +2589,125 @@
         "QueryFilter": Mapping[str, ConditionTypeDef],
         "ConditionalOperator": ConditionalOperatorType,
         "ScanIndexForward": bool,
         "ExclusiveStartKey": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "FilterExpression": str,
         "KeyConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
     },
     total=False,
 )
 
 
 class QueryInputRequestTypeDef(
     _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
 ):
     pass
 
 
+QueryInputTableQueryTypeDef = TypedDict(
+    "QueryInputTableQueryTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ExclusiveStartKey": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": Union[str, ConditionBase],
+        "KeyConditionExpression": Union[str, ConditionBase],
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+    },
+    total=False,
+)
+
 _RequiredScanInputRequestTypeDef = TypedDict(
     "_RequiredScanInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalScanInputRequestTypeDef = TypedDict(
@@ -4104,94 +2719,198 @@
         "Select": SelectType,
         "ScanFilter": Mapping[str, ConditionTypeDef],
         "ConditionalOperator": ConditionalOperatorType,
         "ExclusiveStartKey": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "TotalSegments": int,
         "Segment": int,
         "ProjectionExpression": str,
         "FilterExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
 
 class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
     pass
 
 
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
+
+ScanInputTableScanTypeDef = TypedDict(
+    "ScanInputTableScanTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ExclusiveStartKey": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": Union[str, ConditionBase],
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ConsistentRead": bool,
+    },
+    total=False,
+)
+
 _RequiredDeleteItemInputRequestTypeDef = TypedDict(
     "_RequiredDeleteItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
     },
 )
 _OptionalDeleteItemInputRequestTypeDef = TypedDict(
     "_OptionalDeleteItemInputRequestTypeDef",
     {
@@ -4202,68 +2921,129 @@
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
 ):
     pass
 
 
+_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
+    {
+        "Key": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+    },
+)
+_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionExpression": Union[str, ConditionBase],
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
+    },
+    total=False,
+)
+
+
+class DeleteItemInputTableDeleteItemTypeDef(
+    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
+):
+    pass
+
+
 _RequiredPutItemInputRequestTypeDef = TypedDict(
     "_RequiredPutItemInputRequestTypeDef",
     {
         "TableName": str,
         "Item": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
     },
 )
 _OptionalPutItemInputRequestTypeDef = TypedDict(
     "_OptionalPutItemInputRequestTypeDef",
     {
@@ -4274,68 +3054,129 @@
         "ConditionalOperator": ConditionalOperatorType,
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
     pass
 
 
+_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
+    "_RequiredPutItemInputTablePutItemTypeDef",
+    {
+        "Item": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+    },
+)
+_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
+    "_OptionalPutItemInputTablePutItemTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionalOperator": ConditionalOperatorType,
+        "ConditionExpression": Union[str, ConditionBase],
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
+    },
+    total=False,
+)
+
+
+class PutItemInputTablePutItemTypeDef(
+    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
+):
+    pass
+
+
 _RequiredUpdateItemInputRequestTypeDef = TypedDict(
     "_RequiredUpdateItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
     },
 )
 _OptionalUpdateItemInputRequestTypeDef = TypedDict(
     "_OptionalUpdateItemInputRequestTypeDef",
     {
@@ -4348,44 +3189,109 @@
         "UpdateExpression": str,
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[
             str,
             Union[
                 AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
             ],
         ],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
 
+_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
+    {
+        "Key": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+    },
+)
+_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
+    {
+        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "UpdateExpression": str,
+        "ConditionExpression": Union[str, ConditionBase],
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
+    },
+    total=False,
+)
+
+
+class UpdateItemInputTableUpdateItemTypeDef(
+    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+):
+    pass
+
+
 TransactGetItemTypeDef = TypedDict(
     "TransactGetItemTypeDef",
     {
         "Get": GetTypeDef,
     },
 )
 
@@ -4406,14 +3312,36 @@
 
 class BatchGetItemInputRequestTypeDef(
     _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
 ):
     pass
 
 
+_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "RequestItems": Mapping[str, KeysAndAttributesTypeDef],
+    },
+)
+_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+
+class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
+    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+):
+    pass
+
+
 _RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
     "_RequiredExecuteTransactionInputRequestTypeDef",
     {
         "TransactStatements": Sequence[ParameterizedStatementTypeDef],
     },
 )
 _OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
@@ -4481,224 +3409,141 @@
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicyUpdate": AutoScalingPolicyUpdateTypeDef,
     },
     total=False,
 )
 
-BatchGetItemOutputServiceResourceTypeDef = TypedDict(
-    "BatchGetItemOutputServiceResourceTypeDef",
-    {
-        "Responses": Dict[str, List[Dict[str, "AttributeValueServiceResourceTypeDef"]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteItemOutputTableTypeDef = TypedDict(
-    "DeleteItemOutputTableTypeDef",
-    {
-        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetItemOutputTableTypeDef = TypedDict(
-    "GetItemOutputTableTypeDef",
-    {
-        "Item": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutItemOutputTableTypeDef = TypedDict(
-    "PutItemOutputTableTypeDef",
-    {
-        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-QueryOutputTableTypeDef = TypedDict(
-    "QueryOutputTableTypeDef",
-    {
-        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
-        "Count": int,
-        "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ScanOutputTableTypeDef = TypedDict(
-    "ScanOutputTableTypeDef",
-    {
-        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
-        "Count": int,
-        "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateItemOutputTableTypeDef = TypedDict(
-    "UpdateItemOutputTableTypeDef",
-    {
-        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "Responses": List[ItemResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactWriteItemsOutputTypeDef = TypedDict(
     "TransactWriteItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
     "DescribeContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousBackupsOutputTypeDef = TypedDict(
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
-    "GlobalSecondaryIndexUpdateTableTypeDef",
-    {
-        "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
-        "Create": CreateGlobalSecondaryIndexActionTableTypeDef,
-        "Delete": DeleteGlobalSecondaryIndexActionTableTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateTableInputRequestTypeDef = TypedDict(
     "_RequiredCreateTableInputRequestTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "TableName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
@@ -4722,14 +3567,46 @@
 
 class CreateTableInputRequestTypeDef(
     _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+
+class CreateTableInputServiceResourceCreateTableTypeDef(
+    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
+    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
+):
+    pass
+
+
 _RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromBackupInputRequestTypeDef",
     {
         "TargetTableName": str,
         "BackupArn": str,
     },
 )
@@ -4815,64 +3692,39 @@
         "Update": UpdateGlobalSecondaryIndexActionTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_RequiredCreateReplicationGroupMemberActionTableTypeDef",
-    {
-        "RegionName": str,
-    },
-)
-_OptionalCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_OptionalCreateReplicationGroupMemberActionTableTypeDef",
+ListGlobalTablesOutputTypeDef = TypedDict(
+    "ListGlobalTablesOutputTypeDef",
     {
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-        "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
-        "TableClassOverride": TableClassType,
+        "GlobalTables": List[GlobalTableTypeDef],
+        "LastEvaluatedGlobalTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateReplicationGroupMemberActionTableTypeDef(
-    _RequiredCreateReplicationGroupMemberActionTableTypeDef,
-    _OptionalCreateReplicationGroupMemberActionTableTypeDef,
-):
-    pass
-
-
-_RequiredUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_RequiredUpdateReplicationGroupMemberActionTableTypeDef",
+ReplicaDescriptionTypeDef = TypedDict(
+    "ReplicaDescriptionTypeDef",
     {
         "RegionName": str,
-    },
-)
-_OptionalUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_OptionalUpdateReplicationGroupMemberActionTableTypeDef",
-    {
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
         "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-        "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
-        "TableClassOverride": TableClassType,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
     total=False,
 )
 
-
-class UpdateReplicationGroupMemberActionTableTypeDef(
-    _RequiredUpdateReplicationGroupMemberActionTableTypeDef,
-    _OptionalUpdateReplicationGroupMemberActionTableTypeDef,
-):
-    pass
-
-
 _RequiredCreateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalCreateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -4923,173 +3775,67 @@
     "UpdateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaUpdates": Sequence[ReplicaUpdateTypeDef],
     },
 )
 
-SourceTableFeatureDetailsTypeDef = TypedDict(
-    "SourceTableFeatureDetailsTypeDef",
-    {
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
-        "StreamDescription": StreamSpecificationOutputTypeDef,
-        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "SSEDescription": SSEDescriptionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredTableCreationParametersOutputTypeDef = TypedDict(
     "_RequiredTableCreationParametersOutputTypeDef",
     {
         "TableName": str,
-        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
     },
 )
 _OptionalTableCreationParametersOutputTypeDef = TypedDict(
     "_OptionalTableCreationParametersOutputTypeDef",
     {
         "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-        "SSESpecification": SSESpecificationOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
     },
     total=False,
 )
 
 
 class TableCreationParametersOutputTypeDef(
     _RequiredTableCreationParametersOutputTypeDef, _OptionalTableCreationParametersOutputTypeDef
 ):
     pass
 
 
-_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionServiceResourceTypeDef],
-        "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
-    },
-)
-_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
+SourceTableFeatureDetailsTypeDef = TypedDict(
+    "SourceTableFeatureDetailsTypeDef",
     {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexServiceResourceTypeDef],
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexServiceResourceTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputServiceResourceTypeDef,
-        "StreamSpecification": StreamSpecificationServiceResourceTypeDef,
-        "SSESpecification": SSESpecificationServiceResourceTypeDef,
-        "Tags": Sequence[TagServiceResourceTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
+        "StreamDescription": StreamSpecificationTypeDef,
+        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
     },
     total=False,
 )
 
-
-class CreateTableInputServiceResourceCreateTableTypeDef(
-    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
-    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
-):
-    pass
-
-
-ListGlobalTablesOutputTypeDef = TypedDict(
-    "ListGlobalTablesOutputTypeDef",
-    {
-        "GlobalTables": List[GlobalTableTypeDef],
-        "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ReplicaDescriptionTypeDef = TypedDict(
-    "ReplicaDescriptionTypeDef",
-    {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
-    },
-    total=False,
-)
-
-ReplicaDescriptionTableTypeDef = TypedDict(
-    "ReplicaDescriptionTableTypeDef",
-    {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
-    },
-    total=False,
-)
-
-BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
-    "BatchWriteItemOutputServiceResourceTypeDef",
-    {
-        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
-    {
-        "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
-    },
-)
-_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
-    {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
-    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-):
-    pass
-
-
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
@@ -5112,15 +3858,15 @@
 
 BatchWriteItemOutputTypeDef = TypedDict(
     "BatchWriteItemOutputTypeDef",
     {
         "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputRequestTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
@@ -5138,14 +3884,37 @@
 
 class BatchWriteItemInputRequestTypeDef(
     _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
 ):
     pass
 
 
+_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    {
+        "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
+    },
+)
+_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+    },
+    total=False,
+)
+
+
+class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
+    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+):
+    pass
+
+
 _RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactWriteItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactWriteItemTypeDef],
     },
 )
 _OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
@@ -5287,70 +4056,14 @@
 
 class ImportTableInputRequestTypeDef(
     _RequiredImportTableInputRequestTypeDef, _OptionalImportTableInputRequestTypeDef
 ):
     pass
 
 
-ReplicationGroupUpdateTableTypeDef = TypedDict(
-    "ReplicationGroupUpdateTableTypeDef",
-    {
-        "Create": CreateReplicationGroupMemberActionTableTypeDef,
-        "Update": UpdateReplicationGroupMemberActionTableTypeDef,
-        "Delete": DeleteReplicationGroupMemberActionTableTypeDef,
-    },
-    total=False,
-)
-
-ReplicationGroupUpdateTypeDef = TypedDict(
-    "ReplicationGroupUpdateTypeDef",
-    {
-        "Create": CreateReplicationGroupMemberActionTypeDef,
-        "Update": UpdateReplicationGroupMemberActionTypeDef,
-        "Delete": DeleteReplicationGroupMemberActionTypeDef,
-    },
-    total=False,
-)
-
-BackupDescriptionTypeDef = TypedDict(
-    "BackupDescriptionTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "SourceTableDetails": SourceTableDetailsTypeDef,
-        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
-    },
-    total=False,
-)
-
-ImportTableDescriptionTypeDef = TypedDict(
-    "ImportTableDescriptionTypeDef",
-    {
-        "ImportArn": str,
-        "ImportStatus": ImportStatusType,
-        "TableArn": str,
-        "TableId": str,
-        "ClientToken": str,
-        "S3BucketSource": S3BucketSourceOutputTypeDef,
-        "ErrorCount": int,
-        "CloudWatchLogGroupArn": str,
-        "InputFormat": InputFormatType,
-        "InputFormatOptions": InputFormatOptionsOutputTypeDef,
-        "InputCompressionType": InputCompressionTypeType,
-        "TableCreationParameters": TableCreationParametersOutputTypeDef,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ProcessedSizeBytes": int,
-        "ProcessedItemCount": int,
-        "ImportedItemCount": int,
-        "FailureCode": str,
-        "FailureMessage": str,
-    },
-    total=False,
-)
-
 GlobalTableDescriptionTypeDef = TypedDict(
     "GlobalTableDescriptionTypeDef",
     {
         "ReplicationGroup": List[ReplicaDescriptionTypeDef],
         "GlobalTableArn": str,
         "CreationDateTime": datetime,
         "GlobalTableStatus": GlobalTableStatusType,
@@ -5358,67 +4071,83 @@
     },
     total=False,
 )
 
 TableDescriptionTypeDef = TypedDict(
     "TableDescriptionTypeDef",
     {
-        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
         "TableName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
         "TableStatus": TableStatusType,
         "CreationDateTime": datetime,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "TableSizeBytes": int,
         "ItemCount": int,
         "TableArn": str,
         "TableId": str,
         "BillingModeSummary": BillingModeSummaryTypeDef,
         "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTypeDef],
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTypeDef],
-        "StreamSpecification": StreamSpecificationOutputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
         "LatestStreamLabel": str,
         "LatestStreamArn": str,
         "GlobalTableVersion": str,
         "Replicas": List[ReplicaDescriptionTypeDef],
         "RestoreSummary": RestoreSummaryTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
         "ArchivalSummary": ArchivalSummaryTypeDef,
         "TableClassSummary": TableClassSummaryTypeDef,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
-TableDescriptionTableTypeDef = TypedDict(
-    "TableDescriptionTableTypeDef",
+ReplicationGroupUpdateTypeDef = TypedDict(
+    "ReplicationGroupUpdateTypeDef",
     {
-        "AttributeDefinitions": List[AttributeDefinitionTableOutputTypeDef],
-        "TableName": str,
-        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
-        "TableStatus": TableStatusType,
-        "CreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
-        "TableSizeBytes": int,
-        "ItemCount": int,
+        "Create": CreateReplicationGroupMemberActionTypeDef,
+        "Update": UpdateReplicationGroupMemberActionTypeDef,
+        "Delete": DeleteReplicationGroupMemberActionTypeDef,
+    },
+    total=False,
+)
+
+ImportTableDescriptionTypeDef = TypedDict(
+    "ImportTableDescriptionTypeDef",
+    {
+        "ImportArn": str,
+        "ImportStatus": ImportStatusType,
         "TableArn": str,
         "TableId": str,
-        "BillingModeSummary": BillingModeSummaryTableTypeDef,
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableOutputTypeDef,
-        "LatestStreamLabel": str,
-        "LatestStreamArn": str,
-        "GlobalTableVersion": str,
-        "Replicas": List[ReplicaDescriptionTableTypeDef],
-        "RestoreSummary": RestoreSummaryTableTypeDef,
-        "SSEDescription": SSEDescriptionTableTypeDef,
-        "ArchivalSummary": ArchivalSummaryTableTypeDef,
-        "TableClassSummary": TableClassSummaryTableTypeDef,
-        "DeletionProtectionEnabled": bool,
+        "ClientToken": str,
+        "S3BucketSource": S3BucketSourceTypeDef,
+        "ErrorCount": int,
+        "CloudWatchLogGroupArn": str,
+        "InputFormat": InputFormatType,
+        "InputFormatOptions": InputFormatOptionsOutputTypeDef,
+        "InputCompressionType": InputCompressionTypeType,
+        "TableCreationParameters": TableCreationParametersOutputTypeDef,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ProcessedSizeBytes": int,
+        "ProcessedItemCount": int,
+        "ImportedItemCount": int,
+        "FailureCode": str,
+        "FailureMessage": str,
+    },
+    total=False,
+)
+
+BackupDescriptionTypeDef = TypedDict(
+    "BackupDescriptionTypeDef",
+    {
+        "BackupDetails": BackupDetailsTypeDef,
+        "SourceTableDetails": SourceTableDetailsTypeDef,
+        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
     },
     total=False,
 )
 
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
@@ -5507,168 +4236,160 @@
 
 class ReplicaSettingsUpdateTypeDef(
     _RequiredReplicaSettingsUpdateTypeDef, _OptionalReplicaSettingsUpdateTypeDef
 ):
     pass
 
 
-UpdateTableInputTableUpdateTypeDef = TypedDict(
-    "UpdateTableInputTableUpdateTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "SSESpecification": SSESpecificationTableTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
-_RequiredUpdateTableInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateTableInputRequestTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalUpdateTableInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateTableInputRequestTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
-
-class UpdateTableInputRequestTypeDef(
-    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
-):
-    pass
-
-
-DeleteBackupOutputTypeDef = TypedDict(
-    "DeleteBackupOutputTypeDef",
-    {
-        "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeBackupOutputTypeDef = TypedDict(
-    "DescribeBackupOutputTypeDef",
-    {
-        "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeImportOutputTypeDef = TypedDict(
-    "DescribeImportOutputTypeDef",
-    {
-        "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportTableOutputTypeDef = TypedDict(
-    "ImportTableOutputTypeDef",
-    {
-        "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalTableOutputTypeDef = TypedDict(
     "DescribeGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalTableOutputTypeDef = TypedDict(
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTableOutputTypeDef = TypedDict(
     "DeleteTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableOutputTypeDef = TypedDict(
     "DescribeTableOutputTypeDef",
     {
         "Table": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableFromBackupOutputTypeDef = TypedDict(
     "RestoreTableFromBackupOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableToPointInTimeOutputTypeDef = TypedDict(
     "RestoreTableToPointInTimeOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableOutputTypeDef = TypedDict(
     "UpdateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateTableInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateTableInputRequestTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalUpdateTableInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateTableInputRequestTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
     },
+    total=False,
 )
 
-DeleteTableOutputTableTypeDef = TypedDict(
-    "DeleteTableOutputTableTypeDef",
+
+class UpdateTableInputRequestTypeDef(
+    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
+):
+    pass
+
+
+UpdateTableInputTableUpdateTypeDef = TypedDict(
+    "UpdateTableInputTableUpdateTypeDef",
     {
-        "TableDescription": TableDescriptionTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+DescribeImportOutputTypeDef = TypedDict(
+    "DescribeImportOutputTypeDef",
+    {
+        "ImportTableDescription": ImportTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportTableOutputTypeDef = TypedDict(
+    "ImportTableOutputTypeDef",
+    {
+        "ImportTableDescription": ImportTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBackupOutputTypeDef = TypedDict(
+    "DeleteBackupOutputTypeDef",
+    {
+        "BackupDescription": BackupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupOutputTypeDef = TypedDict(
+    "DescribeBackupOutputTypeDef",
+    {
+        "BackupDescription": BackupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
@@ -5679,24 +4400,24 @@
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalTableSettingsOutputTypeDef = TypedDict(
     "UpdateGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef",
     {
         "TableName": str,
@@ -5750,18 +4471,18 @@
     pass
 
 
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "UpdateTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/waiter.py` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb/waiter.pyi` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/PKG-INFO` & `mypy-boto3-dynamodb-1.28.15/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.28.12
-Summary: Type annotations for boto3.DynamoDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DynamoDB 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -481,152 +481,94 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    ArchivalSummaryTableTypeDef,
+    ResponseMetadataTypeDef,
     ArchivalSummaryTypeDef,
-    AttributeDefinitionOutputTypeDef,
-    AttributeDefinitionServiceResourceTypeDef,
-    AttributeDefinitionTableOutputTypeDef,
-    AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
-    AttributeValueServiceResourceTypeDef,
-    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
-    AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
-    BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
-    KeysAndAttributesServiceResourceTypeDef,
-    KeysAndAttributesServiceResourceOutputTypeDef,
-    ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
-    BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
-    CapacityServiceResourceTypeDef,
-    CapacityTableTypeDef,
     CapacityTypeDef,
-    ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
     ContributorInsightsSummaryTypeDef,
     CreateBackupInputRequestTypeDef,
-    KeySchemaElementTableTypeDef,
-    ProjectionTableTypeDef,
-    ProvisionedThroughputTableTypeDef,
     KeySchemaElementTypeDef,
     ProjectionTypeDef,
     ProvisionedThroughputTypeDef,
     ReplicaTypeDef,
     CreateReplicaActionTypeDef,
-    ProvisionedThroughputOverrideTableTypeDef,
     ProvisionedThroughputOverrideTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
     TagTypeDef,
-    KeySchemaElementServiceResourceTypeDef,
-    ProvisionedThroughputServiceResourceTypeDef,
-    SSESpecificationServiceResourceTypeDef,
-    StreamSpecificationServiceResourceTypeDef,
-    TagServiceResourceTypeDef,
     CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
-    DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
-    ExpectedAttributeValueTableTypeDef,
-    ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
-    DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
-    DeleteRequestServiceResourceOutputTypeDef,
-    DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
-    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
-    KeySchemaElementTableOutputTypeDef,
-    ProjectionTableOutputTypeDef,
-    ProvisionedThroughputDescriptionTableTypeDef,
-    KeySchemaElementOutputTypeDef,
     ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
-    ProvisionedThroughputOutputTypeDef,
-    ProjectionServiceResourceTypeDef,
-    ReplicaOutputTypeDef,
-    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
-    TagTableTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    ProvisionedThroughputOverrideOutputTypeDef,
-    ProvisionedThroughputOverrideTableOutputTypeDef,
-    PutRequestServiceResourceOutputTypeDef,
-    PutRequestServiceResourceTypeDef,
-    TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
-    SSESpecificationOutputTypeDef,
-    SSESpecificationTableTypeDef,
-    StreamSpecificationOutputTypeDef,
-    StreamSpecificationTableOutputTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
-    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
+    ArchivalSummaryResponseTypeDef,
+    BillingModeSummaryResponseTypeDef,
+    DescribeLimitsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListTablesOutputTypeDef,
+    ProvisionedThroughputDescriptionResponseTypeDef,
+    RestoreSummaryResponseTypeDef,
+    SSEDescriptionResponseTypeDef,
+    StreamSpecificationResponseTypeDef,
+    TableClassSummaryResponseTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
     BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
     DeleteRequestOutputTypeDef,
@@ -644,177 +586,151 @@
     PutRequestOutputTypeDef,
     PutRequestTypeDef,
     PutTypeDef,
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
-    ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
-    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    ConsumedCapacityServiceResourceTypeDef,
-    ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    QueryInputTableQueryTypeDef,
-    ScanInputScanPaginateTypeDef,
-    ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    CreateGlobalSecondaryIndexActionTableTypeDef,
-    UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
     GlobalSecondaryIndexTypeDef,
+    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    ReplicaGlobalSecondaryIndexTableTypeDef,
+    GlobalTableTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
-    DeleteItemInputTableDeleteItemTypeDef,
-    PutItemInputTablePutItemTypeDef,
-    UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
-    GlobalSecondaryIndexDescriptionTableTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
     LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
-    GlobalSecondaryIndexOutputTypeDef,
-    SourceTableDetailsTypeDef,
-    GlobalSecondaryIndexServiceResourceTypeDef,
-    LocalSecondaryIndexServiceResourceTypeDef,
-    GlobalTableTypeDef,
     ImportSummaryTypeDef,
-    ListTagsOfResourceOutputTableTypeDef,
-    ListTagsOfResourceOutputTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
-    WriteRequestServiceResourceOutputTypeDef,
-    WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveOutputTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
+    UpdateTimeToLiveOutputTypeDef,
     BatchStatementResponseTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
+    QueryInputQueryPaginateTypeDef,
     QueryInputRequestTypeDef,
+    QueryInputTableQueryTypeDef,
     ScanInputRequestTypeDef,
+    ScanInputScanPaginateTypeDef,
+    ScanInputTableScanTypeDef,
     DeleteItemInputRequestTypeDef,
+    DeleteItemInputTableDeleteItemTypeDef,
     PutItemInputRequestTypeDef,
+    PutItemInputTablePutItemTypeDef,
     UpdateItemInputRequestTypeDef,
+    UpdateItemInputTableUpdateItemTypeDef,
     TransactGetItemTypeDef,
     BatchGetItemInputRequestTypeDef,
+    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     ExecuteTransactionInputRequestTypeDef,
     WriteRequestOutputTypeDef,
     WriteRequestTypeDef,
     TransactWriteItemTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
-    BatchGetItemOutputServiceResourceTypeDef,
-    DeleteItemOutputTableTypeDef,
-    GetItemOutputTableTypeDef,
-    PutItemOutputTableTypeDef,
-    QueryOutputTableTypeDef,
-    ScanOutputTableTypeDef,
-    UpdateItemOutputTableTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
-    GlobalSecondaryIndexUpdateTableTypeDef,
     CreateTableInputRequestTypeDef,
+    CreateTableInputServiceResourceCreateTableTypeDef,
     RestoreTableFromBackupInputRequestTypeDef,
     RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    CreateReplicationGroupMemberActionTableTypeDef,
-    UpdateReplicationGroupMemberActionTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
+    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
-    SourceTableFeatureDetailsTypeDef,
     TableCreationParametersOutputTypeDef,
-    CreateTableInputServiceResourceCreateTableTypeDef,
-    ListGlobalTablesOutputTypeDef,
+    SourceTableFeatureDetailsTypeDef,
     ListImportsOutputTypeDef,
-    ReplicaDescriptionTypeDef,
-    ReplicaDescriptionTableTypeDef,
-    BatchWriteItemOutputServiceResourceTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     BatchExecuteStatementOutputTypeDef,
     TransactGetItemsInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
     BatchWriteItemInputRequestTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     ImportTableInputRequestTypeDef,
-    ReplicationGroupUpdateTableTypeDef,
-    ReplicationGroupUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    TableDescriptionTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    ImportTableDescriptionTypeDef,
+    BackupDescriptionTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
-    UpdateTableInputRequestTypeDef,
-    DeleteBackupOutputTypeDef,
-    DescribeBackupOutputTypeDef,
-    DescribeImportOutputTypeDef,
-    ImportTableOutputTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
+    UpdateTableInputRequestTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    DescribeImportOutputTypeDef,
+    ImportTableOutputTypeDef,
+    DeleteBackupOutputTypeDef,
+    DescribeBackupOutputTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ArchivalSummaryTableResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.28.12/mypy_boto3_dynamodb.egg-info/SOURCES.txt` & `mypy-boto3-dynamodb-1.28.15/mypy_boto3_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.12/setup.py` & `mypy-boto3-dynamodb-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodb",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DynamoDB 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.DynamoDB 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

