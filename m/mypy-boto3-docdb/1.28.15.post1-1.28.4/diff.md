# Comparing `tmp/mypy-boto3-docdb-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-docdb-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-docdb-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:58 2023, max compression
+gzip compressed data, was "mypy-boto3-docdb-1.28.4.tar", last modified: Tue Jul 18 01:01:42 2023, max compression
```

## Comparing `mypy-boto3-docdb-1.28.15.post1.tar` & `mypy-boto3-docdb-1.28.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.941113 mypy-boto3-docdb-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:40.000000 mypy-boto3-docdb-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22634 2023-07-29 10:02:58.933113 mypy-boto3-docdb-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-07-29 09:42:40.000000 mypy-boto3-docdb-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.933113 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-29 09:42:40.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-29 09:42:40.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:42:40.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51205 2023-07-29 09:42:42.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51130 2023-07-29 09:42:40.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-07-29 09:42:42.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-07-29 09:42:42.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-07-29 09:42:42.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-07-29 09:42:42.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:40.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60469 2023-07-29 09:42:44.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60416 2023-07-29 09:42:43.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:40.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-29 09:42:42.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-29 09:42:42.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.933113 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22634 2023-07-29 10:02:58.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-29 10:02:58.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:58.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:02:58.000000 mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:58.941113 mypy-boto3-docdb-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:42:39.000000 mypy-boto3-docdb-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22691 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51205 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51130 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60559 2023-07-18 01:00:30.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60506 2023-07-18 01:00:29.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22691 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-18 01:00:27.000000 mypy-boto3-docdb-1.28.4/setup.py
```

### Comparing `mypy-boto3-docdb-1.28.15.post1/LICENSE` & `mypy-boto3-docdb-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.15.post1/PKG-INFO` & `mypy-boto3-docdb-1.28.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DocDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.4
+Summary: Type annotations for boto3.DocDB 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -418,15 +418,15 @@
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
-    ParameterTypeDef,
+    ParameterOutputTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
@@ -440,27 +440,29 @@
     PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
+    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
@@ -472,30 +474,27 @@
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     CertificateMessageTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
     DBClusterParameterGroupsMessageTypeDef,
     CopyDBClusterSnapshotResultTypeDef,
     CreateDBClusterSnapshotResultTypeDef,
     DBClusterSnapshotMessageTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
@@ -525,16 +524,19 @@
     DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
     CreateDBClusterResultTypeDef,
     DBClusterMessageTypeDef,
```

### Comparing `mypy-boto3-docdb-1.28.15.post1/README.md` & `mypy-boto3-docdb-1.28.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -386,15 +386,15 @@
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
-    ParameterTypeDef,
+    ParameterOutputTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
@@ -408,27 +408,29 @@
     PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
+    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
@@ -440,30 +442,27 @@
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     CertificateMessageTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
     DBClusterParameterGroupsMessageTypeDef,
     CopyDBClusterSnapshotResultTypeDef,
     CreateDBClusterSnapshotResultTypeDef,
     DBClusterSnapshotMessageTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
@@ -493,16 +492,19 @@
     DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
     CreateDBClusterResultTypeDef,
     DBClusterMessageTypeDef,
```

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/__init__.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/__init__.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/__main__.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DocDB 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.DocDB 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/client.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/client.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/literals.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -273,28 +272,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/literals.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -271,28 +270,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/paginator.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/paginator.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/type_defs.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "AvailabilityZoneTypeDef",
     "CertificateTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterMemberTypeDef",
-    "ParameterTypeDef",
+    "ParameterOutputTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "EndpointTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
@@ -54,27 +54,29 @@
     "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
+    "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
+    "TagOutputTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
     "DBClusterParameterGroupNameMessageTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
@@ -86,30 +88,27 @@
     "CreateDBClusterParameterGroupMessageRequestTypeDef",
     "CreateDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
     "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
-    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionTypeDef",
     "SubnetTypeDef",
     "CertificateMessageTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
     "DBClusterParameterGroupsMessageTypeDef",
     "CopyDBClusterSnapshotResultTypeDef",
     "CreateDBClusterSnapshotResultTypeDef",
     "DBClusterSnapshotMessageTypeDef",
     "DeleteDBClusterSnapshotResultTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBClusterTypeDef",
     "DBEngineVersionTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
@@ -139,16 +138,19 @@
     "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
+    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     "CreateDBClusterResultTypeDef",
     "DBClusterMessageTypeDef",
@@ -196,15 +198,14 @@
         "SubscriptionCreationTime": str,
         "SourceType": str,
         "SourceIdsList": List[str],
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -233,28 +234,26 @@
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateIdentifier": str,
         "CertificateType": str,
         "Thumbprint": str,
         "ValidFrom": datetime,
         "ValidTill": datetime,
         "CertificateArn": str,
     },
-    total=False,
 )
 
 CloudwatchLogsExportConfigurationTypeDef = TypedDict(
     "CloudwatchLogsExportConfigurationTypeDef",
     {
         "EnableLogTypes": Sequence[str],
         "DisableLogTypes": Sequence[str],
@@ -266,15 +265,14 @@
     "DBClusterParameterGroupTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBClusterParameterGroupArn": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotTypeDef = TypedDict(
     "DBClusterSnapshotTypeDef",
     {
         "AvailabilityZones": List[str],
         "DBClusterSnapshotIdentifier": str,
@@ -290,15 +288,14 @@
         "SnapshotType": str,
         "PercentProgress": int,
         "StorageEncrypted": bool,
         "KmsKeyId": str,
         "DBClusterSnapshotArn": str,
         "SourceDBClusterSnapshotArn": str,
     },
-    total=False,
 )
 
 _RequiredCreateGlobalClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
     },
@@ -328,92 +325,84 @@
     "DBClusterMemberTypeDef",
     {
         "DBInstanceIdentifier": str,
         "IsClusterWriter": bool,
         "DBClusterParameterGroupStatus": str,
         "PromotionTier": int,
     },
-    total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "ApplyType": str,
         "DataType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
     },
-    total=False,
 )
 
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotAttributeTypeDef = TypedDict(
     "DBClusterSnapshotAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[str],
     },
-    total=False,
 )
 
 VpcSecurityGroupMembershipTypeDef = TypedDict(
     "VpcSecurityGroupMembershipTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
-    total=False,
 )
 
 UpgradeTargetTypeDef = TypedDict(
     "UpgradeTargetTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "Description": str,
         "AutoUpgrade": bool,
         "IsMajorVersionUpgrade": bool,
     },
-    total=False,
 )
 
 DBInstanceStatusInfoTypeDef = TypedDict(
     "DBInstanceStatusInfoTypeDef",
     {
         "StatusType": str,
         "Normal": bool,
         "Status": str,
         "Message": str,
     },
-    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "Port": int,
         "HostedZoneId": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -512,28 +501,26 @@
 
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
-    total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
         "SourceArn": str,
     },
-    total=False,
 )
 
 FailoverDBClusterMessageRequestTypeDef = TypedDict(
     "FailoverDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "TargetDBInstanceIdentifier": str,
@@ -544,14 +531,30 @@
 GlobalClusterMemberTypeDef = TypedDict(
     "GlobalClusterMemberTypeDef",
     {
         "DBClusterArn": str,
         "Readers": List[str],
         "IsWriter": bool,
     },
+)
+
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+        "Description": str,
+        "Source": str,
+        "ApplyType": str,
+        "DataType": str,
+        "AllowedValues": str,
+        "IsModifiable": bool,
+        "MinimumEngineVersion": str,
+        "ApplyMethod": ApplyMethodType,
+    },
     total=False,
 )
 
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
@@ -678,28 +681,26 @@
 
 PendingCloudwatchLogsExportsTypeDef = TypedDict(
     "PendingCloudwatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
-    total=False,
 )
 
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 _RequiredRebootDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredRebootDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
@@ -753,14 +754,22 @@
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1110,43 +1119,33 @@
 class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
     _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
     _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
 ):
     pass
 
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "Vpc": bool,
     },
-    total=False,
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
-    total=False,
 )
 
 CertificateMessageTypeDef = TypedDict(
     "CertificateMessageTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "Marker": str,
@@ -1244,68 +1243,35 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterTypeDef],
-    },
-    total=False,
-)
-
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
     },
 )
 
-_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-    total=False,
-)
-
-
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
-    total=False,
 )
 
 DBClusterTypeDef = TypedDict(
     "DBClusterTypeDef",
     {
         "AvailabilityZones": List[str],
         "BackupRetentionPeriod": int,
@@ -1336,30 +1302,28 @@
         "DBClusterArn": str,
         "AssociatedRoles": List[DBClusterRoleTypeDef],
         "CloneGroupId": str,
         "ClusterCreateTime": datetime,
         "EnabledCloudwatchLogsExports": List[str],
         "DeletionProtection": bool,
     },
-    total=False,
 )
 
 DBEngineVersionTypeDef = TypedDict(
     "DBEngineVersionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "DBEngineDescription": str,
         "DBEngineVersionDescription": str,
         "ValidUpgradeTarget": List[UpgradeTargetTypeDef],
         "ExportableLogTypes": List[str],
         "SupportsLogExportsToCloudwatchLogs": bool,
     },
-    total=False,
 )
 
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "CertificateIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1829,17 +1793,47 @@
         "Engine": str,
         "EngineVersion": str,
         "DatabaseName": str,
         "StorageEncrypted": bool,
         "DeletionProtection": bool,
         "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
     },
+)
+
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
     total=False,
 )
 
+
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
 PendingModifiedValuesTypeDef = TypedDict(
     "PendingModifiedValuesTypeDef",
     {
         "DBInstanceClass": str,
         "AllocatedStorage": int,
         "MasterUserPassword": str,
         "Port": int,
@@ -1850,24 +1844,30 @@
         "Iops": int,
         "DBInstanceIdentifier": str,
         "StorageType": str,
         "CACertificateIdentifier": str,
         "DBSubnetGroupName": str,
         "PendingCloudwatchLogsExports": PendingCloudwatchLogsExportsTypeDef,
     },
-    total=False,
 )
 
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
-    total=False,
+)
+
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
 )
 
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
@@ -1881,15 +1881,14 @@
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
         "DBSubnetGroupArn": str,
     },
-    total=False,
 )
 
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2087,15 +2086,14 @@
         "DbiResourceId": str,
         "CACertificateIdentifier": str,
         "CopyTagsToSnapshot": bool,
         "PromotionTier": int,
         "DBInstanceArn": str,
         "EnabledCloudwatchLogsExports": List[str],
     },
-    total=False,
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
```

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/type_defs.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "AvailabilityZoneTypeDef",
     "CertificateTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterMemberTypeDef",
-    "ParameterTypeDef",
+    "ParameterOutputTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "EndpointTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
@@ -53,27 +53,29 @@
     "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
+    "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
+    "TagOutputTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
     "DBClusterParameterGroupNameMessageTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
@@ -85,30 +87,27 @@
     "CreateDBClusterParameterGroupMessageRequestTypeDef",
     "CreateDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
     "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
-    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionTypeDef",
     "SubnetTypeDef",
     "CertificateMessageTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
     "DBClusterParameterGroupsMessageTypeDef",
     "CopyDBClusterSnapshotResultTypeDef",
     "CreateDBClusterSnapshotResultTypeDef",
     "DBClusterSnapshotMessageTypeDef",
     "DeleteDBClusterSnapshotResultTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBClusterTypeDef",
     "DBEngineVersionTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
@@ -138,16 +137,19 @@
     "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
+    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     "CreateDBClusterResultTypeDef",
     "DBClusterMessageTypeDef",
@@ -195,15 +197,14 @@
         "SubscriptionCreationTime": str,
         "SourceType": str,
         "SourceIdsList": List[str],
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -232,28 +233,26 @@
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateIdentifier": str,
         "CertificateType": str,
         "Thumbprint": str,
         "ValidFrom": datetime,
         "ValidTill": datetime,
         "CertificateArn": str,
     },
-    total=False,
 )
 
 CloudwatchLogsExportConfigurationTypeDef = TypedDict(
     "CloudwatchLogsExportConfigurationTypeDef",
     {
         "EnableLogTypes": Sequence[str],
         "DisableLogTypes": Sequence[str],
@@ -265,15 +264,14 @@
     "DBClusterParameterGroupTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBClusterParameterGroupArn": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotTypeDef = TypedDict(
     "DBClusterSnapshotTypeDef",
     {
         "AvailabilityZones": List[str],
         "DBClusterSnapshotIdentifier": str,
@@ -289,15 +287,14 @@
         "SnapshotType": str,
         "PercentProgress": int,
         "StorageEncrypted": bool,
         "KmsKeyId": str,
         "DBClusterSnapshotArn": str,
         "SourceDBClusterSnapshotArn": str,
     },
-    total=False,
 )
 
 _RequiredCreateGlobalClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
     },
@@ -325,92 +322,84 @@
     "DBClusterMemberTypeDef",
     {
         "DBInstanceIdentifier": str,
         "IsClusterWriter": bool,
         "DBClusterParameterGroupStatus": str,
         "PromotionTier": int,
     },
-    total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "ApplyType": str,
         "DataType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
     },
-    total=False,
 )
 
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotAttributeTypeDef = TypedDict(
     "DBClusterSnapshotAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[str],
     },
-    total=False,
 )
 
 VpcSecurityGroupMembershipTypeDef = TypedDict(
     "VpcSecurityGroupMembershipTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
-    total=False,
 )
 
 UpgradeTargetTypeDef = TypedDict(
     "UpgradeTargetTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "Description": str,
         "AutoUpgrade": bool,
         "IsMajorVersionUpgrade": bool,
     },
-    total=False,
 )
 
 DBInstanceStatusInfoTypeDef = TypedDict(
     "DBInstanceStatusInfoTypeDef",
     {
         "StatusType": str,
         "Normal": bool,
         "Status": str,
         "Message": str,
     },
-    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "Port": int,
         "HostedZoneId": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -507,28 +496,26 @@
 
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
-    total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
         "SourceArn": str,
     },
-    total=False,
 )
 
 FailoverDBClusterMessageRequestTypeDef = TypedDict(
     "FailoverDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "TargetDBInstanceIdentifier": str,
@@ -539,14 +526,30 @@
 GlobalClusterMemberTypeDef = TypedDict(
     "GlobalClusterMemberTypeDef",
     {
         "DBClusterArn": str,
         "Readers": List[str],
         "IsWriter": bool,
     },
+)
+
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+        "Description": str,
+        "Source": str,
+        "ApplyType": str,
+        "DataType": str,
+        "AllowedValues": str,
+        "IsModifiable": bool,
+        "MinimumEngineVersion": str,
+        "ApplyMethod": ApplyMethodType,
+    },
     total=False,
 )
 
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
@@ -663,28 +666,26 @@
 
 PendingCloudwatchLogsExportsTypeDef = TypedDict(
     "PendingCloudwatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
-    total=False,
 )
 
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 _RequiredRebootDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredRebootDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
@@ -736,14 +737,22 @@
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1073,43 +1082,33 @@
 
 class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
     _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
     _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
 ):
     pass
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "Vpc": bool,
     },
-    total=False,
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
-    total=False,
 )
 
 CertificateMessageTypeDef = TypedDict(
     "CertificateMessageTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "Marker": str,
@@ -1205,66 +1204,35 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterTypeDef],
-    },
-    total=False,
-)
-
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-
-_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
+        "Parameters": List[ParameterOutputTypeDef],
     },
 )
-_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-    total=False,
-)
-
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
 
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
-    total=False,
 )
 
 DBClusterTypeDef = TypedDict(
     "DBClusterTypeDef",
     {
         "AvailabilityZones": List[str],
         "BackupRetentionPeriod": int,
@@ -1295,30 +1263,28 @@
         "DBClusterArn": str,
         "AssociatedRoles": List[DBClusterRoleTypeDef],
         "CloneGroupId": str,
         "ClusterCreateTime": datetime,
         "EnabledCloudwatchLogsExports": List[str],
         "DeletionProtection": bool,
     },
-    total=False,
 )
 
 DBEngineVersionTypeDef = TypedDict(
     "DBEngineVersionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "DBEngineDescription": str,
         "DBEngineVersionDescription": str,
         "ValidUpgradeTarget": List[UpgradeTargetTypeDef],
         "ExportableLogTypes": List[str],
         "SupportsLogExportsToCloudwatchLogs": bool,
     },
-    total=False,
 )
 
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "CertificateIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1776,17 +1742,45 @@
         "Engine": str,
         "EngineVersion": str,
         "DatabaseName": str,
         "StorageEncrypted": bool,
         "DeletionProtection": bool,
         "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
     },
+)
+
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
     total=False,
 )
 
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
 PendingModifiedValuesTypeDef = TypedDict(
     "PendingModifiedValuesTypeDef",
     {
         "DBInstanceClass": str,
         "AllocatedStorage": int,
         "MasterUserPassword": str,
         "Port": int,
@@ -1797,24 +1791,30 @@
         "Iops": int,
         "DBInstanceIdentifier": str,
         "StorageType": str,
         "CACertificateIdentifier": str,
         "DBSubnetGroupName": str,
         "PendingCloudwatchLogsExports": PendingCloudwatchLogsExportsTypeDef,
     },
-    total=False,
 )
 
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
-    total=False,
+)
+
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
 )
 
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
@@ -1828,15 +1828,14 @@
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
         "DBSubnetGroupArn": str,
     },
-    total=False,
 )
 
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2034,15 +2033,14 @@
         "DbiResourceId": str,
         "CACertificateIdentifier": str,
         "CopyTagsToSnapshot": bool,
         "PromotionTier": int,
         "DBInstanceArn": str,
         "EnabledCloudwatchLogsExports": List[str],
     },
-    total=False,
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
```

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/waiter.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb/waiter.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb.egg-info/PKG-INFO` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DocDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.4
+Summary: Type annotations for boto3.DocDB 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -418,15 +418,15 @@
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
-    ParameterTypeDef,
+    ParameterOutputTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
@@ -440,27 +440,29 @@
     PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
+    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
@@ -472,30 +474,27 @@
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     CertificateMessageTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
     DBClusterParameterGroupsMessageTypeDef,
     CopyDBClusterSnapshotResultTypeDef,
     CreateDBClusterSnapshotResultTypeDef,
     DBClusterSnapshotMessageTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
@@ -525,16 +524,19 @@
     DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
     CreateDBClusterResultTypeDef,
     DBClusterMessageTypeDef,
```

### Comparing `mypy-boto3-docdb-1.28.15.post1/mypy_boto3_docdb.egg-info/SOURCES.txt` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.15.post1/setup.py` & `mypy-boto3-docdb-1.28.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-docdb",
-    version="1.28.15.post1",
+    version="1.28.4",
     packages=["mypy_boto3_docdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DocDB 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.DocDB 1.28.4 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

