# Comparing `tmp/app_toggles-0.1.1.tar.gz` & `tmp/app_toggles-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_toggles-0.1.1.tar", max compression
+gzip compressed data, was "app_toggles-0.1.2.tar", max compression
```

## Comparing `app_toggles-0.1.1.tar` & `app_toggles-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-07-28 20:42:22.910431 app_toggles-0.1.1/LICENSE
--rw-r--r--   0        0        0     2836 2023-07-28 21:59:51.944691 app_toggles-0.1.1/README.md
--rw-r--r--   0        0        0      160 2023-07-28 18:23:57.836410 app_toggles-0.1.1/app_toggles/__init__.py
--rw-r--r--   0        0        0      242 2023-07-28 18:23:52.819325 app_toggles-0.1.1/app_toggles/_exceptions.py
--rw-r--r--   0        0        0       84 2023-07-28 16:50:02.121909 app_toggles-0.1.1/app_toggles/_toggle_providers/__init__.py
--rw-r--r--   0        0        0      829 2023-07-28 17:46:28.016231 app_toggles-0.1.1/app_toggles/_toggle_providers/json_toggle_provider.py
--rw-r--r--   0        0        0      191 2023-07-28 16:32:11.925889 app_toggles-0.1.1/app_toggles/_toggle_providers/provider.py
--rw-r--r--   0        0        0     1205 2023-07-28 19:54:06.928779 app_toggles-0.1.1/app_toggles/_toggles.py
--rw-r--r--   0        0        0      237 2023-07-28 18:16:55.620977 app_toggles-0.1.1/app_toggles/_types.py
--rw-r--r--   0        0        0      497 2023-07-28 22:04:09.587969 app_toggles-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 app_toggles-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-28 20:42:22.910431 app_toggles-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2836 2023-07-28 21:59:51.944691 app_toggles-0.1.2/README.md
+-rw-r--r--   0        0        0      160 2023-07-28 22:22:12.371329 app_toggles-0.1.2/app_toggles/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-28 18:23:52.819325 app_toggles-0.1.2/app_toggles/_exceptions.py
+-rw-r--r--   0        0        0       84 2023-07-28 22:22:12.375735 app_toggles-0.1.2/app_toggles/_toggle_providers/__init__.py
+-rw-r--r--   0        0        0      913 2023-07-28 23:05:36.227861 app_toggles-0.1.2/app_toggles/_toggle_providers/json_toggle_provider.py
+-rw-r--r--   0        0        0      196 2023-07-28 23:05:51.232015 app_toggles-0.1.2/app_toggles/_toggle_providers/provider.py
+-rw-r--r--   0        0        0     1301 2023-07-28 23:00:02.146742 app_toggles-0.1.2/app_toggles/_toggles.py
+-rw-r--r--   0        0        0      248 2023-07-28 23:06:24.425564 app_toggles-0.1.2/app_toggles/_types.py
+-rw-r--r--   0        0        0      537 2023-07-28 23:10:58.174873 app_toggles-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 app_toggles-0.1.2/PKG-INFO
```

### Comparing `app_toggles-0.1.1/LICENSE` & `app_toggles-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `app_toggles-0.1.1/README.md` & `app_toggles-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `app_toggles-0.1.1/app_toggles/_toggle_providers/json_toggle_provider.py` & `app_toggles-0.1.2/app_toggles/_toggle_providers/json_toggle_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import json
 import typing
 
-from .provider import Provider
 from .._exceptions import ToggleNotFoundError
+from .provider import Provider
 
 
 class JsonToggleProvider(Provider):
     def __init__(self, toggles_file_path: str) -> None:
         self.path = toggles_file_path
 
-    def get_toggles(self, toggle_names: typing.List[str]) -> typing.Tuple[bool]:
+    def get_toggles(self, toggle_names: typing.List[str]) -> typing.Tuple[bool, ...]:
         with open(self.path, "r") as toggles_file:
             toggles = json.load(toggles_file)
 
-            missing_toogles = [toggle for toggle in toggle_names if toggle not in toggles]
+            missing_toogles = [
+                toggle for toggle in toggle_names if toggle not in toggles
+            ]
             if missing_toogles:
-                raise ToggleNotFoundError(f"The follwing toggles where not found: {', '.join(missing_toogles)}")
+                raise ToggleNotFoundError(
+                    f"The follwing toggles where not found: {', '.join(missing_toogles)}"
+                )
 
-            return [
-                toggle_value
+            return tuple(
+                bool(toggle_value)
                 for toggle_name, toggle_value in toggles.items()
                 if toggle_name in toggle_names
-            ]
+            )
```

### Comparing `app_toggles-0.1.1/app_toggles/_toggles.py` & `app_toggles-0.1.2/app_toggles/_toggles.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-from functools import wraps
 import typing
+from functools import wraps
 
+from . import _exceptions, _types
 from ._toggle_providers import Provider
-from . import _types
-from . import _exceptions
 
 
 class Toggles:
     def __init__(self, provider: Provider) -> None:
         self.provider = provider
 
     def toggle_decision(self, decision_function: _types.TOOGLE_DECISION):
         @wraps(decision_function)
-        def _wraps(when_on: _types.TOGGLED_VALUE=None, when_off: _types.TOGGLED_VALUE=None):
+        def _wraps(
+            when_on: _types.TOGGLED_VALUE,
+            when_off: _types.TOGGLED_VALUE,
+        ):
             if str(type(when_on)) != str(type(when_off)):
-                raise _exceptions.InvalidDecisionFunction((
-                    "when_on and when_off parameters must be of the same type. "
-                    f"when_on parameter is {str(type(when_on))} and when_off parameter is {type(when_off)}"
-                ))
+                raise _exceptions.InvalidDecisionFunction(
+                    (
+                        "when_on and when_off parameters must be of the same type. "
+                        f"when_on parameter is {str(type(when_on))} and when_off parameter is {type(when_off)}"
+                    )
+                )
 
             if isinstance(when_on, bool) or isinstance(when_off, bool):
-                raise _exceptions.InvalidDecisionFunction((
-                    "when_on and when_off parameters can't be boolean. "
-                    "We have added this restriction to avoid a lot of is statements in your app"
-                ))
+                raise _exceptions.InvalidDecisionFunction(
+                    (
+                        "when_on and when_off parameters can't be boolean. "
+                        "We have added this restriction to avoid a lot of is statements in your app"
+                    )
+                )
+
+            return decision_function(self.provider.get_toggles, when_on, when_off)
 
-            return decision_function(self.provider.get_toggles, when_on=when_on, when_off=when_off)
         return _wraps
```

### Comparing `app_toggles-0.1.1/PKG-INFO` & `app_toggles-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: app-toggles
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to manage app toggles
 Author: Gustavo Eguez
 Author-email: eguezgustavo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: black (>=23.7.0,<24.0.0)
 Description-Content-Type: text/markdown
 
 # App toggles library
 
 ![CI](https://github.com/eguezgustavo/app_toggles/actions/workflows/cicd.yaml/badge.svg?branch=main)
 
 This library has been created taking into account the work done by [Pete Hodgson](https://thepete.net/) published in [https://martinfowler.com/](https://martinfowler.com/articles/feature-toggles.html).
```

