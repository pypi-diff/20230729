# Comparing `tmp/mypy-boto3-honeycode-1.28.15.tar.gz` & `tmp/mypy-boto3-honeycode-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-honeycode-1.28.15.tar", last modified: Fri Jul 28 20:42:55 2023, max compression
+gzip compressed data, was "mypy-boto3-honeycode-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:15 2023, max compression
```

## Comparing `mypy-boto3-honeycode-1.28.15.tar` & `mypy-boto3-honeycode-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:55.473202 mypy-boto3-honeycode-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-28 20:42:55.469202 mypy-boto3-honeycode-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:55.457202 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-07-28 20:27:22.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-07-28 20:27:22.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:55.469202 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:55.473202 mypy-boto3-honeycode-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:15.981173 mypy-boto3-honeycode-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-29 10:03:15.981173 mypy-boto3-honeycode-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:15.973173 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-07-29 09:46:55.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:54.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:15.981173 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:15.000000 mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:15.981173 mypy-boto3-honeycode-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:46:53.000000 mypy-boto3-honeycode-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-honeycode-1.28.15/LICENSE` & `mypy-boto3-honeycode-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15/PKG-INFO` & `mypy-boto3-honeycode-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-honeycode
-Version: 1.28.15
-Summary: Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-honeycode-1.28.15/README.md` & `mypy-boto3-honeycode-1.28.15.post1/README.md`

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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__init__.py` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__init__.pyi` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__main__.py` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Honeycode 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Honeycode 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode\nOther"
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

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/client.py` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_honeycode.client import HoneycodeClient
 
     session = Session()
     client: HoneycodeClient = session.client("honeycode")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListTableColumnsPaginator,
     ListTableRowsPaginator,
     ListTablesPaginator,
@@ -30,14 +30,15 @@
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     DescribeTableDataImportJobResultTypeDef,
     FilterTypeDef,
     GetScreenDataResultTypeDef,
     ImportDataSourceTypeDef,
+    ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsResultTypeDef,
     ListTableRowsResultTypeDef,
     ListTablesResultTypeDef,
     ListTagsForResourceResultTypeDef,
     QueryTableRowsResultTypeDef,
@@ -297,15 +298,15 @@
     def start_table_data_import_job(
         self,
         *,
         workbookId: str,
         dataSource: ImportDataSourceTypeDef,
         dataFormat: Literal["DELIMITED_TEXT"],
         destinationTableId: str,
-        importOptions: ImportOptionsTypeDef,
+        importOptions: Union[ImportOptionsTypeDef, ImportOptionsOutputTypeDef],
         clientRequestToken: str
     ) -> StartTableDataImportJobResultTypeDef:
         """
         The StartTableDataImportJob API allows you to start an import job on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/client/#start_table_data_import_job)
```

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/client.pyi` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_honeycode.client import HoneycodeClient
 
     session = Session()
     client: HoneycodeClient = session.client("honeycode")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListTableColumnsPaginator,
     ListTableRowsPaginator,
     ListTablesPaginator,
@@ -30,14 +30,15 @@
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     DescribeTableDataImportJobResultTypeDef,
     FilterTypeDef,
     GetScreenDataResultTypeDef,
     ImportDataSourceTypeDef,
+    ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsResultTypeDef,
     ListTableRowsResultTypeDef,
     ListTablesResultTypeDef,
     ListTagsForResourceResultTypeDef,
     QueryTableRowsResultTypeDef,
@@ -277,15 +278,15 @@
     def start_table_data_import_job(
         self,
         *,
         workbookId: str,
         dataSource: ImportDataSourceTypeDef,
         dataFormat: Literal["DELIMITED_TEXT"],
         destinationTableId: str,
-        importOptions: ImportOptionsTypeDef,
+        importOptions: Union[ImportOptionsTypeDef, ImportOptionsOutputTypeDef],
         clientRequestToken: str
     ) -> StartTableDataImportJobResultTypeDef:
         """
         The StartTableDataImportJob API allows you to start an import job on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/client/#start_table_data_import_job)
```

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/literals.py` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/literals.pyi` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/paginator.py` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/paginator.pyi` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/type_defs.py` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/type_defs.pyi` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/PKG-INFO` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-honeycode
-Version: 1.28.15
-Summary: Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/SOURCES.txt` & `mypy-boto3-honeycode-1.28.15.post1/mypy_boto3_honeycode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.15/setup.py` & `mypy-boto3-honeycode-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-honeycode",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_honeycode"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder"
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

