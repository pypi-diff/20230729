# Comparing `tmp/mypy-boto3-appintegrations-1.28.15.tar.gz` & `tmp/mypy-boto3-appintegrations-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appintegrations-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
+gzip compressed data, was "mypy-boto3-appintegrations-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:30 2023, max compression
```

## Comparing `mypy-boto3-appintegrations-1.28.15.tar` & `mypy-boto3-appintegrations-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.284655 mypy-boto3-appintegrations-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-07-28 20:42:16.280655 mypy-boto3-appintegrations-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.272655 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.276655 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.284655 mypy-boto3-appintegrations-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.953007 mypy-boto3-appintegrations-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-29 10:02:30.949007 mypy-boto3-appintegrations-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.941007 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-07-29 09:38:13.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-07-29 09:38:13.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.949007 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:30.953007 mypy-boto3-appintegrations-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-appintegrations-1.28.15/LICENSE` & `mypy-boto3-appintegrations-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.15/PKG-INFO` & `mypy-boto3-appintegrations-1.28.15.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appintegrations
-Version: 1.28.15
-Summary: Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appintegrations-1.28.15/README.md` & `mypy-boto3-appintegrations-1.28.15.post1/README.md`

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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/__main__.py` & `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.AppIntegrationsService 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService\nOther"
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

### Comparing `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/client.py` & `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,23 @@
     from boto3.session import Session
     from mypy_boto3_appintegrations.client import AppIntegrationsServiceClient
 
     session = Session()
     client: AppIntegrationsServiceClient = session.client("appintegrations")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     EventFilterTypeDef,
+    FileConfigurationOutputTypeDef,
     FileConfigurationTypeDef,
     GetDataIntegrationResponseTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
@@ -93,15 +94,15 @@
         Name: str,
         KmsKey: str,
         SourceURI: str,
         ScheduleConfig: ScheduleConfigurationTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...,
-        FileConfiguration: FileConfigurationTypeDef = ...,
+        FileConfiguration: Union[FileConfigurationTypeDef, FileConfigurationOutputTypeDef] = ...,
         ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...
     ) -> CreateDataIntegrationResponseTypeDef:
         """
         Creates and persists a DataIntegration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_data_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/client/#create_data_integration)
```

### Comparing `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/client.pyi` & `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,23 @@
     from boto3.session import Session
     from mypy_boto3_appintegrations.client import AppIntegrationsServiceClient
 
     session = Session()
     client: AppIntegrationsServiceClient = session.client("appintegrations")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     EventFilterTypeDef,
+    FileConfigurationOutputTypeDef,
     FileConfigurationTypeDef,
     GetDataIntegrationResponseTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
@@ -87,15 +88,15 @@
         Name: str,
         KmsKey: str,
         SourceURI: str,
         ScheduleConfig: ScheduleConfigurationTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...,
-        FileConfiguration: FileConfigurationTypeDef = ...,
+        FileConfiguration: Union[FileConfigurationTypeDef, FileConfigurationOutputTypeDef] = ...,
         ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...
     ) -> CreateDataIntegrationResponseTypeDef:
         """
         Creates and persists a DataIntegration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_data_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/client/#create_data_integration)
```

### Comparing `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/literals.py` & `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/literals.pyi` & `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/type_defs.py` & `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/type_defs.pyi` & `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/PKG-INFO` & `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appintegrations
-Version: 1.28.15
-Summary: Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/SOURCES.txt` & `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.15/setup.py` & `mypy-boto3-appintegrations-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appintegrations",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_appintegrations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with"
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

