# Comparing `tmp/mypy-boto3-apprunner-1.28.15.tar.gz` & `tmp/mypy-boto3-apprunner-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apprunner-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
+gzip compressed data, was "mypy-boto3-apprunner-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:31 2023, max compression
```

## Comparing `mypy-boto3-apprunner-1.28.15.tar` & `mypy-boto3-apprunner-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.180694 mypy-boto3-apprunner-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16880 2023-07-28 20:42:19.180694 mypy-boto3-apprunner-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.172694 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25678 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-28 20:19:34.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38636 2023-07-28 20:19:35.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38593 2023-07-28 20:19:35.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.180694 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16880 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.180694 mypy-boto3-apprunner-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.193008 mypy-boto3-apprunner-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-29 10:02:31.193008 mypy-boto3-apprunner-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.185008 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25827 2023-07-29 09:38:26.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25785 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-29 09:38:26.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-29 09:38:26.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38636 2023-07-29 09:38:27.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38593 2023-07-29 09:38:26.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.193008 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:31.193008 mypy-boto3-apprunner-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-apprunner-1.28.15/LICENSE` & `mypy-boto3-apprunner-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.15/PKG-INFO` & `mypy-boto3-apprunner-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apprunner
-Version: 1.28.15
-Summary: Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-apprunner-1.28.15/README.md` & `mypy-boto3-apprunner-1.28.15.post1/README.md`

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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/__main__.py` & `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppRunner 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.AppRunner 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner\nOther"
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

### Comparing `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/client.py` & `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_apprunner.client import AppRunnerClient
 
     session = Session()
     client: AppRunnerClient = session.client("apprunner")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     AssociateCustomDomainResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     CreateConnectionResponseTypeDef,
@@ -52,14 +52,15 @@
     ListVpcConnectorsResponseTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     ListVpcIngressConnectionsResponseTypeDef,
     NetworkConfigurationTypeDef,
     PauseServiceResponseTypeDef,
     ResumeServiceResponseTypeDef,
     ServiceObservabilityConfigurationTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     StartDeploymentResponseTypeDef,
     TagTypeDef,
     TraceConfigurationTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
 )
@@ -178,15 +179,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/client/#create_observability_configuration)
         """
 
     def create_service(
         self,
         *,
         ServiceName: str,
-        SourceConfiguration: SourceConfigurationTypeDef,
+        SourceConfiguration: Union[SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef],
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
         ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
@@ -505,15 +506,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/client/#untag_resource)
         """
 
     def update_service(
         self,
         *,
         ServiceArn: str,
-        SourceConfiguration: SourceConfigurationTypeDef = ...,
+        SourceConfiguration: Union[
+            SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
+        ] = ...,
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
         ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
```

### Comparing `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/client.pyi` & `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_apprunner.client import AppRunnerClient
 
     session = Session()
     client: AppRunnerClient = session.client("apprunner")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     AssociateCustomDomainResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     CreateConnectionResponseTypeDef,
@@ -52,14 +52,15 @@
     ListVpcConnectorsResponseTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     ListVpcIngressConnectionsResponseTypeDef,
     NetworkConfigurationTypeDef,
     PauseServiceResponseTypeDef,
     ResumeServiceResponseTypeDef,
     ServiceObservabilityConfigurationTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     StartDeploymentResponseTypeDef,
     TagTypeDef,
     TraceConfigurationTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
 )
@@ -167,15 +168,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_observability_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/client/#create_observability_configuration)
         """
     def create_service(
         self,
         *,
         ServiceName: str,
-        SourceConfiguration: SourceConfigurationTypeDef,
+        SourceConfiguration: Union[SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef],
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
         ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
@@ -464,15 +465,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/client/#untag_resource)
         """
     def update_service(
         self,
         *,
         ServiceArn: str,
-        SourceConfiguration: SourceConfigurationTypeDef = ...,
+        SourceConfiguration: Union[
+            SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
+        ] = ...,
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
         ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
```

### Comparing `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/literals.py` & `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/literals.pyi` & `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/type_defs.py` & `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/type_defs.pyi` & `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/PKG-INFO` & `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apprunner
-Version: 1.28.15
-Summary: Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/SOURCES.txt` & `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.15/setup.py` & `mypy-boto3-apprunner-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apprunner",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_apprunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder"
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

