# Comparing `tmp/mypy-boto3-nimble-1.28.15.tar.gz` & `tmp/mypy-boto3-nimble-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-nimble-1.28.15.tar", last modified: Fri Jul 28 20:43:22 2023, max compression
+gzip compressed data, was "mypy-boto3-nimble-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:47 2023, max compression
```

## Comparing `mypy-boto3-nimble-1.28.15.tar` & `mypy-boto3-nimble-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:22.905579 mypy-boto3-nimble-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:36.000000 mypy-boto3-nimble-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-07-28 20:43:22.901579 mypy-boto3-nimble-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23135 2023-07-28 20:32:36.000000 mypy-boto3-nimble-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:22.901579 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-28 20:32:36.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-28 20:32:36.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:32:36.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44528 2023-07-28 20:32:37.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44450 2023-07-28 20:32:37.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-28 20:32:37.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-07-28 20:32:37.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-28 20:32:37.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-07-28 20:32:37.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:36.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71497 2023-07-28 20:32:39.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71378 2023-07-28 20:32:38.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:36.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-07-28 20:32:37.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-07-28 20:32:37.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:22.901579 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-07-28 20:43:22.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:22.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:22.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:22.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:22.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:22.000000 mypy-boto3-nimble-1.28.15/mypy_boto3_nimble.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:22.905579 mypy-boto3-nimble-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-28 20:32:36.000000 mypy-boto3-nimble-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.389314 mypy-boto3-nimble-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24630 2023-07-29 10:03:47.381314 mypy-boto3-nimble-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23135 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.373314 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44726 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44648 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-29 09:52:17.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71497 2023-07-29 09:52:18.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71378 2023-07-29 09:52:17.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-07-29 09:52:16.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.381314 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24630 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:47.000000 mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:47.389314 mypy-boto3-nimble-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-29 09:52:15.000000 mypy-boto3-nimble-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-nimble-1.28.15/LICENSE` & `mypy-boto3-nimble-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/PKG-INFO` & `mypy-boto3-nimble-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-nimble
-Version: 1.28.15
-Summary: Type annotations for boto3.NimbleStudio 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.NimbleStudio 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/
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
 [mypy-boto3-nimble docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-nimble-1.28.15/README.md` & `mypy-boto3-nimble-1.28.15.post1/README.md`

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
 [mypy-boto3-nimble docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/__init__.py` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/__init__.pyi` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/__main__.py` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.NimbleStudio 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.NimbleStudio 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio\nOther"
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

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/client.py` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_nimble.client import NimbleStudioClient
 
     session = Session()
     client: NimbleStudioClient = session.client("nimble")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     LaunchProfileStateType,
     StreamingInstanceTypeType,
     StudioComponentStateType,
@@ -77,14 +77,15 @@
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
     ScriptParameterKeyValueTypeDef,
     StartStreamingSessionResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
     StreamConfigurationCreateTypeDef,
+    StudioComponentConfigurationOutputTypeDef,
     StudioComponentConfigurationTypeDef,
     StudioComponentInitializationScriptTypeDef,
     StudioEncryptionConfigurationTypeDef,
     UpdateLaunchProfileMemberResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
@@ -267,15 +268,17 @@
     def create_studio_component(
         self,
         *,
         name: str,
         studioId: str,
         type: StudioComponentTypeType,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationTypeDef = ...,
+        configuration: Union[
+            StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
+        ] = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
@@ -771,15 +774,17 @@
 
     def update_studio_component(
         self,
         *,
         studioComponentId: str,
         studioId: str,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationTypeDef = ...,
+        configuration: Union[
+            StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
+        ] = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         name: str = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
```

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/client.pyi` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_nimble.client import NimbleStudioClient
 
     session = Session()
     client: NimbleStudioClient = session.client("nimble")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     LaunchProfileStateType,
     StreamingInstanceTypeType,
     StudioComponentStateType,
@@ -77,14 +77,15 @@
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
     ScriptParameterKeyValueTypeDef,
     StartStreamingSessionResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
     StreamConfigurationCreateTypeDef,
+    StudioComponentConfigurationOutputTypeDef,
     StudioComponentConfigurationTypeDef,
     StudioComponentInitializationScriptTypeDef,
     StudioEncryptionConfigurationTypeDef,
     UpdateLaunchProfileMemberResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
@@ -254,15 +255,17 @@
     def create_studio_component(
         self,
         *,
         name: str,
         studioId: str,
         type: StudioComponentTypeType,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationTypeDef = ...,
+        configuration: Union[
+            StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
+        ] = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
@@ -715,15 +718,17 @@
         """
     def update_studio_component(
         self,
         *,
         studioComponentId: str,
         studioId: str,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationTypeDef = ...,
+        configuration: Union[
+            StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
+        ] = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         name: str = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
```

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/literals.py` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/literals.pyi` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/paginator.py` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/paginator.pyi` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/type_defs.py` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/type_defs.pyi` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/waiter.py` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble/waiter.pyi` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble.egg-info/PKG-INFO` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-nimble
-Version: 1.28.15
-Summary: Type annotations for boto3.NimbleStudio 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.NimbleStudio 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/
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
 [mypy-boto3-nimble docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_nimble/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-nimble-1.28.15/mypy_boto3_nimble.egg-info/SOURCES.txt` & `mypy-boto3-nimble-1.28.15.post1/mypy_boto3_nimble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-nimble-1.28.15/setup.py` & `mypy-boto3-nimble-1.28.15.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-nimble",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_nimble"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.NimbleStudio 1.28.15 service generated with mypy-boto3-builder"
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

