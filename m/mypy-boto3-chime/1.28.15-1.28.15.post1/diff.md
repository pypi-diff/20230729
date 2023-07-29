# Comparing `tmp/mypy-boto3-chime-1.28.15.tar.gz` & `tmp/mypy-boto3-chime-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:38 2023, max compression
```

## Comparing `mypy-boto3-chime-1.28.15.tar` & `mypy-boto3-chime-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.352738 mypy-boto3-chime-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32817 2023-07-28 20:42:22.352738 mypy-boto3-chime-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31338 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.352738 mypy-boto3-chime-1.28.15/mypy_boto3_chime/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   121396 2023-07-28 20:20:27.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   121196 2023-07-28 20:20:26.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-28 20:20:27.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-07-28 20:20:27.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-28 20:20:27.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-28 20:20:27.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   146654 2023-07-28 20:20:32.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   146493 2023-07-28 20:20:30.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.352738 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32817 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.352738 mypy-boto3-chime-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.097036 mypy-boto3-chime-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32823 2023-07-29 10:02:38.097036 mypy-boto3-chime-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31338 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.077036 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121941 2023-07-29 09:39:20.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121741 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-29 09:39:20.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-07-29 09:39:20.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-29 09:39:20.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-29 09:39:20.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   146654 2023-07-29 09:39:25.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146493 2023-07-29 09:39:22.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:18.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:38.097036 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32823 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:02:37.000000 mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:38.097036 mypy-boto3-chime-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:39:17.000000 mypy-boto3-chime-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-chime-1.28.15/LICENSE` & `mypy-boto3-chime-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15/PKG-INFO` & `mypy-boto3-chime-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.28.15
-Summary: Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-1.28.15/README.md` & `mypy-boto3-chime-1.28.15.post1/README.md`

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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/__init__.py` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/__init__.pyi` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/__main__.py` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Chime 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Chime 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime\nOther"
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

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/client.py` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     BatchCreateRoomMembershipResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
     BatchUnsuspendUserResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     BatchUpdateUserResponseTypeDef,
     BusinessCallingSettingsTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     CreateAccountResponseTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeResponseTypeDef,
@@ -91,14 +92,15 @@
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetAccountResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
@@ -160,14 +162,15 @@
     ListUsersResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     LoggingConfigurationTypeDef,
     MeetingNotificationConfigurationTypeDef,
     MembershipItemTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     PutRetentionSettingsResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
@@ -183,16 +186,18 @@
     RetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     SigninDelegateGroupTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
     TagTypeDef,
+    TerminationOutputTypeDef,
     TerminationTypeDef,
     TranscriptionConfigurationTypeDef,
     UpdateAccountResponseTypeDef,
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
@@ -541,15 +546,17 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...
+        ChimeSdkMeetingConfiguration: Union[
+            ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+        ] = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_media_capture_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#create_media_capture_pipeline)
         """
@@ -1899,15 +1906,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_sip_media_application_logging_configuration)
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
         Puts emergency calling configuration details to the specified Amazon Chime Voice
         Connector, such as emergency phone numbers and calling countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_emergency_calling_configuration)
@@ -1920,15 +1929,18 @@
         Adds a logging configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_logging_configuration)
         """
 
     def put_voice_connector_origination(
-        self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
+        self,
+        *,
+        VoiceConnectorId: str,
+        Origination: Union[OriginationTypeDef, OriginationOutputTypeDef]
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Adds origination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_origination)
         """
@@ -1947,25 +1959,33 @@
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_proxy)
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
         Adds a streaming configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_streaming_configuration)
         """
 
     def put_voice_connector_termination(
-        self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
+        self,
+        *,
+        VoiceConnectorId: str,
+        Termination: Union[TerminationTypeDef, TerminationOutputTypeDef]
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Adds termination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_termination)
         """
```

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/client.pyi` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     BatchCreateRoomMembershipResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
     BatchUnsuspendUserResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     BatchUpdateUserResponseTypeDef,
     BusinessCallingSettingsTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     CreateAccountResponseTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeResponseTypeDef,
@@ -91,14 +92,15 @@
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetAccountResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
@@ -160,14 +162,15 @@
     ListUsersResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     LoggingConfigurationTypeDef,
     MeetingNotificationConfigurationTypeDef,
     MembershipItemTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     PutRetentionSettingsResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
@@ -183,16 +186,18 @@
     RetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     SigninDelegateGroupTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
     TagTypeDef,
+    TerminationOutputTypeDef,
     TerminationTypeDef,
     TranscriptionConfigurationTypeDef,
     UpdateAccountResponseTypeDef,
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
@@ -512,15 +517,17 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...
+        ChimeSdkMeetingConfiguration: Union[
+            ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+        ] = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_media_capture_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#create_media_capture_pipeline)
         """
@@ -1745,15 +1752,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_sip_media_application_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_sip_media_application_logging_configuration)
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
         Puts emergency calling configuration details to the specified Amazon Chime Voice
         Connector, such as emergency phone numbers and calling countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_emergency_calling_configuration)
@@ -1764,15 +1773,18 @@
         """
         Adds a logging configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_logging_configuration)
         """
     def put_voice_connector_origination(
-        self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
+        self,
+        *,
+        VoiceConnectorId: str,
+        Origination: Union[OriginationTypeDef, OriginationOutputTypeDef]
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Adds origination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_origination)
         """
@@ -1789,24 +1801,32 @@
         Puts the specified proxy configuration to the specified Amazon Chime Voice
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_proxy)
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
         Adds a streaming configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_streaming_configuration)
         """
     def put_voice_connector_termination(
-        self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
+        self,
+        *,
+        VoiceConnectorId: str,
+        Termination: Union[TerminationTypeDef, TerminationOutputTypeDef]
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Adds termination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#put_voice_connector_termination)
         """
```

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/literals.py` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/literals.pyi` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/paginator.py` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/paginator.pyi` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/type_defs.py` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime/type_defs.pyi` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/PKG-INFO` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.28.15
-Summary: Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/SOURCES.txt` & `mypy-boto3-chime-1.28.15.post1/mypy_boto3_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.15/setup.py` & `mypy-boto3-chime-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

