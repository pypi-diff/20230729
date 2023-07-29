# Comparing `tmp/mypy-boto3-ivs-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ivs-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:23 2023, max compression
+gzip compressed data, was "mypy-boto3-ivs-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-ivs-1.28.15.post1.tar` & `mypy-boto3-ivs-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.905200 mypy-boto3-ivs-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:24.000000 mypy-boto3-ivs-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-07-29 10:03:23.893200 mypy-boto3-ivs-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-07-29 09:48:24.000000 mypy-boto3-ivs-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.885200 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-29 09:48:24.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-29 09:48:24.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:48:24.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23151 2023-07-29 09:48:25.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-07-29 09:48:24.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-29 09:48:25.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-29 09:48:25.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-29 09:48:25.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-29 09:48:25.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:24.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27686 2023-07-29 09:48:26.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27659 2023-07-29 09:48:25.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:24.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.893200 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-07-29 10:03:23.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:03:23.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:23.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:23.000000 mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:23.905200 mypy-boto3-ivs-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:48:24.000000 mypy-boto3-ivs-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16775 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.965310 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22888 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26821 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16775 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/setup.py
```

### Comparing `mypy-boto3-ivs-1.28.15.post1/LICENSE` & `mypy-boto3-ivs-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.15.post1/PKG-INFO` & `mypy-boto3-ivs-1.28.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IVS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.4
+Summary: Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,14 +364,15 @@
     RenditionConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
@@ -408,14 +409,15 @@
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
@@ -423,17 +425,17 @@
     ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
-    CreateRecordingConfigurationRequestRequestTypeDef,
     RecordingConfigurationSummaryTypeDef,
     RecordingConfigurationTypeDef,
+    CreateRecordingConfigurationRequestRequestTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     GetRecordingConfigurationResponseTypeDef,
     StreamSessionTypeDef,
     GetStreamSessionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ivs-1.28.15.post1/README.md` & `mypy-boto3-ivs-1.28.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,14 +332,15 @@
     RenditionConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
@@ -376,14 +377,15 @@
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
@@ -391,17 +393,17 @@
     ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
-    CreateRecordingConfigurationRequestRequestTypeDef,
     RecordingConfigurationSummaryTypeDef,
     RecordingConfigurationTypeDef,
+    CreateRecordingConfigurationRequestRequestTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     GetRecordingConfigurationResponseTypeDef,
     StreamSessionTypeDef,
     GetStreamSessionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/__init__.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/__init__.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/__main__.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IVS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.IVS 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/client.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ivs.client import IVSClient
 
     session = Session()
     client: IVSClient = session.client("ivs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ChannelLatencyModeType, ChannelTypeType, TranscodePresetType
 from .paginator import (
     ListChannelsPaginator,
     ListPlaybackKeyPairsPaginator,
@@ -46,18 +46,16 @@
     ListChannelsResponseTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    RenditionConfigurationOutputTypeDef,
     RenditionConfigurationTypeDef,
     StreamFiltersTypeDef,
-    ThumbnailConfigurationOutputTypeDef,
     ThumbnailConfigurationTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -170,21 +168,17 @@
 
     def create_recording_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
-        renditionConfiguration: Union[
-            RenditionConfigurationTypeDef, RenditionConfigurationOutputTypeDef
-        ] = ...,
+        renditionConfiguration: RenditionConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        thumbnailConfiguration: Union[
-            ThumbnailConfigurationTypeDef, ThumbnailConfigurationOutputTypeDef
-        ] = ...
+        thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#create_recording_configuration)
         """
```

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/client.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ivs.client import IVSClient
 
     session = Session()
     client: IVSClient = session.client("ivs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ChannelLatencyModeType, ChannelTypeType, TranscodePresetType
 from .paginator import (
     ListChannelsPaginator,
     ListPlaybackKeyPairsPaginator,
@@ -46,18 +46,16 @@
     ListChannelsResponseTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    RenditionConfigurationOutputTypeDef,
     RenditionConfigurationTypeDef,
     StreamFiltersTypeDef,
-    ThumbnailConfigurationOutputTypeDef,
     ThumbnailConfigurationTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -159,21 +157,17 @@
         """
     def create_recording_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
-        renditionConfiguration: Union[
-            RenditionConfigurationTypeDef, RenditionConfigurationOutputTypeDef
-        ] = ...,
+        renditionConfiguration: RenditionConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        thumbnailConfiguration: Union[
-            ThumbnailConfigurationTypeDef, ThumbnailConfigurationOutputTypeDef
-        ] = ...
+        thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#create_recording_configuration)
         """
```

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/literals.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,14 @@
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
@@ -263,28 +262,26 @@
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

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/literals.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.pyi`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/paginator.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/paginator.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/type_defs.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     "RenditionConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetPlaybackKeyPairRequestRequestTypeDef",
     "PlaybackKeyPairTypeDef",
     "GetRecordingConfigurationRequestRequestTypeDef",
     "GetStreamKeyRequestRequestTypeDef",
     "GetStreamRequestRequestTypeDef",
@@ -94,14 +95,15 @@
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
     "BatchStartViewerSessionRevocationResponseTypeDef",
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
@@ -109,17 +111,17 @@
     "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
-    "CreateRecordingConfigurationRequestRequestTypeDef",
     "RecordingConfigurationSummaryTypeDef",
     "RecordingConfigurationTypeDef",
+    "CreateRecordingConfigurationRequestRequestTypeDef",
     "ListRecordingConfigurationsResponseTypeDef",
     "CreateRecordingConfigurationResponseTypeDef",
     "GetRecordingConfigurationResponseTypeDef",
     "StreamSessionTypeDef",
     "GetStreamSessionResponseTypeDef",
 )
 
@@ -127,25 +129,23 @@
     "AudioConfigurationTypeDef",
     {
         "channels": int,
         "codec": str,
         "sampleRate": int,
         "targetBitrate": int,
     },
-    total=False,
 )
 
 BatchErrorTypeDef = TypedDict(
     "BatchErrorTypeDef",
     {
         "arn": str,
         "code": str,
         "message": str,
     },
-    total=False,
 )
 
 BatchGetChannelRequestRequestTypeDef = TypedDict(
     "BatchGetChannelRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -162,15 +162,14 @@
         "name": str,
         "playbackUrl": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -191,41 +190,26 @@
     "StreamKeyTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
-    total=False,
 )
 
-_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+BatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationErrorTypeDef",
     {
         "channelArn": str,
-        "viewerId": str,
-    },
-)
-_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
-    {
         "code": str,
         "message": str,
+        "viewerId": str,
     },
-    total=False,
 )
 
-
-class BatchStartViewerSessionRevocationErrorTypeDef(
-    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
-    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
-):
-    pass
-
-
 _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
     "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
     },
 )
@@ -254,15 +238,14 @@
         "latencyMode": ChannelLatencyModeType,
         "name": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
         "insecureIngest": bool,
@@ -341,14 +324,21 @@
 DeleteStreamKeyRequestRequestTypeDef = TypedDict(
     "DeleteStreamKeyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+S3DestinationConfigurationOutputTypeDef = TypedDict(
+    "S3DestinationConfigurationOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+
 S3DestinationConfigurationTypeDef = TypedDict(
     "S3DestinationConfigurationTypeDef",
     {
         "bucketName": str,
     },
 )
 
@@ -370,15 +360,14 @@
     "PlaybackKeyPairTypeDef",
     {
         "arn": str,
         "fingerprint": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 GetRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecordingConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
@@ -405,15 +394,14 @@
         "health": StreamHealthType,
         "playbackUrl": str,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 _RequiredGetStreamSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetStreamSessionRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -464,15 +452,14 @@
         "codec": str,
         "encoder": str,
         "targetBitrate": int,
         "targetFramerate": int,
         "videoHeight": int,
         "videoWidth": int,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -504,15 +491,14 @@
 PlaybackKeyPairSummaryTypeDef = TypedDict(
     "PlaybackKeyPairSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 ListRecordingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListRecordingConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
@@ -545,15 +531,14 @@
 StreamKeySummaryTypeDef = TypedDict(
     "StreamKeySummaryTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredListStreamSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamSessionsRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -579,15 +564,14 @@
     "StreamSessionSummaryTypeDef",
     {
         "endTime": datetime,
         "hasErrorEvent": bool,
         "startTime": datetime,
         "streamId": str,
     },
-    total=False,
 )
 
 StreamFiltersTypeDef = TypedDict(
     "StreamFiltersTypeDef",
     {
         "health": StreamHealthType,
     },
@@ -600,15 +584,14 @@
         "channelArn": str,
         "health": StreamHealthType,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
@@ -624,26 +607,24 @@
 
 RenditionConfigurationOutputTypeDef = TypedDict(
     "RenditionConfigurationOutputTypeDef",
     {
         "renditionSelection": RenditionConfigurationRenditionSelectionType,
         "renditions": List[RenditionConfigurationRenditionType],
     },
-    total=False,
 )
 
 ThumbnailConfigurationOutputTypeDef = TypedDict(
     "ThumbnailConfigurationOutputTypeDef",
     {
         "recordingMode": RecordingModeType,
         "resolution": ThumbnailConfigurationResolutionType,
         "storage": List[ThumbnailConfigurationStorageType],
         "targetIntervalSeconds": int,
     },
-    total=False,
 )
 
 _RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
@@ -675,15 +656,14 @@
 StreamEventTypeDef = TypedDict(
     "StreamEventTypeDef",
     {
         "eventTime": datetime,
         "name": str,
         "type": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -819,14 +799,21 @@
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "s3": S3DestinationConfigurationOutputTypeDef,
+    },
+)
+
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "s3": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
@@ -857,15 +844,14 @@
 
 IngestConfigurationTypeDef = TypedDict(
     "IngestConfigurationTypeDef",
     {
         "audio": AudioConfigurationTypeDef,
         "video": VideoConfigurationTypeDef,
     },
-    total=False,
 )
 
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "filterByName": str,
         "filterByRecordingConfigurationArn": str,
@@ -963,87 +949,61 @@
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
-    {
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
+RecordingConfigurationSummaryTypeDef = TypedDict(
+    "RecordingConfigurationSummaryTypeDef",
     {
+        "arn": str,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
-        "recordingReconnectWindowSeconds": int,
-        "renditionConfiguration": RenditionConfigurationTypeDef,
-        "tags": Mapping[str, str],
-        "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
+        "state": RecordingConfigurationStateType,
+        "tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class CreateRecordingConfigurationRequestRequestTypeDef(
-    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
-    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationSummaryTypeDef",
+RecordingConfigurationTypeDef = TypedDict(
+    "RecordingConfigurationTypeDef",
     {
         "arn": str,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
-    },
-)
-_OptionalRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationSummaryTypeDef",
-    {
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
+        "recordingReconnectWindowSeconds": int,
+        "renditionConfiguration": RenditionConfigurationOutputTypeDef,
+        "state": RecordingConfigurationStateType,
         "tags": Dict[str, str],
+        "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
-
-class RecordingConfigurationSummaryTypeDef(
-    _RequiredRecordingConfigurationSummaryTypeDef, _OptionalRecordingConfigurationSummaryTypeDef
-):
-    pass
-
-
-_RequiredRecordingConfigurationTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationTypeDef",
+_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
         "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
     },
 )
-_OptionalRecordingConfigurationTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationTypeDef",
+_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "recordingReconnectWindowSeconds": int,
-        "renditionConfiguration": RenditionConfigurationOutputTypeDef,
-        "tags": Dict[str, str],
-        "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
+        "renditionConfiguration": RenditionConfigurationTypeDef,
+        "tags": Mapping[str, str],
+        "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class RecordingConfigurationTypeDef(
-    _RequiredRecordingConfigurationTypeDef, _OptionalRecordingConfigurationTypeDef
+class CreateRecordingConfigurationRequestRequestTypeDef(
+    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
+    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
@@ -1076,15 +1036,14 @@
         "endTime": datetime,
         "ingestConfiguration": IngestConfigurationTypeDef,
         "recordingConfiguration": RecordingConfigurationTypeDef,
         "startTime": datetime,
         "streamId": str,
         "truncatedEvents": List[StreamEventTypeDef],
     },
-    total=False,
 )
 
 GetStreamSessionResponseTypeDef = TypedDict(
     "GetStreamSessionResponseTypeDef",
     {
         "streamSession": StreamSessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs/type_defs.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     "RenditionConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetPlaybackKeyPairRequestRequestTypeDef",
     "PlaybackKeyPairTypeDef",
     "GetRecordingConfigurationRequestRequestTypeDef",
     "GetStreamKeyRequestRequestTypeDef",
     "GetStreamRequestRequestTypeDef",
@@ -93,14 +94,15 @@
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
     "BatchStartViewerSessionRevocationResponseTypeDef",
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
@@ -108,17 +110,17 @@
     "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
-    "CreateRecordingConfigurationRequestRequestTypeDef",
     "RecordingConfigurationSummaryTypeDef",
     "RecordingConfigurationTypeDef",
+    "CreateRecordingConfigurationRequestRequestTypeDef",
     "ListRecordingConfigurationsResponseTypeDef",
     "CreateRecordingConfigurationResponseTypeDef",
     "GetRecordingConfigurationResponseTypeDef",
     "StreamSessionTypeDef",
     "GetStreamSessionResponseTypeDef",
 )
 
@@ -126,25 +128,23 @@
     "AudioConfigurationTypeDef",
     {
         "channels": int,
         "codec": str,
         "sampleRate": int,
         "targetBitrate": int,
     },
-    total=False,
 )
 
 BatchErrorTypeDef = TypedDict(
     "BatchErrorTypeDef",
     {
         "arn": str,
         "code": str,
         "message": str,
     },
-    total=False,
 )
 
 BatchGetChannelRequestRequestTypeDef = TypedDict(
     "BatchGetChannelRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -161,15 +161,14 @@
         "name": str,
         "playbackUrl": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -190,39 +189,26 @@
     "StreamKeyTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
-    total=False,
 )
 
-_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+BatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationErrorTypeDef",
     {
         "channelArn": str,
-        "viewerId": str,
-    },
-)
-_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
-    {
         "code": str,
         "message": str,
+        "viewerId": str,
     },
-    total=False,
 )
 
-class BatchStartViewerSessionRevocationErrorTypeDef(
-    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
-    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
-):
-    pass
-
 _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
     "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
     },
 )
@@ -249,15 +235,14 @@
         "latencyMode": ChannelLatencyModeType,
         "name": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
         "insecureIngest": bool,
@@ -334,14 +319,21 @@
 DeleteStreamKeyRequestRequestTypeDef = TypedDict(
     "DeleteStreamKeyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+S3DestinationConfigurationOutputTypeDef = TypedDict(
+    "S3DestinationConfigurationOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+
 S3DestinationConfigurationTypeDef = TypedDict(
     "S3DestinationConfigurationTypeDef",
     {
         "bucketName": str,
     },
 )
 
@@ -363,15 +355,14 @@
     "PlaybackKeyPairTypeDef",
     {
         "arn": str,
         "fingerprint": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 GetRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecordingConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
@@ -398,15 +389,14 @@
         "health": StreamHealthType,
         "playbackUrl": str,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 _RequiredGetStreamSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetStreamSessionRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -453,15 +443,14 @@
         "codec": str,
         "encoder": str,
         "targetBitrate": int,
         "targetFramerate": int,
         "videoHeight": int,
         "videoWidth": int,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -493,15 +482,14 @@
 PlaybackKeyPairSummaryTypeDef = TypedDict(
     "PlaybackKeyPairSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 ListRecordingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListRecordingConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
@@ -532,15 +520,14 @@
 StreamKeySummaryTypeDef = TypedDict(
     "StreamKeySummaryTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredListStreamSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamSessionsRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -564,15 +551,14 @@
     "StreamSessionSummaryTypeDef",
     {
         "endTime": datetime,
         "hasErrorEvent": bool,
         "startTime": datetime,
         "streamId": str,
     },
-    total=False,
 )
 
 StreamFiltersTypeDef = TypedDict(
     "StreamFiltersTypeDef",
     {
         "health": StreamHealthType,
     },
@@ -585,15 +571,14 @@
         "channelArn": str,
         "health": StreamHealthType,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
@@ -609,26 +594,24 @@
 
 RenditionConfigurationOutputTypeDef = TypedDict(
     "RenditionConfigurationOutputTypeDef",
     {
         "renditionSelection": RenditionConfigurationRenditionSelectionType,
         "renditions": List[RenditionConfigurationRenditionType],
     },
-    total=False,
 )
 
 ThumbnailConfigurationOutputTypeDef = TypedDict(
     "ThumbnailConfigurationOutputTypeDef",
     {
         "recordingMode": RecordingModeType,
         "resolution": ThumbnailConfigurationResolutionType,
         "storage": List[ThumbnailConfigurationStorageType],
         "targetIntervalSeconds": int,
     },
-    total=False,
 )
 
 _RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
@@ -658,15 +641,14 @@
 StreamEventTypeDef = TypedDict(
     "StreamEventTypeDef",
     {
         "eventTime": datetime,
         "name": str,
         "type": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -800,14 +782,21 @@
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "s3": S3DestinationConfigurationOutputTypeDef,
+    },
+)
+
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "s3": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
@@ -838,15 +827,14 @@
 
 IngestConfigurationTypeDef = TypedDict(
     "IngestConfigurationTypeDef",
     {
         "audio": AudioConfigurationTypeDef,
         "video": VideoConfigurationTypeDef,
     },
-    total=False,
 )
 
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "filterByName": str,
         "filterByRecordingConfigurationArn": str,
@@ -942,82 +930,60 @@
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
-    {
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
+RecordingConfigurationSummaryTypeDef = TypedDict(
+    "RecordingConfigurationSummaryTypeDef",
     {
+        "arn": str,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
-        "recordingReconnectWindowSeconds": int,
-        "renditionConfiguration": RenditionConfigurationTypeDef,
-        "tags": Mapping[str, str],
-        "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
+        "state": RecordingConfigurationStateType,
+        "tags": Dict[str, str],
     },
-    total=False,
 )
 
-class CreateRecordingConfigurationRequestRequestTypeDef(
-    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
-    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationSummaryTypeDef",
+RecordingConfigurationTypeDef = TypedDict(
+    "RecordingConfigurationTypeDef",
     {
         "arn": str,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
-    },
-)
-_OptionalRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationSummaryTypeDef",
-    {
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
+        "recordingReconnectWindowSeconds": int,
+        "renditionConfiguration": RenditionConfigurationOutputTypeDef,
+        "state": RecordingConfigurationStateType,
         "tags": Dict[str, str],
+        "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
-class RecordingConfigurationSummaryTypeDef(
-    _RequiredRecordingConfigurationSummaryTypeDef, _OptionalRecordingConfigurationSummaryTypeDef
-):
-    pass
-
-_RequiredRecordingConfigurationTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationTypeDef",
+_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
         "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
     },
 )
-_OptionalRecordingConfigurationTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationTypeDef",
+_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "recordingReconnectWindowSeconds": int,
-        "renditionConfiguration": RenditionConfigurationOutputTypeDef,
-        "tags": Dict[str, str],
-        "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
+        "renditionConfiguration": RenditionConfigurationTypeDef,
+        "tags": Mapping[str, str],
+        "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
-class RecordingConfigurationTypeDef(
-    _RequiredRecordingConfigurationTypeDef, _OptionalRecordingConfigurationTypeDef
+class CreateRecordingConfigurationRequestRequestTypeDef(
+    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
+    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
         "nextToken": str,
@@ -1049,15 +1015,14 @@
         "endTime": datetime,
         "ingestConfiguration": IngestConfigurationTypeDef,
         "recordingConfiguration": RecordingConfigurationTypeDef,
         "startTime": datetime,
         "streamId": str,
         "truncatedEvents": List[StreamEventTypeDef],
     },
-    total=False,
 )
 
 GetStreamSessionResponseTypeDef = TypedDict(
     "GetStreamSessionResponseTypeDef",
     {
         "streamSession": StreamSessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs.egg-info/PKG-INFO` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IVS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.4
+Summary: Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ivs"></a>
 
 # mypy-boto3-ivs
 
 [![PyPI - mypy-boto3-ivs](https://img.shields.io/pypi/v/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,14 +364,15 @@
     RenditionConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
@@ -408,14 +409,15 @@
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
@@ -423,17 +425,17 @@
     ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
-    CreateRecordingConfigurationRequestRequestTypeDef,
     RecordingConfigurationSummaryTypeDef,
     RecordingConfigurationTypeDef,
+    CreateRecordingConfigurationRequestRequestTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     GetRecordingConfigurationResponseTypeDef,
     StreamSessionTypeDef,
     GetStreamSessionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ivs-1.28.15.post1/mypy_boto3_ivs.egg-info/SOURCES.txt` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.15.post1/setup.py` & `mypy-boto3-ivs-1.28.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivs",
-    version="1.28.15.post1",
+    version="1.28.4",
     packages=["mypy_boto3_ivs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IVS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

