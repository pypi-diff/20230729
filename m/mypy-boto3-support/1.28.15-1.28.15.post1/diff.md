# Comparing `tmp/mypy-boto3-support-1.28.15.tar.gz` & `tmp/mypy-boto3-support-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-support-1.28.15.tar", last modified: Fri Jul 28 20:43:51 2023, max compression
+gzip compressed data, was "mypy-boto3-support-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:19 2023, max compression
```

## Comparing `mypy-boto3-support-1.28.15.tar` & `mypy-boto3-support-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:51.909976 mypy-boto3-support-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-07-28 20:43:51.905976 mypy-boto3-support-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:51.889976 mypy-boto3-support-1.28.15/mypy_boto3_support/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14850 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-28 20:40:24.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-07-28 20:40:24.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-07-28 20:40:24.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/mypy_boto3_support/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:51.905976 mypy-boto3-support-1.28.15/mypy_boto3_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-07-28 20:43:51.000000 mypy-boto3-support-1.28.15/mypy_boto3_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:43:51.000000 mypy-boto3-support-1.28.15/mypy_boto3_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:51.000000 mypy-boto3-support-1.28.15/mypy_boto3_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:51.000000 mypy-boto3-support-1.28.15/mypy_boto3_support.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:51.000000 mypy-boto3-support-1.28.15/mypy_boto3_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:43:51.000000 mypy-boto3-support-1.28.15/mypy_boto3_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:51.909976 mypy-boto3-support-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:40:23.000000 mypy-boto3-support-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.565433 mypy-boto3-support-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-07-29 10:04:19.561433 mypy-boto3-support-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.557433 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-29 10:00:36.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-07-29 10:00:36.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-07-29 10:00:36.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:19.561433 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:04:19.000000 mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:19.565433 mypy-boto3-support-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 10:00:35.000000 mypy-boto3-support-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-support-1.28.15/LICENSE` & `mypy-boto3-support-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15/PKG-INFO` & `mypy-boto3-support-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.28.15
-Summary: Type annotations for boto3.Support 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Support 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,19 +321,19 @@
 ### Typed dictionaries
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
+    AttachmentOutputTypeDef,
     AttachmentTypeDef,
     ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
     AttachmentDetailsTypeDef,
-    AttachmentOutputTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
@@ -355,17 +355,17 @@
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
     AddAttachmentsToSetRequestRequestTypeDef,
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
     CreateCaseResponseTypeDef,
+    DescribeAttachmentResponseTypeDef,
     ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
-    DescribeAttachmentResponseTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
     DescribeCasesRequestDescribeCasesPaginateTypeDef,
     DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
@@ -381,15 +381,15 @@
     CaseDetailsTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentTypeDef:
+def get_structure() -> AttachmentOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-support-1.28.15/README.md` & `mypy-boto3-support-1.28.15.post1/README.md`

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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,19 +289,19 @@
 ### Typed dictionaries
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
+    AttachmentOutputTypeDef,
     AttachmentTypeDef,
     ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
     AttachmentDetailsTypeDef,
-    AttachmentOutputTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
@@ -323,17 +323,17 @@
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
     AddAttachmentsToSetRequestRequestTypeDef,
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
     CreateCaseResponseTypeDef,
+    DescribeAttachmentResponseTypeDef,
     ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
-    DescribeAttachmentResponseTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
     DescribeCasesRequestDescribeCasesPaginateTypeDef,
     DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
@@ -349,15 +349,15 @@
     CaseDetailsTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentTypeDef:
+def get_structure() -> AttachmentOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/__init__.py` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/__init__.pyi` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/__main__.py` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Support 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Support 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\nOther"
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

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/client.py` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,23 @@
     from mypy_boto3_support.client import SupportClient
 
     session = Session()
     client: SupportClient = session.client("support")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 from .type_defs import (
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
+    AttachmentOutputTypeDef,
     AttachmentTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
@@ -84,15 +85,18 @@
         SupportClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#exceptions)
         """
 
     def add_attachments_to_set(
-        self, *, attachments: Sequence[AttachmentTypeDef], attachmentSetId: str = ...
+        self,
+        *,
+        attachments: Sequence[Union[AttachmentTypeDef, AttachmentOutputTypeDef]],
+        attachmentSetId: str = ...
     ) -> AddAttachmentsToSetResponseTypeDef:
         """
         Adds one or more attachments to an attachment set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#add_attachments_to_set)
         """
```

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/client.pyi` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,23 @@
     from mypy_boto3_support.client import SupportClient
 
     session = Session()
     client: SupportClient = session.client("support")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 from .type_defs import (
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
+    AttachmentOutputTypeDef,
     AttachmentTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
@@ -79,15 +80,18 @@
         """
         SupportClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#exceptions)
         """
     def add_attachments_to_set(
-        self, *, attachments: Sequence[AttachmentTypeDef], attachmentSetId: str = ...
+        self,
+        *,
+        attachments: Sequence[Union[AttachmentTypeDef, AttachmentOutputTypeDef]],
+        attachmentSetId: str = ...
     ) -> AddAttachmentsToSetResponseTypeDef:
         """
         Adds one or more attachments to an attachment set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/client/#add_attachments_to_set)
         """
```

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/literals.py` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/literals.pyi` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/paginator.py` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/paginator.pyi` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/type_defs.py` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 Type annotations for support service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_support.type_defs import AttachmentTypeDef
+    from mypy_boto3_support.type_defs import AttachmentOutputTypeDef
 
-    data: AttachmentTypeDef = {...}
+    data: AttachmentOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AttachmentOutputTypeDef",
     "AttachmentTypeDef",
     "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
     "AttachmentDetailsTypeDef",
-    "AttachmentOutputTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeCasesRequestRequestTypeDef",
@@ -53,17 +53,17 @@
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
     "AddAttachmentsToSetRequestRequestTypeDef",
     "AddAttachmentsToSetResponseTypeDef",
     "AddCommunicationToCaseResponseTypeDef",
     "CreateCaseResponseTypeDef",
+    "DescribeAttachmentResponseTypeDef",
     "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
-    "DescribeAttachmentResponseTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
     "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
@@ -78,14 +78,23 @@
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
 )
 
+AttachmentOutputTypeDef = TypedDict(
+    "AttachmentOutputTypeDef",
+    {
+        "fileName": str,
+        "data": bytes,
+    },
+    total=False,
+)
+
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "fileName": str,
         "data": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
@@ -131,23 +140,14 @@
     {
         "attachmentId": str,
         "fileName": str,
     },
     total=False,
 )
 
-AttachmentOutputTypeDef = TypedDict(
-    "AttachmentOutputTypeDef",
-    {
-        "fileName": str,
-        "data": bytes,
-    },
-    total=False,
-)
-
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
         "code": str,
         "name": str,
     },
     total=False,
@@ -431,15 +431,15 @@
         "resourcesSuppressed": int,
     },
 )
 
 _RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
     "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
     {
-        "attachments": Sequence[AttachmentTypeDef],
+        "attachments": Sequence[Union[AttachmentTypeDef, AttachmentOutputTypeDef]],
     },
 )
 _OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
     "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
     {
         "attachmentSetId": str,
     },
@@ -475,14 +475,22 @@
     "CreateCaseResponseTypeDef",
     {
         "caseId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ResolveCaseResponseTypeDef = TypedDict(
     "ResolveCaseResponseTypeDef",
     {
         "initialCaseStatus": str,
         "finalCaseStatus": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -496,22 +504,14 @@
         "submittedBy": str,
         "timeCreated": str,
         "attachmentSet": List[AttachmentDetailsTypeDef],
     },
     total=False,
 )
 
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
-    {
-        "attachment": AttachmentOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "code": str,
         "name": str,
         "categories": List[CategoryTypeDef],
     },
```

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support/type_defs.pyi` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 Type annotations for support service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_support.type_defs import AttachmentTypeDef
+    from mypy_boto3_support.type_defs import AttachmentOutputTypeDef
 
-    data: AttachmentTypeDef = {...}
+    data: AttachmentOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AttachmentOutputTypeDef",
     "AttachmentTypeDef",
     "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
     "AttachmentDetailsTypeDef",
-    "AttachmentOutputTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeCasesRequestRequestTypeDef",
@@ -52,17 +52,17 @@
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
     "AddAttachmentsToSetRequestRequestTypeDef",
     "AddAttachmentsToSetResponseTypeDef",
     "AddCommunicationToCaseResponseTypeDef",
     "CreateCaseResponseTypeDef",
+    "DescribeAttachmentResponseTypeDef",
     "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
-    "DescribeAttachmentResponseTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
     "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
@@ -77,14 +77,23 @@
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
 )
 
+AttachmentOutputTypeDef = TypedDict(
+    "AttachmentOutputTypeDef",
+    {
+        "fileName": str,
+        "data": bytes,
+    },
+    total=False,
+)
+
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "fileName": str,
         "data": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
@@ -128,23 +137,14 @@
     {
         "attachmentId": str,
         "fileName": str,
     },
     total=False,
 )
 
-AttachmentOutputTypeDef = TypedDict(
-    "AttachmentOutputTypeDef",
-    {
-        "fileName": str,
-        "data": bytes,
-    },
-    total=False,
-)
-
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
         "code": str,
         "name": str,
     },
     total=False,
@@ -420,15 +420,15 @@
         "resourcesSuppressed": int,
     },
 )
 
 _RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
     "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
     {
-        "attachments": Sequence[AttachmentTypeDef],
+        "attachments": Sequence[Union[AttachmentTypeDef, AttachmentOutputTypeDef]],
     },
 )
 _OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
     "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
     {
         "attachmentSetId": str,
     },
@@ -462,14 +462,22 @@
     "CreateCaseResponseTypeDef",
     {
         "caseId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ResolveCaseResponseTypeDef = TypedDict(
     "ResolveCaseResponseTypeDef",
     {
         "initialCaseStatus": str,
         "finalCaseStatus": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -483,22 +491,14 @@
         "submittedBy": str,
         "timeCreated": str,
         "attachmentSet": List[AttachmentDetailsTypeDef],
     },
     total=False,
 )
 
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
-    {
-        "attachment": AttachmentOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "code": str,
         "name": str,
         "categories": List[CategoryTypeDef],
     },
```

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support.egg-info/PKG-INFO` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.28.15
-Summary: Type annotations for boto3.Support 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Support 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,19 +321,19 @@
 ### Typed dictionaries
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
+    AttachmentOutputTypeDef,
     AttachmentTypeDef,
     ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
     AttachmentDetailsTypeDef,
-    AttachmentOutputTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
@@ -355,17 +355,17 @@
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
     AddAttachmentsToSetRequestRequestTypeDef,
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
     CreateCaseResponseTypeDef,
+    DescribeAttachmentResponseTypeDef,
     ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
-    DescribeAttachmentResponseTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
     DescribeCasesRequestDescribeCasesPaginateTypeDef,
     DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
@@ -381,15 +381,15 @@
     CaseDetailsTypeDef,
     DescribeTrustedAdvisorCheckResultResponseTypeDef,
     DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
     DescribeCasesResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentTypeDef:
+def get_structure() -> AttachmentOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-support-1.28.15/mypy_boto3_support.egg-info/SOURCES.txt` & `mypy-boto3-support-1.28.15.post1/mypy_boto3_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.15/setup.py` & `mypy-boto3-support-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-support",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_support"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Support 1.28.15 service generated with mypy-boto3-builder"
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

