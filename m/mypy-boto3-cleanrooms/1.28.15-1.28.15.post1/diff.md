# Comparing `tmp/mypy-boto3-cleanrooms-1.28.15.tar.gz` & `tmp/mypy-boto3-cleanrooms-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cleanrooms-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
+gzip compressed data, was "mypy-boto3-cleanrooms-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:41 2023, max compression
```

## Comparing `mypy-boto3-cleanrooms-1.28.15.tar` & `mypy-boto3-cleanrooms-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.356780 mypy-boto3-cleanrooms-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19147 2023-07-28 20:42:25.356780 mypy-boto3-cleanrooms-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.356780 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-07-28 20:20:47.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29837 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-28 20:20:47.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-28 20:20:47.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-07-28 20:20:47.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-28 20:20:47.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43817 2023-07-28 20:20:48.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43758 2023-07-28 20:20:48.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.356780 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19147 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.356780 mypy-boto3-cleanrooms-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.277049 mypy-boto3-cleanrooms-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:39.000000 mypy-boto3-cleanrooms-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19153 2023-07-29 10:02:41.277049 mypy-boto3-cleanrooms-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-07-29 09:39:39.000000 mypy-boto3-cleanrooms-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.273049 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:39:39.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-29 09:39:39.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:39:39.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30101 2023-07-29 09:39:40.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30050 2023-07-29 09:39:39.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-29 09:39:40.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-29 09:39:40.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-07-29 09:39:40.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-29 09:39:40.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:39.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43817 2023-07-29 09:39:41.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43758 2023-07-29 09:39:41.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:39.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.277049 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19153 2023-07-29 10:02:41.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:02:41.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:41.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:41.000000 mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:41.277049 mypy-boto3-cleanrooms-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:39:39.000000 mypy-boto3-cleanrooms-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-cleanrooms-1.28.15/LICENSE` & `mypy-boto3-cleanrooms-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.15/PKG-INFO` & `mypy-boto3-cleanrooms-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.28.15
-Summary: Type annotations for boto3.CleanRoomsService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CleanRoomsService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cleanrooms-1.28.15/README.md` & `mypy-boto3-cleanrooms-1.28.15.post1/README.md`

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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__init__.py` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__init__.pyi` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__main__.py` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CleanRoomsService 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.CleanRoomsService 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService\nOther"
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

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/client.py` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_cleanrooms.client import CleanRoomsServiceClient
 
     session = Session()
     client: CleanRoomsServiceClient = session.client("cleanrooms")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
@@ -35,14 +35,15 @@
     ListMembershipsPaginator,
     ListMembersPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
 )
 from .type_defs import (
     BatchGetSchemaOutputTypeDef,
+    ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateCollaborationOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     CreateConfiguredTableOutputTypeDef,
     CreateMembershipOutputTypeDef,
     DataEncryptionMetadataTypeDef,
@@ -183,15 +184,17 @@
         """
 
     def create_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: Union[
+            ConfiguredTableAnalysisRulePolicyTypeDef, ConfiguredTableAnalysisRulePolicyOutputTypeDef
+        ]
     ) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Creates a new analysis rule for a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_configured_table_analysis_rule)
         """
@@ -519,15 +522,17 @@
         """
 
     def update_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: Union[
+            ConfiguredTableAnalysisRulePolicyTypeDef, ConfiguredTableAnalysisRulePolicyOutputTypeDef
+        ]
     ) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Updates a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#update_configured_table_analysis_rule)
         """
```

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/client.pyi` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_cleanrooms.client import CleanRoomsServiceClient
 
     session = Session()
     client: CleanRoomsServiceClient = session.client("cleanrooms")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
@@ -35,14 +35,15 @@
     ListMembershipsPaginator,
     ListMembersPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
 )
 from .type_defs import (
     BatchGetSchemaOutputTypeDef,
+    ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateCollaborationOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     CreateConfiguredTableOutputTypeDef,
     CreateMembershipOutputTypeDef,
     DataEncryptionMetadataTypeDef,
@@ -173,15 +174,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_configured_table)
         """
     def create_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: Union[
+            ConfiguredTableAnalysisRulePolicyTypeDef, ConfiguredTableAnalysisRulePolicyOutputTypeDef
+        ]
     ) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Creates a new analysis rule for a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#create_configured_table_analysis_rule)
         """
@@ -478,15 +481,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#update_configured_table)
         """
     def update_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: Union[
+            ConfiguredTableAnalysisRulePolicyTypeDef, ConfiguredTableAnalysisRulePolicyOutputTypeDef
+        ]
     ) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Updates a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/client/#update_configured_table_analysis_rule)
         """
```

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/literals.py` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/literals.pyi` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/paginator.py` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/paginator.pyi` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/type_defs.py` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/type_defs.pyi` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/PKG-INFO` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.28.15
-Summary: Type annotations for boto3.CleanRoomsService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CleanRoomsService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/SOURCES.txt` & `mypy-boto3-cleanrooms-1.28.15.post1/mypy_boto3_cleanrooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.15/setup.py` & `mypy-boto3-cleanrooms-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cleanrooms",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_cleanrooms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CleanRoomsService 1.28.15 service generated with"
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

