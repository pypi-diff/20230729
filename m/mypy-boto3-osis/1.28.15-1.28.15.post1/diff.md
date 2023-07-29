# Comparing `tmp/mypy-boto3-osis-1.28.15.tar.gz` & `tmp/mypy-boto3-osis-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-osis-1.28.15.tar", last modified: Fri Jul 28 20:43:24 2023, max compression
+gzip compressed data, was "mypy-boto3-osis-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:49 2023, max compression
```

## Comparing `mypy-boto3-osis-1.28.15.tar` & `mypy-boto3-osis-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.925606 mypy-boto3-osis-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-28 20:43:24.921606 mypy-boto3-osis-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.921606 mypy-boto3-osis-1.28.15/mypy_boto3_osis/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-28 20:33:07.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-28 20:33:07.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.921606 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:24.925606 mypy-boto3-osis-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:49.945324 mypy-boto3-osis-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-07-29 10:03:49.945324 mypy-boto3-osis-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:49.929324 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11168 2023-07-29 09:52:47.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-29 09:52:47.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-29 09:52:47.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-29 09:52:47.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-29 09:52:47.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:49.929324 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:03:49.000000 mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:49.945324 mypy-boto3-osis-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-29 09:52:46.000000 mypy-boto3-osis-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-osis-1.28.15/LICENSE` & `mypy-boto3-osis-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.15/PKG-INFO` & `mypy-boto3-osis-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.28.15
-Summary: Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-osis-1.28.15/README.md` & `mypy-boto3-osis-1.28.15.post1/README.md`

 * *Files 1% similar despite different names*

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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-osis-1.28.15/mypy_boto3_osis/__main__.py` & `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchIngestion 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.OpenSearchIngestion 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion\nOther"
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

### Comparing `mypy-boto3-osis-1.28.15/mypy_boto3_osis/client.py` & `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_osis.client import OpenSearchIngestionClient
 
     session = Session()
     client: OpenSearchIngestionClient = session.client("osis")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     CreatePipelineResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
@@ -27,14 +27,15 @@
     ListTagsForResourceResponseTypeDef,
     LogPublishingOptionsTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     TagTypeDef,
     UpdatePipelineResponseTypeDef,
     ValidatePipelineResponseTypeDef,
+    VpcOptionsOutputTypeDef,
     VpcOptionsTypeDef,
 )
 
 __all__ = ("OpenSearchIngestionClient",)
 
 
 class BotocoreClientError(BaseException):
@@ -94,15 +95,15 @@
         self,
         *,
         PipelineName: str,
         MinUnits: int,
         MaxUnits: int,
         PipelineConfigurationBody: str,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
-        VpcOptions: VpcOptionsTypeDef = ...,
+        VpcOptions: Union[VpcOptionsTypeDef, VpcOptionsOutputTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/client/#create_pipeline)
```

### Comparing `mypy-boto3-osis-1.28.15/mypy_boto3_osis/client.pyi` & `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_osis.client import OpenSearchIngestionClient
 
     session = Session()
     client: OpenSearchIngestionClient = session.client("osis")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     CreatePipelineResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
@@ -27,14 +27,15 @@
     ListTagsForResourceResponseTypeDef,
     LogPublishingOptionsTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     TagTypeDef,
     UpdatePipelineResponseTypeDef,
     ValidatePipelineResponseTypeDef,
+    VpcOptionsOutputTypeDef,
     VpcOptionsTypeDef,
 )
 
 __all__ = ("OpenSearchIngestionClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -88,15 +89,15 @@
         self,
         *,
         PipelineName: str,
         MinUnits: int,
         MaxUnits: int,
         PipelineConfigurationBody: str,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
-        VpcOptions: VpcOptionsTypeDef = ...,
+        VpcOptions: Union[VpcOptionsTypeDef, VpcOptionsOutputTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.create_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/client/#create_pipeline)
```

### Comparing `mypy-boto3-osis-1.28.15/mypy_boto3_osis/literals.py` & `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.15/mypy_boto3_osis/literals.pyi` & `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.15/mypy_boto3_osis/type_defs.py` & `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.15/mypy_boto3_osis/type_defs.pyi` & `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/PKG-INFO` & `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.28.15
-Summary: Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/SOURCES.txt` & `mypy-boto3-osis-1.28.15.post1/mypy_boto3_osis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.15/setup.py` & `mypy-boto3-osis-1.28.15.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-osis",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_osis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with"
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

