# Comparing `tmp/mypy-boto3-events-1.28.15.tar.gz` & `tmp/mypy-boto3-events-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-events-1.28.15.tar", last modified: Fri Jul 28 20:42:47 2023, max compression
+gzip compressed data, was "mypy-boto3-events-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:07 2023, max compression
```

## Comparing `mypy-boto3-events-1.28.15.tar` & `mypy-boto3-events-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.117087 mypy-boto3-events-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-07-28 20:42:47.105087 mypy-boto3-events-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18700 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.105087 mypy-boto3-events-1.28.15/mypy_boto3_events/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37779 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-28 20:25:41.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-28 20:25:41.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64838 2023-07-28 20:25:42.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64757 2023-07-28 20:25:42.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.105087 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:47.117087 mypy-boto3-events-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:07.281147 mypy-boto3-events-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20194 2023-07-29 10:03:07.281147 mypy-boto3-events-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18700 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:07.273147 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37939 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37873 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64866 2023-07-29 09:45:15.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64785 2023-07-29 09:45:12.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:07.281147 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20194 2023-07-29 10:03:06.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:03:07.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:07.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:06.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:07.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:07.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:07.281147 mypy-boto3-events-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-events-1.28.15/LICENSE` & `mypy-boto3-events-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15/PKG-INFO` & `mypy-boto3-events-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.28.15
-Summary: Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-events-1.28.15/README.md` & `mypy-boto3-events-1.28.15.post1/README.md`

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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/__init__.py` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/__init__.pyi` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/__main__.py` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridge 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.EventBridge 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge\nOther"
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

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/client.py` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,21 @@
     PutEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
+    ReplayDestinationOutputTypeDef,
     ReplayDestinationTypeDef,
     ReplicationConfigTypeDef,
     RoutingConfigTypeDef,
     StartReplayResponseTypeDef,
     TagTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
     TestEventPatternResponseTypeDef,
     UpdateApiDestinationResponseTypeDef,
     UpdateArchiveResponseTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     UpdateEndpointResponseTypeDef,
@@ -659,15 +661,19 @@
         Creates or updates the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#put_rule)
         """
 
     def put_targets(
-        self, *, Rule: str, Targets: Sequence[TargetTypeDef], EventBusName: str = ...
+        self,
+        *,
+        Rule: str,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        EventBusName: str = ...
     ) -> PutTargetsResponseTypeDef:
         """
         Adds the specified targets to the specified rule, or updates the targets if they
         are already associated with the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#put_targets)
@@ -697,15 +703,15 @@
     def start_replay(
         self,
         *,
         ReplayName: str,
         EventSourceArn: str,
         EventStartTime: Union[datetime, str],
         EventEndTime: Union[datetime, str],
-        Destination: ReplayDestinationTypeDef,
+        Destination: Union[ReplayDestinationTypeDef, ReplayDestinationOutputTypeDef],
         Description: str = ...
     ) -> StartReplayResponseTypeDef:
         """
         Starts the specified replay.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#start_replay)
```

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/client.pyi` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,21 @@
     PutEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
+    ReplayDestinationOutputTypeDef,
     ReplayDestinationTypeDef,
     ReplicationConfigTypeDef,
     RoutingConfigTypeDef,
     StartReplayResponseTypeDef,
     TagTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
     TestEventPatternResponseTypeDef,
     UpdateApiDestinationResponseTypeDef,
     UpdateArchiveResponseTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     UpdateEndpointResponseTypeDef,
@@ -606,15 +608,19 @@
         """
         Creates or updates the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#put_rule)
         """
     def put_targets(
-        self, *, Rule: str, Targets: Sequence[TargetTypeDef], EventBusName: str = ...
+        self,
+        *,
+        Rule: str,
+        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
+        EventBusName: str = ...
     ) -> PutTargetsResponseTypeDef:
         """
         Adds the specified targets to the specified rule, or updates the targets if they
         are already associated with the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#put_targets)
@@ -641,15 +647,15 @@
     def start_replay(
         self,
         *,
         ReplayName: str,
         EventSourceArn: str,
         EventStartTime: Union[datetime, str],
         EventEndTime: Union[datetime, str],
-        Destination: ReplayDestinationTypeDef,
+        Destination: Union[ReplayDestinationTypeDef, ReplayDestinationOutputTypeDef],
         Description: str = ...
     ) -> StartReplayResponseTypeDef:
         """
         Starts the specified replay.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#start_replay)
```

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/literals.py` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/literals.pyi` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/paginator.py` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/paginator.pyi` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/type_defs.py` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2474,15 +2474,15 @@
     },
 )
 
 _RequiredPutTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredPutTargetsRequestRequestTypeDef",
     {
         "Rule": str,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
     },
 )
 _OptionalPutTargetsRequestRequestTypeDef = TypedDict(
     "_OptionalPutTargetsRequestRequestTypeDef",
     {
         "EventBusName": str,
     },
```

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events/type_defs.pyi` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2399,15 +2399,15 @@
     },
 )
 
 _RequiredPutTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredPutTargetsRequestRequestTypeDef",
     {
         "Rule": str,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
     },
 )
 _OptionalPutTargetsRequestRequestTypeDef = TypedDict(
     "_OptionalPutTargetsRequestRequestTypeDef",
     {
         "EventBusName": str,
     },
```

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/PKG-INFO` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.28.15
-Summary: Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/SOURCES.txt` & `mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15/setup.py` & `mypy-boto3-events-1.28.15.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-events",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder"
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

