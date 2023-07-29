# Comparing `tmp/mypy-boto3-opensearch-1.28.15.tar.gz` & `tmp/mypy-boto3-opensearch-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opensearch-1.28.15.tar", last modified: Fri Jul 28 20:43:24 2023, max compression
+gzip compressed data, was "mypy-boto3-opensearch-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:47 2023, max compression
```

## Comparing `mypy-boto3-opensearch-1.28.15.tar` & `mypy-boto3-opensearch-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.149596 mypy-boto3-opensearch-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-28 20:43:24.149596 mypy-boto3-opensearch-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19304 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.149596 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41084 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41023 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68707 2023-07-28 20:32:51.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68650 2023-07-28 20:32:50.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.149596 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:24.149596 mypy-boto3-opensearch-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.785315 mypy-boto3-opensearch-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-29 10:03:47.777315 mypy-boto3-opensearch-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19304 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.773315 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-29 09:52:29.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-29 09:52:29.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68707 2023-07-29 09:52:31.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68650 2023-07-29 09:52:30.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.777315 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:47.785315 mypy-boto3-opensearch-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-opensearch-1.28.15/LICENSE` & `mypy-boto3-opensearch-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.15/PKG-INFO` & `mypy-boto3-opensearch-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.28.15
-Summary: Type annotations for boto3.OpenSearchService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.OpenSearchService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-opensearch-1.28.15/README.md` & `mypy-boto3-opensearch-1.28.15.post1/README.md`

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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/__main__.py` & `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchService 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.OpenSearchService 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService\nOther"
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

### Comparing `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/client.py` & `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_opensearch.client import OpenSearchServiceClient
 
     session = Session()
     client: OpenSearchServiceClient = session.client("opensearch")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionTypeType,
     ConnectionModeType,
     DryRunModeType,
@@ -28,14 +28,15 @@
     ScheduleAtType,
 )
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
     ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
@@ -735,15 +736,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
+        AutoTuneOptions: Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef] = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
```

### Comparing `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/client.pyi` & `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_opensearch.client import OpenSearchServiceClient
 
     session = Session()
     client: OpenSearchServiceClient = session.client("opensearch")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionTypeType,
     ConnectionModeType,
     DryRunModeType,
@@ -28,14 +28,15 @@
     ScheduleAtType,
 )
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
     ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
@@ -678,15 +679,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
+        AutoTuneOptions: Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef] = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
```

### Comparing `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/literals.py` & `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/literals.pyi` & `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/type_defs.py` & `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/type_defs.pyi` & `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/PKG-INFO` & `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.28.15
-Summary: Type annotations for boto3.OpenSearchService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.OpenSearchService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/SOURCES.txt` & `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.15/setup.py` & `mypy-boto3-opensearch-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opensearch",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_opensearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.OpenSearchService 1.28.15 service generated with"
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

