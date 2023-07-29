# Comparing `tmp/mypy-boto3-lex-models-1.28.15.tar.gz` & `tmp/mypy-boto3-lex-models-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lex-models-1.28.15.tar", last modified: Fri Jul 28 20:43:08 2023, max compression
+gzip compressed data, was "mypy-boto3-lex-models-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:30 2023, max compression
```

## Comparing `mypy-boto3-lex-models-1.28.15.tar` & `mypy-boto3-lex-models-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.621383 mypy-boto3-lex-models-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19425 2023-07-28 20:43:08.621383 mypy-boto3-lex-models-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.621383 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35106 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35047 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11225 2023-07-28 20:29:40.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-28 20:29:40.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48627 2023-07-28 20:29:43.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48567 2023-07-28 20:29:40.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.621383 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19425 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:08.621383 mypy-boto3-lex-models-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.541232 mypy-boto3-lex-models-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-07-29 10:03:30.541232 mypy-boto3-lex-models-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.525232 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35521 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35462 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11225 2023-07-29 09:49:17.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-29 09:49:17.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48713 2023-07-29 09:49:18.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48653 2023-07-29 09:49:17.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.537232 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:30.541232 mypy-boto3-lex-models-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-lex-models-1.28.15/LICENSE` & `mypy-boto3-lex-models-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15/PKG-INFO` & `mypy-boto3-lex-models-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-models
-Version: 1.28.15
-Summary: Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lex-models-1.28.15/README.md` & `mypy-boto3-lex-models-1.28.15.post1/README.md`

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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__init__.py` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__init__.pyi` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__main__.py` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.LexModelBuildingService 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService\nOther"
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

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/client.py` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
 from .type_defs import (
     CodeHookTypeDef,
     ConversationLogsRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EnumerationValueOutputTypeDef,
     EnumerationValueTypeDef,
+    FollowUpPromptOutputTypeDef,
     FollowUpPromptTypeDef,
     FulfillmentActivityTypeDef,
     GetBotAliasesResponseTypeDef,
     GetBotAliasResponseTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotResponseTypeDef,
@@ -76,23 +78,26 @@
     GetSlotTypeVersionsResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     InputContextTypeDef,
     IntentTypeDef,
     KendraConfigurationTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputContextTypeDef,
+    PromptOutputTypeDef,
     PromptTypeDef,
     PutBotAliasResponseTypeDef,
     PutBotResponseTypeDef,
     PutIntentResponseTypeDef,
     PutSlotTypeResponseTypeDef,
+    SlotOutputTypeDef,
     SlotTypeConfigurationTypeDef,
     SlotTypeDef,
     StartImportResponseTypeDef,
     StartMigrationResponseTypeDef,
+    StatementOutputTypeDef,
     StatementTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -516,16 +521,16 @@
         name: str,
         locale: LocaleType,
         childDirected: bool,
         description: str = ...,
         intents: Sequence[IntentTypeDef] = ...,
         enableModelImprovements: bool = ...,
         nluIntentConfidenceThreshold: float = ...,
-        clarificationPrompt: PromptTypeDef = ...,
-        abortStatement: StatementTypeDef = ...,
+        clarificationPrompt: Union[PromptTypeDef, PromptOutputTypeDef] = ...,
+        abortStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
         idleSessionTTLInSeconds: int = ...,
         voiceId: str = ...,
         checksum: str = ...,
         processBehavior: ProcessBehaviorType = ...,
         detectSentiment: bool = ...,
         createVersion: bool = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -557,20 +562,20 @@
         """
 
     def put_intent(
         self,
         *,
         name: str,
         description: str = ...,
-        slots: Sequence[SlotTypeDef] = ...,
+        slots: Sequence[Union[SlotTypeDef, SlotOutputTypeDef]] = ...,
         sampleUtterances: Sequence[str] = ...,
-        confirmationPrompt: PromptTypeDef = ...,
-        rejectionStatement: StatementTypeDef = ...,
-        followUpPrompt: FollowUpPromptTypeDef = ...,
-        conclusionStatement: StatementTypeDef = ...,
+        confirmationPrompt: Union[PromptTypeDef, PromptOutputTypeDef] = ...,
+        rejectionStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
+        followUpPrompt: Union[FollowUpPromptTypeDef, FollowUpPromptOutputTypeDef] = ...,
+        conclusionStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
         dialogCodeHook: CodeHookTypeDef = ...,
         fulfillmentActivity: FulfillmentActivityTypeDef = ...,
         parentIntentSignature: str = ...,
         checksum: str = ...,
         createVersion: bool = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
@@ -584,15 +589,17 @@
         """
 
     def put_slot_type(
         self,
         *,
         name: str,
         description: str = ...,
-        enumerationValues: Sequence[EnumerationValueTypeDef] = ...,
+        enumerationValues: Sequence[
+            Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
+        ] = ...,
         checksum: str = ...,
         valueSelectionStrategy: SlotValueSelectionStrategyType = ...,
         createVersion: bool = ...,
         parentSlotTypeSignature: str = ...,
         slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...
     ) -> PutSlotTypeResponseTypeDef:
         """
```

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/client.pyi` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
 from .type_defs import (
     CodeHookTypeDef,
     ConversationLogsRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EnumerationValueOutputTypeDef,
     EnumerationValueTypeDef,
+    FollowUpPromptOutputTypeDef,
     FollowUpPromptTypeDef,
     FulfillmentActivityTypeDef,
     GetBotAliasesResponseTypeDef,
     GetBotAliasResponseTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotResponseTypeDef,
@@ -76,23 +78,26 @@
     GetSlotTypeVersionsResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     InputContextTypeDef,
     IntentTypeDef,
     KendraConfigurationTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputContextTypeDef,
+    PromptOutputTypeDef,
     PromptTypeDef,
     PutBotAliasResponseTypeDef,
     PutBotResponseTypeDef,
     PutIntentResponseTypeDef,
     PutSlotTypeResponseTypeDef,
+    SlotOutputTypeDef,
     SlotTypeConfigurationTypeDef,
     SlotTypeDef,
     StartImportResponseTypeDef,
     StartMigrationResponseTypeDef,
+    StatementOutputTypeDef,
     StatementTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -474,16 +479,16 @@
         name: str,
         locale: LocaleType,
         childDirected: bool,
         description: str = ...,
         intents: Sequence[IntentTypeDef] = ...,
         enableModelImprovements: bool = ...,
         nluIntentConfidenceThreshold: float = ...,
-        clarificationPrompt: PromptTypeDef = ...,
-        abortStatement: StatementTypeDef = ...,
+        clarificationPrompt: Union[PromptTypeDef, PromptOutputTypeDef] = ...,
+        abortStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
         idleSessionTTLInSeconds: int = ...,
         voiceId: str = ...,
         checksum: str = ...,
         processBehavior: ProcessBehaviorType = ...,
         detectSentiment: bool = ...,
         createVersion: bool = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -513,20 +518,20 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#put_bot_alias)
         """
     def put_intent(
         self,
         *,
         name: str,
         description: str = ...,
-        slots: Sequence[SlotTypeDef] = ...,
+        slots: Sequence[Union[SlotTypeDef, SlotOutputTypeDef]] = ...,
         sampleUtterances: Sequence[str] = ...,
-        confirmationPrompt: PromptTypeDef = ...,
-        rejectionStatement: StatementTypeDef = ...,
-        followUpPrompt: FollowUpPromptTypeDef = ...,
-        conclusionStatement: StatementTypeDef = ...,
+        confirmationPrompt: Union[PromptTypeDef, PromptOutputTypeDef] = ...,
+        rejectionStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
+        followUpPrompt: Union[FollowUpPromptTypeDef, FollowUpPromptOutputTypeDef] = ...,
+        conclusionStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
         dialogCodeHook: CodeHookTypeDef = ...,
         fulfillmentActivity: FulfillmentActivityTypeDef = ...,
         parentIntentSignature: str = ...,
         checksum: str = ...,
         createVersion: bool = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
@@ -539,15 +544,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#put_intent)
         """
     def put_slot_type(
         self,
         *,
         name: str,
         description: str = ...,
-        enumerationValues: Sequence[EnumerationValueTypeDef] = ...,
+        enumerationValues: Sequence[
+            Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
+        ] = ...,
         checksum: str = ...,
         valueSelectionStrategy: SlotValueSelectionStrategyType = ...,
         createVersion: bool = ...,
         parentSlotTypeSignature: str = ...,
         slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...
     ) -> PutSlotTypeResponseTypeDef:
         """
```

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/literals.py` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/literals.pyi` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/paginator.py` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/paginator.pyi` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/type_defs.py` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1747,15 +1747,17 @@
         "name": str,
     },
 )
 _OptionalPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_OptionalPutSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "enumerationValues": Sequence[EnumerationValueTypeDef],
+        "enumerationValues": Sequence[
+            Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
+        ],
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
@@ -1886,15 +1888,15 @@
         "name": str,
     },
 )
 _OptionalPutIntentRequestRequestTypeDef = TypedDict(
     "_OptionalPutIntentRequestRequestTypeDef",
     {
         "description": str,
-        "slots": Sequence[SlotTypeDef],
+        "slots": Sequence[Union[SlotTypeDef, SlotOutputTypeDef]],
         "sampleUtterances": Sequence[str],
         "confirmationPrompt": PromptTypeDef,
         "rejectionStatement": StatementTypeDef,
         "followUpPrompt": FollowUpPromptTypeDef,
         "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
```

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/type_defs.pyi` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1690,15 +1690,17 @@
         "name": str,
     },
 )
 _OptionalPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_OptionalPutSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "enumerationValues": Sequence[EnumerationValueTypeDef],
+        "enumerationValues": Sequence[
+            Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
+        ],
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
@@ -1827,15 +1829,15 @@
         "name": str,
     },
 )
 _OptionalPutIntentRequestRequestTypeDef = TypedDict(
     "_OptionalPutIntentRequestRequestTypeDef",
     {
         "description": str,
-        "slots": Sequence[SlotTypeDef],
+        "slots": Sequence[Union[SlotTypeDef, SlotOutputTypeDef]],
         "sampleUtterances": Sequence[str],
         "confirmationPrompt": PromptTypeDef,
         "rejectionStatement": StatementTypeDef,
         "followUpPrompt": FollowUpPromptTypeDef,
         "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
```

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/PKG-INFO` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-models
-Version: 1.28.15
-Summary: Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/SOURCES.txt` & `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15/setup.py` & `mypy-boto3-lex-models-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lex-models",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_lex_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with"
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

