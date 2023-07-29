# Comparing `tmp/iam_actions-1.2.20230728.tar.gz` & `tmp/iam_actions-1.2.20230729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230728.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230729.tar", max compression
```

## Comparing `iam_actions-1.2.20230728.tar` & `iam_actions-1.2.20230729.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/README.md
--rw-r--r--   0        0        0      228 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/iam_actions/__init__.py
--rw-r--r--   0        0        0  4380617 2023-07-28 02:26:11.756842 iam_actions-1.2.20230728/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-28 02:24:13.053848 iam_actions-1.2.20230728/iam_actions/generate/services.py
--rw-r--r--   0        0        0   565126 2023-07-28 02:26:11.756842 iam_actions-1.2.20230728/iam_actions/policies.json
--rw-r--r--   0        0        0   196251 2023-07-28 02:26:11.756842 iam_actions-1.2.20230728/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   548189 2023-07-28 02:26:11.756842 iam_actions-1.2.20230728/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-28 02:26:12.668893 iam_actions-1.2.20230728/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230728/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230728/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-29 02:20:11.852894 iam_actions-1.2.20230729/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-29 02:20:11.852894 iam_actions-1.2.20230729/README.md
+-rw-r--r--   0        0        0      228 2023-07-29 02:20:11.852894 iam_actions-1.2.20230729/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4382239 2023-07-29 02:21:49.753647 iam_actions-1.2.20230729/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-29 02:20:11.852894 iam_actions-1.2.20230729/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-29 02:20:11.852894 iam_actions-1.2.20230729/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-29 02:20:11.852894 iam_actions-1.2.20230729/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-29 02:20:11.856895 iam_actions-1.2.20230729/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-29 02:20:11.856895 iam_actions-1.2.20230729/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-29 02:20:11.856895 iam_actions-1.2.20230729/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-29 02:20:11.856895 iam_actions-1.2.20230729/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-29 02:20:11.856895 iam_actions-1.2.20230729/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   565259 2023-07-29 02:21:49.753647 iam_actions-1.2.20230729/iam_actions/policies.json
+-rw-r--r--   0        0        0   196251 2023-07-29 02:21:49.753647 iam_actions-1.2.20230729/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   548317 2023-07-29 02:21:49.753647 iam_actions-1.2.20230729/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-29 02:21:50.529653 iam_actions-1.2.20230729/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230729/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230729/PKG-INFO
```

### Comparing `iam_actions-1.2.20230728/LICENSE` & `iam_actions-1.2.20230729/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230728/README.md` & `iam_actions-1.2.20230729/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230728/iam_actions/actions.json` & `iam_actions-1.2.20230729/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998786515675427%*

 * *Differences: {"'ce'": "{'GetSavingsPlanPurchaseRecommendationDetails': {'access_level': 'Read', 'description': "*

 * *         "'Grants permission to retrieve the Savings Plan recommendation details for your "*

 * *         "account'}}",*

 * * "'ivs'": "{'BatchStartViewerSessionRevocation': {'access_level': 'Write', 'description': 'Grants "*

 * *          'permission to perform StartViewerSessionRevocation on multiple channel ARN and viewer '*

 * *          "ID pairs simultaneously', 'resources': ['Channel']}, 'StartViewerSessionRevocation': "*

 * * […]*

```diff
@@ -14409,18 +14409,18 @@
             "action": "GetRightsizingRecommendation",
             "condition_keys": [],
             "description": "Grants permission to retrieve the rightsizing recommendations for your account",
             "orphan": false,
             "resources": []
         },
         "GetSavingsPlanPurchaseRecommendationDetails": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetSavingsPlanPurchaseRecommendationDetails",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve the Savings Plan recommendation details for your account",
             "orphan": false,
             "resources": []
         },
         "GetSavingsPlansCoverage": {
             "access_level": "Read",
             "action": "GetSavingsPlansCoverage",
             "condition_keys": [],
@@ -83445,20 +83445,22 @@
             "description": "Grants permission to get multiple stream keys simultaneously by stream key ARN",
             "orphan": false,
             "resources": [
                 "Stream-Key"
             ]
         },
         "BatchStartViewerSessionRevocation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "BatchStartViewerSessionRevocation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to perform StartViewerSessionRevocation on multiple channel ARN and viewer ID pairs simultaneously",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Channel"
+            ]
         },
         "CreateChannel": {
             "access_level": "Write",
             "action": "CreateChannel",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -83811,20 +83813,22 @@
             "description": "Grants permission to insert metadata into an RTMP stream for a specified channel",
             "orphan": false,
             "resources": [
                 "Channel"
             ]
         },
         "StartViewerSessionRevocation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartViewerSessionRevocation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start the process of revoking the viewer session associated with a specified channel ARN and viewer ID",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Channel"
+            ]
         },
         "StopStream": {
             "access_level": "Write",
             "action": "StopStream",
             "condition_keys": [],
             "description": "Grants permission to disconnect a streamer on a specified channel",
             "orphan": false,
@@ -84202,14 +84206,22 @@
             "access_level": "Read",
             "action": "DescribeClusterOperation",
             "condition_keys": [],
             "description": "Grants permission to describe the cluster operation that is specified by the given ARN",
             "orphan": false,
             "resources": []
         },
+        "DescribeClusterOperationV2": {
+            "access_level": "Undocumented",
+            "action": "DescribeClusterOperationV2",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeClusterV2": {
             "access_level": "Read",
             "action": "DescribeClusterV2",
             "condition_keys": [],
             "description": "Grants permission to describe an MSK cluster",
             "orphan": false,
             "resources": [
@@ -84288,14 +84300,22 @@
             "condition_keys": [],
             "description": "Grants permission to return a list of all the operations that have been performed on the specified MSK cluster",
             "orphan": false,
             "resources": [
                 "cluster"
             ]
         },
+        "ListClusterOperationsV2": {
+            "access_level": "Undocumented",
+            "action": "ListClusterOperationsV2",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListClusters": {
             "access_level": "List",
             "action": "ListClusters",
             "condition_keys": [],
             "description": "Grants permission to list all MSK clusters in this account",
             "orphan": false,
             "resources": []
@@ -89537,36 +89557,42 @@
             "action": "ListImports",
             "condition_keys": [],
             "description": "Grants permission to list existing imports",
             "orphan": false,
             "resources": []
         },
         "ListIntentMetrics": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListIntentMetrics",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list intent analytics metrics for a bot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "bot"
+            ]
         },
         "ListIntentPaths": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListIntentPaths",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list intent path analytics for a bot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "bot"
+            ]
         },
         "ListIntentStageMetrics": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListIntentStageMetrics",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list intentStage analytics metrics for a bot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "bot"
+            ]
         },
         "ListIntents": {
             "access_level": "List",
             "action": "ListIntents",
             "condition_keys": [],
             "description": "Grants permission to list intents in a bot",
             "orphan": false,
@@ -89581,28 +89607,32 @@
             "description": "Grants permission to get a list of recommended intents provided by the bot recommendation",
             "orphan": false,
             "resources": [
                 "bot"
             ]
         },
         "ListSessionAnalyticsData": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListSessionAnalyticsData",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list session analytics data for a bot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "bot"
+            ]
         },
         "ListSessionMetrics": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListSessionMetrics",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list session analytics metrics for a bot",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "bot"
+            ]
         },
         "ListSlotTypes": {
             "access_level": "List",
             "action": "ListSlotTypes",
             "condition_keys": [],
             "description": "Grants permission to list slot types in a bot",
             "orphan": false,
@@ -95070,26 +95100,26 @@
             "action": "Invoke",
             "condition_keys": [],
             "description": "Grants permission to create WebSocket connections to an Ethereum node",
             "orphan": false,
             "resources": []
         },
         "InvokeRpcBitcoinMainnet": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "InvokeRpcBitcoinMainnet",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to invoke the Bitcoin Mainnet RPCs",
             "orphan": false,
             "resources": []
         },
         "InvokeRpcBitcoinTestnet": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "InvokeRpcBitcoinTestnet",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to invoke the Bitcoin Testnet RPCs",
             "orphan": false,
             "resources": []
         },
         "ListAccessors": {
             "access_level": "List",
             "action": "ListAccessors",
             "condition_keys": [],
@@ -110472,14 +110502,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete component",
             "orphan": false,
             "resources": [
                 "component"
             ]
         },
+        "DeleteDeployment": {
+            "access_level": "Undocumented",
+            "action": "DeleteDeployment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteEnvironment": {
             "access_level": "Write",
             "action": "DeleteEnvironment",
             "condition_keys": [
                 "proton:EnvironmentTemplate"
             ],
             "description": "Grants permission to delete an environment",
@@ -110638,14 +110676,22 @@
             "condition_keys": [],
             "description": "Grants permission to describe a component",
             "orphan": false,
             "resources": [
                 "component"
             ]
         },
+        "GetDeployment": {
+            "access_level": "Undocumented",
+            "action": "GetDeployment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetEnvironment": {
             "access_level": "Read",
             "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Grants permission to describe an environment",
             "orphan": false,
             "resources": [
@@ -110864,14 +110910,22 @@
             "orphan": false,
             "resources": [
                 "environment",
                 "service",
                 "service-instance"
             ]
         },
+        "ListDeployments": {
+            "access_level": "Undocumented",
+            "action": "ListDeployments",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListEnvironmentAccountConnections": {
             "access_level": "List",
             "action": "ListEnvironmentAccountConnections",
             "condition_keys": [],
             "description": "Grants permission to list environment account connections",
             "orphan": false,
             "resources": []
@@ -148773,18 +148827,18 @@
             "action": "SetOrganizationAccess",
             "condition_keys": [],
             "description": "Grants permission to enable the organizational view feature for AWS Trusted Advisor",
             "orphan": false,
             "resources": []
         },
         "UpdateEngagement": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateEngagement",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update the details of an engagement",
             "orphan": false,
             "resources": []
         },
         "UpdateEngagementStatus": {
             "access_level": "Write",
             "action": "UpdateEngagementStatus",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230728/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230729/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230728/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230729/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230728/iam_actions/generate/generate.py` & `iam_actions-1.2.20230729/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230728/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230729/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230728/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230729/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230728/iam_actions/generate/services.py` & `iam_actions-1.2.20230729/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230728/iam_actions/policies.json` & `iam_actions-1.2.20230729/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999992450063095%*

 * *Differences: {"'serviceMap'": "{'AWS Proton': {'Actions': {insert: [(23, 'DeleteDeployment'), (41, "*

 * *                 "'GetDeployment'), (66, 'ListDeployments')]}}, 'Amazon Managed Streaming for "*

 * *                 "Apache Kafka': {'Actions': {insert: [(12, 'DescribeClusterOperationV2'), (22, "*

 * *                 "'ListClusterOperationsV2')]}}}"}*

```diff
@@ -7623,14 +7623,15 @@
                 "CreateServiceTemplate",
                 "CreateServiceTemplateMajorVersion",
                 "CreateServiceTemplateMinorVersion",
                 "CreateServiceTemplateVersion",
                 "CreateTemplateSyncConfig",
                 "DeleteAccountRoles",
                 "DeleteComponent",
+                "DeleteDeployment",
                 "DeleteEnvironment",
                 "DeleteEnvironmentAccountConnection",
                 "DeleteEnvironmentTemplate",
                 "DeleteEnvironmentTemplateMajorVersion",
                 "DeleteEnvironmentTemplateMinorVersion",
                 "DeleteEnvironmentTemplateVersion",
                 "DeleteRepository",
@@ -7640,14 +7641,15 @@
                 "DeleteServiceTemplateMajorVersion",
                 "DeleteServiceTemplateMinorVersion",
                 "DeleteServiceTemplateVersion",
                 "DeleteTemplateSyncConfig",
                 "GetAccountRoles",
                 "GetAccountSettings",
                 "GetComponent",
+                "GetDeployment",
                 "GetEnvironment",
                 "GetEnvironmentAccountConnection",
                 "GetEnvironmentTemplate",
                 "GetEnvironmentTemplateMajorVersion",
                 "GetEnvironmentTemplateMinorVersion",
                 "GetEnvironmentTemplateVersion",
                 "GetRepository",
@@ -7664,14 +7666,15 @@
                 "GetServiceTemplateMinorVersion",
                 "GetServiceTemplateVersion",
                 "GetTemplateSyncConfig",
                 "GetTemplateSyncStatus",
                 "ListComponentOutputs",
                 "ListComponentProvisionedResources",
                 "ListComponents",
+                "ListDeployments",
                 "ListEnvironmentAccountConnections",
                 "ListEnvironmentOutputs",
                 "ListEnvironmentProvisionedResources",
                 "ListEnvironmentTemplateMajorVersions",
                 "ListEnvironmentTemplateMinorVersions",
                 "ListEnvironmentTemplateVersions",
                 "ListEnvironmentTemplates",
@@ -16243,23 +16246,25 @@
                 "CreateVpcConnection",
                 "DeleteCluster",
                 "DeleteClusterPolicy",
                 "DeleteConfiguration",
                 "DeleteVpcConnection",
                 "DescribeCluster",
                 "DescribeClusterOperation",
+                "DescribeClusterOperationV2",
                 "DescribeClusterV2",
                 "DescribeConfiguration",
                 "DescribeConfigurationRevision",
                 "DescribeVpcConnection",
                 "GetBootstrapBrokers",
                 "GetClusterPolicy",
                 "GetCompatibleKafkaVersions",
                 "ListClientVpcConnections",
                 "ListClusterOperations",
+                "ListClusterOperationsV2",
                 "ListClusters",
                 "ListClustersV2",
                 "ListConfigurationRevisions",
                 "ListConfigurations",
                 "ListKafkaVersions",
                 "ListNodes",
                 "ListScramSecrets",
```

### Comparing `iam_actions-1.2.20230728/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230729/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230728/iam_actions/services.json` & `iam_actions-1.2.20230729/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999921003384973%*

 * *Differences: {"'kafka'": "{'Actions': {insert: [(12, 'DescribeClusterOperationV2'), (22, "*

 * *            "'ListClusterOperationsV2')]}}",*

 * * "'proton'": "{'Actions': {insert: [(23, 'DeleteDeployment'), (41, 'GetDeployment'), (66, "*

 * *             "'ListDeployments')]}}"}*

```diff
@@ -11683,23 +11683,25 @@
             "CreateVpcConnection",
             "DeleteCluster",
             "DeleteClusterPolicy",
             "DeleteConfiguration",
             "DeleteVpcConnection",
             "DescribeCluster",
             "DescribeClusterOperation",
+            "DescribeClusterOperationV2",
             "DescribeClusterV2",
             "DescribeConfiguration",
             "DescribeConfigurationRevision",
             "DescribeVpcConnection",
             "GetBootstrapBrokers",
             "GetClusterPolicy",
             "GetCompatibleKafkaVersions",
             "ListClientVpcConnections",
             "ListClusterOperations",
+            "ListClusterOperationsV2",
             "ListClusters",
             "ListClustersV2",
             "ListConfigurationRevisions",
             "ListConfigurations",
             "ListKafkaVersions",
             "ListNodes",
             "ListScramSecrets",
@@ -15618,14 +15620,15 @@
             "CreateServiceTemplate",
             "CreateServiceTemplateMajorVersion",
             "CreateServiceTemplateMinorVersion",
             "CreateServiceTemplateVersion",
             "CreateTemplateSyncConfig",
             "DeleteAccountRoles",
             "DeleteComponent",
+            "DeleteDeployment",
             "DeleteEnvironment",
             "DeleteEnvironmentAccountConnection",
             "DeleteEnvironmentTemplate",
             "DeleteEnvironmentTemplateMajorVersion",
             "DeleteEnvironmentTemplateMinorVersion",
             "DeleteEnvironmentTemplateVersion",
             "DeleteRepository",
@@ -15635,14 +15638,15 @@
             "DeleteServiceTemplateMajorVersion",
             "DeleteServiceTemplateMinorVersion",
             "DeleteServiceTemplateVersion",
             "DeleteTemplateSyncConfig",
             "GetAccountRoles",
             "GetAccountSettings",
             "GetComponent",
+            "GetDeployment",
             "GetEnvironment",
             "GetEnvironmentAccountConnection",
             "GetEnvironmentTemplate",
             "GetEnvironmentTemplateMajorVersion",
             "GetEnvironmentTemplateMinorVersion",
             "GetEnvironmentTemplateVersion",
             "GetRepository",
@@ -15659,14 +15663,15 @@
             "GetServiceTemplateMinorVersion",
             "GetServiceTemplateVersion",
             "GetTemplateSyncConfig",
             "GetTemplateSyncStatus",
             "ListComponentOutputs",
             "ListComponentProvisionedResources",
             "ListComponents",
+            "ListDeployments",
             "ListEnvironmentAccountConnections",
             "ListEnvironmentOutputs",
             "ListEnvironmentProvisionedResources",
             "ListEnvironmentTemplateMajorVersions",
             "ListEnvironmentTemplateMinorVersions",
             "ListEnvironmentTemplateVersions",
             "ListEnvironmentTemplates",
```

### Comparing `iam_actions-1.2.20230728/pyproject.toml` & `iam_actions-1.2.20230729/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230728"
+version = "1.2.20230729"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230728/setup.py` & `iam_actions-1.2.20230729/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230728',
+    'version': '1.2.20230729',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230728/PKG-INFO` & `iam_actions-1.2.20230729/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230728
+Version: 1.2.20230729
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

