# Comparing `tmp/mypy-boto3-wisdom-1.28.15.tar.gz` & `tmp/mypy-boto3-wisdom-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wisdom-1.28.15.tar", last modified: Fri Jul 28 20:43:56 2023, max compression
+gzip compressed data, was "mypy-boto3-wisdom-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:26 2023, max compression
```

## Comparing `mypy-boto3-wisdom-1.28.15.tar` & `mypy-boto3-wisdom-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.794043 mypy-boto3-wisdom-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-07-28 20:43:56.790043 mypy-boto3-wisdom-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.782043 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37013 2023-07-28 20:41:31.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.790043 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:56.794043 mypy-boto3-wisdom-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.117458 mypy-boto3-wisdom-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-07-29 10:04:26.117458 mypy-boto3-wisdom-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.109458 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25143 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25098 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-29 10:01:39.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-29 10:01:39.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37013 2023-07-29 10:01:40.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-07-29 10:01:39.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.117458 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:04:25.000000 mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:26.117458 mypy-boto3-wisdom-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 10:01:38.000000 mypy-boto3-wisdom-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-wisdom-1.28.15/LICENSE` & `mypy-boto3-wisdom-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15/PKG-INFO` & `mypy-boto3-wisdom-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.28.15
-Summary: Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wisdom-1.28.15/README.md` & `mypy-boto3-wisdom-1.28.15.post1/README.md`

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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__init__.py` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__init__.pyi` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__main__.py` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectWisdomService 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.ConnectWisdomService 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService\nOther"
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

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/client.py` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_wisdom.client import ConnectWisdomServiceClient
 
     session = Session()
     client: ConnectWisdomServiceClient = session.client("wisdom")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import KnowledgeBaseTypeType
 from .paginator import (
     ListAssistantAssociationsPaginator,
     ListAssistantsPaginator,
@@ -50,14 +50,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     QueryAssistantResponseTypeDef,
     RenderingConfigurationTypeDef,
     SearchContentResponseTypeDef,
     SearchExpressionTypeDef,
     SearchSessionsResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -179,15 +180,17 @@
         *,
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        sourceConfiguration: SourceConfigurationTypeDef = ...,
+        sourceConfiguration: Union[
+            SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
+        ] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/client/#create_knowledge_base)
```

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/client.pyi` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_wisdom.client import ConnectWisdomServiceClient
 
     session = Session()
     client: ConnectWisdomServiceClient = session.client("wisdom")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import KnowledgeBaseTypeType
 from .paginator import (
     ListAssistantAssociationsPaginator,
     ListAssistantsPaginator,
@@ -50,14 +50,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     QueryAssistantResponseTypeDef,
     RenderingConfigurationTypeDef,
     SearchContentResponseTypeDef,
     SearchExpressionTypeDef,
     SearchSessionsResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -169,15 +170,17 @@
         *,
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        sourceConfiguration: SourceConfigurationTypeDef = ...,
+        sourceConfiguration: Union[
+            SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
+        ] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/client/#create_knowledge_base)
```

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/literals.py` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/literals.pyi` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/paginator.py` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/paginator.pyi` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/type_defs.py` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/type_defs.pyi` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/PKG-INFO` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.28.15
-Summary: Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/SOURCES.txt` & `mypy-boto3-wisdom-1.28.15.post1/mypy_boto3_wisdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.15/setup.py` & `mypy-boto3-wisdom-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wisdom",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_wisdom"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with"
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

