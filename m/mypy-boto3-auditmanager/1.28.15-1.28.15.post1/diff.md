# Comparing `tmp/mypy-boto3-auditmanager-1.28.15.tar.gz` & `tmp/mypy-boto3-auditmanager-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-auditmanager-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
+gzip compressed data, was "mypy-boto3-auditmanager-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
```

## Comparing `mypy-boto3-auditmanager-1.28.15.tar` & `mypy-boto3-auditmanager-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.200695 mypy-boto3-auditmanager-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-07-28 20:42:19.200695 mypy-boto3-auditmanager-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.196694 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43294 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43226 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57940 2023-07-28 20:19:53.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57895 2023-07-28 20:19:53.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.200695 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.200695 mypy-boto3-auditmanager-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:19:50.000000 mypy-boto3-auditmanager-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.469021 mypy-boto3-auditmanager-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-07-29 10:02:34.469021 mypy-boto3-auditmanager-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.465021 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43379 2023-07-29 09:38:43.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43311 2023-07-29 09:38:43.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-07-29 09:38:43.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-29 09:38:43.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57940 2023-07-29 09:38:46.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57895 2023-07-29 09:38:45.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.469021 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:02:34.000000 mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.469021 mypy-boto3-auditmanager-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:38:42.000000 mypy-boto3-auditmanager-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-auditmanager-1.28.15/LICENSE` & `mypy-boto3-auditmanager-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.15/PKG-INFO` & `mypy-boto3-auditmanager-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.28.15
-Summary: Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-auditmanager-1.28.15/README.md` & `mypy-boto3-auditmanager-1.28.15.post1/README.md`

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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/__main__.py` & `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AuditManager 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.AuditManager 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager\nOther"
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

### Comparing `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/client.py` & `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_auditmanager.client import AuditManagerClient
 
     session = Session()
     client: AuditManagerClient = session.client("auditmanager")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssessmentStatusType,
     ControlSetStatusType,
     ControlStatusType,
@@ -76,14 +76,15 @@
     ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManualEvidenceTypeDef,
     RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountResponseTypeDef,
     RoleTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     UpdateAssessmentControlSetStatusResponseTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
@@ -219,15 +220,15 @@
         """
 
     def create_assessment(
         self,
         *,
         name: str,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef,
-        scope: ScopeTypeDef,
+        scope: Union[ScopeTypeDef, ScopeOutputTypeDef],
         roles: Sequence[RoleTypeDef],
         frameworkId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAssessmentResponseTypeDef:
         """
         Creates an assessment in Audit Manager.
@@ -735,15 +736,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#untag_resource)
         """
 
     def update_assessment(
         self,
         *,
         assessmentId: str,
-        scope: ScopeTypeDef,
+        scope: Union[ScopeTypeDef, ScopeOutputTypeDef],
         assessmentName: str = ...,
         assessmentDescription: str = ...,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         roles: Sequence[RoleTypeDef] = ...
     ) -> UpdateAssessmentResponseTypeDef:
         """
         Edits an Audit Manager assessment.
```

### Comparing `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/client.pyi` & `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_auditmanager.client import AuditManagerClient
 
     session = Session()
     client: AuditManagerClient = session.client("auditmanager")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssessmentStatusType,
     ControlSetStatusType,
     ControlStatusType,
@@ -76,14 +76,15 @@
     ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManualEvidenceTypeDef,
     RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountResponseTypeDef,
     RoleTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     UpdateAssessmentControlSetStatusResponseTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
@@ -207,15 +208,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#close)
         """
     def create_assessment(
         self,
         *,
         name: str,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef,
-        scope: ScopeTypeDef,
+        scope: Union[ScopeTypeDef, ScopeOutputTypeDef],
         roles: Sequence[RoleTypeDef],
         frameworkId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAssessmentResponseTypeDef:
         """
         Creates an assessment in Audit Manager.
@@ -675,15 +676,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#untag_resource)
         """
     def update_assessment(
         self,
         *,
         assessmentId: str,
-        scope: ScopeTypeDef,
+        scope: Union[ScopeTypeDef, ScopeOutputTypeDef],
         assessmentName: str = ...,
         assessmentDescription: str = ...,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         roles: Sequence[RoleTypeDef] = ...
     ) -> UpdateAssessmentResponseTypeDef:
         """
         Edits an Audit Manager assessment.
```

### Comparing `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/literals.py` & `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/literals.pyi` & `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/type_defs.py` & `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/type_defs.pyi` & `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/PKG-INFO` & `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.28.15
-Summary: Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/SOURCES.txt` & `mypy-boto3-auditmanager-1.28.15.post1/mypy_boto3_auditmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.15/setup.py` & `mypy-boto3-auditmanager-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-auditmanager",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_auditmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder"
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

