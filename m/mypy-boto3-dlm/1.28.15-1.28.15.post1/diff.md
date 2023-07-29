# Comparing `tmp/mypy-boto3-dlm-1.28.15.tar.gz` & `tmp/mypy-boto3-dlm-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dlm-1.28.15.tar", last modified: Fri Jul 28 20:42:38 2023, max compression
+gzip compressed data, was "mypy-boto3-dlm-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:58 2023, max compression
```

## Comparing `mypy-boto3-dlm-1.28.15.tar` & `mypy-boto3-dlm-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.156963 mypy-boto3-dlm-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-28 20:42:38.152963 mypy-boto3-dlm-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.152963 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-07-28 20:23:03.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.152963 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:38.156963 mypy-boto3-dlm-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.353111 mypy-boto3-dlm-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-07-29 10:02:58.349111 mypy-boto3-dlm-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.337111 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-07-29 09:42:30.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-07-29 09:42:30.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.349111 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:58.353111 mypy-boto3-dlm-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-dlm-1.28.15/LICENSE` & `mypy-boto3-dlm-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.15/PKG-INFO` & `mypy-boto3-dlm-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dlm
-Version: 1.28.15
-Summary: Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-dlm-1.28.15/README.md` & `mypy-boto3-dlm-1.28.15.post1/README.md`

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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/__main__.py` & `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DLM 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.DLM 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM\nOther"
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

### Comparing `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/client.py` & `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,29 @@
     from boto3.session import Session
     from mypy_boto3_dlm.client import DLMClient
 
     session = Session()
     client: DLMClient = session.client("dlm")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     GettablePolicyStateValuesType,
     ResourceTypeValuesType,
     SettablePolicyStateValuesType,
 )
 from .type_defs import (
     CreateLifecyclePolicyResponseTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
 )
 
 __all__ = ("DLMClient",)
 
 
 class BotocoreClientError(BaseException):
@@ -84,15 +85,15 @@
 
     def create_lifecycle_policy(
         self,
         *,
         ExecutionRoleArn: str,
         Description: str,
         State: SettablePolicyStateValuesType,
-        PolicyDetails: PolicyDetailsTypeDef,
+        PolicyDetails: Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef],
         Tags: Mapping[str, str] = ...
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates a policy to manage the lifecycle of the specified Amazon Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.create_lifecycle_policy)
@@ -173,15 +174,15 @@
     def update_lifecycle_policy(
         self,
         *,
         PolicyId: str,
         ExecutionRoleArn: str = ...,
         State: SettablePolicyStateValuesType = ...,
         Description: str = ...,
-        PolicyDetails: PolicyDetailsTypeDef = ...
+        PolicyDetails: Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.update_lifecycle_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/client/#update_lifecycle_policy)
         """
```

### Comparing `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/client.pyi` & `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,29 @@
     from boto3.session import Session
     from mypy_boto3_dlm.client import DLMClient
 
     session = Session()
     client: DLMClient = session.client("dlm")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     GettablePolicyStateValuesType,
     ResourceTypeValuesType,
     SettablePolicyStateValuesType,
 )
 from .type_defs import (
     CreateLifecyclePolicyResponseTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
 )
 
 __all__ = ("DLMClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -78,15 +79,15 @@
         """
     def create_lifecycle_policy(
         self,
         *,
         ExecutionRoleArn: str,
         Description: str,
         State: SettablePolicyStateValuesType,
-        PolicyDetails: PolicyDetailsTypeDef,
+        PolicyDetails: Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef],
         Tags: Mapping[str, str] = ...
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates a policy to manage the lifecycle of the specified Amazon Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.create_lifecycle_policy)
@@ -159,15 +160,15 @@
     def update_lifecycle_policy(
         self,
         *,
         PolicyId: str,
         ExecutionRoleArn: str = ...,
         State: SettablePolicyStateValuesType = ...,
         Description: str = ...,
-        PolicyDetails: PolicyDetailsTypeDef = ...
+        PolicyDetails: Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.update_lifecycle_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/client/#update_lifecycle_policy)
         """
```

### Comparing `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/literals.py` & `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/literals.pyi` & `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/type_defs.py` & `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/type_defs.pyi` & `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/PKG-INFO` & `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dlm
-Version: 1.28.15
-Summary: Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/SOURCES.txt` & `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.15/setup.py` & `mypy-boto3-dlm-1.28.15.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dlm",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_dlm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

