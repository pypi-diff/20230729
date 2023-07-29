# Comparing `tmp/mypy-boto3-elasticache-1.28.15.tar.gz` & `tmp/mypy-boto3-elasticache-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticache-1.28.15.tar", last modified: Fri Jul 28 20:42:44 2023, max compression
+gzip compressed data, was "mypy-boto3-elasticache-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:03 2023, max compression
```

## Comparing `mypy-boto3-elasticache-1.28.15.tar` & `mypy-boto3-elasticache-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.997044 mypy-boto3-elasticache-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27283 2023-07-28 20:42:43.997044 mypy-boto3-elasticache-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.989044 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67995 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67902 2023-07-28 20:25:06.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86615 2023-07-28 20:25:11.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86548 2023-07-28 20:25:08.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.997044 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27283 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.997044 mypy-boto3-elasticache-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:03.013130 mypy-boto3-elasticache-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27289 2023-07-29 10:03:03.013130 mypy-boto3-elasticache-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.993130 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68102 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68009 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-07-29 09:44:38.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86681 2023-07-29 09:44:40.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86614 2023-07-29 09:44:39.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:35.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-29 09:44:37.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:03.013130 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27289 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:03:02.000000 mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:03.013130 mypy-boto3-elasticache-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:44:34.000000 mypy-boto3-elasticache-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-elasticache-1.28.15/LICENSE` & `mypy-boto3-elasticache-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15/PKG-INFO` & `mypy-boto3-elasticache-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.28.15
-Summary: Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -488,14 +488,15 @@
     ParameterTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
     NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     DeleteCacheClusterMessageRequestTypeDef,
     DeleteCacheParameterGroupMessageRequestTypeDef,
     DeleteCacheSecurityGroupMessageRequestTypeDef,
     DeleteCacheSubnetGroupMessageRequestTypeDef,
@@ -533,15 +534,14 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
-    NodeGroupConfigurationOutputTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
@@ -573,14 +573,15 @@
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
+    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
     DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
     DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
@@ -604,15 +605,14 @@
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
-    NodeSnapshotTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
     UpdateActionResultsMessageTypeDef,
@@ -622,45 +622,45 @@
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
+    SnapshotTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
-    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ReplicationGroupPendingModifiedValuesTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.28.15/README.md` & `mypy-boto3-elasticache-1.28.15.post1/README.md`

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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -456,14 +456,15 @@
     ParameterTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
     NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     DeleteCacheClusterMessageRequestTypeDef,
     DeleteCacheParameterGroupMessageRequestTypeDef,
     DeleteCacheSecurityGroupMessageRequestTypeDef,
     DeleteCacheSubnetGroupMessageRequestTypeDef,
@@ -501,15 +502,14 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
-    NodeGroupConfigurationOutputTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
@@ -541,14 +541,15 @@
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
+    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
     DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
     DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
@@ -572,15 +573,14 @@
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
-    NodeSnapshotTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
     UpdateActionResultsMessageTypeDef,
@@ -590,45 +590,45 @@
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
+    SnapshotTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
-    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ReplicationGroupPendingModifiedValuesTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__init__.py` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__init__.pyi` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__main__.py` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElastiCache 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.ElastiCache 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\nOther"
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

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/client.py` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     IncreaseReplicaCountResultTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     ModifyCacheClusterResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     ModifyReplicationGroupResultTypeDef,
     ModifyReplicationGroupShardConfigurationResultTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
     NodeGroupConfigurationTypeDef,
     ParameterNameValueTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     RebootCacheClusterResultTypeDef,
     RegionalConfigurationTypeDef,
     ReplicationGroupMessageTypeDef,
@@ -429,15 +430,17 @@
         PrimaryClusterId: str = ...,
         AutomaticFailoverEnabled: bool = ...,
         MultiAZEnabled: bool = ...,
         NumCacheClusters: int = ...,
         PreferredCacheClusterAZs: Sequence[str] = ...,
         NumNodeGroups: int = ...,
         ReplicasPerNodeGroup: int = ...,
-        NodeGroupConfiguration: Sequence[NodeGroupConfigurationTypeDef] = ...,
+        NodeGroupConfiguration: Sequence[
+            Union[NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef]
+        ] = ...,
         CacheNodeType: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         CacheSubnetGroupName: str = ...,
         CacheSecurityGroupNames: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
```

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/client.pyi` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     IncreaseReplicaCountResultTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     ModifyCacheClusterResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     ModifyReplicationGroupResultTypeDef,
     ModifyReplicationGroupShardConfigurationResultTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
     NodeGroupConfigurationTypeDef,
     ParameterNameValueTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     RebootCacheClusterResultTypeDef,
     RegionalConfigurationTypeDef,
     ReplicationGroupMessageTypeDef,
@@ -411,15 +412,17 @@
         PrimaryClusterId: str = ...,
         AutomaticFailoverEnabled: bool = ...,
         MultiAZEnabled: bool = ...,
         NumCacheClusters: int = ...,
         PreferredCacheClusterAZs: Sequence[str] = ...,
         NumNodeGroups: int = ...,
         ReplicasPerNodeGroup: int = ...,
-        NodeGroupConfiguration: Sequence[NodeGroupConfigurationTypeDef] = ...,
+        NodeGroupConfiguration: Sequence[
+            Union[NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef]
+        ] = ...,
         CacheNodeType: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         CacheSubnetGroupName: str = ...,
         CacheSecurityGroupNames: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
```

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/literals.py` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/literals.pyi` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/paginator.py` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/paginator.pyi` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/type_defs.py` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     "ParameterTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationOutputTypeDef",
     "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteCacheClusterMessageRequestTypeDef",
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     "DeleteCacheSecurityGroupMessageRequestTypeDef",
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
@@ -119,15 +120,14 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
-    "NodeGroupConfigurationOutputTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
@@ -159,14 +159,15 @@
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
+    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
     "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
@@ -190,15 +191,14 @@
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
-    "NodeSnapshotTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
     "UpdateActionResultsMessageTypeDef",
@@ -208,45 +208,45 @@
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
+    "SnapshotTypeDef",
     "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "DeleteGlobalReplicationGroupResultTypeDef",
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
-    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReplicationGroupPendingModifiedValuesTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -556,14 +556,28 @@
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
+NodeGroupConfigurationOutputTypeDef = TypedDict(
+    "NodeGroupConfigurationOutputTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
 NodeGroupConfigurationTypeDef = TypedDict(
     "NodeGroupConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "Slots": str,
         "ReplicaCount": int,
         "PrimaryAvailabilityZone": str,
@@ -1109,28 +1123,14 @@
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
 
-NodeGroupConfigurationOutputTypeDef = TypedDict(
-    "NodeGroupConfigurationOutputTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
-    },
-    total=False,
-)
-
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1686,14 +1686,28 @@
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
@@ -2088,28 +2102,14 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2289,14 +2289,49 @@
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 LogDeliveryConfigurationRequestTypeDef = TypedDict(
     "LogDeliveryConfigurationRequestTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
         "DestinationDetails": DestinationDetailsTypeDef,
         "LogFormat": LogFormatType,
@@ -2422,49 +2457,14 @@
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
-    {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
-        "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
-    },
-    total=False,
-)
-
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2537,14 +2537,47 @@
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalCreateCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2605,15 +2638,17 @@
         "PrimaryClusterId": str,
         "AutomaticFailoverEnabled": bool,
         "MultiAZEnabled": bool,
         "NumCacheClusters": int,
         "PreferredCacheClusterAZs": Sequence[str],
         "NumNodeGroups": int,
         "ReplicasPerNodeGroup": int,
-        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationTypeDef],
+        "NodeGroupConfiguration": Sequence[
+            Union[NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef]
+        ],
         "CacheNodeType": str,
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupName": str,
         "CacheSubnetGroupName": str,
         "CacheSecurityGroupNames": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -2766,47 +2801,14 @@
         "TransitEncryptionEnabled": bool,
         "TransitEncryptionMode": TransitEncryptionModeType,
         "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
-    {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/type_defs.pyi` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "ParameterTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationOutputTypeDef",
     "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteCacheClusterMessageRequestTypeDef",
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     "DeleteCacheSecurityGroupMessageRequestTypeDef",
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
@@ -118,15 +119,14 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
-    "NodeGroupConfigurationOutputTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
@@ -158,14 +158,15 @@
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
+    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
     "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
@@ -189,15 +190,14 @@
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
-    "NodeSnapshotTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
     "UpdateActionResultsMessageTypeDef",
@@ -207,45 +207,45 @@
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
+    "SnapshotTypeDef",
     "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "DeleteGlobalReplicationGroupResultTypeDef",
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
-    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReplicationGroupPendingModifiedValuesTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -545,14 +545,28 @@
 
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+NodeGroupConfigurationOutputTypeDef = TypedDict(
+    "NodeGroupConfigurationOutputTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
 NodeGroupConfigurationTypeDef = TypedDict(
     "NodeGroupConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "Slots": str,
         "ReplicaCount": int,
         "PrimaryAvailabilityZone": str,
@@ -1082,28 +1096,14 @@
 )
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
-NodeGroupConfigurationOutputTypeDef = TypedDict(
-    "NodeGroupConfigurationOutputTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
-    },
-    total=False,
-)
-
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1637,14 +1637,28 @@
 
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
@@ -2031,28 +2045,14 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2232,14 +2232,49 @@
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 LogDeliveryConfigurationRequestTypeDef = TypedDict(
     "LogDeliveryConfigurationRequestTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
         "DestinationDetails": DestinationDetailsTypeDef,
         "LogFormat": LogFormatType,
@@ -2363,49 +2398,14 @@
 
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
-    {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
-        "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
-    },
-    total=False,
-)
-
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2478,14 +2478,47 @@
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalCreateCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2544,15 +2577,17 @@
         "PrimaryClusterId": str,
         "AutomaticFailoverEnabled": bool,
         "MultiAZEnabled": bool,
         "NumCacheClusters": int,
         "PreferredCacheClusterAZs": Sequence[str],
         "NumNodeGroups": int,
         "ReplicasPerNodeGroup": int,
-        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationTypeDef],
+        "NodeGroupConfiguration": Sequence[
+            Union[NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef]
+        ],
         "CacheNodeType": str,
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupName": str,
         "CacheSubnetGroupName": str,
         "CacheSecurityGroupNames": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -2699,47 +2734,14 @@
         "TransitEncryptionEnabled": bool,
         "TransitEncryptionMode": TransitEncryptionModeType,
         "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
-    {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/waiter.py` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/waiter.pyi` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/PKG-INFO` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.28.15
-Summary: Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -488,14 +488,15 @@
     ParameterTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
     NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     DeleteCacheClusterMessageRequestTypeDef,
     DeleteCacheParameterGroupMessageRequestTypeDef,
     DeleteCacheSecurityGroupMessageRequestTypeDef,
     DeleteCacheSubnetGroupMessageRequestTypeDef,
@@ -533,15 +534,14 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
-    NodeGroupConfigurationOutputTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
@@ -573,14 +573,15 @@
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
+    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
     DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
     DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
@@ -604,15 +605,14 @@
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
-    NodeSnapshotTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
     UpdateActionResultsMessageTypeDef,
@@ -622,45 +622,45 @@
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
+    SnapshotTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
-    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ReplicationGroupPendingModifiedValuesTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/SOURCES.txt` & `mypy-boto3-elasticache-1.28.15.post1/mypy_boto3_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.15/setup.py` & `mypy-boto3-elasticache-1.28.15.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticache",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder"
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

