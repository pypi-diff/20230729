# Comparing `tmp/mypy-boto3-chime-sdk-voice-1.28.15.tar.gz` & `tmp/mypy-boto3-chime-sdk-voice-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:40 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-voice-1.28.15.tar` & `mypy-boto3-chime-sdk-voice-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.332780 mypy-boto3-chime-sdk-voice-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23696 2023-07-28 20:42:25.332780 mypy-boto3-chime-sdk-voice-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.332780 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66722 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66620 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71721 2023-07-28 20:20:46.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71668 2023-07-28 20:20:44.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.332780 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23696 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.332780 mypy-boto3-chime-sdk-voice-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:40.685047 mypy-boto3-chime-sdk-voice-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:35.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-07-29 10:02:40.685047 mypy-boto3-chime-sdk-voice-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-29 09:39:35.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:40.673047 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-29 09:39:35.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-29 09:39:35.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:39:35.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67315 2023-07-29 09:39:36.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67213 2023-07-29 09:39:35.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-29 09:39:36.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-29 09:39:36.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-29 09:39:36.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-29 09:39:36.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:35.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71721 2023-07-29 09:39:39.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71668 2023-07-29 09:39:37.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:35.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:40.685047 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:02:40.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:40.685047 mypy-boto3-chime-sdk-voice-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-29 09:39:35.000000 mypy-boto3-chime-sdk-voice-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/LICENSE` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/PKG-INFO` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.28.15
-Summary: Type annotations for boto3.ChimeSDKVoice 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ChimeSDKVoice 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/README.md` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/README.md`

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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__init__.py` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__init__.pyi` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__main__.py` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKVoice 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.ChimeSDKVoice 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice\nOther"
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

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/client.py` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_chime_sdk_voice.client import ChimeSDKVoiceClient
 
     session = Session()
     client: ChimeSDKVoiceClient = session.client("chime-sdk-voice")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CallLegTypeType,
     CapabilityType,
     GeoMatchLevelType,
@@ -44,14 +44,15 @@
     CreateVoiceConnectorGroupResponseTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     CreateVoiceProfileDomainResponseTypeDef,
     CreateVoiceProfileResponseTypeDef,
     CredentialTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetGlobalSettingsResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
@@ -83,34 +84,38 @@
     ListTagsForResourceResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
     LoggingConfigurationTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
     StartSpeakerSearchTaskResponseTypeDef,
     StartVoiceToneAnalysisTaskResponseTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
     TagTypeDef,
+    TerminationOutputTypeDef,
     TerminationTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
@@ -908,15 +913,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profiles)
         """
 
     def put_sip_media_application_alexa_skill_configuration(
         self,
         *,
         SipMediaApplicationId: str,
-        SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationTypeDef = ...
+        SipMediaApplicationAlexaSkillConfiguration: Union[
+            SipMediaApplicationAlexaSkillConfigurationTypeDef,
+            SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
+        ] = ...
     ) -> PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:
         """
         Updates the Alexa Skill configuration for the SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_alexa_skill_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_alexa_skill_configuration)
         """
@@ -934,15 +942,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_logging_configuration)
         """
 
     def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
+        EmergencyCallingConfiguration: Union[
+            EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
+        ]
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Updates a Voice Connector's emergency calling configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_emergency_calling_configuration)
         """
@@ -954,15 +964,18 @@
         Updates a Voice Connector's logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_logging_configuration)
         """
 
     def put_voice_connector_origination(
-        self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
+        self,
+        *,
+        VoiceConnectorId: str,
+        Origination: Union[OriginationTypeDef, OriginationOutputTypeDef]
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Updates a Voice Connector's origination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_origination)
         """
@@ -981,25 +994,33 @@
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_proxy)
         """
 
     def put_voice_connector_streaming_configuration(
-        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationTypeDef
+        self,
+        *,
+        VoiceConnectorId: str,
+        StreamingConfiguration: Union[
+            StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
+        ]
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
         Updates a Voice Connector's streaming configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_streaming_configuration)
         """
 
     def put_voice_connector_termination(
-        self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
+        self,
+        *,
+        VoiceConnectorId: str,
+        Termination: Union[TerminationTypeDef, TerminationOutputTypeDef]
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Updates a Voice Connector's termination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_termination)
         """
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/client.pyi` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_chime_sdk_voice.client import ChimeSDKVoiceClient
 
     session = Session()
     client: ChimeSDKVoiceClient = session.client("chime-sdk-voice")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CallLegTypeType,
     CapabilityType,
     GeoMatchLevelType,
@@ -44,14 +44,15 @@
     CreateVoiceConnectorGroupResponseTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     CreateVoiceProfileDomainResponseTypeDef,
     CreateVoiceProfileResponseTypeDef,
     CredentialTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetGlobalSettingsResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
@@ -83,34 +84,38 @@
     ListTagsForResourceResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
     LoggingConfigurationTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
     StartSpeakerSearchTaskResponseTypeDef,
     StartVoiceToneAnalysisTaskResponseTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
     TagTypeDef,
+    TerminationOutputTypeDef,
     TerminationTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
@@ -836,15 +841,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profiles)
         """
     def put_sip_media_application_alexa_skill_configuration(
         self,
         *,
         SipMediaApplicationId: str,
-        SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationTypeDef = ...
+        SipMediaApplicationAlexaSkillConfiguration: Union[
+            SipMediaApplicationAlexaSkillConfigurationTypeDef,
+            SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
+        ] = ...
     ) -> PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:
         """
         Updates the Alexa Skill configuration for the SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_alexa_skill_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_alexa_skill_configuration)
         """
@@ -860,15 +868,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_logging_configuration)
         """
     def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
+        EmergencyCallingConfiguration: Union[
+            EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
+        ]
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Updates a Voice Connector's emergency calling configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_emergency_calling_configuration)
         """
@@ -878,15 +888,18 @@
         """
         Updates a Voice Connector's logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_logging_configuration)
         """
     def put_voice_connector_origination(
-        self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
+        self,
+        *,
+        VoiceConnectorId: str,
+        Origination: Union[OriginationTypeDef, OriginationOutputTypeDef]
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Updates a Voice Connector's origination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_origination)
         """
@@ -903,24 +916,32 @@
         Puts the specified proxy configuration to the specified Amazon Chime SDK Voice
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_proxy)
         """
     def put_voice_connector_streaming_configuration(
-        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationTypeDef
+        self,
+        *,
+        VoiceConnectorId: str,
+        StreamingConfiguration: Union[
+            StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
+        ]
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
         Updates a Voice Connector's streaming configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_streaming_configuration)
         """
     def put_voice_connector_termination(
-        self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
+        self,
+        *,
+        VoiceConnectorId: str,
+        Termination: Union[TerminationTypeDef, TerminationOutputTypeDef]
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Updates a Voice Connector's termination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_termination)
         """
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/literals.py` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/literals.pyi` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/paginator.py` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/paginator.pyi` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/type_defs.py` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/type_defs.pyi` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.28.15
-Summary: Type annotations for boto3.ChimeSDKVoice 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ChimeSDKVoice 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.15/setup.py` & `mypy-boto3-chime-sdk-voice-1.28.15.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-voice",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_chime_sdk_voice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ChimeSDKVoice 1.28.15 service generated with mypy-boto3-builder"
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

