# Comparing `tmp/autopack_tools-0.4.4.tar.gz` & `tmp/autopack_tools-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.4.4.tar", max compression
+gzip compressed data, was "autopack_tools-0.4.5.tar", max compression
```

## Comparing `autopack_tools-0.4.4.tar` & `autopack_tools-0.4.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.4/LICENSE
--rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.4/README.md
--rw-r--r--   0        0        0        6 2023-07-27 22:24:02.938972 autopack_tools-0.4.4/autopack/VERSION
--rw-r--r--   0        0        0       51 2023-07-27 22:24:02.910492 autopack_tools-0.4.4/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-07-27 22:24:02.910843 autopack_tools-0.4.4/autopack/__main__.py
--rw-r--r--   0        0        0     2824 2023-07-27 22:27:08.593199 autopack_tools-0.4.4/autopack/api.py
--rw-r--r--   0        0        0     1091 2023-07-27 22:24:02.924162 autopack_tools-0.4.4/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-07-27 22:24:02.924415 autopack_tools-0.4.4/autopack/errors.py
--rw-r--r--   0        0        0        0 2023-07-27 22:24:02.929186 autopack_tools-0.4.4/autopack/filesystem_emulation/__init__.py
--rw-r--r--   0        0        0      950 2023-07-27 22:24:02.935685 autopack_tools-0.4.4/autopack/filesystem_emulation/file_manager.py
--rw-r--r--   0        0        0     3562 2023-07-27 22:24:02.927211 autopack_tools-0.4.4/autopack/filesystem_emulation/filesystem_file_manager.py
--rw-r--r--   0        0        0     2985 2023-07-27 22:24:02.928880 autopack_tools-0.4.4/autopack/filesystem_emulation/ram_file_manager.py
--rw-r--r--   0        0        0     4052 2023-07-27 22:24:02.934181 autopack_tools-0.4.4/autopack/filesystem_emulation/workspace_file_manager.py
--rw-r--r--   0        0        0     3199 2023-07-27 22:24:02.936287 autopack_tools-0.4.4/autopack/get_pack.py
--rw-r--r--   0        0        0     4063 2023-07-27 22:24:02.936559 autopack_tools-0.4.4/autopack/installation.py
--rw-r--r--   0        0        0      746 2023-07-27 22:24:02.936811 autopack_tools-0.4.4/autopack/langchain_wrapper.py
--rw-r--r--   0        0        0     5529 2023-07-27 22:24:02.937091 autopack_tools-0.4.4/autopack/pack.py
--rw-r--r--   0        0        0     3309 2023-07-27 22:26:44.374185 autopack_tools-0.4.4/autopack/pack_config.py
--rw-r--r--   0        0        0      502 2023-07-27 22:24:02.937629 autopack_tools-0.4.4/autopack/pack_response.py
--rw-r--r--   0        0        0     2217 2023-07-27 22:24:02.937878 autopack_tools-0.4.4/autopack/prompts.py
--rw-r--r--   0        0        0      394 2023-07-27 22:24:02.938125 autopack_tools-0.4.4/autopack/search.py
--rw-r--r--   0        0        0     4930 2023-07-27 22:24:02.938390 autopack_tools-0.4.4/autopack/selection.py
--rw-r--r--   0        0        0     8049 2023-07-28 20:01:33.520893 autopack_tools-0.4.4/autopack/utils.py
--rw-r--r--   0        0        0     1101 2023-07-28 20:01:33.521215 autopack_tools-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.5/LICENSE
+-rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.5/README.md
+-rw-r--r--   0        0        0        6 2023-07-27 22:24:02.938972 autopack_tools-0.4.5/autopack/VERSION
+-rw-r--r--   0        0        0       51 2023-07-27 22:24:02.910492 autopack_tools-0.4.5/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-07-27 22:24:02.910843 autopack_tools-0.4.5/autopack/__main__.py
+-rw-r--r--   0        0        0     2824 2023-07-27 22:27:08.593199 autopack_tools-0.4.5/autopack/api.py
+-rw-r--r--   0        0        0     1078 2023-07-29 02:31:38.503800 autopack_tools-0.4.5/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-07-27 22:24:02.924415 autopack_tools-0.4.5/autopack/errors.py
+-rw-r--r--   0        0        0        0 2023-07-27 22:24:02.929186 autopack_tools-0.4.5/autopack/filesystem_emulation/__init__.py
+-rw-r--r--   0        0        0      950 2023-07-27 22:24:02.935685 autopack_tools-0.4.5/autopack/filesystem_emulation/file_manager.py
+-rw-r--r--   0        0        0     3562 2023-07-27 22:24:02.927211 autopack_tools-0.4.5/autopack/filesystem_emulation/filesystem_file_manager.py
+-rw-r--r--   0        0        0     2985 2023-07-27 22:24:02.928880 autopack_tools-0.4.5/autopack/filesystem_emulation/ram_file_manager.py
+-rw-r--r--   0        0        0     4052 2023-07-27 22:24:02.934181 autopack_tools-0.4.5/autopack/filesystem_emulation/workspace_file_manager.py
+-rw-r--r--   0        0        0     3199 2023-07-27 22:24:02.936287 autopack_tools-0.4.5/autopack/get_pack.py
+-rw-r--r--   0        0        0     4063 2023-07-27 22:24:02.936559 autopack_tools-0.4.5/autopack/installation.py
+-rw-r--r--   0        0        0      746 2023-07-27 22:24:02.936811 autopack_tools-0.4.5/autopack/langchain_wrapper.py
+-rw-r--r--   0        0        0     5529 2023-07-27 22:24:02.937091 autopack_tools-0.4.5/autopack/pack.py
+-rw-r--r--   0        0        0     3309 2023-07-27 22:26:44.374185 autopack_tools-0.4.5/autopack/pack_config.py
+-rw-r--r--   0        0        0      502 2023-07-27 22:24:02.937629 autopack_tools-0.4.5/autopack/pack_response.py
+-rw-r--r--   0        0        0     2217 2023-07-27 22:24:02.937878 autopack_tools-0.4.5/autopack/prompts.py
+-rw-r--r--   0        0        0      394 2023-07-27 22:24:02.938125 autopack_tools-0.4.5/autopack/search.py
+-rw-r--r--   0        0        0     4930 2023-07-27 22:24:02.938390 autopack_tools-0.4.5/autopack/selection.py
+-rw-r--r--   0        0        0     8049 2023-07-28 20:01:33.520893 autopack_tools-0.4.5/autopack/utils.py
+-rw-r--r--   0        0        0     1101 2023-07-29 04:38:49.091229 autopack_tools-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.5/PKG-INFO
```

### Comparing `autopack_tools-0.4.4/LICENSE` & `autopack_tools-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/README.md` & `autopack_tools-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/api.py` & `autopack_tools-0.4.5/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/cli.py` & `autopack_tools-0.4.5/autopack/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
 
     if args.command == "install":
-        result = install_pack(args.pack, args.force, quiet=False)
+        result = install_pack(args.pack, args.force)
         if result:
             print("Installation completed")
         else:
             print("Installation failed")
 
     if args.command == "search":
         print_search(args.query)
```

### Comparing `autopack_tools-0.4.4/autopack/filesystem_emulation/file_manager.py` & `autopack_tools-0.4.5/autopack/filesystem_emulation/file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/filesystem_emulation/filesystem_file_manager.py` & `autopack_tools-0.4.5/autopack/filesystem_emulation/filesystem_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/filesystem_emulation/ram_file_manager.py` & `autopack_tools-0.4.5/autopack/filesystem_emulation/ram_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/filesystem_emulation/workspace_file_manager.py` & `autopack_tools-0.4.5/autopack/filesystem_emulation/workspace_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/get_pack.py` & `autopack_tools-0.4.5/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/installation.py` & `autopack_tools-0.4.5/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/langchain_wrapper.py` & `autopack_tools-0.4.5/autopack/langchain_wrapper.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/pack.py` & `autopack_tools-0.4.5/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/pack_config.py` & `autopack_tools-0.4.5/autopack/pack_config.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/prompts.py` & `autopack_tools-0.4.5/autopack/prompts.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/selection.py` & `autopack_tools-0.4.5/autopack/selection.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/autopack/utils.py` & `autopack_tools-0.4.5/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.4/pyproject.toml` & `autopack_tools-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.4.4"
+version = "0.4.5"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.4.4/PKG-INFO` & `autopack_tools-0.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.4.4
+Version: 0.4.5
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

