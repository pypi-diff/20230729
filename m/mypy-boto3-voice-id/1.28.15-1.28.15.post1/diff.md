# Comparing `tmp/mypy-boto3-voice-id-1.28.15.tar.gz` & `tmp/mypy-boto3-voice-id-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-voice-id-1.28.15.tar", last modified: Fri Jul 28 20:43:55 2023, max compression
+gzip compressed data, was "mypy-boto3-voice-id-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:23 2023, max compression
```

## Comparing `mypy-boto3-voice-id-1.28.15.tar` & `mypy-boto3-voice-id-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.214021 mypy-boto3-voice-id-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-07-28 20:43:55.214021 mypy-boto3-voice-id-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16038 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.210021 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33375 2023-07-28 20:40:56.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33338 2023-07-28 20:40:56.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.214021 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-07-28 20:43:54.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:43:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:54.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:54.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:54.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:54.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:55.214021 mypy-boto3-voice-id-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.673449 mypy-boto3-voice-id-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-07-29 10:04:23.669449 mypy-boto3-voice-id-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16038 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.661449 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23305 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23263 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33375 2023-07-29 10:01:08.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33338 2023-07-29 10:01:08.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.669449 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:04:23.000000 mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:23.673449 mypy-boto3-voice-id-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-29 10:01:07.000000 mypy-boto3-voice-id-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-voice-id-1.28.15/LICENSE` & `mypy-boto3-voice-id-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15/PKG-INFO` & `mypy-boto3-voice-id-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.28.15
-Summary: Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-voice-id-1.28.15/README.md` & `mypy-boto3-voice-id-1.28.15.post1/README.md`

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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__init__.py` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__init__.pyi` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__main__.py` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VoiceID 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.VoiceID 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID\nOther"
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

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/client.py` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_voice_id.client import VoiceIDClient
 
     session = Session()
     client: VoiceIDClient = session.client("voice-id")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FraudsterRegistrationJobStatusType, SpeakerEnrollmentJobStatusType
 from .paginator import (
     ListDomainsPaginator,
     ListFraudsterRegistrationJobsPaginator,
@@ -35,26 +35,28 @@
     DescribeFraudsterRegistrationJobResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EnrollmentConfigOutputTypeDef,
     EnrollmentConfigTypeDef,
     EvaluateSessionResponseTypeDef,
     InputDataConfigTypeDef,
     ListDomainsResponseTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListFraudstersResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     ListSpeakersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     OutputDataConfigTypeDef,
+    RegistrationConfigOutputTypeDef,
     RegistrationConfigTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     TagTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
@@ -374,15 +376,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         JobName: str = ...,
-        RegistrationConfig: RegistrationConfigTypeDef = ...
+        RegistrationConfig: Union[RegistrationConfigTypeDef, RegistrationConfigOutputTypeDef] = ...
     ) -> StartFraudsterRegistrationJobResponseTypeDef:
         """
         Starts a new batch fraudster registration job using provided details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_fraudster_registration_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/client/#start_fraudster_registration_job)
         """
@@ -391,15 +393,15 @@
         self,
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
-        EnrollmentConfig: EnrollmentConfigTypeDef = ...,
+        EnrollmentConfig: Union[EnrollmentConfigTypeDef, EnrollmentConfigOutputTypeDef] = ...,
         JobName: str = ...
     ) -> StartSpeakerEnrollmentJobResponseTypeDef:
         """
         Starts a new batch speaker enrollment job using specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_speaker_enrollment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/client/#start_speaker_enrollment_job)
```

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/client.pyi` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_voice_id.client import VoiceIDClient
 
     session = Session()
     client: VoiceIDClient = session.client("voice-id")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FraudsterRegistrationJobStatusType, SpeakerEnrollmentJobStatusType
 from .paginator import (
     ListDomainsPaginator,
     ListFraudsterRegistrationJobsPaginator,
@@ -35,26 +35,28 @@
     DescribeFraudsterRegistrationJobResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EnrollmentConfigOutputTypeDef,
     EnrollmentConfigTypeDef,
     EvaluateSessionResponseTypeDef,
     InputDataConfigTypeDef,
     ListDomainsResponseTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListFraudstersResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     ListSpeakersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     OutputDataConfigTypeDef,
+    RegistrationConfigOutputTypeDef,
     RegistrationConfigTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     TagTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
@@ -343,15 +345,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         JobName: str = ...,
-        RegistrationConfig: RegistrationConfigTypeDef = ...
+        RegistrationConfig: Union[RegistrationConfigTypeDef, RegistrationConfigOutputTypeDef] = ...
     ) -> StartFraudsterRegistrationJobResponseTypeDef:
         """
         Starts a new batch fraudster registration job using provided details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_fraudster_registration_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/client/#start_fraudster_registration_job)
         """
@@ -359,15 +361,15 @@
         self,
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
-        EnrollmentConfig: EnrollmentConfigTypeDef = ...,
+        EnrollmentConfig: Union[EnrollmentConfigTypeDef, EnrollmentConfigOutputTypeDef] = ...,
         JobName: str = ...
     ) -> StartSpeakerEnrollmentJobResponseTypeDef:
         """
         Starts a new batch speaker enrollment job using specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_speaker_enrollment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/client/#start_speaker_enrollment_job)
```

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/literals.py` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/literals.pyi` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/paginator.py` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/paginator.pyi` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/type_defs.py` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/type_defs.pyi` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/PKG-INFO` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.28.15
-Summary: Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/SOURCES.txt` & `mypy-boto3-voice-id-1.28.15.post1/mypy_boto3_voice_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.15/setup.py` & `mypy-boto3-voice-id-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-voice-id",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_voice_id"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder"
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

