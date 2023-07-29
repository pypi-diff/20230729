# Comparing `tmp/mypy-boto3-cur-1.28.15.tar.gz` & `tmp/mypy-boto3-cur-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cur-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
+gzip compressed data, was "mypy-boto3-cur-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:54 2023, max compression
```

## Comparing `mypy-boto3-cur-1.28.15.tar` & `mypy-boto3-cur-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.884916 mypy-boto3-cur-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-07-28 20:42:34.884916 mypy-boto3-cur-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.880915 mypy-boto3-cur-1.28.15/mypy_boto3_cur/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.884916 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.884916 mypy-boto3-cur-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.085095 mypy-boto3-cur-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-29 10:02:54.085095 mypy-boto3-cur-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.081095 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.085095 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:54.085095 mypy-boto3-cur-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-cur-1.28.15/LICENSE` & `mypy-boto3-cur-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15/PKG-INFO` & `mypy-boto3-cur-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.28.15
-Summary: Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cur-1.28.15/README.md` & `mypy-boto3-cur-1.28.15.post1/README.md`

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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/__init__.py` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/__init__.pyi` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/__main__.py` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.CostandUsageReportService 1.28.15\nVersion:        "
-        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService\nOther"
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

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/client.py` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,23 @@
     from mypy_boto3_cur.client import CostandUsageReportServiceClient
 
     session = Session()
     client: CostandUsageReportServiceClient = session.client("cur")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Type
+from typing import Any, Dict, Mapping, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeReportDefinitionsPaginator
 from .type_defs import (
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
+    ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -114,24 +115,29 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#generate_presigned_url)
         """
 
     def modify_report_definition(
-        self, *, ReportName: str, ReportDefinition: ReportDefinitionTypeDef
+        self,
+        *,
+        ReportName: str,
+        ReportDefinition: Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Allows you to programatically update your report preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.modify_report_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#modify_report_definition)
         """
 
-    def put_report_definition(self, *, ReportDefinition: ReportDefinitionTypeDef) -> Dict[str, Any]:
+    def put_report_definition(
+        self, *, ReportDefinition: Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
+    ) -> Dict[str, Any]:
         """
         Creates a new report using the description that you provide.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.put_report_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#put_report_definition)
         """
```

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/client.pyi` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,23 @@
     from mypy_boto3_cur.client import CostandUsageReportServiceClient
 
     session = Session()
     client: CostandUsageReportServiceClient = session.client("cur")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Type
+from typing import Any, Dict, Mapping, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeReportDefinitionsPaginator
 from .type_defs import (
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
+    ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -104,23 +105,28 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#generate_presigned_url)
         """
     def modify_report_definition(
-        self, *, ReportName: str, ReportDefinition: ReportDefinitionTypeDef
+        self,
+        *,
+        ReportName: str,
+        ReportDefinition: Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Allows you to programatically update your report preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.modify_report_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#modify_report_definition)
         """
-    def put_report_definition(self, *, ReportDefinition: ReportDefinitionTypeDef) -> Dict[str, Any]:
+    def put_report_definition(
+        self, *, ReportDefinition: Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
+    ) -> Dict[str, Any]:
         """
         Creates a new report using the description that you provide.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.put_report_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#put_report_definition)
         """
     def get_paginator(
```

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/literals.py` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/literals.pyi` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/paginator.py` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/paginator.pyi` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/type_defs.py` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur/type_defs.pyi` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/PKG-INFO` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.28.15
-Summary: Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/SOURCES.txt` & `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15/setup.py` & `mypy-boto3-cur-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cur",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_cur"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with"
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

