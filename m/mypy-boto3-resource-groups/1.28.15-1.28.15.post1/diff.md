# Comparing `tmp/mypy-boto3-resource-groups-1.28.15.tar.gz` & `tmp/mypy-boto3-resource-groups-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resource-groups-1.28.15.tar", last modified: Fri Jul 28 20:43:34 2023, max compression
+gzip compressed data, was "mypy-boto3-resource-groups-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:01 2023, max compression
```

## Comparing `mypy-boto3-resource-groups-1.28.15.tar` & `mypy-boto3-resource-groups-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:34.181733 mypy-boto3-resource-groups-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-28 20:43:34.181733 mypy-boto3-resource-groups-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:34.181733 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16986 2023-07-28 20:37:00.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-07-28 20:37:00.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:34.181733 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:34.181733 mypy-boto3-resource-groups-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.221365 mypy-boto3-resource-groups-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-29 10:04:01.217365 mypy-boto3-resource-groups-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.205365 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-29 09:57:05.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-07-29 09:57:05.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17125 2023-07-29 09:57:05.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17106 2023-07-29 09:57:05.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.217365 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-29 10:04:00.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:04:01.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:00.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:00.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:00.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:04:00.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:01.221365 mypy-boto3-resource-groups-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-resource-groups-1.28.15/LICENSE` & `mypy-boto3-resource-groups-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15/PKG-INFO` & `mypy-boto3-resource-groups-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.28.15
-Summary: Type annotations for boto3.ResourceGroups 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ResourceGroups 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-resource-groups-1.28.15/README.md` & `mypy-boto3-resource-groups-1.28.15.post1/README.md`

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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__init__.py` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__init__.pyi` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__main__.py` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceGroups 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.ResourceGroups 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups\nOther"
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

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/client.py` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,29 @@
     from mypy_boto3_resource_groups.client import ResourceGroupsClient
 
     session = Session()
     client: ResourceGroupsClient = session.client("resource-groups")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import GroupLifecycleEventsDesiredStatusType
 from .paginator import ListGroupResourcesPaginator, ListGroupsPaginator, SearchResourcesPaginator
 from .type_defs import (
     CreateGroupOutputTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
     GetGroupOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     GetTagsOutputTypeDef,
+    GroupConfigurationItemOutputTypeDef,
     GroupConfigurationItemTypeDef,
     GroupFilterTypeDef,
     GroupResourcesOutputTypeDef,
     ListGroupResourcesOutputTypeDef,
     ListGroupsOutputTypeDef,
     ResourceFilterTypeDef,
     ResourceQueryTypeDef,
@@ -108,15 +109,17 @@
     def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        Configuration: Sequence[
+            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
+        ] = ...
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#create_group)
         """
@@ -225,15 +228,20 @@
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#list_groups)
         """
 
     def put_group_configuration(
-        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        self,
+        *,
+        Group: str = ...,
+        Configuration: Sequence[
+            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Attaches a service configuration to the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.put_group_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#put_group_configuration)
         """
```

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/client.pyi` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,29 @@
     from mypy_boto3_resource_groups.client import ResourceGroupsClient
 
     session = Session()
     client: ResourceGroupsClient = session.client("resource-groups")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import GroupLifecycleEventsDesiredStatusType
 from .paginator import ListGroupResourcesPaginator, ListGroupsPaginator, SearchResourcesPaginator
 from .type_defs import (
     CreateGroupOutputTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
     GetGroupOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     GetTagsOutputTypeDef,
+    GroupConfigurationItemOutputTypeDef,
     GroupConfigurationItemTypeDef,
     GroupFilterTypeDef,
     GroupResourcesOutputTypeDef,
     ListGroupResourcesOutputTypeDef,
     ListGroupsOutputTypeDef,
     ResourceFilterTypeDef,
     ResourceQueryTypeDef,
@@ -101,15 +102,17 @@
     def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        Configuration: Sequence[
+            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
+        ] = ...
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#create_group)
         """
@@ -207,15 +210,20 @@
         """
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#list_groups)
         """
     def put_group_configuration(
-        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        self,
+        *,
+        Group: str = ...,
+        Configuration: Sequence[
+            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Attaches a service configuration to the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.put_group_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#put_group_configuration)
         """
```

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/literals.py` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/literals.pyi` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/paginator.py` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/paginator.pyi` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/type_defs.py` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_resource_groups.type_defs import AccountSettingsTypeDef
 
     data: AccountSettingsTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     GroupConfigurationStatusType,
     GroupFilterNameType,
     GroupLifecycleEventsDesiredStatusType,
     GroupLifecycleEventsStatusType,
     QueryErrorCodeType,
@@ -28,15 +28,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
@@ -122,19 +121,17 @@
     "_OptionalGroupTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -204,43 +201,39 @@
     "_OptionalGroupConfigurationParameterOutputTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
 
-
 class GroupConfigurationParameterOutputTypeDef(
     _RequiredGroupConfigurationParameterOutputTypeDef,
     _OptionalGroupConfigurationParameterOutputTypeDef,
 ):
     pass
 
-
 _RequiredGroupConfigurationParameterTypeDef = TypedDict(
     "_RequiredGroupConfigurationParameterTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGroupConfigurationParameterTypeDef = TypedDict(
     "_OptionalGroupConfigurationParameterTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
-
 class GroupConfigurationParameterTypeDef(
     _RequiredGroupConfigurationParameterTypeDef, _OptionalGroupConfigurationParameterTypeDef
 ):
     pass
 
-
 GroupFilterTypeDef = TypedDict(
     "GroupFilterTypeDef",
     {
         "Name": GroupFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -375,21 +368,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchResourcesInputRequestTypeDef(
     _RequiredSearchResourcesInputRequestTypeDef, _OptionalSearchResourcesInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateGroupQueryInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupQueryInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalUpdateGroupQueryInputRequestTypeDef = TypedDict(
@@ -397,21 +388,19 @@
     {
         "GroupName": str,
         "Group": str,
     },
     total=False,
 )
 
-
 class UpdateGroupQueryInputRequestTypeDef(
     _RequiredUpdateGroupQueryInputRequestTypeDef, _OptionalUpdateGroupQueryInputRequestTypeDef
 ):
     pass
 
-
 DeleteGroupOutputTypeDef = TypedDict(
     "DeleteGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -485,42 +474,38 @@
     "_OptionalGroupConfigurationItemOutputTypeDef",
     {
         "Parameters": List[GroupConfigurationParameterOutputTypeDef],
     },
     total=False,
 )
 
-
 class GroupConfigurationItemOutputTypeDef(
     _RequiredGroupConfigurationItemOutputTypeDef, _OptionalGroupConfigurationItemOutputTypeDef
 ):
     pass
 
-
 _RequiredGroupConfigurationItemTypeDef = TypedDict(
     "_RequiredGroupConfigurationItemTypeDef",
     {
         "Type": str,
     },
 )
 _OptionalGroupConfigurationItemTypeDef = TypedDict(
     "_OptionalGroupConfigurationItemTypeDef",
     {
         "Parameters": Sequence[GroupConfigurationParameterTypeDef],
     },
     total=False,
 )
 
-
 class GroupConfigurationItemTypeDef(
     _RequiredGroupConfigurationItemTypeDef, _OptionalGroupConfigurationItemTypeDef
 ):
     pass
 
-
 ListGroupsInputRequestTypeDef = TypedDict(
     "ListGroupsInputRequestTypeDef",
     {
         "Filters": Sequence[GroupFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -576,22 +561,20 @@
     "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchResourcesInputSearchResourcesPaginateTypeDef(
     _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
     _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
 ):
     pass
 
-
 ListGroupResourcesInputListGroupResourcesPaginateTypeDef = TypedDict(
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     {
         "GroupName": str,
         "Group": str,
         "Filters": Sequence[ResourceFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -665,31 +648,33 @@
 )
 _OptionalCreateGroupInputRequestTypeDef = TypedDict(
     "_OptionalCreateGroupInputRequestTypeDef",
     {
         "Description": str,
         "ResourceQuery": ResourceQueryTypeDef,
         "Tags": Mapping[str, str],
-        "Configuration": Sequence[GroupConfigurationItemTypeDef],
+        "Configuration": Sequence[
+            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
+        ],
     },
     total=False,
 )
 
-
 class CreateGroupInputRequestTypeDef(
     _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
 ):
     pass
 
-
 PutGroupConfigurationInputRequestTypeDef = TypedDict(
     "PutGroupConfigurationInputRequestTypeDef",
     {
         "Group": str,
-        "Configuration": Sequence[GroupConfigurationItemTypeDef],
+        "Configuration": Sequence[
+            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
```

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/type_defs.pyi` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_resource_groups.type_defs import AccountSettingsTypeDef
 
     data: AccountSettingsTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     GroupConfigurationStatusType,
     GroupFilterNameType,
     GroupLifecycleEventsDesiredStatusType,
     GroupLifecycleEventsStatusType,
     QueryErrorCodeType,
@@ -28,14 +28,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
@@ -121,17 +122,19 @@
     "_OptionalGroupTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -201,39 +204,43 @@
     "_OptionalGroupConfigurationParameterOutputTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
 
+
 class GroupConfigurationParameterOutputTypeDef(
     _RequiredGroupConfigurationParameterOutputTypeDef,
     _OptionalGroupConfigurationParameterOutputTypeDef,
 ):
     pass
 
+
 _RequiredGroupConfigurationParameterTypeDef = TypedDict(
     "_RequiredGroupConfigurationParameterTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGroupConfigurationParameterTypeDef = TypedDict(
     "_OptionalGroupConfigurationParameterTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
+
 class GroupConfigurationParameterTypeDef(
     _RequiredGroupConfigurationParameterTypeDef, _OptionalGroupConfigurationParameterTypeDef
 ):
     pass
 
+
 GroupFilterTypeDef = TypedDict(
     "GroupFilterTypeDef",
     {
         "Name": GroupFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -368,19 +375,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchResourcesInputRequestTypeDef(
     _RequiredSearchResourcesInputRequestTypeDef, _OptionalSearchResourcesInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateGroupQueryInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupQueryInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalUpdateGroupQueryInputRequestTypeDef = TypedDict(
@@ -388,19 +397,21 @@
     {
         "GroupName": str,
         "Group": str,
     },
     total=False,
 )
 
+
 class UpdateGroupQueryInputRequestTypeDef(
     _RequiredUpdateGroupQueryInputRequestTypeDef, _OptionalUpdateGroupQueryInputRequestTypeDef
 ):
     pass
 
+
 DeleteGroupOutputTypeDef = TypedDict(
     "DeleteGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -474,38 +485,42 @@
     "_OptionalGroupConfigurationItemOutputTypeDef",
     {
         "Parameters": List[GroupConfigurationParameterOutputTypeDef],
     },
     total=False,
 )
 
+
 class GroupConfigurationItemOutputTypeDef(
     _RequiredGroupConfigurationItemOutputTypeDef, _OptionalGroupConfigurationItemOutputTypeDef
 ):
     pass
 
+
 _RequiredGroupConfigurationItemTypeDef = TypedDict(
     "_RequiredGroupConfigurationItemTypeDef",
     {
         "Type": str,
     },
 )
 _OptionalGroupConfigurationItemTypeDef = TypedDict(
     "_OptionalGroupConfigurationItemTypeDef",
     {
         "Parameters": Sequence[GroupConfigurationParameterTypeDef],
     },
     total=False,
 )
 
+
 class GroupConfigurationItemTypeDef(
     _RequiredGroupConfigurationItemTypeDef, _OptionalGroupConfigurationItemTypeDef
 ):
     pass
 
+
 ListGroupsInputRequestTypeDef = TypedDict(
     "ListGroupsInputRequestTypeDef",
     {
         "Filters": Sequence[GroupFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -561,20 +576,22 @@
     "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchResourcesInputSearchResourcesPaginateTypeDef(
     _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
     _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
 ):
     pass
 
+
 ListGroupResourcesInputListGroupResourcesPaginateTypeDef = TypedDict(
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     {
         "GroupName": str,
         "Group": str,
         "Filters": Sequence[ResourceFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -648,29 +665,35 @@
 )
 _OptionalCreateGroupInputRequestTypeDef = TypedDict(
     "_OptionalCreateGroupInputRequestTypeDef",
     {
         "Description": str,
         "ResourceQuery": ResourceQueryTypeDef,
         "Tags": Mapping[str, str],
-        "Configuration": Sequence[GroupConfigurationItemTypeDef],
+        "Configuration": Sequence[
+            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
+        ],
     },
     total=False,
 )
 
+
 class CreateGroupInputRequestTypeDef(
     _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
 ):
     pass
 
+
 PutGroupConfigurationInputRequestTypeDef = TypedDict(
     "PutGroupConfigurationInputRequestTypeDef",
     {
         "Group": str,
-        "Configuration": Sequence[GroupConfigurationItemTypeDef],
+        "Configuration": Sequence[
+            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
```

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/PKG-INFO` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.28.15
-Summary: Type annotations for boto3.ResourceGroups 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ResourceGroups 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/SOURCES.txt` & `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15/setup.py` & `mypy-boto3-resource-groups-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resource-groups",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_resource_groups"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ResourceGroups 1.28.15 service generated with"
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

