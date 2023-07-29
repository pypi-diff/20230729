# Comparing `tmp/wicked_expressions-0.8.1.tar.gz` & `tmp/wicked_expressions-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.8.1.tar", max compression
+gzip compressed data, was "wicked_expressions-0.8.2.tar", max compression
```

## Comparing `wicked_expressions-0.8.1.tar` & `wicked_expressions-0.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-07-12 04:48:26.629774 wicked_expressions-0.8.1/LICENSE
--rw-r--r--   0        0        0     2166 2023-07-12 04:48:26.629774 wicked_expressions-0.8.1/README.md
--rw-r--r--   0        0        0     1219 2023-07-12 04:49:47.058801 wicked_expressions-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      321 2023-07-12 04:49:47.042800 wicked_expressions-0.8.1/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      725 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     9084 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0      305 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/config.bolt
--rw-r--r--   0        0        0     1850 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0      402 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/nbtlib.bolt
--rw-r--r--   0        0        0     8436 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/raw_operations.bolt
--rw-r--r--   0        0        0      375 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/rebindable.bolt
--rw-r--r--   0        0        0      596 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/safe_load.bolt
--rw-r--r--   0        0        0     3118 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0     1181 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1460 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     6454 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-07-12 04:48:26.637774 wicked_expressions-0.8.1/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 wicked_expressions-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-29 21:15:09.001132 wicked_expressions-0.8.2/LICENSE
+-rw-r--r--   0        0        0     2166 2023-07-29 21:15:09.001132 wicked_expressions-0.8.2/README.md
+-rw-r--r--   0        0        0     1219 2023-07-29 21:16:42.924840 wicked_expressions-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-07-29 21:16:42.908840 wicked_expressions-0.8.2/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      725 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     9084 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      305 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     1850 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      402 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8436 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0      375 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/rebindable.bolt
+-rw-r--r--   0        0        0      596 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/safe_load.bolt
+-rw-r--r--   0        0        0     3118 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1460 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     6496 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-07-29 21:15:09.009132 wicked_expressions-0.8.2/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 wicked_expressions-0.8.2/PKG-INFO
```

### Comparing `wicked_expressions-0.8.1/LICENSE` & `wicked_expressions-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.1/README.md` & `wicked_expressions-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.1/pyproject.toml` & `wicked_expressions-0.8.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.8.1"
+version = "0.8.2"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
```

### Comparing `wicked_expressions-0.8.1/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.8.2/wicked_expressions/modules/api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.1/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.8.2/wicked_expressions/modules/comparison.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.1/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.8.2/wicked_expressions/modules/internal_api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.1/wicked_expressions/modules/raw_operations.bolt` & `wicked_expressions-0.8.2/wicked_expressions/modules/raw_operations.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.1/wicked_expressions/modules/safe_load.bolt` & `wicked_expressions-0.8.2/wicked_expressions/modules/safe_load.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.1/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.8.2/wicked_expressions/modules/sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.1/wicked_expressions/modules/utils.bolt` & `wicked_expressions-0.8.2/wicked_expressions/modules/utils.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.1/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.8.2/wicked_expressions/modules/var.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.8.1/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.8.2/wicked_expressions/modules/var_sources.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
     def _rebind(self, source, value):
         if not isinstance(value, ExpressionNode):
             value = nbtlib.String(value)
         return super()._rebind(source, value)
 
 class ListSource(VarStorageSource):
-    _default_nbt_type = 'list'
+    _default_nbt_type = 'int'   # has to be 'int', else it bricks itself
     _var_type = 'list'
     _default_slot_value = []
 
 class IntArraySource(VarStorageSource):
     _default_nbt_type = 'int_array'
     _var_type = 'int_array'
     _default_slot_value = nbtlib.IntArray([])
```

### Comparing `wicked_expressions-0.8.1/PKG-INFO` & `wicked_expressions-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.8.1
+Version: 0.8.2
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

