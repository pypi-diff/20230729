# Comparing `tmp/mypy-boto3-iotdeviceadvisor-1.28.15.tar.gz` & `tmp/mypy-boto3-iotdeviceadvisor-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotdeviceadvisor-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
+gzip compressed data, was "mypy-boto3-iotdeviceadvisor-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:20 2023, max compression
```

## Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.tar` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.409256 mypy-boto3-iotdeviceadvisor-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-07-28 20:42:59.405256 mypy-boto3-iotdeviceadvisor-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.401256 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-07-28 20:28:20.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.405256 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.409256 mypy-boto3-iotdeviceadvisor-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.173183 mypy-boto3-iotdeviceadvisor-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-29 10:03:20.173183 mypy-boto3-iotdeviceadvisor-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.173183 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-07-29 09:47:53.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-07-29 09:47:53.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.173183 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:20.197183 mypy-boto3-iotdeviceadvisor-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/LICENSE` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/PKG-INFO` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotdeviceadvisor
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/README.md` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/README.md`

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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/__main__.py` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTDeviceAdvisor 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.IoTDeviceAdvisor 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor\nOther"
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

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/client.py` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,30 +9,32 @@
     from boto3.session import Session
     from mypy_boto3_iotdeviceadvisor.client import IoTDeviceAdvisorClient
 
     session = Session()
     client: IoTDeviceAdvisorClient = session.client("iotdeviceadvisor")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AuthenticationMethodType
 from .type_defs import (
     CreateSuiteDefinitionResponseTypeDef,
     GetEndpointResponseTypeDef,
     GetSuiteDefinitionResponseTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunResponseTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     ListSuiteRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartSuiteRunResponseTypeDef,
+    SuiteDefinitionConfigurationOutputTypeDef,
     SuiteDefinitionConfigurationTypeDef,
+    SuiteRunConfigurationOutputTypeDef,
     SuiteRunConfigurationTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
 )
 
 __all__ = ("IoTDeviceAdvisorClient",)
 
 
@@ -84,15 +86,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#close)
         """
 
     def create_suite_definition(
         self,
         *,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef,
+        suiteDefinitionConfiguration: Union[
+            SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
+        ],
         tags: Mapping[str, str] = ...
     ) -> CreateSuiteDefinitionResponseTypeDef:
         """
         Creates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#create_suite_definition)
@@ -199,15 +203,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#list_tags_for_resource)
         """
 
     def start_suite_run(
         self,
         *,
         suiteDefinitionId: str,
-        suiteRunConfiguration: SuiteRunConfigurationTypeDef,
+        suiteRunConfiguration: Union[
+            SuiteRunConfigurationTypeDef, SuiteRunConfigurationOutputTypeDef
+        ],
         suiteDefinitionVersion: str = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSuiteRunResponseTypeDef:
         """
         Starts a Device Advisor test suite run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)
@@ -238,15 +244,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#untag_resource)
         """
 
     def update_suite_definition(
         self,
         *,
         suiteDefinitionId: str,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef
+        suiteDefinitionConfiguration: Union[
+            SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
+        ]
     ) -> UpdateSuiteDefinitionResponseTypeDef:
         """
         Updates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#update_suite_definition)
         """
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/client.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,32 @@
     from boto3.session import Session
     from mypy_boto3_iotdeviceadvisor.client import IoTDeviceAdvisorClient
 
     session = Session()
     client: IoTDeviceAdvisorClient = session.client("iotdeviceadvisor")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AuthenticationMethodType
 from .type_defs import (
     CreateSuiteDefinitionResponseTypeDef,
     GetEndpointResponseTypeDef,
     GetSuiteDefinitionResponseTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunResponseTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     ListSuiteRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartSuiteRunResponseTypeDef,
+    SuiteDefinitionConfigurationOutputTypeDef,
     SuiteDefinitionConfigurationTypeDef,
+    SuiteRunConfigurationOutputTypeDef,
     SuiteRunConfigurationTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
 )
 
 __all__ = ("IoTDeviceAdvisorClient",)
 
 class BotocoreClientError(BaseException):
@@ -78,15 +80,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#close)
         """
     def create_suite_definition(
         self,
         *,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef,
+        suiteDefinitionConfiguration: Union[
+            SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
+        ],
         tags: Mapping[str, str] = ...
     ) -> CreateSuiteDefinitionResponseTypeDef:
         """
         Creates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#create_suite_definition)
@@ -183,15 +187,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#list_tags_for_resource)
         """
     def start_suite_run(
         self,
         *,
         suiteDefinitionId: str,
-        suiteRunConfiguration: SuiteRunConfigurationTypeDef,
+        suiteRunConfiguration: Union[
+            SuiteRunConfigurationTypeDef, SuiteRunConfigurationOutputTypeDef
+        ],
         suiteDefinitionVersion: str = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSuiteRunResponseTypeDef:
         """
         Starts a Device Advisor test suite run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)
@@ -218,15 +224,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#untag_resource)
         """
     def update_suite_definition(
         self,
         *,
         suiteDefinitionId: str,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef
+        suiteDefinitionConfiguration: Union[
+            SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
+        ]
     ) -> UpdateSuiteDefinitionResponseTypeDef:
         """
         Updates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#update_suite_definition)
         """
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/literals.py` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/literals.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/type_defs.py` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/type_defs.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotdeviceadvisor
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15/setup.py` & `mypy-boto3-iotdeviceadvisor-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotdeviceadvisor",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_iotdeviceadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with"
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

