# Comparing `tmp/mypy-boto3-ssm-incidents-1.28.15.tar.gz` & `tmp/mypy-boto3-ssm-incidents-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-incidents-1.28.15.tar", last modified: Fri Jul 28 20:43:48 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-incidents-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:16 2023, max compression
```

## Comparing `mypy-boto3-ssm-incidents-1.28.15.tar` & `mypy-boto3-ssm-incidents-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.757933 mypy-boto3-ssm-incidents-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-07-28 20:43:48.757933 mypy-boto3-ssm-incidents-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.757933 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35552 2023-07-28 20:40:06.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35484 2023-07-28 20:40:06.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.757933 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:48.757933 mypy-boto3-ssm-incidents-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-28 20:40:04.000000 mypy-boto3-ssm-incidents-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.089419 mypy-boto3-ssm-incidents-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-29 10:04:16.089419 mypy-boto3-ssm-incidents-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.085419 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25970 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35608 2023-07-29 10:00:18.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35540 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.089419 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:16.089419 mypy-boto3-ssm-incidents-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15/LICENSE` & `mypy-boto3-ssm-incidents-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15/PKG-INFO` & `mypy-boto3-ssm-incidents-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-incidents
-Version: 1.28.15
-Summary: Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15/README.md` & `mypy-boto3-ssm-incidents-1.28.15.post1/README.md`

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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__init__.py` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__init__.pyi` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__main__.py` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSMIncidents 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.SSMIncidents 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents\nOther"
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

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/client.py` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,26 +25,29 @@
     ListIncidentRecordsPaginator,
     ListRelatedItemsPaginator,
     ListReplicationSetsPaginator,
     ListResponsePlansPaginator,
     ListTimelineEventsPaginator,
 )
 from .type_defs import (
+    ActionOutputTypeDef,
     ActionTypeDef,
+    ChatChannelOutputTypeDef,
     ChatChannelTypeDef,
     CreateReplicationSetOutputTypeDef,
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     EventReferenceTypeDef,
     FilterTypeDef,
     GetIncidentRecordOutputTypeDef,
     GetReplicationSetOutputTypeDef,
     GetResourcePoliciesOutputTypeDef,
     GetResponsePlanOutputTypeDef,
     GetTimelineEventOutputTypeDef,
+    IncidentTemplateOutputTypeDef,
     IncidentTemplateTypeDef,
     IntegrationTypeDef,
     ListIncidentRecordsOutputTypeDef,
     ListRelatedItemsOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListResponsePlansOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -135,18 +138,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_replication_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#create_replication_set)
         """
 
     def create_response_plan(
         self,
         *,
-        incidentTemplate: IncidentTemplateTypeDef,
+        incidentTemplate: Union[IncidentTemplateTypeDef, IncidentTemplateOutputTypeDef],
         name: str,
-        actions: Sequence[ActionTypeDef] = ...,
-        chatChannel: ChatChannelTypeDef = ...,
+        actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
+        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         integrations: Sequence[IntegrationTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResponsePlanOutputTypeDef:
         """
@@ -393,15 +396,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_deletion_protection)
         """
 
     def update_incident_record(
         self,
         *,
         arn: str,
-        chatChannel: ChatChannelTypeDef = ...,
+        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
         clientToken: str = ...,
         impact: int = ...,
         notificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         status: IncidentRecordStatusType = ...,
         summary: str = ...,
         title: str = ...
     ) -> Dict[str, Any]:
@@ -440,16 +443,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_replication_set)
         """
 
     def update_response_plan(
         self,
         *,
         arn: str,
-        actions: Sequence[ActionTypeDef] = ...,
-        chatChannel: ChatChannelTypeDef = ...,
+        actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
+        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         incidentTemplateDedupeString: str = ...,
         incidentTemplateImpact: int = ...,
         incidentTemplateNotificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         incidentTemplateSummary: str = ...,
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/client.pyi` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,26 +25,29 @@
     ListIncidentRecordsPaginator,
     ListRelatedItemsPaginator,
     ListReplicationSetsPaginator,
     ListResponsePlansPaginator,
     ListTimelineEventsPaginator,
 )
 from .type_defs import (
+    ActionOutputTypeDef,
     ActionTypeDef,
+    ChatChannelOutputTypeDef,
     ChatChannelTypeDef,
     CreateReplicationSetOutputTypeDef,
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     EventReferenceTypeDef,
     FilterTypeDef,
     GetIncidentRecordOutputTypeDef,
     GetReplicationSetOutputTypeDef,
     GetResourcePoliciesOutputTypeDef,
     GetResponsePlanOutputTypeDef,
     GetTimelineEventOutputTypeDef,
+    IncidentTemplateOutputTypeDef,
     IncidentTemplateTypeDef,
     IntegrationTypeDef,
     ListIncidentRecordsOutputTypeDef,
     ListRelatedItemsOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListResponsePlansOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -127,18 +130,18 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_replication_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#create_replication_set)
         """
     def create_response_plan(
         self,
         *,
-        incidentTemplate: IncidentTemplateTypeDef,
+        incidentTemplate: Union[IncidentTemplateTypeDef, IncidentTemplateOutputTypeDef],
         name: str,
-        actions: Sequence[ActionTypeDef] = ...,
-        chatChannel: ChatChannelTypeDef = ...,
+        actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
+        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         integrations: Sequence[IntegrationTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResponsePlanOutputTypeDef:
         """
@@ -361,15 +364,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_deletion_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_deletion_protection)
         """
     def update_incident_record(
         self,
         *,
         arn: str,
-        chatChannel: ChatChannelTypeDef = ...,
+        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
         clientToken: str = ...,
         impact: int = ...,
         notificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         status: IncidentRecordStatusType = ...,
         summary: str = ...,
         title: str = ...
     ) -> Dict[str, Any]:
@@ -405,16 +408,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_replication_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_replication_set)
         """
     def update_response_plan(
         self,
         *,
         arn: str,
-        actions: Sequence[ActionTypeDef] = ...,
-        chatChannel: ChatChannelTypeDef = ...,
+        actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
+        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         incidentTemplateDedupeString: str = ...,
         incidentTemplateImpact: int = ...,
         incidentTemplateNotificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         incidentTemplateSummary: str = ...,
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/literals.py` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/literals.pyi` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/paginator.py` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/paginator.pyi` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/type_defs.py` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1308,15 +1308,15 @@
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
 )
 _OptionalCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalCreateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[ActionTypeDef],
+        "actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
@@ -1350,15 +1350,15 @@
     {
         "arn": str,
     },
 )
 _OptionalUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalUpdateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[ActionTypeDef],
+        "actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "incidentTemplateDedupeString": str,
         "incidentTemplateImpact": int,
         "incidentTemplateNotificationTargets": Sequence[NotificationTargetItemTypeDef],
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/type_defs.pyi` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1247,15 +1247,15 @@
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
 )
 _OptionalCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalCreateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[ActionTypeDef],
+        "actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
@@ -1287,15 +1287,15 @@
     {
         "arn": str,
     },
 )
 _OptionalUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalUpdateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[ActionTypeDef],
+        "actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "incidentTemplateDedupeString": str,
         "incidentTemplateImpact": int,
         "incidentTemplateNotificationTargets": Sequence[NotificationTargetItemTypeDef],
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/waiter.py` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/waiter.pyi` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/PKG-INFO` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-incidents
-Version: 1.28.15
-Summary: Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt` & `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15/setup.py` & `mypy-boto3-ssm-incidents-1.28.15.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-incidents",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_ssm_incidents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder"
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

