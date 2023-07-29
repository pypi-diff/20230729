# Comparing `tmp/mypy-boto3-waf-regional-1.28.15.tar.gz` & `tmp/mypy-boto3-waf-regional-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-waf-regional-1.28.15.tar", last modified: Fri Jul 28 20:43:55 2023, max compression
+gzip compressed data, was "mypy-boto3-waf-regional-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:25 2023, max compression
```

## Comparing `mypy-boto3-waf-regional-1.28.15.tar` & `mypy-boto3-waf-regional-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.638027 mypy-boto3-waf-regional-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-07-28 20:43:55.634027 mypy-boto3-waf-regional-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.630027 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57158 2023-07-28 20:41:10.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57107 2023-07-28 20:41:09.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.634027 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:55.638027 mypy-boto3-waf-regional-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.273455 mypy-boto3-waf-regional-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20545 2023-07-29 10:04:25.269455 mypy-boto3-waf-regional-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.261455 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46413 2023-07-29 10:01:21.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46325 2023-07-29 10:01:20.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-29 10:01:21.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-29 10:01:21.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57158 2023-07-29 10:01:23.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57107 2023-07-29 10:01:22.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.269455 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20545 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:25.273455 mypy-boto3-waf-regional-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-waf-regional-1.28.15/LICENSE` & `mypy-boto3-waf-regional-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.15/PKG-INFO` & `mypy-boto3-waf-regional-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.28.15
-Summary: Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-waf-regional-1.28.15/README.md` & `mypy-boto3-waf-regional-1.28.15.post1/README.md`

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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/client.py` & `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_waf_regional.client import WAFRegionalClient
 
     session = Session()
     client: WAFRegionalClient = session.client("waf-regional")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ResourceTypeType
 from .type_defs import (
     ByteMatchSetUpdateTypeDef,
     CreateByteMatchSetResponseTypeDef,
@@ -80,23 +80,25 @@
     ListRulesResponseTypeDef,
     ListSizeConstraintSetsResponseTypeDef,
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetUpdateTypeDef,
     RegexPatternSetUpdateTypeDef,
     RuleGroupUpdateTypeDef,
     RuleUpdateTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     TagTypeDef,
+    TimeWindowOutputTypeDef,
     TimeWindowTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
@@ -592,15 +594,20 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#get_rule_group)
         """
 
     def get_sampled_requests(
-        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowTypeDef, MaxItems: int
+        self,
+        *,
+        WebAclId: str,
+        RuleId: str,
+        TimeWindow: Union[TimeWindowTypeDef, TimeWindowOutputTypeDef],
+        MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_sampled_requests)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#get_sampled_requests)
         """
@@ -812,15 +819,17 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_xss_match_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#list_xss_match_sets)
         """
 
     def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
+        self,
+        *,
+        LoggingConfiguration: Union[LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef]
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.put_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#put_logging_configuration)
         """
```

### Comparing `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/client.pyi` & `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_waf_regional.client import WAFRegionalClient
 
     session = Session()
     client: WAFRegionalClient = session.client("waf-regional")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ResourceTypeType
 from .type_defs import (
     ByteMatchSetUpdateTypeDef,
     CreateByteMatchSetResponseTypeDef,
@@ -80,23 +80,25 @@
     ListRulesResponseTypeDef,
     ListSizeConstraintSetsResponseTypeDef,
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetUpdateTypeDef,
     RegexPatternSetUpdateTypeDef,
     RuleGroupUpdateTypeDef,
     RuleUpdateTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     TagTypeDef,
+    TimeWindowOutputTypeDef,
     TimeWindowTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
@@ -542,15 +544,20 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#get_rule_group)
         """
     def get_sampled_requests(
-        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowTypeDef, MaxItems: int
+        self,
+        *,
+        WebAclId: str,
+        RuleId: str,
+        TimeWindow: Union[TimeWindowTypeDef, TimeWindowOutputTypeDef],
+        MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_sampled_requests)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#get_sampled_requests)
         """
@@ -739,15 +746,17 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_xss_match_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#list_xss_match_sets)
         """
     def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
+        self,
+        *,
+        LoggingConfiguration: Union[LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef]
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.put_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#put_logging_configuration)
         """
```

### Comparing `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/literals.py` & `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/literals.pyi` & `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/type_defs.py` & `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/type_defs.pyi` & `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/PKG-INFO` & `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.28.15
-Summary: Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/SOURCES.txt` & `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.15/setup.py` & `mypy-boto3-waf-regional-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-waf-regional",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_waf_regional"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder"
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

