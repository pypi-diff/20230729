# Comparing `tmp/mypy-boto3-gamelift-1.28.15.tar.gz` & `tmp/mypy-boto3-gamelift-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-gamelift-1.28.15.tar", last modified: Fri Jul 28 20:42:50 2023, max compression
+gzip compressed data, was "mypy-boto3-gamelift-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:11 2023, max compression
```

## Comparing `mypy-boto3-gamelift-1.28.15.tar` & `mypy-boto3-gamelift-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.197129 mypy-boto3-gamelift-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:21.000000 mypy-boto3-gamelift-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29054 2023-07-28 20:42:50.197129 mypy-boto3-gamelift-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27563 2023-07-28 20:26:21.000000 mypy-boto3-gamelift-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.197129 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-28 20:26:21.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-28 20:26:21.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:26:21.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84696 2023-07-28 20:26:22.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    84563 2023-07-28 20:26:21.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-07-28 20:26:23.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20728 2023-07-28 20:26:22.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26546 2023-07-28 20:26:22.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26522 2023-07-28 20:26:22.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:21.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    99318 2023-07-28 20:26:26.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    99219 2023-07-28 20:26:24.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:21.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.197129 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29054 2023-07-28 20:42:49.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:42:50.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:49.000000 mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:50.197129 mypy-boto3-gamelift-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:26:21.000000 mypy-boto3-gamelift-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:11.289161 mypy-boto3-gamelift-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29060 2023-07-29 10:03:11.289161 mypy-boto3-gamelift-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27563 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:11.285161 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85312 2023-07-29 09:45:54.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85179 2023-07-29 09:45:54.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-07-29 09:45:55.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20728 2023-07-29 09:45:55.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26546 2023-07-29 09:45:54.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26522 2023-07-29 09:45:54.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    99374 2023-07-29 09:45:59.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99275 2023-07-29 09:45:56.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:11.289161 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29060 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:11.289161 mypy-boto3-gamelift-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-gamelift-1.28.15/LICENSE` & `mypy-boto3-gamelift-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15/PKG-INFO` & `mypy-boto3-gamelift-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamelift
-Version: 1.28.15
-Summary: Type annotations for boto3.GameLift 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.GameLift 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/
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
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-gamelift-1.28.15/README.md` & `mypy-boto3-gamelift-1.28.15.post1/README.md`

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
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/__init__.py` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/__init__.pyi` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/__main__.py` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GameLift 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.GameLift 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift\nOther"
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

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/client.py` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     DescribeRuntimeConfigurationOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     DescribeScriptOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
     DesiredPlayerSessionTypeDef,
     EmptyResponseMetadataTypeDef,
+    FilterConfigurationOutputTypeDef,
     FilterConfigurationTypeDef,
     GamePropertyTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
     GameSessionQueueDestinationTypeDef,
     GetComputeAccessOutputTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
@@ -139,24 +140,27 @@
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     LocationConfigurationTypeDef,
     PlayerLatencyPolicyTypeDef,
     PlayerLatencyTypeDef,
+    PlayerOutputTypeDef,
     PlayerTypeDef,
+    PriorityConfigurationOutputTypeDef,
     PriorityConfigurationTypeDef,
     PutScalingPolicyOutputTypeDef,
     RegisterComputeOutputTypeDef,
     RegisterGameServerOutputTypeDef,
     RequestUploadCredentialsOutputTypeDef,
     ResolveAliasOutputTypeDef,
     ResourceCreationLimitPolicyTypeDef,
     ResumeGameServerGroupOutputTypeDef,
     RoutingStrategyTypeDef,
+    RuntimeConfigurationOutputTypeDef,
     RuntimeConfigurationTypeDef,
     S3LocationTypeDef,
     SearchGameSessionsOutputTypeDef,
     StartFleetActionsOutputTypeDef,
     StartGameSessionPlacementOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
@@ -317,15 +321,17 @@
         ScriptId: str = ...,
         ServerLaunchPath: str = ...,
         ServerLaunchParameters: str = ...,
         LogPaths: Sequence[str] = ...,
         EC2InstanceType: EC2InstanceTypeType = ...,
         EC2InboundPermissions: Sequence[IpPermissionTypeDef] = ...,
         NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,
-        RuntimeConfiguration: RuntimeConfigurationTypeDef = ...,
+        RuntimeConfiguration: Union[
+            RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef
+        ] = ...,
         ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,
         MetricGroups: Sequence[str] = ...,
         PeerVpcAwsAccountId: str = ...,
         PeerVpcId: str = ...,
         FleetType: FleetTypeType = ...,
         InstanceRoleArn: str = ...,
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
@@ -402,16 +408,20 @@
     def create_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: FilterConfigurationTypeDef = ...,
-        PriorityConfiguration: PriorityConfigurationTypeDef = ...,
+        FilterConfiguration: Union[
+            FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
+        ] = ...,
+        PriorityConfiguration: Union[
+            PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
+        ] = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateGameSessionQueueOutputTypeDef:
         """
         Creates a placement queue that processes requests for new game sessions.
 
@@ -1298,27 +1308,31 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_game_session_placement)
         """
 
     def start_match_backfill(
         self,
         *,
         ConfigurationName: str,
-        Players: Sequence[PlayerTypeDef],
+        Players: Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
         TicketId: str = ...,
         GameSessionArn: str = ...
     ) -> StartMatchBackfillOutputTypeDef:
         """
         Finds new players to fill open slots in currently running game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_match_backfill)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_match_backfill)
         """
 
     def start_matchmaking(
-        self, *, ConfigurationName: str, Players: Sequence[PlayerTypeDef], TicketId: str = ...
+        self,
+        *,
+        ConfigurationName: str,
+        Players: Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
+        TicketId: str = ...
     ) -> StartMatchmakingOutputTypeDef:
         """
         Uses FlexMatch to create a game match for a group of players based on custom
         matchmaking rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_matchmaking)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_matchmaking)
@@ -1514,16 +1528,20 @@
     def update_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: FilterConfigurationTypeDef = ...,
-        PriorityConfiguration: PriorityConfigurationTypeDef = ...,
+        FilterConfiguration: Union[
+            FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
+        ] = ...,
+        PriorityConfiguration: Union[
+            PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
+        ] = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...
     ) -> UpdateGameSessionQueueOutputTypeDef:
         """
         Updates the configuration of a game session queue, which determines how the
         queue processes new game session requests.
 
@@ -1553,15 +1571,18 @@
         Updates settings for a FlexMatch matchmaking configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_matchmaking_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_matchmaking_configuration)
         """
 
     def update_runtime_configuration(
-        self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationTypeDef
+        self,
+        *,
+        FleetId: str,
+        RuntimeConfiguration: Union[RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef]
     ) -> UpdateRuntimeConfigurationOutputTypeDef:
         """
         Updates the current runtime configuration for the specified fleet, which tells
         Amazon GameLift how to launch server processes on all instances in the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_runtime_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_runtime_configuration)
```

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/client.pyi` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     DescribeRuntimeConfigurationOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     DescribeScriptOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
     DesiredPlayerSessionTypeDef,
     EmptyResponseMetadataTypeDef,
+    FilterConfigurationOutputTypeDef,
     FilterConfigurationTypeDef,
     GamePropertyTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
     GameSessionQueueDestinationTypeDef,
     GetComputeAccessOutputTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
@@ -139,24 +140,27 @@
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     LocationConfigurationTypeDef,
     PlayerLatencyPolicyTypeDef,
     PlayerLatencyTypeDef,
+    PlayerOutputTypeDef,
     PlayerTypeDef,
+    PriorityConfigurationOutputTypeDef,
     PriorityConfigurationTypeDef,
     PutScalingPolicyOutputTypeDef,
     RegisterComputeOutputTypeDef,
     RegisterGameServerOutputTypeDef,
     RequestUploadCredentialsOutputTypeDef,
     ResolveAliasOutputTypeDef,
     ResourceCreationLimitPolicyTypeDef,
     ResumeGameServerGroupOutputTypeDef,
     RoutingStrategyTypeDef,
+    RuntimeConfigurationOutputTypeDef,
     RuntimeConfigurationTypeDef,
     S3LocationTypeDef,
     SearchGameSessionsOutputTypeDef,
     StartFleetActionsOutputTypeDef,
     StartGameSessionPlacementOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
@@ -306,15 +310,17 @@
         ScriptId: str = ...,
         ServerLaunchPath: str = ...,
         ServerLaunchParameters: str = ...,
         LogPaths: Sequence[str] = ...,
         EC2InstanceType: EC2InstanceTypeType = ...,
         EC2InboundPermissions: Sequence[IpPermissionTypeDef] = ...,
         NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,
-        RuntimeConfiguration: RuntimeConfigurationTypeDef = ...,
+        RuntimeConfiguration: Union[
+            RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef
+        ] = ...,
         ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,
         MetricGroups: Sequence[str] = ...,
         PeerVpcAwsAccountId: str = ...,
         PeerVpcId: str = ...,
         FleetType: FleetTypeType = ...,
         InstanceRoleArn: str = ...,
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
@@ -387,16 +393,20 @@
     def create_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: FilterConfigurationTypeDef = ...,
-        PriorityConfiguration: PriorityConfigurationTypeDef = ...,
+        FilterConfiguration: Union[
+            FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
+        ] = ...,
+        PriorityConfiguration: Union[
+            PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
+        ] = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateGameSessionQueueOutputTypeDef:
         """
         Creates a placement queue that processes requests for new game sessions.
 
@@ -1207,26 +1217,30 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_game_session_placement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_game_session_placement)
         """
     def start_match_backfill(
         self,
         *,
         ConfigurationName: str,
-        Players: Sequence[PlayerTypeDef],
+        Players: Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
         TicketId: str = ...,
         GameSessionArn: str = ...
     ) -> StartMatchBackfillOutputTypeDef:
         """
         Finds new players to fill open slots in currently running game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_match_backfill)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_match_backfill)
         """
     def start_matchmaking(
-        self, *, ConfigurationName: str, Players: Sequence[PlayerTypeDef], TicketId: str = ...
+        self,
+        *,
+        ConfigurationName: str,
+        Players: Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
+        TicketId: str = ...
     ) -> StartMatchmakingOutputTypeDef:
         """
         Uses FlexMatch to create a game match for a group of players based on custom
         matchmaking rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_matchmaking)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_matchmaking)
@@ -1407,16 +1421,20 @@
     def update_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: FilterConfigurationTypeDef = ...,
-        PriorityConfiguration: PriorityConfigurationTypeDef = ...,
+        FilterConfiguration: Union[
+            FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
+        ] = ...,
+        PriorityConfiguration: Union[
+            PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
+        ] = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...
     ) -> UpdateGameSessionQueueOutputTypeDef:
         """
         Updates the configuration of a game session queue, which determines how the
         queue processes new game session requests.
 
@@ -1444,15 +1462,18 @@
         """
         Updates settings for a FlexMatch matchmaking configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_matchmaking_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_matchmaking_configuration)
         """
     def update_runtime_configuration(
-        self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationTypeDef
+        self,
+        *,
+        FleetId: str,
+        RuntimeConfiguration: Union[RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef]
     ) -> UpdateRuntimeConfigurationOutputTypeDef:
         """
         Updates the current runtime configuration for the specified fleet, which tells
         Amazon GameLift how to launch server processes on all instances in the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_runtime_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_runtime_configuration)
```

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/literals.py` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/literals.pyi` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/paginator.py` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/paginator.pyi` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/type_defs.py` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3318,15 +3318,15 @@
     },
 )
 
 _RequiredStartMatchBackfillInputRequestTypeDef = TypedDict(
     "_RequiredStartMatchBackfillInputRequestTypeDef",
     {
         "ConfigurationName": str,
-        "Players": Sequence[PlayerTypeDef],
+        "Players": Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
     },
 )
 _OptionalStartMatchBackfillInputRequestTypeDef = TypedDict(
     "_OptionalStartMatchBackfillInputRequestTypeDef",
     {
         "TicketId": str,
         "GameSessionArn": str,
@@ -3341,15 +3341,15 @@
     pass
 
 
 _RequiredStartMatchmakingInputRequestTypeDef = TypedDict(
     "_RequiredStartMatchmakingInputRequestTypeDef",
     {
         "ConfigurationName": str,
-        "Players": Sequence[PlayerTypeDef],
+        "Players": Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
     },
 )
 _OptionalStartMatchmakingInputRequestTypeDef = TypedDict(
     "_OptionalStartMatchmakingInputRequestTypeDef",
     {
         "TicketId": str,
     },
```

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift/type_defs.pyi` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -3227,15 +3227,15 @@
     },
 )
 
 _RequiredStartMatchBackfillInputRequestTypeDef = TypedDict(
     "_RequiredStartMatchBackfillInputRequestTypeDef",
     {
         "ConfigurationName": str,
-        "Players": Sequence[PlayerTypeDef],
+        "Players": Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
     },
 )
 _OptionalStartMatchBackfillInputRequestTypeDef = TypedDict(
     "_OptionalStartMatchBackfillInputRequestTypeDef",
     {
         "TicketId": str,
         "GameSessionArn": str,
@@ -3248,15 +3248,15 @@
 ):
     pass
 
 _RequiredStartMatchmakingInputRequestTypeDef = TypedDict(
     "_RequiredStartMatchmakingInputRequestTypeDef",
     {
         "ConfigurationName": str,
-        "Players": Sequence[PlayerTypeDef],
+        "Players": Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
     },
 )
 _OptionalStartMatchmakingInputRequestTypeDef = TypedDict(
     "_OptionalStartMatchmakingInputRequestTypeDef",
     {
         "TicketId": str,
     },
```

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift.egg-info/PKG-INFO` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamelift
-Version: 1.28.15
-Summary: Type annotations for boto3.GameLift 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.GameLift 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/
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
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-gamelift-1.28.15/mypy_boto3_gamelift.egg-info/SOURCES.txt` & `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15/setup.py` & `mypy-boto3-gamelift-1.28.15.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-gamelift",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_gamelift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.GameLift 1.28.15 service generated with mypy-boto3-builder"
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

