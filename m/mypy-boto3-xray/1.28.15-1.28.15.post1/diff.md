# Comparing `tmp/mypy-boto3-xray-1.28.15.tar.gz` & `tmp/mypy-boto3-xray-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-xray-1.28.15.tar", last modified: Fri Jul 28 20:43:58 2023, max compression
+gzip compressed data, was "mypy-boto3-xray-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:27 2023, max compression
```

## Comparing `mypy-boto3-xray-1.28.15.tar` & `mypy-boto3-xray-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:58.386065 mypy-boto3-xray-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-07-28 20:43:58.386065 mypy-boto3-xray-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:58.378065 mypy-boto3-xray-1.28.15/mypy_boto3_xray/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25850 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-28 20:41:50.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44015 2023-07-28 20:41:51.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43964 2023-07-28 20:41:50.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:58.386065 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:58.386065 mypy-boto3-xray-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.845465 mypy-boto3-xray-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-29 10:04:27.845465 mypy-boto3-xray-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.845465 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-07-29 10:01:59.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25939 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-29 10:01:59.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-07-29 10:01:59.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-29 10:01:59.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-29 10:01:59.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44015 2023-07-29 10:02:00.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43964 2023-07-29 10:02:00.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:27.845465 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:04:27.000000 mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:27.845465 mypy-boto3-xray-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-29 10:01:58.000000 mypy-boto3-xray-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-xray-1.28.15/LICENSE` & `mypy-boto3-xray-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15/PKG-INFO` & `mypy-boto3-xray-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-xray
-Version: 1.28.15
-Summary: Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-xray-1.28.15/README.md` & `mypy-boto3-xray-1.28.15.post1/README.md`

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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/__init__.py` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/__init__.pyi` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/__main__.py` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.XRay 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.XRay 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay\nOther"
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

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/client.py` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     GetTraceSummariesResultTypeDef,
     InsightsConfigurationTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutEncryptionConfigResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
+    SamplingRuleOutputTypeDef,
     SamplingRuleTypeDef,
     SamplingRuleUpdateTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingStrategyTypeDef,
     TagTypeDef,
     TelemetryRecordTypeDef,
     UpdateGroupResultTypeDef,
@@ -153,15 +154,18 @@
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_group)
         """
 
     def create_sampling_rule(
-        self, *, SamplingRule: SamplingRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        SamplingRule: Union[SamplingRuleTypeDef, SamplingRuleOutputTypeDef],
+        Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSamplingRuleResultTypeDef:
         """
         Creates a rule to control sampling behavior for instrumented applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_sampling_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_sampling_rule)
         """
```

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/client.pyi` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     GetTraceSummariesResultTypeDef,
     InsightsConfigurationTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutEncryptionConfigResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
+    SamplingRuleOutputTypeDef,
     SamplingRuleTypeDef,
     SamplingRuleUpdateTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingStrategyTypeDef,
     TagTypeDef,
     TelemetryRecordTypeDef,
     UpdateGroupResultTypeDef,
@@ -144,15 +145,18 @@
         """
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_group)
         """
     def create_sampling_rule(
-        self, *, SamplingRule: SamplingRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self,
+        *,
+        SamplingRule: Union[SamplingRuleTypeDef, SamplingRuleOutputTypeDef],
+        Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSamplingRuleResultTypeDef:
         """
         Creates a rule to control sampling behavior for instrumented applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_sampling_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/client/#create_sampling_rule)
         """
```

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/literals.py` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/literals.pyi` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/paginator.py` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/paginator.pyi` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/type_defs.py` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray/type_defs.pyi` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/PKG-INFO` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-xray
-Version: 1.28.15
-Summary: Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/SOURCES.txt` & `mypy-boto3-xray-1.28.15.post1/mypy_boto3_xray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.15/setup.py` & `mypy-boto3-xray-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-xray",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_xray"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

