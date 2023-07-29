# Comparing `tmp/mypy-boto3-translate-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-translate-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-translate-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:22 2023, max compression
+gzip compressed data, was "mypy-boto3-translate-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-translate-1.28.15.post1.tar` & `mypy-boto3-translate-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.921446 mypy-boto3-translate-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:03.000000 mypy-boto3-translate-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-07-29 10:04:22.921446 mypy-boto3-translate-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-29 10:01:03.000000 mypy-boto3-translate-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.921446 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-29 10:01:03.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-29 10:01:03.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 10:01:03.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-29 10:01:04.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-29 10:01:04.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-29 10:01:04.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-29 10:01:04.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-29 10:01:04.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-29 10:01:04.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:03.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-07-29 10:01:05.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20101 2023-07-29 10:01:04.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:03.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.921446 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-07-29 10:04:22.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:04:22.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:22.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:04:22.000000 mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:22.921446 mypy-boto3-translate-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 10:01:03.000000 mypy-boto3-translate-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.766719 mypy-boto3-translate-1.28.5/mypy_boto3_translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-07-18 19:32:30.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21207 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/setup.py
```

### Comparing `mypy-boto3-translate-1.28.15.post1/LICENSE` & `mypy-boto3-translate-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.15.post1/PKG-INFO` & `mypy-boto3-translate-1.28.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-translate
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Translate 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.5
+Summary: Type annotations for boto3.Translate 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-translate)](https://pepy.tech/project/mypy-boto3-translate)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,55 +334,61 @@
 
 ```python
 from mypy_boto3_translate.type_defs import (
     TermTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
+    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
     DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EncryptionKeyOutputTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ParallelDataConfigOutputTypeDef,
+    ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
+    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
+    StopTextTranslationJobResponseTypeDef,
+    TranslationSettingsOutputTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
-    TerminologyPropertiesTypeDef,
-    ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
+    OutputDataConfigOutputTypeDef,
+    TerminologyPropertiesTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
+    ParallelDataPropertiesTypeDef,
     TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.15.post1/README.md` & `mypy-boto3-translate-1.28.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-translate)](https://pepy.tech/project/mypy-boto3-translate)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,55 +302,61 @@
 
 ```python
 from mypy_boto3_translate.type_defs import (
     TermTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
+    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
     DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EncryptionKeyOutputTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ParallelDataConfigOutputTypeDef,
+    ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
+    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
+    StopTextTranslationJobResponseTypeDef,
+    TranslationSettingsOutputTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
-    TerminologyPropertiesTypeDef,
-    ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
+    OutputDataConfigOutputTypeDef,
+    TerminologyPropertiesTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
+    ParallelDataPropertiesTypeDef,
     TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/__init__.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/__init__.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/__main__.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Translate 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Translate 1.28.5\nVersion:         1.28.5\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/client.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/client.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/literals.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,14 @@
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
@@ -261,28 +260,26 @@
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

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/literals.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,14 @@
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
@@ -259,28 +258,26 @@
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

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/paginator.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListTerminologiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTerminologiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
         """
```

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/paginator.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListTerminologiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTerminologiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
         """
```

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/type_defs.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -32,61 +32,66 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TermTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateParallelDataResponseTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
+    "DeleteParallelDataResponseTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
     "DocumentTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EncryptionKeyOutputTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
     "TerminologyDataTypeDef",
+    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
     "LanguageTypeDef",
     "ListLanguagesRequestRequestTypeDef",
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTerminologiesRequestRequestTypeDef",
     "TextTranslationJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
+    "ParallelDataConfigOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TranslationSettingsTypeDef",
+    "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
+    "StopTextTranslationJobResponseTypeDef",
+    "TranslationSettingsOutputTypeDef",
     "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateParallelDataResponseTypeDef",
     "AppliedTerminologyTypeDef",
     "OutputDataConfigTypeDef",
-    "TerminologyPropertiesTypeDef",
-    "ParallelDataPropertiesTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateParallelDataResponseTypeDef",
-    "DeleteParallelDataResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartTextTranslationJobResponseTypeDef",
-    "StopTextTranslationJobResponseTypeDef",
-    "UpdateParallelDataResponseTypeDef",
+    "OutputDataConfigOutputTypeDef",
+    "TerminologyPropertiesTypeDef",
     "ImportTerminologyRequestRequestTypeDef",
     "ListLanguagesResponseTypeDef",
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTextTranslationJobsRequestRequestTypeDef",
+    "ParallelDataPropertiesTypeDef",
     "TranslateDocumentRequestRequestTypeDef",
     "TranslateTextRequestRequestTypeDef",
     "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
     "TextTranslationJobPropertiesTypeDef",
     "GetTerminologyResponseTypeDef",
@@ -100,15 +105,14 @@
 
 TermTypeDef = TypedDict(
     "TermTypeDef",
     {
         "SourceText": str,
         "TargetText": str,
     },
-    total=False,
 )
 
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "Type": Literal["KMS"],
         "Id": str,
@@ -127,32 +131,39 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateParallelDataResponseTypeDef = TypedDict(
+    "CreateParallelDataResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteParallelDataRequestRequestTypeDef = TypedDict(
     "DeleteParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteParallelDataResponseTypeDef = TypedDict(
+    "DeleteParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTerminologyRequestRequestTypeDef = TypedDict(
     "DeleteTerminologyRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -167,14 +178,29 @@
     "DocumentTypeDef",
     {
         "Content": Union[str, bytes, IO[Any], StreamingBody],
         "ContentType": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EncryptionKeyOutputTypeDef = TypedDict(
+    "EncryptionKeyOutputTypeDef",
+    {
+        "Type": Literal["KMS"],
+        "Id": str,
+    },
+)
+
 GetParallelDataRequestRequestTypeDef = TypedDict(
     "GetParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -196,21 +222,19 @@
     "_OptionalGetTerminologyRequestRequestTypeDef",
     {
         "TerminologyDataFormat": TerminologyDataFormatType,
     },
     total=False,
 )
 
-
 class GetTerminologyRequestRequestTypeDef(
     _RequiredGetTerminologyRequestRequestTypeDef, _OptionalGetTerminologyRequestRequestTypeDef
 ):
     pass
 
-
 TerminologyDataLocationTypeDef = TypedDict(
     "TerminologyDataLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
     },
 )
@@ -226,18 +250,24 @@
     "_OptionalTerminologyDataTypeDef",
     {
         "Directionality": DirectionalityType,
     },
     total=False,
 )
 
-
 class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
     pass
 
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "ContentType": str,
+    },
+)
 
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
         "ContentType": str,
     },
@@ -246,15 +276,14 @@
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "TranslatedDocumentsCount": int,
         "DocumentsWithErrorsCount": int,
         "InputDocumentsCount": int,
     },
-    total=False,
 )
 
 LanguageTypeDef = TypedDict(
     "LanguageTypeDef",
     {
         "LanguageName": str,
         "LanguageCode": str,
@@ -283,20 +312,26 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
+    },
+)
+
+ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTerminologiesRequestRequestTypeDef = TypedDict(
     "ListTerminologiesRequestRequestTypeDef",
     {
@@ -313,30 +348,85 @@
         "JobStatus": JobStatusType,
         "SubmittedBeforeTime": Union[datetime, str],
         "SubmittedAfterTime": Union[datetime, str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+ParallelDataConfigOutputTypeDef = TypedDict(
+    "ParallelDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "Format": ParallelDataFormatType,
+    },
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 TranslationSettingsTypeDef = TypedDict(
     "TranslationSettingsTypeDef",
     {
         "Formality": FormalityType,
         "Profanity": Literal["MASK"],
     },
     total=False,
 )
 
+StartTextTranslationJobResponseTypeDef = TypedDict(
+    "StartTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopTextTranslationJobRequestRequestTypeDef = TypedDict(
     "StopTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopTextTranslationJobResponseTypeDef = TypedDict(
+    "StopTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TranslationSettingsOutputTypeDef = TypedDict(
+    "TranslationSettingsOutputTypeDef",
+    {
+        "Formality": FormalityType,
+        "Profanity": Literal["MASK"],
+    },
+)
+
 TranslatedDocumentTypeDef = TypedDict(
     "TranslatedDocumentTypeDef",
     {
         "Content": bytes,
     },
 )
 
@@ -344,21 +434,31 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateParallelDataResponseTypeDef = TypedDict(
+    "UpdateParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppliedTerminologyTypeDef = TypedDict(
     "AppliedTerminologyTypeDef",
     {
         "Name": str,
         "Terms": List[TermTypeDef],
     },
-    total=False,
 )
 
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
@@ -367,64 +467,17 @@
     "_OptionalOutputDataConfigTypeDef",
     {
         "EncryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
-
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
-
-TerminologyPropertiesTypeDef = TypedDict(
-    "TerminologyPropertiesTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Arn": str,
-        "SourceLanguageCode": str,
-        "TargetLanguageCodes": List[str],
-        "EncryptionKey": EncryptionKeyTypeDef,
-        "SizeBytes": int,
-        "TermCount": int,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Directionality": DirectionalityType,
-        "Message": str,
-        "SkippedTermCount": int,
-        "Format": TerminologyDataFormatType,
-    },
-    total=False,
-)
-
-ParallelDataPropertiesTypeDef = TypedDict(
-    "ParallelDataPropertiesTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Description": str,
-        "Status": ParallelDataStatusType,
-        "SourceLanguageCode": str,
-        "TargetLanguageCodes": List[str],
-        "ParallelDataConfig": ParallelDataConfigTypeDef,
-        "Message": str,
-        "ImportedDataSize": int,
-        "ImportedRecordCount": int,
-        "FailedRecordCount": int,
-        "SkippedRecordCount": int,
-        "EncryptionKey": EncryptionKeyTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -433,22 +486,20 @@
     "_OptionalUpdateParallelDataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateParallelDataRequestRequestTypeDef(
     _RequiredUpdateParallelDataRequestRequestTypeDef,
     _OptionalUpdateParallelDataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -459,89 +510,53 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateParallelDataResponseTypeDef = TypedDict(
-    "CreateParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteParallelDataResponseTypeDef = TypedDict(
-    "DeleteParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTextTranslationJobResponseTypeDef = TypedDict(
-    "StartTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopTextTranslationJobResponseTypeDef = TypedDict(
-    "StopTextTranslationJobResponseTypeDef",
+OutputDataConfigOutputTypeDef = TypedDict(
+    "OutputDataConfigOutputTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "S3Uri": str,
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
     },
 )
 
-UpdateParallelDataResponseTypeDef = TypedDict(
-    "UpdateParallelDataResponseTypeDef",
+TerminologyPropertiesTypeDef = TypedDict(
+    "TerminologyPropertiesTypeDef",
     {
         "Name": str,
-        "Status": ParallelDataStatusType,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Description": str,
+        "Arn": str,
+        "SourceLanguageCode": str,
+        "TargetLanguageCodes": List[str],
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
+        "SizeBytes": int,
+        "TermCount": int,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Directionality": DirectionalityType,
+        "Message": str,
+        "SkippedTermCount": int,
+        "Format": TerminologyDataFormatType,
     },
 )
 
 _RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
     "_RequiredImportTerminologyRequestRequestTypeDef",
     {
         "Name": str,
@@ -555,49 +570,70 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ImportTerminologyRequestRequestTypeDef(
     _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
 ):
     pass
 
-
 ListLanguagesResponseTypeDef = TypedDict(
     "ListLanguagesResponseTypeDef",
     {
         "Languages": List[LanguageTypeDef],
         "DisplayLanguageCode": DisplayLanguageCodeType,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
     "ListTextTranslationJobsRequestRequestTypeDef",
     {
         "Filter": TextTranslationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ParallelDataPropertiesTypeDef = TypedDict(
+    "ParallelDataPropertiesTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Description": str,
+        "Status": ParallelDataStatusType,
+        "SourceLanguageCode": str,
+        "TargetLanguageCodes": List[str],
+        "ParallelDataConfig": ParallelDataConfigOutputTypeDef,
+        "Message": str,
+        "ImportedDataSize": int,
+        "ImportedRecordCount": int,
+        "FailedRecordCount": int,
+        "SkippedRecordCount": int,
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+    },
+)
+
 _RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateDocumentRequestRequestTypeDef",
     {
         "Document": DocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -607,21 +643,19 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class TranslateDocumentRequestRequestTypeDef(
     _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -631,42 +665,40 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
-
 TranslateDocumentResponseTypeDef = TypedDict(
     "TranslateDocumentResponseTypeDef",
     {
         "TranslatedDocument": TranslatedDocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
-        "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppliedSettings": TranslationSettingsOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
-        "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppliedSettings": TranslationSettingsOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTextTranslationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextTranslationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
@@ -684,101 +716,98 @@
         "TerminologyNames": Sequence[str],
         "ParallelDataNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class StartTextTranslationJobRequestRequestTypeDef(
     _RequiredStartTextTranslationJobRequestRequestTypeDef,
     _OptionalStartTextTranslationJobRequestRequestTypeDef,
 ):
     pass
 
-
 TextTranslationJobPropertiesTypeDef = TypedDict(
     "TextTranslationJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "JobDetails": JobDetailsTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCodes": List[str],
         "TerminologyNames": List[str],
         "ParallelDataNames": List[str],
         "Message": str,
         "SubmittedTime": datetime,
         "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
         "DataAccessRoleArn": str,
-        "Settings": TranslationSettingsTypeDef,
+        "Settings": TranslationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 GetTerminologyResponseTypeDef = TypedDict(
     "GetTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "TerminologyDataLocation": TerminologyDataLocationTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTerminologyResponseTypeDef = TypedDict(
     "ImportTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTerminologiesResponseTypeDef = TypedDict(
     "ListTerminologiesResponseTypeDef",
     {
         "TerminologyPropertiesList": List[TerminologyPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParallelDataResponseTypeDef = TypedDict(
     "GetParallelDataResponseTypeDef",
     {
         "ParallelDataProperties": ParallelDataPropertiesTypeDef,
         "DataLocation": ParallelDataDataLocationTypeDef,
         "AuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
         "LatestUpdateAttemptAuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListParallelDataResponseTypeDef = TypedDict(
     "ListParallelDataResponseTypeDef",
     {
         "ParallelDataPropertiesList": List[ParallelDataPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTextTranslationJobResponseTypeDef = TypedDict(
     "DescribeTextTranslationJobResponseTypeDef",
     {
         "TextTranslationJobProperties": TextTranslationJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTextTranslationJobsResponseTypeDef = TypedDict(
     "ListTextTranslationJobsResponseTypeDef",
     {
         "TextTranslationJobPropertiesList": List[TextTranslationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate/type_defs.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,60 +32,67 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TermTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateParallelDataResponseTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
+    "DeleteParallelDataResponseTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
     "DocumentTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EncryptionKeyOutputTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
     "TerminologyDataTypeDef",
+    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
     "LanguageTypeDef",
     "ListLanguagesRequestRequestTypeDef",
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTerminologiesRequestRequestTypeDef",
     "TextTranslationJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
+    "ParallelDataConfigOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TranslationSettingsTypeDef",
+    "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
+    "StopTextTranslationJobResponseTypeDef",
+    "TranslationSettingsOutputTypeDef",
     "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateParallelDataResponseTypeDef",
     "AppliedTerminologyTypeDef",
     "OutputDataConfigTypeDef",
-    "TerminologyPropertiesTypeDef",
-    "ParallelDataPropertiesTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateParallelDataResponseTypeDef",
-    "DeleteParallelDataResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartTextTranslationJobResponseTypeDef",
-    "StopTextTranslationJobResponseTypeDef",
-    "UpdateParallelDataResponseTypeDef",
+    "OutputDataConfigOutputTypeDef",
+    "TerminologyPropertiesTypeDef",
     "ImportTerminologyRequestRequestTypeDef",
     "ListLanguagesResponseTypeDef",
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTextTranslationJobsRequestRequestTypeDef",
+    "ParallelDataPropertiesTypeDef",
     "TranslateDocumentRequestRequestTypeDef",
     "TranslateTextRequestRequestTypeDef",
     "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
     "TextTranslationJobPropertiesTypeDef",
     "GetTerminologyResponseTypeDef",
@@ -99,15 +106,14 @@
 
 TermTypeDef = TypedDict(
     "TermTypeDef",
     {
         "SourceText": str,
         "TargetText": str,
     },
-    total=False,
 )
 
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "Type": Literal["KMS"],
         "Id": str,
@@ -126,32 +132,39 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateParallelDataResponseTypeDef = TypedDict(
+    "CreateParallelDataResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteParallelDataRequestRequestTypeDef = TypedDict(
     "DeleteParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteParallelDataResponseTypeDef = TypedDict(
+    "DeleteParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTerminologyRequestRequestTypeDef = TypedDict(
     "DeleteTerminologyRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -166,14 +179,29 @@
     "DocumentTypeDef",
     {
         "Content": Union[str, bytes, IO[Any], StreamingBody],
         "ContentType": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EncryptionKeyOutputTypeDef = TypedDict(
+    "EncryptionKeyOutputTypeDef",
+    {
+        "Type": Literal["KMS"],
+        "Id": str,
+    },
+)
+
 GetParallelDataRequestRequestTypeDef = TypedDict(
     "GetParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -195,19 +223,21 @@
     "_OptionalGetTerminologyRequestRequestTypeDef",
     {
         "TerminologyDataFormat": TerminologyDataFormatType,
     },
     total=False,
 )
 
+
 class GetTerminologyRequestRequestTypeDef(
     _RequiredGetTerminologyRequestRequestTypeDef, _OptionalGetTerminologyRequestRequestTypeDef
 ):
     pass
 
+
 TerminologyDataLocationTypeDef = TypedDict(
     "TerminologyDataLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
     },
 )
@@ -223,17 +253,27 @@
     "_OptionalTerminologyDataTypeDef",
     {
         "Directionality": DirectionalityType,
     },
     total=False,
 )
 
+
 class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
     pass
 
+
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "ContentType": str,
+    },
+)
+
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
         "ContentType": str,
     },
 )
@@ -241,15 +281,14 @@
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "TranslatedDocumentsCount": int,
         "DocumentsWithErrorsCount": int,
         "InputDocumentsCount": int,
     },
-    total=False,
 )
 
 LanguageTypeDef = TypedDict(
     "LanguageTypeDef",
     {
         "LanguageName": str,
         "LanguageCode": str,
@@ -278,20 +317,26 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
+    },
+)
+
+ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTerminologiesRequestRequestTypeDef = TypedDict(
     "ListTerminologiesRequestRequestTypeDef",
     {
@@ -308,30 +353,85 @@
         "JobStatus": JobStatusType,
         "SubmittedBeforeTime": Union[datetime, str],
         "SubmittedAfterTime": Union[datetime, str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+ParallelDataConfigOutputTypeDef = TypedDict(
+    "ParallelDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "Format": ParallelDataFormatType,
+    },
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 TranslationSettingsTypeDef = TypedDict(
     "TranslationSettingsTypeDef",
     {
         "Formality": FormalityType,
         "Profanity": Literal["MASK"],
     },
     total=False,
 )
 
+StartTextTranslationJobResponseTypeDef = TypedDict(
+    "StartTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopTextTranslationJobRequestRequestTypeDef = TypedDict(
     "StopTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopTextTranslationJobResponseTypeDef = TypedDict(
+    "StopTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TranslationSettingsOutputTypeDef = TypedDict(
+    "TranslationSettingsOutputTypeDef",
+    {
+        "Formality": FormalityType,
+        "Profanity": Literal["MASK"],
+    },
+)
+
 TranslatedDocumentTypeDef = TypedDict(
     "TranslatedDocumentTypeDef",
     {
         "Content": bytes,
     },
 )
 
@@ -339,21 +439,31 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateParallelDataResponseTypeDef = TypedDict(
+    "UpdateParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppliedTerminologyTypeDef = TypedDict(
     "AppliedTerminologyTypeDef",
     {
         "Name": str,
         "Terms": List[TermTypeDef],
     },
-    total=False,
 )
 
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
@@ -362,61 +472,18 @@
     "_OptionalOutputDataConfigTypeDef",
     {
         "EncryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
+
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
-TerminologyPropertiesTypeDef = TypedDict(
-    "TerminologyPropertiesTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Arn": str,
-        "SourceLanguageCode": str,
-        "TargetLanguageCodes": List[str],
-        "EncryptionKey": EncryptionKeyTypeDef,
-        "SizeBytes": int,
-        "TermCount": int,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Directionality": DirectionalityType,
-        "Message": str,
-        "SkippedTermCount": int,
-        "Format": TerminologyDataFormatType,
-    },
-    total=False,
-)
-
-ParallelDataPropertiesTypeDef = TypedDict(
-    "ParallelDataPropertiesTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Description": str,
-        "Status": ParallelDataStatusType,
-        "SourceLanguageCode": str,
-        "TargetLanguageCodes": List[str],
-        "ParallelDataConfig": ParallelDataConfigTypeDef,
-        "Message": str,
-        "ImportedDataSize": int,
-        "ImportedRecordCount": int,
-        "FailedRecordCount": int,
-        "SkippedRecordCount": int,
-        "EncryptionKey": EncryptionKeyTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-    },
-    total=False,
-)
 
 _RequiredUpdateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
@@ -426,20 +493,22 @@
     "_OptionalUpdateParallelDataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateParallelDataRequestRequestTypeDef(
     _RequiredUpdateParallelDataRequestRequestTypeDef,
     _OptionalUpdateParallelDataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -450,87 +519,55 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateParallelDataResponseTypeDef = TypedDict(
-    "CreateParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteParallelDataResponseTypeDef = TypedDict(
-    "DeleteParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTextTranslationJobResponseTypeDef = TypedDict(
-    "StartTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopTextTranslationJobResponseTypeDef = TypedDict(
-    "StopTextTranslationJobResponseTypeDef",
+OutputDataConfigOutputTypeDef = TypedDict(
+    "OutputDataConfigOutputTypeDef",
     {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "S3Uri": str,
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
     },
 )
 
-UpdateParallelDataResponseTypeDef = TypedDict(
-    "UpdateParallelDataResponseTypeDef",
+TerminologyPropertiesTypeDef = TypedDict(
+    "TerminologyPropertiesTypeDef",
     {
         "Name": str,
-        "Status": ParallelDataStatusType,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Description": str,
+        "Arn": str,
+        "SourceLanguageCode": str,
+        "TargetLanguageCodes": List[str],
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
+        "SizeBytes": int,
+        "TermCount": int,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Directionality": DirectionalityType,
+        "Message": str,
+        "SkippedTermCount": int,
+        "Format": TerminologyDataFormatType,
     },
 )
 
 _RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
     "_RequiredImportTerminologyRequestRequestTypeDef",
     {
         "Name": str,
@@ -544,47 +581,72 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ImportTerminologyRequestRequestTypeDef(
     _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
 ):
     pass
 
+
 ListLanguagesResponseTypeDef = TypedDict(
     "ListLanguagesResponseTypeDef",
     {
         "Languages": List[LanguageTypeDef],
         "DisplayLanguageCode": DisplayLanguageCodeType,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
     "ListTextTranslationJobsRequestRequestTypeDef",
     {
         "Filter": TextTranslationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ParallelDataPropertiesTypeDef = TypedDict(
+    "ParallelDataPropertiesTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Description": str,
+        "Status": ParallelDataStatusType,
+        "SourceLanguageCode": str,
+        "TargetLanguageCodes": List[str],
+        "ParallelDataConfig": ParallelDataConfigOutputTypeDef,
+        "Message": str,
+        "ImportedDataSize": int,
+        "ImportedRecordCount": int,
+        "FailedRecordCount": int,
+        "SkippedRecordCount": int,
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+    },
+)
+
 _RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateDocumentRequestRequestTypeDef",
     {
         "Document": DocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -594,19 +656,21 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class TranslateDocumentRequestRequestTypeDef(
     _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -616,40 +680,42 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
+
 TranslateDocumentResponseTypeDef = TypedDict(
     "TranslateDocumentResponseTypeDef",
     {
         "TranslatedDocument": TranslatedDocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
-        "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppliedSettings": TranslationSettingsOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
-        "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppliedSettings": TranslationSettingsOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTextTranslationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextTranslationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
@@ -667,99 +733,100 @@
         "TerminologyNames": Sequence[str],
         "ParallelDataNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class StartTextTranslationJobRequestRequestTypeDef(
     _RequiredStartTextTranslationJobRequestRequestTypeDef,
     _OptionalStartTextTranslationJobRequestRequestTypeDef,
 ):
     pass
 
+
 TextTranslationJobPropertiesTypeDef = TypedDict(
     "TextTranslationJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "JobDetails": JobDetailsTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCodes": List[str],
         "TerminologyNames": List[str],
         "ParallelDataNames": List[str],
         "Message": str,
         "SubmittedTime": datetime,
         "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
         "DataAccessRoleArn": str,
-        "Settings": TranslationSettingsTypeDef,
+        "Settings": TranslationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 GetTerminologyResponseTypeDef = TypedDict(
     "GetTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "TerminologyDataLocation": TerminologyDataLocationTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTerminologyResponseTypeDef = TypedDict(
     "ImportTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTerminologiesResponseTypeDef = TypedDict(
     "ListTerminologiesResponseTypeDef",
     {
         "TerminologyPropertiesList": List[TerminologyPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParallelDataResponseTypeDef = TypedDict(
     "GetParallelDataResponseTypeDef",
     {
         "ParallelDataProperties": ParallelDataPropertiesTypeDef,
         "DataLocation": ParallelDataDataLocationTypeDef,
         "AuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
         "LatestUpdateAttemptAuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListParallelDataResponseTypeDef = TypedDict(
     "ListParallelDataResponseTypeDef",
     {
         "ParallelDataPropertiesList": List[ParallelDataPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTextTranslationJobResponseTypeDef = TypedDict(
     "DescribeTextTranslationJobResponseTypeDef",
     {
         "TextTranslationJobProperties": TextTranslationJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTextTranslationJobsResponseTypeDef = TypedDict(
     "ListTextTranslationJobsResponseTypeDef",
     {
         "TextTranslationJobPropertiesList": List[TextTranslationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate.egg-info/PKG-INFO` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-translate
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Translate 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.5
+Summary: Type annotations for boto3.Translate 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-translate)](https://pepy.tech/project/mypy-boto3-translate)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,55 +334,61 @@
 
 ```python
 from mypy_boto3_translate.type_defs import (
     TermTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
+    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
     DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EncryptionKeyOutputTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ParallelDataConfigOutputTypeDef,
+    ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
+    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
+    StopTextTranslationJobResponseTypeDef,
+    TranslationSettingsOutputTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
-    TerminologyPropertiesTypeDef,
-    ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
+    OutputDataConfigOutputTypeDef,
+    TerminologyPropertiesTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
+    ParallelDataPropertiesTypeDef,
     TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.15.post1/mypy_boto3_translate.egg-info/SOURCES.txt` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.15.post1/setup.py` & `mypy-boto3-translate-1.28.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-translate",
-    version="1.28.15.post1",
+    version="1.28.5",
     packages=["mypy_boto3_translate"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Translate 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Translate 1.28.5 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

