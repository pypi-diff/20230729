# Comparing `tmp/mypy-boto3-mturk-1.28.15.tar.gz` & `tmp/mypy-boto3-mturk-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mturk-1.28.15.tar", last modified: Fri Jul 28 20:43:21 2023, max compression
+gzip compressed data, was "mypy-boto3-mturk-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:44 2023, max compression
```

## Comparing `mypy-boto3-mturk-1.28.15.tar` & `mypy-boto3-mturk-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.389558 mypy-boto3-mturk-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-07-28 20:43:21.385558 mypy-boto3-mturk-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.381558 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33295 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33240 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39176 2023-07-28 20:32:14.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39118 2023-07-28 20:32:14.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.385558 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:21.389558 mypy-boto3-mturk-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.877303 mypy-boto3-mturk-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-07-29 10:03:44.877303 mypy-boto3-mturk-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.877303 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33641 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33586 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-29 09:51:52.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39312 2023-07-29 09:51:55.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39254 2023-07-29 09:51:52.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.877303 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:44.000000 mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:44.877303 mypy-boto3-mturk-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:51:51.000000 mypy-boto3-mturk-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-mturk-1.28.15/LICENSE` & `mypy-boto3-mturk-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15/PKG-INFO` & `mypy-boto3-mturk-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mturk
-Version: 1.28.15
-Summary: Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mturk-1.28.15/README.md` & `mypy-boto3-mturk-1.28.15.post1/README.md`

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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__init__.py` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__init__.pyi` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__main__.py` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MTurk 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.MTurk 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk\nOther"
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

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/client.py` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,17 @@
     ListQualificationTypesResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersResponseTypeDef,
+    QualificationRequirementOutputTypeDef,
     QualificationRequirementTypeDef,
+    ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     UpdateQualificationTypeResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -180,18 +182,20 @@
         Title: str,
         Description: str,
         MaxAssignments: int = ...,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...,
+        QualificationRequirements: Sequence[
+            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
+        ] = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyTypeDef = ...,
+        AssignmentReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
+        HITReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITResponseTypeDef:
         """
         The `CreateHIT` operation creates a new Human Intelligence Task (HIT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit)
@@ -203,15 +207,17 @@
         *,
         AssignmentDurationInSeconds: int,
         Reward: str,
         Title: str,
         Description: str,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...
+        QualificationRequirements: Sequence[
+            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
+        ] = ...
     ) -> CreateHITTypeResponseTypeDef:
         """
         The `CreateHITType` operation creates a new HIT type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#create_hit_type)
         """
@@ -221,16 +227,16 @@
         *,
         HITTypeId: str,
         LifetimeInSeconds: int,
         MaxAssignments: int = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyTypeDef = ...,
+        AssignmentReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
+        HITReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITWithHITTypeResponseTypeDef:
         """
         The `CreateHITWithHITType` operation creates a new Human Intelligence Task (HIT)
         using an existing HITTypeID generated by the `CreateHITType` operation.
```

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/client.pyi` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,17 @@
     ListQualificationTypesResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersResponseTypeDef,
+    QualificationRequirementOutputTypeDef,
     QualificationRequirementTypeDef,
+    ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     UpdateQualificationTypeResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -169,18 +171,20 @@
         Title: str,
         Description: str,
         MaxAssignments: int = ...,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...,
+        QualificationRequirements: Sequence[
+            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
+        ] = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyTypeDef = ...,
+        AssignmentReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
+        HITReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITResponseTypeDef:
         """
         The `CreateHIT` operation creates a new Human Intelligence Task (HIT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit)
@@ -191,15 +195,17 @@
         *,
         AssignmentDurationInSeconds: int,
         Reward: str,
         Title: str,
         Description: str,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...
+        QualificationRequirements: Sequence[
+            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
+        ] = ...
     ) -> CreateHITTypeResponseTypeDef:
         """
         The `CreateHITType` operation creates a new HIT type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/client/#create_hit_type)
         """
@@ -208,16 +214,16 @@
         *,
         HITTypeId: str,
         LifetimeInSeconds: int,
         MaxAssignments: int = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyTypeDef = ...,
+        AssignmentReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
+        HITReviewPolicy: Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef] = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITWithHITTypeResponseTypeDef:
         """
         The `CreateHITWithHITType` operation creates a new Human Intelligence Task (HIT)
         using an existing HITTypeID generated by the `CreateHITType` operation.
```

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/literals.py` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/literals.pyi` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/paginator.py` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/paginator.pyi` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/type_defs.py` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1251,15 +1251,17 @@
     },
 )
 _OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateHITTypeRequestRequestTypeDef",
     {
         "AutoApprovalDelayInSeconds": int,
         "Keywords": str,
-        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+        "QualificationRequirements": Sequence[
+            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class CreateHITTypeRequestRequestTypeDef(
     _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
@@ -1415,15 +1417,17 @@
     "_OptionalCreateHITRequestRequestTypeDef",
     {
         "MaxAssignments": int,
         "AutoApprovalDelayInSeconds": int,
         "Keywords": str,
         "Question": str,
         "RequesterAnnotation": str,
-        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+        "QualificationRequirements": Sequence[
+            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
+        ],
         "UniqueRequestToken": str,
         "AssignmentReviewPolicy": ReviewPolicyTypeDef,
         "HITReviewPolicy": ReviewPolicyTypeDef,
         "HITLayoutId": str,
         "HITLayoutParameters": Sequence[HITLayoutParameterTypeDef],
     },
     total=False,
```

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/type_defs.pyi` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1202,15 +1202,17 @@
     },
 )
 _OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateHITTypeRequestRequestTypeDef",
     {
         "AutoApprovalDelayInSeconds": int,
         "Keywords": str,
-        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+        "QualificationRequirements": Sequence[
+            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 class CreateHITTypeRequestRequestTypeDef(
     _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
 ):
@@ -1360,15 +1362,17 @@
     "_OptionalCreateHITRequestRequestTypeDef",
     {
         "MaxAssignments": int,
         "AutoApprovalDelayInSeconds": int,
         "Keywords": str,
         "Question": str,
         "RequesterAnnotation": str,
-        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+        "QualificationRequirements": Sequence[
+            Union[QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef]
+        ],
         "UniqueRequestToken": str,
         "AssignmentReviewPolicy": ReviewPolicyTypeDef,
         "HITReviewPolicy": ReviewPolicyTypeDef,
         "HITLayoutId": str,
         "HITLayoutParameters": Sequence[HITLayoutParameterTypeDef],
     },
     total=False,
```

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/PKG-INFO` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mturk
-Version: 1.28.15
-Summary: Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/SOURCES.txt` & `mypy-boto3-mturk-1.28.15.post1/mypy_boto3_mturk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.15/setup.py` & `mypy-boto3-mturk-1.28.15.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mturk",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_mturk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

