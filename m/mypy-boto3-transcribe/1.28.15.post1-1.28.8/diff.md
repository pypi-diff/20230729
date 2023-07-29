# Comparing `tmp/mypy-boto3-transcribe-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-transcribe-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transcribe-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:22 2023, max compression
+gzip compressed data, was "mypy-boto3-transcribe-1.28.8.tar", last modified: Thu Jul 20 19:47:57 2023, max compression
```

## Comparing `mypy-boto3-transcribe-1.28.15.post1.tar` & `mypy-boto3-transcribe-1.28.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.585445 mypy-boto3-transcribe-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:53.000000 mypy-boto3-transcribe-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-07-29 10:04:22.585445 mypy-boto3-transcribe-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-29 10:00:53.000000 mypy-boto3-transcribe-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.577444 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-29 10:00:54.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-29 10:00:54.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 10:00:54.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30273 2023-07-29 10:00:54.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30227 2023-07-29 10:00:54.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-07-29 10:00:54.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-29 10:00:54.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:54.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42672 2023-07-29 10:00:55.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42635 2023-07-29 10:00:55.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:54.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.585445 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-07-29 10:04:22.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 10:04:22.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:22.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:04:22.000000 mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:22.585445 mypy-boto3-transcribe-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 10:00:53.000000 mypy-boto3-transcribe-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29784 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44839 2023-07-20 19:47:45.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/setup.py
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/LICENSE` & `mypy-boto3-transcribe-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.15.post1/PKG-INFO` & `mypy-boto3-transcribe-1.28.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.TranscribeService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.8
+Summary: Type annotations for boto3.TranscribeService 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,25 +318,29 @@
 ### Typed dictionaries
 
 `mypy_boto3_transcribe.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transcribe.type_defs import (
+    AbsoluteTimeRangeOutputTypeDef,
     AbsoluteTimeRangeTypeDef,
     ContentRedactionOutputTypeDef,
-    LanguageIdSettingsTypeDef,
+    LanguageIdSettingsOutputTypeDef,
     ContentRedactionTypeDef,
+    LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
-    ChannelDefinitionTypeDef,
-    MediaTypeDef,
+    ChannelDefinitionOutputTypeDef,
+    MediaOutputTypeDef,
     TranscriptTypeDef,
+    ChannelDefinitionTypeDef,
     ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
+    InputDataConfigOutputTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
@@ -345,37 +349,44 @@
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
     GetVocabularyRequestRequestTypeDef,
+    RelativeTimeRangeOutputTypeDef,
     RelativeTimeRangeTypeDef,
+    JobExecutionSettingsOutputTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
     MedicalTranscriptionJobSummaryTypeDef,
     ListMedicalVocabulariesRequestRequestTypeDef,
     VocabularyInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
+    MediaTypeDef,
     MedicalTranscriptTypeDef,
+    MedicalTranscriptionSettingOutputTypeDef,
     MedicalTranscriptionSettingTypeDef,
+    ModelSettingsOutputTypeDef,
     ModelSettingsTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
-    ToxicityDetectionSettingsOutputTypeDef,
     ToxicityDetectionSettingsTypeDef,
     SubtitlesOutputTypeDef,
+    ToxicityDetectionSettingsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
     CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
@@ -385,36 +396,38 @@
     GetMedicalVocabularyResponseTypeDef,
     GetVocabularyFilterResponseTypeDef,
     GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
-    CreateLanguageModelResponseTypeDef,
-    LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateLanguageModelResponseTypeDef,
+    LanguageModelTypeDef,
+    InterruptionFilterOutputTypeDef,
+    NonTalkTimeFilterOutputTypeDef,
+    SentimentFilterOutputTypeDef,
+    TranscriptFilterOutputTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
-    SentimentFilterOutputTypeDef,
     SentimentFilterTypeDef,
-    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
-    TranscriptionJobSummaryTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
+    TranscriptionJobSummaryTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
     StartCallAnalyticsJobRequestRequestTypeDef,
     DescribeLanguageModelResponseTypeDef,
     ListLanguageModelsResponseTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
@@ -431,15 +444,15 @@
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_structure() -> AbsoluteTimeRangeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/README.md` & `mypy-boto3-transcribe-1.28.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,25 +286,29 @@
 ### Typed dictionaries
 
 `mypy_boto3_transcribe.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transcribe.type_defs import (
+    AbsoluteTimeRangeOutputTypeDef,
     AbsoluteTimeRangeTypeDef,
     ContentRedactionOutputTypeDef,
-    LanguageIdSettingsTypeDef,
+    LanguageIdSettingsOutputTypeDef,
     ContentRedactionTypeDef,
+    LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
-    ChannelDefinitionTypeDef,
-    MediaTypeDef,
+    ChannelDefinitionOutputTypeDef,
+    MediaOutputTypeDef,
     TranscriptTypeDef,
+    ChannelDefinitionTypeDef,
     ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
+    InputDataConfigOutputTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
@@ -313,37 +317,44 @@
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
     GetVocabularyRequestRequestTypeDef,
+    RelativeTimeRangeOutputTypeDef,
     RelativeTimeRangeTypeDef,
+    JobExecutionSettingsOutputTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
     MedicalTranscriptionJobSummaryTypeDef,
     ListMedicalVocabulariesRequestRequestTypeDef,
     VocabularyInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
+    MediaTypeDef,
     MedicalTranscriptTypeDef,
+    MedicalTranscriptionSettingOutputTypeDef,
     MedicalTranscriptionSettingTypeDef,
+    ModelSettingsOutputTypeDef,
     ModelSettingsTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
-    ToxicityDetectionSettingsOutputTypeDef,
     ToxicityDetectionSettingsTypeDef,
     SubtitlesOutputTypeDef,
+    ToxicityDetectionSettingsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
     CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
@@ -353,36 +364,38 @@
     GetMedicalVocabularyResponseTypeDef,
     GetVocabularyFilterResponseTypeDef,
     GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
-    CreateLanguageModelResponseTypeDef,
-    LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateLanguageModelResponseTypeDef,
+    LanguageModelTypeDef,
+    InterruptionFilterOutputTypeDef,
+    NonTalkTimeFilterOutputTypeDef,
+    SentimentFilterOutputTypeDef,
+    TranscriptFilterOutputTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
-    SentimentFilterOutputTypeDef,
     SentimentFilterTypeDef,
-    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
-    TranscriptionJobSummaryTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
+    TranscriptionJobSummaryTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
     StartCallAnalyticsJobRequestRequestTypeDef,
     DescribeLanguageModelResponseTypeDef,
     ListLanguageModelsResponseTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
@@ -399,15 +412,15 @@
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_structure() -> AbsoluteTimeRangeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/__main__.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TranscribeService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.TranscribeService 1.28.8\nVersion:         1.28.8\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/client.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_transcribe.client import TranscribeServiceClient
 
     session = Session()
     client: TranscribeServiceClient = session.client("transcribe")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BaseModelNameType,
     CallAnalyticsJobStatusType,
     CLMLanguageCodeType,
@@ -27,18 +27,16 @@
     MediaFormatType,
     ModelStatusType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyStateType,
 )
 from .type_defs import (
-    CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
     ChannelDefinitionTypeDef,
-    ContentRedactionOutputTypeDef,
     ContentRedactionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
     CreateVocabularyFilterResponseTypeDef,
     CreateVocabularyResponseTypeDef,
     DescribeLanguageModelResponseTypeDef,
@@ -61,56 +59,50 @@
     ListTagsForResourceResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MediaTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    RuleOutputTypeDef,
     RuleTypeDef,
     SettingsTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     SubtitlesTypeDef,
     TagTypeDef,
-    ToxicityDetectionSettingsOutputTypeDef,
     ToxicityDetectionSettingsTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TranscribeServiceClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
 
-
 class TranscribeServiceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/)
     """
 
     meta: ClientMeta
@@ -119,45 +111,37 @@
     def exceptions(self) -> Exceptions:
         """
         TranscribeServiceClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#close)
         """
-
     def create_call_analytics_category(
-        self,
-        *,
-        CategoryName: str,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
-        InputType: InputTypeType = ...
+        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
     ) -> CreateCallAnalyticsCategoryResponseTypeDef:
         """
         Creates a new Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_call_analytics_category)
         """
-
     def create_language_model(
         self,
         *,
         LanguageCode: CLMLanguageCodeType,
         BaseModelName: BaseModelNameType,
         ModelName: str,
         InputDataConfig: InputDataConfigTypeDef,
@@ -165,30 +149,28 @@
     ) -> CreateLanguageModelResponseTypeDef:
         """
         Creates a new custom language model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_language_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_language_model)
         """
-
     def create_medical_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         VocabularyFileUri: str,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMedicalVocabularyResponseTypeDef:
         """
         Creates a new custom medical vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_medical_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_medical_vocabulary)
         """
-
     def create_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
@@ -197,15 +179,14 @@
     ) -> CreateVocabularyResponseTypeDef:
         """
         Creates a new custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_vocabulary)
         """
-
     def create_vocabulary_filter(
         self,
         *,
         VocabularyFilterName: str,
         LanguageCode: LanguageCodeType,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
@@ -214,229 +195,207 @@
     ) -> CreateVocabularyFilterResponseTypeDef:
         """
         Creates a new custom vocabulary filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_vocabulary_filter)
         """
-
     def delete_call_analytics_category(self, *, CategoryName: str) -> Dict[str, Any]:
         """
         Deletes a Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_call_analytics_category)
         """
-
     def delete_call_analytics_job(self, *, CallAnalyticsJobName: str) -> Dict[str, Any]:
         """
         Deletes a Call Analytics job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_call_analytics_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_call_analytics_job)
         """
-
     def delete_language_model(self, *, ModelName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a custom language model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_language_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_language_model)
         """
-
     def delete_medical_transcription_job(
         self, *, MedicalTranscriptionJobName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a medical transcription job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_medical_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_medical_transcription_job)
         """
-
     def delete_medical_vocabulary(self, *, VocabularyName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a custom medical vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_medical_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_medical_vocabulary)
         """
-
     def delete_transcription_job(
         self, *, TranscriptionJobName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a transcription job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_transcription_job)
         """
-
     def delete_vocabulary(self, *, VocabularyName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_vocabulary)
         """
-
     def delete_vocabulary_filter(
         self, *, VocabularyFilterName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a custom vocabulary filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_vocabulary_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_vocabulary_filter)
         """
-
     def describe_language_model(self, *, ModelName: str) -> DescribeLanguageModelResponseTypeDef:
         """
         Provides information about the specified custom language model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.describe_language_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#describe_language_model)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#generate_presigned_url)
         """
-
     def get_call_analytics_category(
         self, *, CategoryName: str
     ) -> GetCallAnalyticsCategoryResponseTypeDef:
         """
         Provides information about the specified Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_call_analytics_category)
         """
-
     def get_call_analytics_job(
         self, *, CallAnalyticsJobName: str
     ) -> GetCallAnalyticsJobResponseTypeDef:
         """
         Provides information about the specified Call Analytics job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_call_analytics_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_call_analytics_job)
         """
-
     def get_medical_transcription_job(
         self, *, MedicalTranscriptionJobName: str
     ) -> GetMedicalTranscriptionJobResponseTypeDef:
         """
         Provides information about the specified medical transcription job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_medical_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_medical_transcription_job)
         """
-
     def get_medical_vocabulary(self, *, VocabularyName: str) -> GetMedicalVocabularyResponseTypeDef:
         """
         Provides information about the specified custom medical vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_medical_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_medical_vocabulary)
         """
-
     def get_transcription_job(
         self, *, TranscriptionJobName: str
     ) -> GetTranscriptionJobResponseTypeDef:
         """
         Provides information about the specified transcription job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_transcription_job)
         """
-
     def get_vocabulary(self, *, VocabularyName: str) -> GetVocabularyResponseTypeDef:
         """
         Provides information about the specified custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_vocabulary)
         """
-
     def get_vocabulary_filter(
         self, *, VocabularyFilterName: str
     ) -> GetVocabularyFilterResponseTypeDef:
         """
         Provides information about the specified custom vocabulary filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_vocabulary_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_vocabulary_filter)
         """
-
     def list_call_analytics_categories(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListCallAnalyticsCategoriesResponseTypeDef:
         """
         Provides a list of Call Analytics categories, including all rules that make up
         each category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_call_analytics_categories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_call_analytics_categories)
         """
-
     def list_call_analytics_jobs(
         self,
         *,
         Status: CallAnalyticsJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListCallAnalyticsJobsResponseTypeDef:
         """
         Provides a list of Call Analytics jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_call_analytics_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_call_analytics_jobs)
         """
-
     def list_language_models(
         self,
         *,
         StatusEquals: ModelStatusType = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListLanguageModelsResponseTypeDef:
         """
         Provides a list of custom language models that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_language_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_language_models)
         """
-
     def list_medical_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListMedicalTranscriptionJobsResponseTypeDef:
         """
         Provides a list of medical transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_transcription_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_medical_transcription_jobs)
         """
-
     def list_medical_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
         NameContains: str = ...
@@ -444,85 +403,77 @@
         """
         Provides a list of custom medical vocabularies that match the specified
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_medical_vocabularies)
         """
-
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all tags associated with the specified transcription job, vocabulary,
         model, or resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_tags_for_resource)
         """
-
     def list_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListTranscriptionJobsResponseTypeDef:
         """
         Provides a list of transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_transcription_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_transcription_jobs)
         """
-
     def list_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
         NameContains: str = ...
     ) -> ListVocabulariesResponseTypeDef:
         """
         Provides a list of custom vocabularies that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_vocabularies)
         """
-
     def list_vocabulary_filters(
         self, *, NextToken: str = ..., MaxResults: int = ..., NameContains: str = ...
     ) -> ListVocabularyFiltersResponseTypeDef:
         """
         Provides a list of custom vocabulary filters that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_vocabulary_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_vocabulary_filters)
         """
-
     def start_call_analytics_job(
         self,
         *,
         CallAnalyticsJobName: str,
         Media: MediaTypeDef,
         OutputLocation: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         DataAccessRoleArn: str = ...,
-        Settings: Union[
-            CallAnalyticsJobSettingsTypeDef, CallAnalyticsJobSettingsOutputTypeDef
-        ] = ...,
+        Settings: CallAnalyticsJobSettingsTypeDef = ...,
         ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...
     ) -> StartCallAnalyticsJobResponseTypeDef:
         """
         Transcribes the audio from a customer service call and applies any additional
         Request Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#start_call_analytics_job)
         """
-
     def start_medical_transcription_job(
         self,
         *,
         MedicalTranscriptionJobName: str,
         LanguageCode: LanguageCodeType,
         Media: MediaTypeDef,
         OutputBucketName: str,
@@ -540,15 +491,14 @@
         """
         Transcribes the audio from a medical dictation or conversation and applies any
         additional Request Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#start_medical_transcription_job)
         """
-
     def start_transcription_job(
         self,
         *,
         TranscriptionJobName: str,
         Media: MediaTypeDef,
         LanguageCode: LanguageCodeType = ...,
         MediaSampleRateHertz: int = ...,
@@ -556,74 +506,63 @@
         OutputBucketName: str = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: SettingsTypeDef = ...,
         ModelSettings: ModelSettingsTypeDef = ...,
         JobExecutionSettings: JobExecutionSettingsTypeDef = ...,
-        ContentRedaction: Union[ContentRedactionTypeDef, ContentRedactionOutputTypeDef] = ...,
+        ContentRedaction: ContentRedactionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,
-        ToxicityDetection: Sequence[
-            Union[ToxicityDetectionSettingsTypeDef, ToxicityDetectionSettingsOutputTypeDef]
-        ] = ...
+        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...
     ) -> StartTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a media file and applies any additional Request
         Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#start_transcription_job)
         """
-
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds one or more custom tags, each in the form of a key:value pair, to the
         specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the specified tags from the specified Amazon Transcribe resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#untag_resource)
         """
-
     def update_call_analytics_category(
-        self,
-        *,
-        CategoryName: str,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
-        InputType: InputTypeType = ...
+        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
     ) -> UpdateCallAnalyticsCategoryResponseTypeDef:
         """
         Updates the specified Call Analytics category with new rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_call_analytics_category)
         """
-
     def update_medical_vocabulary(
         self, *, VocabularyName: str, LanguageCode: LanguageCodeType, VocabularyFileUri: str
     ) -> UpdateMedicalVocabularyResponseTypeDef:
         """
         Updates an existing custom medical vocabulary with new values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_medical_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_medical_vocabulary)
         """
-
     def update_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
@@ -631,15 +570,14 @@
     ) -> UpdateVocabularyResponseTypeDef:
         """
         Updates an existing custom vocabulary with new values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_vocabulary)
         """
-
     def update_vocabulary_filter(
         self,
         *,
         VocabularyFilterName: str,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
         DataAccessRoleArn: str = ...
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/client.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_transcribe.client import TranscribeServiceClient
 
     session = Session()
     client: TranscribeServiceClient = session.client("transcribe")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BaseModelNameType,
     CallAnalyticsJobStatusType,
     CLMLanguageCodeType,
@@ -27,18 +27,16 @@
     MediaFormatType,
     ModelStatusType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyStateType,
 )
 from .type_defs import (
-    CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
     ChannelDefinitionTypeDef,
-    ContentRedactionOutputTypeDef,
     ContentRedactionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
     CreateVocabularyFilterResponseTypeDef,
     CreateVocabularyResponseTypeDef,
     DescribeLanguageModelResponseTypeDef,
@@ -61,52 +59,54 @@
     ListTagsForResourceResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MediaTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    RuleOutputTypeDef,
     RuleTypeDef,
     SettingsTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     SubtitlesTypeDef,
     TagTypeDef,
-    ToxicityDetectionSettingsOutputTypeDef,
     ToxicityDetectionSettingsTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("TranscribeServiceClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
 
+
 class TranscribeServiceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/)
     """
 
     meta: ClientMeta
@@ -115,41 +115,41 @@
     def exceptions(self) -> Exceptions:
         """
         TranscribeServiceClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#close)
         """
+
     def create_call_analytics_category(
-        self,
-        *,
-        CategoryName: str,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
-        InputType: InputTypeType = ...
+        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
     ) -> CreateCallAnalyticsCategoryResponseTypeDef:
         """
         Creates a new Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_call_analytics_category)
         """
+
     def create_language_model(
         self,
         *,
         LanguageCode: CLMLanguageCodeType,
         BaseModelName: BaseModelNameType,
         ModelName: str,
         InputDataConfig: InputDataConfigTypeDef,
@@ -157,28 +157,30 @@
     ) -> CreateLanguageModelResponseTypeDef:
         """
         Creates a new custom language model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_language_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_language_model)
         """
+
     def create_medical_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         VocabularyFileUri: str,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMedicalVocabularyResponseTypeDef:
         """
         Creates a new custom medical vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_medical_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_medical_vocabulary)
         """
+
     def create_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
@@ -187,14 +189,15 @@
     ) -> CreateVocabularyResponseTypeDef:
         """
         Creates a new custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_vocabulary)
         """
+
     def create_vocabulary_filter(
         self,
         *,
         VocabularyFilterName: str,
         LanguageCode: LanguageCodeType,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
@@ -203,207 +206,229 @@
     ) -> CreateVocabularyFilterResponseTypeDef:
         """
         Creates a new custom vocabulary filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_vocabulary_filter)
         """
+
     def delete_call_analytics_category(self, *, CategoryName: str) -> Dict[str, Any]:
         """
         Deletes a Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_call_analytics_category)
         """
+
     def delete_call_analytics_job(self, *, CallAnalyticsJobName: str) -> Dict[str, Any]:
         """
         Deletes a Call Analytics job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_call_analytics_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_call_analytics_job)
         """
+
     def delete_language_model(self, *, ModelName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a custom language model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_language_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_language_model)
         """
+
     def delete_medical_transcription_job(
         self, *, MedicalTranscriptionJobName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a medical transcription job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_medical_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_medical_transcription_job)
         """
+
     def delete_medical_vocabulary(self, *, VocabularyName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a custom medical vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_medical_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_medical_vocabulary)
         """
+
     def delete_transcription_job(
         self, *, TranscriptionJobName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a transcription job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_transcription_job)
         """
+
     def delete_vocabulary(self, *, VocabularyName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_vocabulary)
         """
+
     def delete_vocabulary_filter(
         self, *, VocabularyFilterName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a custom vocabulary filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.delete_vocabulary_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#delete_vocabulary_filter)
         """
+
     def describe_language_model(self, *, ModelName: str) -> DescribeLanguageModelResponseTypeDef:
         """
         Provides information about the specified custom language model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.describe_language_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#describe_language_model)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#generate_presigned_url)
         """
+
     def get_call_analytics_category(
         self, *, CategoryName: str
     ) -> GetCallAnalyticsCategoryResponseTypeDef:
         """
         Provides information about the specified Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_call_analytics_category)
         """
+
     def get_call_analytics_job(
         self, *, CallAnalyticsJobName: str
     ) -> GetCallAnalyticsJobResponseTypeDef:
         """
         Provides information about the specified Call Analytics job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_call_analytics_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_call_analytics_job)
         """
+
     def get_medical_transcription_job(
         self, *, MedicalTranscriptionJobName: str
     ) -> GetMedicalTranscriptionJobResponseTypeDef:
         """
         Provides information about the specified medical transcription job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_medical_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_medical_transcription_job)
         """
+
     def get_medical_vocabulary(self, *, VocabularyName: str) -> GetMedicalVocabularyResponseTypeDef:
         """
         Provides information about the specified custom medical vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_medical_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_medical_vocabulary)
         """
+
     def get_transcription_job(
         self, *, TranscriptionJobName: str
     ) -> GetTranscriptionJobResponseTypeDef:
         """
         Provides information about the specified transcription job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_transcription_job)
         """
+
     def get_vocabulary(self, *, VocabularyName: str) -> GetVocabularyResponseTypeDef:
         """
         Provides information about the specified custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_vocabulary)
         """
+
     def get_vocabulary_filter(
         self, *, VocabularyFilterName: str
     ) -> GetVocabularyFilterResponseTypeDef:
         """
         Provides information about the specified custom vocabulary filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.get_vocabulary_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#get_vocabulary_filter)
         """
+
     def list_call_analytics_categories(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListCallAnalyticsCategoriesResponseTypeDef:
         """
         Provides a list of Call Analytics categories, including all rules that make up
         each category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_call_analytics_categories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_call_analytics_categories)
         """
+
     def list_call_analytics_jobs(
         self,
         *,
         Status: CallAnalyticsJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListCallAnalyticsJobsResponseTypeDef:
         """
         Provides a list of Call Analytics jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_call_analytics_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_call_analytics_jobs)
         """
+
     def list_language_models(
         self,
         *,
         StatusEquals: ModelStatusType = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListLanguageModelsResponseTypeDef:
         """
         Provides a list of custom language models that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_language_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_language_models)
         """
+
     def list_medical_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListMedicalTranscriptionJobsResponseTypeDef:
         """
         Provides a list of medical transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_transcription_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_medical_transcription_jobs)
         """
+
     def list_medical_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
         NameContains: str = ...
@@ -411,79 +436,83 @@
         """
         Provides a list of custom medical vocabularies that match the specified
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_medical_vocabularies)
         """
+
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all tags associated with the specified transcription job, vocabulary,
         model, or resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_tags_for_resource)
         """
+
     def list_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListTranscriptionJobsResponseTypeDef:
         """
         Provides a list of transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_transcription_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_transcription_jobs)
         """
+
     def list_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
         NameContains: str = ...
     ) -> ListVocabulariesResponseTypeDef:
         """
         Provides a list of custom vocabularies that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_vocabularies)
         """
+
     def list_vocabulary_filters(
         self, *, NextToken: str = ..., MaxResults: int = ..., NameContains: str = ...
     ) -> ListVocabularyFiltersResponseTypeDef:
         """
         Provides a list of custom vocabulary filters that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_vocabulary_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_vocabulary_filters)
         """
+
     def start_call_analytics_job(
         self,
         *,
         CallAnalyticsJobName: str,
         Media: MediaTypeDef,
         OutputLocation: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         DataAccessRoleArn: str = ...,
-        Settings: Union[
-            CallAnalyticsJobSettingsTypeDef, CallAnalyticsJobSettingsOutputTypeDef
-        ] = ...,
+        Settings: CallAnalyticsJobSettingsTypeDef = ...,
         ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...
     ) -> StartCallAnalyticsJobResponseTypeDef:
         """
         Transcribes the audio from a customer service call and applies any additional
         Request Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#start_call_analytics_job)
         """
+
     def start_medical_transcription_job(
         self,
         *,
         MedicalTranscriptionJobName: str,
         LanguageCode: LanguageCodeType,
         Media: MediaTypeDef,
         OutputBucketName: str,
@@ -501,14 +530,15 @@
         """
         Transcribes the audio from a medical dictation or conversation and applies any
         additional Request Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#start_medical_transcription_job)
         """
+
     def start_transcription_job(
         self,
         *,
         TranscriptionJobName: str,
         Media: MediaTypeDef,
         LanguageCode: LanguageCodeType = ...,
         MediaSampleRateHertz: int = ...,
@@ -516,69 +546,68 @@
         OutputBucketName: str = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: SettingsTypeDef = ...,
         ModelSettings: ModelSettingsTypeDef = ...,
         JobExecutionSettings: JobExecutionSettingsTypeDef = ...,
-        ContentRedaction: Union[ContentRedactionTypeDef, ContentRedactionOutputTypeDef] = ...,
+        ContentRedaction: ContentRedactionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,
-        ToxicityDetection: Sequence[
-            Union[ToxicityDetectionSettingsTypeDef, ToxicityDetectionSettingsOutputTypeDef]
-        ] = ...
+        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...
     ) -> StartTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a media file and applies any additional Request
         Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#start_transcription_job)
         """
+
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds one or more custom tags, each in the form of a key:value pair, to the
         specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the specified tags from the specified Amazon Transcribe resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#untag_resource)
         """
+
     def update_call_analytics_category(
-        self,
-        *,
-        CategoryName: str,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
-        InputType: InputTypeType = ...
+        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
     ) -> UpdateCallAnalyticsCategoryResponseTypeDef:
         """
         Updates the specified Call Analytics category with new rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_call_analytics_category)
         """
+
     def update_medical_vocabulary(
         self, *, VocabularyName: str, LanguageCode: LanguageCodeType, VocabularyFileUri: str
     ) -> UpdateMedicalVocabularyResponseTypeDef:
         """
         Updates an existing custom medical vocabulary with new values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_medical_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_medical_vocabulary)
         """
+
     def update_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
@@ -586,14 +615,15 @@
     ) -> UpdateVocabularyResponseTypeDef:
         """
         Updates an existing custom vocabulary with new values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_vocabulary)
         """
+
     def update_vocabulary_filter(
         self,
         *,
         VocabularyFilterName: str,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
         DataAccessRoleArn: str = ...
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/literals.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,15 +240,14 @@
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
@@ -327,15 +326,14 @@
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
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/literals.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,14 @@
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
@@ -325,15 +324,14 @@
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
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/type_defs.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for transcribe service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeTypeDef
+    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeOutputTypeDef
 
-    data: AbsoluteTimeRangeTypeDef = {...}
+    data: AbsoluteTimeRangeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     BaseModelNameType,
     CallAnalyticsJobStatusType,
     CLMLanguageCodeType,
     InputTypeType,
     LanguageCodeType,
@@ -42,25 +42,29 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AbsoluteTimeRangeOutputTypeDef",
     "AbsoluteTimeRangeTypeDef",
     "ContentRedactionOutputTypeDef",
-    "LanguageIdSettingsTypeDef",
+    "LanguageIdSettingsOutputTypeDef",
     "ContentRedactionTypeDef",
+    "LanguageIdSettingsTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
-    "ChannelDefinitionTypeDef",
-    "MediaTypeDef",
+    "ChannelDefinitionOutputTypeDef",
+    "MediaOutputTypeDef",
     "TranscriptTypeDef",
+    "ChannelDefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
+    "InputDataConfigOutputTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     "DeleteCallAnalyticsJobRequestRequestTypeDef",
     "DeleteLanguageModelRequestRequestTypeDef",
     "DeleteMedicalTranscriptionJobRequestRequestTypeDef",
     "DeleteMedicalVocabularyRequestRequestTypeDef",
     "DeleteTranscriptionJobRequestRequestTypeDef",
     "DeleteVocabularyFilterRequestRequestTypeDef",
@@ -69,37 +73,44 @@
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     "GetCallAnalyticsJobRequestRequestTypeDef",
     "GetMedicalTranscriptionJobRequestRequestTypeDef",
     "GetMedicalVocabularyRequestRequestTypeDef",
     "GetTranscriptionJobRequestRequestTypeDef",
     "GetVocabularyFilterRequestRequestTypeDef",
     "GetVocabularyRequestRequestTypeDef",
+    "RelativeTimeRangeOutputTypeDef",
     "RelativeTimeRangeTypeDef",
+    "JobExecutionSettingsOutputTypeDef",
     "JobExecutionSettingsTypeDef",
     "LanguageCodeItemTypeDef",
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     "ListCallAnalyticsJobsRequestRequestTypeDef",
     "ListLanguageModelsRequestRequestTypeDef",
     "ListMedicalTranscriptionJobsRequestRequestTypeDef",
     "MedicalTranscriptionJobSummaryTypeDef",
     "ListMedicalVocabulariesRequestRequestTypeDef",
     "VocabularyInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTranscriptionJobsRequestRequestTypeDef",
     "ListVocabulariesRequestRequestTypeDef",
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
+    "MediaTypeDef",
     "MedicalTranscriptTypeDef",
+    "MedicalTranscriptionSettingOutputTypeDef",
     "MedicalTranscriptionSettingTypeDef",
+    "ModelSettingsOutputTypeDef",
     "ModelSettingsTypeDef",
+    "SettingsOutputTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
-    "ToxicityDetectionSettingsOutputTypeDef",
     "ToxicityDetectionSettingsTypeDef",
     "SubtitlesOutputTypeDef",
+    "ToxicityDetectionSettingsOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
     "CallAnalyticsJobSettingsOutputTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
     "CreateMedicalVocabularyResponseTypeDef",
@@ -109,36 +120,38 @@
     "GetMedicalVocabularyResponseTypeDef",
     "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyResponseTypeDef",
     "ListCallAnalyticsJobsResponseTypeDef",
     "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyResponseTypeDef",
-    "CreateLanguageModelResponseTypeDef",
-    "LanguageModelTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateLanguageModelResponseTypeDef",
+    "LanguageModelTypeDef",
+    "InterruptionFilterOutputTypeDef",
+    "NonTalkTimeFilterOutputTypeDef",
+    "SentimentFilterOutputTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
-    "SentimentFilterOutputTypeDef",
     "SentimentFilterTypeDef",
-    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
-    "TranscriptionJobSummaryTypeDef",
     "StartTranscriptionJobRequestRequestTypeDef",
+    "TranscriptionJobSummaryTypeDef",
     "TranscriptionJobTypeDef",
     "CallAnalyticsJobTypeDef",
     "StartCallAnalyticsJobRequestRequestTypeDef",
     "DescribeLanguageModelResponseTypeDef",
     "ListLanguageModelsResponseTypeDef",
     "RuleOutputTypeDef",
     "RuleTypeDef",
@@ -154,55 +167,51 @@
     "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
 )
 
+AbsoluteTimeRangeOutputTypeDef = TypedDict(
+    "AbsoluteTimeRangeOutputTypeDef",
+    {
+        "StartTime": int,
+        "EndTime": int,
+        "First": int,
+        "Last": int,
+    },
+)
+
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
-_RequiredContentRedactionOutputTypeDef = TypedDict(
-    "_RequiredContentRedactionOutputTypeDef",
+ContentRedactionOutputTypeDef = TypedDict(
+    "ContentRedactionOutputTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
-    },
-)
-_OptionalContentRedactionOutputTypeDef = TypedDict(
-    "_OptionalContentRedactionOutputTypeDef",
-    {
         "PiiEntityTypes": List[PiiEntityTypeType],
     },
-    total=False,
 )
 
-
-class ContentRedactionOutputTypeDef(
-    _RequiredContentRedactionOutputTypeDef, _OptionalContentRedactionOutputTypeDef
-):
-    pass
-
-
-LanguageIdSettingsTypeDef = TypedDict(
-    "LanguageIdSettingsTypeDef",
+LanguageIdSettingsOutputTypeDef = TypedDict(
+    "LanguageIdSettingsOutputTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "LanguageModelName": str,
     },
-    total=False,
 )
 
 _RequiredContentRedactionTypeDef = TypedDict(
     "_RequiredContentRedactionTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
@@ -217,52 +226,67 @@
 )
 
 
 class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
     pass
 
 
+LanguageIdSettingsTypeDef = TypedDict(
+    "LanguageIdSettingsTypeDef",
+    {
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "LanguageModelName": str,
+    },
+    total=False,
+)
+
 CallAnalyticsJobSummaryTypeDef = TypedDict(
     "CallAnalyticsJobSummaryTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-ChannelDefinitionTypeDef = TypedDict(
-    "ChannelDefinitionTypeDef",
+ChannelDefinitionOutputTypeDef = TypedDict(
+    "ChannelDefinitionOutputTypeDef",
     {
         "ChannelId": int,
         "ParticipantRole": ParticipantRoleType,
     },
-    total=False,
 )
 
-MediaTypeDef = TypedDict(
-    "MediaTypeDef",
+MediaOutputTypeDef = TypedDict(
+    "MediaOutputTypeDef",
     {
         "MediaFileUri": str,
         "RedactedMediaFileUri": str,
     },
-    total=False,
 )
 
 TranscriptTypeDef = TypedDict(
     "TranscriptTypeDef",
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
     },
+)
+
+ChannelDefinitionTypeDef = TypedDict(
+    "ChannelDefinitionTypeDef",
+    {
+        "ChannelId": int,
+        "ParticipantRole": ParticipantRoleType,
+    },
     total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -297,14 +321,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "TuningDataS3Uri": str,
+        "DataAccessRoleArn": str,
+    },
+)
+
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -409,25 +442,43 @@
 GetVocabularyRequestRequestTypeDef = TypedDict(
     "GetVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
+RelativeTimeRangeOutputTypeDef = TypedDict(
+    "RelativeTimeRangeOutputTypeDef",
+    {
+        "StartPercentage": int,
+        "EndPercentage": int,
+        "First": int,
+        "Last": int,
+    },
+)
+
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
+JobExecutionSettingsOutputTypeDef = TypedDict(
+    "JobExecutionSettingsOutputTypeDef",
+    {
+        "AllowDeferredExecution": bool,
+        "DataAccessRoleArn": str,
+    },
+)
+
 JobExecutionSettingsTypeDef = TypedDict(
     "JobExecutionSettingsTypeDef",
     {
         "AllowDeferredExecution": bool,
         "DataAccessRoleArn": str,
     },
     total=False,
@@ -435,15 +486,14 @@
 
 LanguageCodeItemTypeDef = TypedDict(
     "LanguageCodeItemTypeDef",
     {
         "LanguageCode": LanguageCodeType,
         "DurationInSeconds": float,
     },
-    total=False,
 )
 
 ListCallAnalyticsCategoriesRequestRequestTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -495,15 +545,14 @@
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
         "Specialty": Literal["PRIMARYCARE"],
         "ContentIdentificationType": Literal["PHI"],
         "Type": TypeType,
     },
-    total=False,
 )
 
 ListMedicalVocabulariesRequestRequestTypeDef = TypedDict(
     "ListMedicalVocabulariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -517,24 +566,31 @@
     "VocabularyInfoTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 ListTranscriptionJobsRequestRequestTypeDef = TypedDict(
     "ListTranscriptionJobsRequestRequestTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "JobNameContains": str,
         "NextToken": str,
         "MaxResults": int,
@@ -566,23 +622,42 @@
 VocabularyFilterInfoTypeDef = TypedDict(
     "VocabularyFilterInfoTypeDef",
     {
         "VocabularyFilterName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
     },
+)
+
+MediaTypeDef = TypedDict(
+    "MediaTypeDef",
+    {
+        "MediaFileUri": str,
+        "RedactedMediaFileUri": str,
+    },
     total=False,
 )
 
 MedicalTranscriptTypeDef = TypedDict(
     "MedicalTranscriptTypeDef",
     {
         "TranscriptFileUri": str,
     },
-    total=False,
+)
+
+MedicalTranscriptionSettingOutputTypeDef = TypedDict(
+    "MedicalTranscriptionSettingOutputTypeDef",
+    {
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyName": str,
+    },
 )
 
 MedicalTranscriptionSettingTypeDef = TypedDict(
     "MedicalTranscriptionSettingTypeDef",
     {
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
@@ -590,22 +665,43 @@
         "ShowAlternatives": bool,
         "MaxAlternatives": int,
         "VocabularyName": str,
     },
     total=False,
 )
 
+ModelSettingsOutputTypeDef = TypedDict(
+    "ModelSettingsOutputTypeDef",
+    {
+        "LanguageModelName": str,
+    },
+)
+
 ModelSettingsTypeDef = TypedDict(
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
     },
     total=False,
 )
 
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
+    {
+        "VocabularyName": str,
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+    },
+)
+
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
@@ -622,36 +718,35 @@
     {
         "Formats": Sequence[SubtitleFormatType],
         "OutputStartIndex": int,
     },
     total=False,
 )
 
-ToxicityDetectionSettingsOutputTypeDef = TypedDict(
-    "ToxicityDetectionSettingsOutputTypeDef",
-    {
-        "ToxicityCategories": List[Literal["ALL"]],
-    },
-)
-
 ToxicityDetectionSettingsTypeDef = TypedDict(
     "ToxicityDetectionSettingsTypeDef",
     {
         "ToxicityCategories": Sequence[Literal["ALL"]],
     },
 )
 
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": List[SubtitleFormatType],
         "SubtitleFileUris": List[str],
         "OutputStartIndex": int,
     },
-    total=False,
+)
+
+ToxicityDetectionSettingsOutputTypeDef = TypedDict(
+    "ToxicityDetectionSettingsOutputTypeDef",
+    {
+        "ToxicityCategories": List[Literal["ALL"]],
+    },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
@@ -720,17 +815,16 @@
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionOutputTypeDef,
         "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
@@ -859,42 +953,14 @@
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateLanguageModelResponseTypeDef = TypedDict(
-    "CreateLanguageModelResponseTypeDef",
-    {
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelName": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "ModelStatus": ModelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LanguageModelTypeDef = TypedDict(
-    "LanguageModelTypeDef",
-    {
-        "ModelName": str,
-        "CreateTime": datetime,
-        "LastModifiedTime": datetime,
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelStatus": ModelStatusType,
-        "UpgradeAvailability": bool,
-        "FailureReason": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateLanguageModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLanguageModelRequestRequestTypeDef",
     {
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
         "ModelName": str,
         "InputDataConfig": InputDataConfigTypeDef,
@@ -987,122 +1053,135 @@
 
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateLanguageModelResponseTypeDef = TypedDict(
+    "CreateLanguageModelResponseTypeDef",
+    {
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelName": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "ModelStatus": ModelStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+LanguageModelTypeDef = TypedDict(
+    "LanguageModelTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "ModelName": str,
+        "CreateTime": datetime,
+        "LastModifiedTime": datetime,
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelStatus": ModelStatusType,
+        "UpgradeAvailability": bool,
+        "FailureReason": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
     },
 )
 
-InterruptionFilterTypeDef = TypedDict(
-    "InterruptionFilterTypeDef",
+InterruptionFilterOutputTypeDef = TypedDict(
+    "InterruptionFilterOutputTypeDef",
     {
         "Threshold": int,
         "ParticipantRole": ParticipantRoleType,
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
-NonTalkTimeFilterTypeDef = TypedDict(
-    "NonTalkTimeFilterTypeDef",
+NonTalkTimeFilterOutputTypeDef = TypedDict(
+    "NonTalkTimeFilterOutputTypeDef",
     {
         "Threshold": int,
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
-_RequiredSentimentFilterOutputTypeDef = TypedDict(
-    "_RequiredSentimentFilterOutputTypeDef",
+SentimentFilterOutputTypeDef = TypedDict(
+    "SentimentFilterOutputTypeDef",
     {
         "Sentiments": List[SentimentValueType],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
     },
 )
-_OptionalSentimentFilterOutputTypeDef = TypedDict(
-    "_OptionalSentimentFilterOutputTypeDef",
+
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
     {
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "TranscriptFilterType": Literal["EXACT"],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
+        "Targets": List[str],
     },
-    total=False,
 )
 
-
-class SentimentFilterOutputTypeDef(
-    _RequiredSentimentFilterOutputTypeDef, _OptionalSentimentFilterOutputTypeDef
-):
-    pass
-
-
-_RequiredSentimentFilterTypeDef = TypedDict(
-    "_RequiredSentimentFilterTypeDef",
+InterruptionFilterTypeDef = TypedDict(
+    "InterruptionFilterTypeDef",
     {
-        "Sentiments": Sequence[SentimentValueType],
+        "Threshold": int,
+        "ParticipantRole": ParticipantRoleType,
+        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "Negate": bool,
     },
+    total=False,
 )
-_OptionalSentimentFilterTypeDef = TypedDict(
-    "_OptionalSentimentFilterTypeDef",
+
+NonTalkTimeFilterTypeDef = TypedDict(
+    "NonTalkTimeFilterTypeDef",
     {
+        "Threshold": int,
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
-        "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
-
-class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
-    pass
-
-
-_RequiredTranscriptFilterOutputTypeDef = TypedDict(
-    "_RequiredTranscriptFilterOutputTypeDef",
+_RequiredSentimentFilterTypeDef = TypedDict(
+    "_RequiredSentimentFilterTypeDef",
     {
-        "TranscriptFilterType": Literal["EXACT"],
-        "Targets": List[str],
+        "Sentiments": Sequence[SentimentValueType],
     },
 )
-_OptionalTranscriptFilterOutputTypeDef = TypedDict(
-    "_OptionalTranscriptFilterOutputTypeDef",
+_OptionalSentimentFilterTypeDef = TypedDict(
+    "_OptionalSentimentFilterTypeDef",
     {
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
 
-class TranscriptFilterOutputTypeDef(
-    _RequiredTranscriptFilterOutputTypeDef, _OptionalTranscriptFilterOutputTypeDef
-):
+class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
     pass
 
 
 _RequiredTranscriptFilterTypeDef = TypedDict(
     "_RequiredTranscriptFilterTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
@@ -1151,14 +1230,23 @@
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
         "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1168,27 +1256,26 @@
     "MedicalTranscriptionJobTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": MedicalTranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": MedicalTranscriptionSettingTypeDef,
+        "Settings": MedicalTranscriptionSettingOutputTypeDef,
         "ContentIdentificationType": Literal["PHI"],
         "Specialty": Literal["PRIMARYCARE"],
         "Type": TypeType,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartMedicalTranscriptionJobRequestRequestTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "LanguageCode": LanguageCodeType,
@@ -1217,36 +1304,14 @@
 class StartMedicalTranscriptionJobRequestRequestTypeDef(
     _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef,
     _OptionalStartMedicalTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
 
-TranscriptionJobSummaryTypeDef = TypedDict(
-    "TranscriptionJobSummaryTypeDef",
-    {
-        "TranscriptionJobName": str,
-        "CreationTime": datetime,
-        "StartTime": datetime,
-        "CompletionTime": datetime,
-        "LanguageCode": LanguageCodeType,
-        "TranscriptionJobStatus": TranscriptionJobStatusType,
-        "FailureReason": str,
-        "OutputLocationType": OutputLocationTypeType,
-        "ContentRedaction": ContentRedactionOutputTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "IdentifyLanguage": bool,
-        "IdentifyMultipleLanguages": bool,
-        "IdentifiedLanguageScore": float,
-        "LanguageCodes": List[LanguageCodeItemTypeDef],
-        "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
-    },
-    total=False,
-)
-
 _RequiredStartTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
         "Media": MediaTypeDef,
     },
 )
@@ -1266,80 +1331,97 @@
         "ContentRedaction": ContentRedactionTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": Sequence[LanguageCodeType],
         "Subtitles": SubtitlesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
-        "ToxicityDetection": Sequence[
-            Union[ToxicityDetectionSettingsTypeDef, ToxicityDetectionSettingsOutputTypeDef]
-        ],
+        "ToxicityDetection": Sequence[ToxicityDetectionSettingsTypeDef],
     },
     total=False,
 )
 
 
 class StartTranscriptionJobRequestRequestTypeDef(
     _RequiredStartTranscriptionJobRequestRequestTypeDef,
     _OptionalStartTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
 
+TranscriptionJobSummaryTypeDef = TypedDict(
+    "TranscriptionJobSummaryTypeDef",
+    {
+        "TranscriptionJobName": str,
+        "CreationTime": datetime,
+        "StartTime": datetime,
+        "CompletionTime": datetime,
+        "LanguageCode": LanguageCodeType,
+        "TranscriptionJobStatus": TranscriptionJobStatusType,
+        "FailureReason": str,
+        "OutputLocationType": OutputLocationTypeType,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
+        "IdentifyLanguage": bool,
+        "IdentifyMultipleLanguages": bool,
+        "IdentifiedLanguageScore": float,
+        "LanguageCodes": List[LanguageCodeItemTypeDef],
+        "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
+    },
+)
+
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": SettingsTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "JobExecutionSettings": JobExecutionSettingsTypeDef,
+        "Settings": SettingsOutputTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
+        "JobExecutionSettings": JobExecutionSettingsOutputTypeDef,
         "ContentRedaction": ContentRedactionOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": List[LanguageCodeType],
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
         "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
         "Settings": CallAnalyticsJobSettingsOutputTypeDef,
-        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
+        "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
@@ -1381,20 +1463,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleOutputTypeDef = TypedDict(
     "RuleOutputTypeDef",
     {
-        "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
-        "InterruptionFilter": InterruptionFilterTypeDef,
+        "NonTalkTimeFilter": NonTalkTimeFilterOutputTypeDef,
+        "InterruptionFilter": InterruptionFilterOutputTypeDef,
         "TranscriptFilter": TranscriptFilterOutputTypeDef,
         "SentimentFilter": SentimentFilterOutputTypeDef,
     },
-    total=False,
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
         "InterruptionFilter": InterruptionFilterTypeDef,
@@ -1467,22 +1548,21 @@
     {
         "CategoryName": str,
         "Rules": List[RuleOutputTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
-    total=False,
 )
 
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 _OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
@@ -1497,15 +1577,15 @@
     pass
 
 
 _RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 _OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe/type_defs.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for transcribe service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeTypeDef
+    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeOutputTypeDef
 
-    data: AbsoluteTimeRangeTypeDef = {...}
+    data: AbsoluteTimeRangeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     BaseModelNameType,
     CallAnalyticsJobStatusType,
     CLMLanguageCodeType,
     InputTypeType,
     LanguageCodeType,
@@ -41,25 +41,29 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AbsoluteTimeRangeOutputTypeDef",
     "AbsoluteTimeRangeTypeDef",
     "ContentRedactionOutputTypeDef",
-    "LanguageIdSettingsTypeDef",
+    "LanguageIdSettingsOutputTypeDef",
     "ContentRedactionTypeDef",
+    "LanguageIdSettingsTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
-    "ChannelDefinitionTypeDef",
-    "MediaTypeDef",
+    "ChannelDefinitionOutputTypeDef",
+    "MediaOutputTypeDef",
     "TranscriptTypeDef",
+    "ChannelDefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
+    "InputDataConfigOutputTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     "DeleteCallAnalyticsJobRequestRequestTypeDef",
     "DeleteLanguageModelRequestRequestTypeDef",
     "DeleteMedicalTranscriptionJobRequestRequestTypeDef",
     "DeleteMedicalVocabularyRequestRequestTypeDef",
     "DeleteTranscriptionJobRequestRequestTypeDef",
     "DeleteVocabularyFilterRequestRequestTypeDef",
@@ -68,37 +72,44 @@
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     "GetCallAnalyticsJobRequestRequestTypeDef",
     "GetMedicalTranscriptionJobRequestRequestTypeDef",
     "GetMedicalVocabularyRequestRequestTypeDef",
     "GetTranscriptionJobRequestRequestTypeDef",
     "GetVocabularyFilterRequestRequestTypeDef",
     "GetVocabularyRequestRequestTypeDef",
+    "RelativeTimeRangeOutputTypeDef",
     "RelativeTimeRangeTypeDef",
+    "JobExecutionSettingsOutputTypeDef",
     "JobExecutionSettingsTypeDef",
     "LanguageCodeItemTypeDef",
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     "ListCallAnalyticsJobsRequestRequestTypeDef",
     "ListLanguageModelsRequestRequestTypeDef",
     "ListMedicalTranscriptionJobsRequestRequestTypeDef",
     "MedicalTranscriptionJobSummaryTypeDef",
     "ListMedicalVocabulariesRequestRequestTypeDef",
     "VocabularyInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTranscriptionJobsRequestRequestTypeDef",
     "ListVocabulariesRequestRequestTypeDef",
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
+    "MediaTypeDef",
     "MedicalTranscriptTypeDef",
+    "MedicalTranscriptionSettingOutputTypeDef",
     "MedicalTranscriptionSettingTypeDef",
+    "ModelSettingsOutputTypeDef",
     "ModelSettingsTypeDef",
+    "SettingsOutputTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
-    "ToxicityDetectionSettingsOutputTypeDef",
     "ToxicityDetectionSettingsTypeDef",
     "SubtitlesOutputTypeDef",
+    "ToxicityDetectionSettingsOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
     "CallAnalyticsJobSettingsOutputTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
     "CreateMedicalVocabularyResponseTypeDef",
@@ -108,36 +119,38 @@
     "GetMedicalVocabularyResponseTypeDef",
     "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyResponseTypeDef",
     "ListCallAnalyticsJobsResponseTypeDef",
     "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyResponseTypeDef",
-    "CreateLanguageModelResponseTypeDef",
-    "LanguageModelTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateLanguageModelResponseTypeDef",
+    "LanguageModelTypeDef",
+    "InterruptionFilterOutputTypeDef",
+    "NonTalkTimeFilterOutputTypeDef",
+    "SentimentFilterOutputTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
-    "SentimentFilterOutputTypeDef",
     "SentimentFilterTypeDef",
-    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
-    "TranscriptionJobSummaryTypeDef",
     "StartTranscriptionJobRequestRequestTypeDef",
+    "TranscriptionJobSummaryTypeDef",
     "TranscriptionJobTypeDef",
     "CallAnalyticsJobTypeDef",
     "StartCallAnalyticsJobRequestRequestTypeDef",
     "DescribeLanguageModelResponseTypeDef",
     "ListLanguageModelsResponseTypeDef",
     "RuleOutputTypeDef",
     "RuleTypeDef",
@@ -153,53 +166,51 @@
     "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
 )
 
+AbsoluteTimeRangeOutputTypeDef = TypedDict(
+    "AbsoluteTimeRangeOutputTypeDef",
+    {
+        "StartTime": int,
+        "EndTime": int,
+        "First": int,
+        "Last": int,
+    },
+)
+
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
-_RequiredContentRedactionOutputTypeDef = TypedDict(
-    "_RequiredContentRedactionOutputTypeDef",
+ContentRedactionOutputTypeDef = TypedDict(
+    "ContentRedactionOutputTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
-    },
-)
-_OptionalContentRedactionOutputTypeDef = TypedDict(
-    "_OptionalContentRedactionOutputTypeDef",
-    {
         "PiiEntityTypes": List[PiiEntityTypeType],
     },
-    total=False,
 )
 
-class ContentRedactionOutputTypeDef(
-    _RequiredContentRedactionOutputTypeDef, _OptionalContentRedactionOutputTypeDef
-):
-    pass
-
-LanguageIdSettingsTypeDef = TypedDict(
-    "LanguageIdSettingsTypeDef",
+LanguageIdSettingsOutputTypeDef = TypedDict(
+    "LanguageIdSettingsOutputTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "LanguageModelName": str,
     },
-    total=False,
 )
 
 _RequiredContentRedactionTypeDef = TypedDict(
     "_RequiredContentRedactionTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
@@ -212,52 +223,67 @@
     },
     total=False,
 )
 
 class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
     pass
 
+LanguageIdSettingsTypeDef = TypedDict(
+    "LanguageIdSettingsTypeDef",
+    {
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "LanguageModelName": str,
+    },
+    total=False,
+)
+
 CallAnalyticsJobSummaryTypeDef = TypedDict(
     "CallAnalyticsJobSummaryTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-ChannelDefinitionTypeDef = TypedDict(
-    "ChannelDefinitionTypeDef",
+ChannelDefinitionOutputTypeDef = TypedDict(
+    "ChannelDefinitionOutputTypeDef",
     {
         "ChannelId": int,
         "ParticipantRole": ParticipantRoleType,
     },
-    total=False,
 )
 
-MediaTypeDef = TypedDict(
-    "MediaTypeDef",
+MediaOutputTypeDef = TypedDict(
+    "MediaOutputTypeDef",
     {
         "MediaFileUri": str,
         "RedactedMediaFileUri": str,
     },
-    total=False,
 )
 
 TranscriptTypeDef = TypedDict(
     "TranscriptTypeDef",
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
     },
+)
+
+ChannelDefinitionTypeDef = TypedDict(
+    "ChannelDefinitionTypeDef",
+    {
+        "ChannelId": int,
+        "ParticipantRole": ParticipantRoleType,
+    },
     total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -290,14 +316,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "TuningDataS3Uri": str,
+        "DataAccessRoleArn": str,
+    },
+)
+
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -402,25 +437,43 @@
 GetVocabularyRequestRequestTypeDef = TypedDict(
     "GetVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
+RelativeTimeRangeOutputTypeDef = TypedDict(
+    "RelativeTimeRangeOutputTypeDef",
+    {
+        "StartPercentage": int,
+        "EndPercentage": int,
+        "First": int,
+        "Last": int,
+    },
+)
+
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
+JobExecutionSettingsOutputTypeDef = TypedDict(
+    "JobExecutionSettingsOutputTypeDef",
+    {
+        "AllowDeferredExecution": bool,
+        "DataAccessRoleArn": str,
+    },
+)
+
 JobExecutionSettingsTypeDef = TypedDict(
     "JobExecutionSettingsTypeDef",
     {
         "AllowDeferredExecution": bool,
         "DataAccessRoleArn": str,
     },
     total=False,
@@ -428,15 +481,14 @@
 
 LanguageCodeItemTypeDef = TypedDict(
     "LanguageCodeItemTypeDef",
     {
         "LanguageCode": LanguageCodeType,
         "DurationInSeconds": float,
     },
-    total=False,
 )
 
 ListCallAnalyticsCategoriesRequestRequestTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -488,15 +540,14 @@
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
         "Specialty": Literal["PRIMARYCARE"],
         "ContentIdentificationType": Literal["PHI"],
         "Type": TypeType,
     },
-    total=False,
 )
 
 ListMedicalVocabulariesRequestRequestTypeDef = TypedDict(
     "ListMedicalVocabulariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -510,24 +561,31 @@
     "VocabularyInfoTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 ListTranscriptionJobsRequestRequestTypeDef = TypedDict(
     "ListTranscriptionJobsRequestRequestTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "JobNameContains": str,
         "NextToken": str,
         "MaxResults": int,
@@ -559,23 +617,42 @@
 VocabularyFilterInfoTypeDef = TypedDict(
     "VocabularyFilterInfoTypeDef",
     {
         "VocabularyFilterName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
     },
+)
+
+MediaTypeDef = TypedDict(
+    "MediaTypeDef",
+    {
+        "MediaFileUri": str,
+        "RedactedMediaFileUri": str,
+    },
     total=False,
 )
 
 MedicalTranscriptTypeDef = TypedDict(
     "MedicalTranscriptTypeDef",
     {
         "TranscriptFileUri": str,
     },
-    total=False,
+)
+
+MedicalTranscriptionSettingOutputTypeDef = TypedDict(
+    "MedicalTranscriptionSettingOutputTypeDef",
+    {
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyName": str,
+    },
 )
 
 MedicalTranscriptionSettingTypeDef = TypedDict(
     "MedicalTranscriptionSettingTypeDef",
     {
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
@@ -583,22 +660,43 @@
         "ShowAlternatives": bool,
         "MaxAlternatives": int,
         "VocabularyName": str,
     },
     total=False,
 )
 
+ModelSettingsOutputTypeDef = TypedDict(
+    "ModelSettingsOutputTypeDef",
+    {
+        "LanguageModelName": str,
+    },
+)
+
 ModelSettingsTypeDef = TypedDict(
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
     },
     total=False,
 )
 
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
+    {
+        "VocabularyName": str,
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+    },
+)
+
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
@@ -615,36 +713,35 @@
     {
         "Formats": Sequence[SubtitleFormatType],
         "OutputStartIndex": int,
     },
     total=False,
 )
 
-ToxicityDetectionSettingsOutputTypeDef = TypedDict(
-    "ToxicityDetectionSettingsOutputTypeDef",
-    {
-        "ToxicityCategories": List[Literal["ALL"]],
-    },
-)
-
 ToxicityDetectionSettingsTypeDef = TypedDict(
     "ToxicityDetectionSettingsTypeDef",
     {
         "ToxicityCategories": Sequence[Literal["ALL"]],
     },
 )
 
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": List[SubtitleFormatType],
         "SubtitleFileUris": List[str],
         "OutputStartIndex": int,
     },
-    total=False,
+)
+
+ToxicityDetectionSettingsOutputTypeDef = TypedDict(
+    "ToxicityDetectionSettingsOutputTypeDef",
+    {
+        "ToxicityCategories": List[Literal["ALL"]],
+    },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
@@ -709,17 +806,16 @@
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionOutputTypeDef,
         "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
@@ -848,42 +944,14 @@
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateLanguageModelResponseTypeDef = TypedDict(
-    "CreateLanguageModelResponseTypeDef",
-    {
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelName": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "ModelStatus": ModelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LanguageModelTypeDef = TypedDict(
-    "LanguageModelTypeDef",
-    {
-        "ModelName": str,
-        "CreateTime": datetime,
-        "LastModifiedTime": datetime,
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelStatus": ModelStatusType,
-        "UpgradeAvailability": bool,
-        "FailureReason": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateLanguageModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLanguageModelRequestRequestTypeDef",
     {
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
         "ModelName": str,
         "InputDataConfig": InputDataConfigTypeDef,
@@ -968,117 +1036,134 @@
 )
 
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateLanguageModelResponseTypeDef = TypedDict(
+    "CreateLanguageModelResponseTypeDef",
+    {
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelName": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "ModelStatus": ModelStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+LanguageModelTypeDef = TypedDict(
+    "LanguageModelTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "ModelName": str,
+        "CreateTime": datetime,
+        "LastModifiedTime": datetime,
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelStatus": ModelStatusType,
+        "UpgradeAvailability": bool,
+        "FailureReason": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
     },
 )
 
-InterruptionFilterTypeDef = TypedDict(
-    "InterruptionFilterTypeDef",
+InterruptionFilterOutputTypeDef = TypedDict(
+    "InterruptionFilterOutputTypeDef",
     {
         "Threshold": int,
         "ParticipantRole": ParticipantRoleType,
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
-NonTalkTimeFilterTypeDef = TypedDict(
-    "NonTalkTimeFilterTypeDef",
+NonTalkTimeFilterOutputTypeDef = TypedDict(
+    "NonTalkTimeFilterOutputTypeDef",
     {
         "Threshold": int,
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
-_RequiredSentimentFilterOutputTypeDef = TypedDict(
-    "_RequiredSentimentFilterOutputTypeDef",
+SentimentFilterOutputTypeDef = TypedDict(
+    "SentimentFilterOutputTypeDef",
     {
         "Sentiments": List[SentimentValueType],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
     },
 )
-_OptionalSentimentFilterOutputTypeDef = TypedDict(
-    "_OptionalSentimentFilterOutputTypeDef",
+
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
     {
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "TranscriptFilterType": Literal["EXACT"],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
+        "Targets": List[str],
     },
-    total=False,
 )
 
-class SentimentFilterOutputTypeDef(
-    _RequiredSentimentFilterOutputTypeDef, _OptionalSentimentFilterOutputTypeDef
-):
-    pass
-
-_RequiredSentimentFilterTypeDef = TypedDict(
-    "_RequiredSentimentFilterTypeDef",
+InterruptionFilterTypeDef = TypedDict(
+    "InterruptionFilterTypeDef",
     {
-        "Sentiments": Sequence[SentimentValueType],
+        "Threshold": int,
+        "ParticipantRole": ParticipantRoleType,
+        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "Negate": bool,
     },
+    total=False,
 )
-_OptionalSentimentFilterTypeDef = TypedDict(
-    "_OptionalSentimentFilterTypeDef",
+
+NonTalkTimeFilterTypeDef = TypedDict(
+    "NonTalkTimeFilterTypeDef",
     {
+        "Threshold": int,
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
-        "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
-class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
-    pass
-
-_RequiredTranscriptFilterOutputTypeDef = TypedDict(
-    "_RequiredTranscriptFilterOutputTypeDef",
+_RequiredSentimentFilterTypeDef = TypedDict(
+    "_RequiredSentimentFilterTypeDef",
     {
-        "TranscriptFilterType": Literal["EXACT"],
-        "Targets": List[str],
+        "Sentiments": Sequence[SentimentValueType],
     },
 )
-_OptionalTranscriptFilterOutputTypeDef = TypedDict(
-    "_OptionalTranscriptFilterOutputTypeDef",
+_OptionalSentimentFilterTypeDef = TypedDict(
+    "_OptionalSentimentFilterTypeDef",
     {
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
-class TranscriptFilterOutputTypeDef(
-    _RequiredTranscriptFilterOutputTypeDef, _OptionalTranscriptFilterOutputTypeDef
-):
+class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
     pass
 
 _RequiredTranscriptFilterTypeDef = TypedDict(
     "_RequiredTranscriptFilterTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
         "Targets": Sequence[str],
@@ -1124,14 +1209,23 @@
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
         "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1141,27 +1235,26 @@
     "MedicalTranscriptionJobTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": MedicalTranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": MedicalTranscriptionSettingTypeDef,
+        "Settings": MedicalTranscriptionSettingOutputTypeDef,
         "ContentIdentificationType": Literal["PHI"],
         "Specialty": Literal["PRIMARYCARE"],
         "Type": TypeType,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartMedicalTranscriptionJobRequestRequestTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "LanguageCode": LanguageCodeType,
@@ -1188,36 +1281,14 @@
 
 class StartMedicalTranscriptionJobRequestRequestTypeDef(
     _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef,
     _OptionalStartMedicalTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
-TranscriptionJobSummaryTypeDef = TypedDict(
-    "TranscriptionJobSummaryTypeDef",
-    {
-        "TranscriptionJobName": str,
-        "CreationTime": datetime,
-        "StartTime": datetime,
-        "CompletionTime": datetime,
-        "LanguageCode": LanguageCodeType,
-        "TranscriptionJobStatus": TranscriptionJobStatusType,
-        "FailureReason": str,
-        "OutputLocationType": OutputLocationTypeType,
-        "ContentRedaction": ContentRedactionOutputTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "IdentifyLanguage": bool,
-        "IdentifyMultipleLanguages": bool,
-        "IdentifiedLanguageScore": float,
-        "LanguageCodes": List[LanguageCodeItemTypeDef],
-        "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
-    },
-    total=False,
-)
-
 _RequiredStartTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
         "Media": MediaTypeDef,
     },
 )
@@ -1237,78 +1308,95 @@
         "ContentRedaction": ContentRedactionTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": Sequence[LanguageCodeType],
         "Subtitles": SubtitlesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
-        "ToxicityDetection": Sequence[
-            Union[ToxicityDetectionSettingsTypeDef, ToxicityDetectionSettingsOutputTypeDef]
-        ],
+        "ToxicityDetection": Sequence[ToxicityDetectionSettingsTypeDef],
     },
     total=False,
 )
 
 class StartTranscriptionJobRequestRequestTypeDef(
     _RequiredStartTranscriptionJobRequestRequestTypeDef,
     _OptionalStartTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
+TranscriptionJobSummaryTypeDef = TypedDict(
+    "TranscriptionJobSummaryTypeDef",
+    {
+        "TranscriptionJobName": str,
+        "CreationTime": datetime,
+        "StartTime": datetime,
+        "CompletionTime": datetime,
+        "LanguageCode": LanguageCodeType,
+        "TranscriptionJobStatus": TranscriptionJobStatusType,
+        "FailureReason": str,
+        "OutputLocationType": OutputLocationTypeType,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
+        "IdentifyLanguage": bool,
+        "IdentifyMultipleLanguages": bool,
+        "IdentifiedLanguageScore": float,
+        "LanguageCodes": List[LanguageCodeItemTypeDef],
+        "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
+    },
+)
+
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": SettingsTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "JobExecutionSettings": JobExecutionSettingsTypeDef,
+        "Settings": SettingsOutputTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
+        "JobExecutionSettings": JobExecutionSettingsOutputTypeDef,
         "ContentRedaction": ContentRedactionOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": List[LanguageCodeType],
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
         "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
         "Settings": CallAnalyticsJobSettingsOutputTypeDef,
-        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
+        "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
@@ -1348,20 +1436,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleOutputTypeDef = TypedDict(
     "RuleOutputTypeDef",
     {
-        "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
-        "InterruptionFilter": InterruptionFilterTypeDef,
+        "NonTalkTimeFilter": NonTalkTimeFilterOutputTypeDef,
+        "InterruptionFilter": InterruptionFilterOutputTypeDef,
         "TranscriptFilter": TranscriptFilterOutputTypeDef,
         "SentimentFilter": SentimentFilterOutputTypeDef,
     },
-    total=False,
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
         "InterruptionFilter": InterruptionFilterTypeDef,
@@ -1434,22 +1521,21 @@
     {
         "CategoryName": str,
         "Rules": List[RuleOutputTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
-    total=False,
 )
 
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 _OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
@@ -1462,15 +1548,15 @@
 ):
     pass
 
 _RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 _OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe.egg-info/PKG-INFO` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.TranscribeService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.8
+Summary: Type annotations for boto3.TranscribeService 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,25 +318,29 @@
 ### Typed dictionaries
 
 `mypy_boto3_transcribe.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transcribe.type_defs import (
+    AbsoluteTimeRangeOutputTypeDef,
     AbsoluteTimeRangeTypeDef,
     ContentRedactionOutputTypeDef,
-    LanguageIdSettingsTypeDef,
+    LanguageIdSettingsOutputTypeDef,
     ContentRedactionTypeDef,
+    LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
-    ChannelDefinitionTypeDef,
-    MediaTypeDef,
+    ChannelDefinitionOutputTypeDef,
+    MediaOutputTypeDef,
     TranscriptTypeDef,
+    ChannelDefinitionTypeDef,
     ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
+    InputDataConfigOutputTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
@@ -345,37 +349,44 @@
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
     GetVocabularyRequestRequestTypeDef,
+    RelativeTimeRangeOutputTypeDef,
     RelativeTimeRangeTypeDef,
+    JobExecutionSettingsOutputTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
     MedicalTranscriptionJobSummaryTypeDef,
     ListMedicalVocabulariesRequestRequestTypeDef,
     VocabularyInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
+    MediaTypeDef,
     MedicalTranscriptTypeDef,
+    MedicalTranscriptionSettingOutputTypeDef,
     MedicalTranscriptionSettingTypeDef,
+    ModelSettingsOutputTypeDef,
     ModelSettingsTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
-    ToxicityDetectionSettingsOutputTypeDef,
     ToxicityDetectionSettingsTypeDef,
     SubtitlesOutputTypeDef,
+    ToxicityDetectionSettingsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
     CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
@@ -385,36 +396,38 @@
     GetMedicalVocabularyResponseTypeDef,
     GetVocabularyFilterResponseTypeDef,
     GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
-    CreateLanguageModelResponseTypeDef,
-    LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateLanguageModelResponseTypeDef,
+    LanguageModelTypeDef,
+    InterruptionFilterOutputTypeDef,
+    NonTalkTimeFilterOutputTypeDef,
+    SentimentFilterOutputTypeDef,
+    TranscriptFilterOutputTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
-    SentimentFilterOutputTypeDef,
     SentimentFilterTypeDef,
-    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
-    TranscriptionJobSummaryTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
+    TranscriptionJobSummaryTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
     StartCallAnalyticsJobRequestRequestTypeDef,
     DescribeLanguageModelResponseTypeDef,
     ListLanguageModelsResponseTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
@@ -431,15 +444,15 @@
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_structure() -> AbsoluteTimeRangeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transcribe-1.28.15.post1/mypy_boto3_transcribe.egg-info/SOURCES.txt` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.15.post1/setup.py` & `mypy-boto3-transcribe-1.28.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transcribe",
-    version="1.28.15.post1",
+    version="1.28.8",
     packages=["mypy_boto3_transcribe"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TranscribeService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.TranscribeService 1.28.8 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

