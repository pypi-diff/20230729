# Comparing `tmp/mentat-ai-0.1.3.tar.gz` & `tmp/mentat-ai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentat-ai-0.1.3.tar", last modified: Thu Jul 27 13:53:07 2023, max compression
+gzip compressed data, was "mentat-ai-0.1.4.tar", last modified: Fri Jul 28 23:49:48 2023, max compression
```

## Comparing `mentat-ai-0.1.3.tar` & `mentat-ai-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.749173 mentat-ai-0.1.3/
--rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.3/LICENSE
--rw-r--r--   0 biobootloader   (501) staff       (20)       75 2023-07-27 13:53:07.749057 mentat-ai-0.1.3/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)     2961 2023-07-27 13:51:20.000000 mentat-ai-0.1.3/README.md
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.745394 mentat-ai-0.1.3/mentat/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.3/mentat/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      166 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/mentat/__main__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     6025 2023-07-27 13:51:20.000000 mentat-ai-0.1.3/mentat/app.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/change_conflict_resolution.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/code_change.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/code_change_display.py
--rw-r--r--   0 biobootloader   (501) staff       (20)    13189 2023-07-27 13:51:20.000000 mentat-ai-0.1.3/mentat/code_file_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1536 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/mentat/config_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2340 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/conversation.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      325 2023-07-25 13:34:36.000000 mentat-ai-0.1.3/mentat/default_config.json
--rw-r--r--   0 biobootloader   (501) staff       (20)     3798 2023-07-25 13:33:37.000000 mentat-ai-0.1.3/mentat/llm_api.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/logging_config.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/parsing.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.3/mentat/prompts.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/mentat/streaming_printer.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/mentat/user_input_manager.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.746084 mentat-ai-0.1.3/mentat_ai.egg-info/
--rw-r--r--   0 biobootloader   (501) staff       (20)       75 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)      997 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/SOURCES.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/dependency_links.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/entry_points.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)      765 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/requires.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/top_level.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/pyproject.toml
--rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-27 13:53:07.749204 mentat-ai-0.1.3/setup.cfg
--rw-r--r--   0 biobootloader   (501) staff       (20)      463 2023-07-27 13:52:38.000000 mentat-ai-0.1.3/setup.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.746187 mentat-ai-0.1.3/testbed/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.3/testbed/__init__.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.746772 mentat-ai-0.1.3/testbed/multifile_calculator/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.3/testbed/multifile_calculator/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.3/testbed/multifile_calculator/calculator.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.3/testbed/multifile_calculator/operations.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.748889 mentat-ai-0.1.3/tests/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.3/tests/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/tests/benchmark_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2700 2023-07-27 13:51:20.000000 mentat-ai-0.1.3/tests/code_file_manager_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     7507 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/tests/codechange_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      148 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/tests/config_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3689 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/tests/conftest.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.3/tests/measure_api_speed.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.3/tests/record_benchmark.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/tests/system_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/tests/ui_test.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-28 23:49:48.837306 mentat-ai-0.1.4/
+-rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.4/LICENSE
+-rw-r--r--   0 biobootloader   (501) staff       (20)       99 2023-07-28 23:49:48.837203 mentat-ai-0.1.4/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2997 2023-07-28 22:38:12.000000 mentat-ai-0.1.4/README.md
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-28 23:49:48.833923 mentat-ai-0.1.4/mentat/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.4/mentat/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      342 2023-07-28 22:38:12.000000 mentat-ai-0.1.4/mentat/__main__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     6025 2023-07-28 22:38:06.000000 mentat-ai-0.1.4/mentat/app.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.4/mentat/change_conflict_resolution.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.4/mentat/code_change.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.4/mentat/code_change_display.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)    14002 2023-07-28 23:48:43.000000 mentat-ai-0.1.4/mentat/code_file_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1645 2023-07-28 23:48:43.000000 mentat-ai-0.1.4/mentat/config_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1728 2023-07-28 22:38:12.000000 mentat-ai-0.1.4/mentat/conversation.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      359 2023-07-28 23:48:43.000000 mentat-ai-0.1.4/mentat/default_config.json
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4821 2023-07-28 22:38:12.000000 mentat-ai-0.1.4/mentat/llm_api.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.4/mentat/logging_config.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-27 16:52:26.000000 mentat-ai-0.1.4/mentat/parsing.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.4/mentat/prompts.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.4/mentat/streaming_printer.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.4/mentat/user_input_manager.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-28 23:49:48.834546 mentat-ai-0.1.4/mentat_ai.egg-info/
+-rw-r--r--   0 biobootloader   (501) staff       (20)       99 2023-07-28 23:49:48.000000 mentat-ai-0.1.4/mentat_ai.egg-info/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)      997 2023-07-28 23:49:48.000000 mentat-ai-0.1.4/mentat_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-28 23:49:48.000000 mentat-ai-0.1.4/mentat_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-28 23:49:48.000000 mentat-ai-0.1.4/mentat_ai.egg-info/entry_points.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)      765 2023-07-28 23:49:48.000000 mentat-ai-0.1.4/mentat_ai.egg-info/requires.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-28 23:49:48.000000 mentat-ai-0.1.4/mentat_ai.egg-info/top_level.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.4/pyproject.toml
+-rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-28 23:49:48.837334 mentat-ai-0.1.4/setup.cfg
+-rw-r--r--   0 biobootloader   (501) staff       (20)      493 2023-07-28 23:48:43.000000 mentat-ai-0.1.4/setup.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-28 23:49:48.834644 mentat-ai-0.1.4/testbed/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.4/testbed/__init__.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-28 23:49:48.835178 mentat-ai-0.1.4/testbed/multifile_calculator/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.4/testbed/multifile_calculator/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.4/testbed/multifile_calculator/calculator.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.4/testbed/multifile_calculator/operations.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-28 23:49:48.837061 mentat-ai-0.1.4/tests/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.4/tests/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.4/tests/benchmark_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3872 2023-07-28 23:48:43.000000 mentat-ai-0.1.4/tests/code_file_manager_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7507 2023-07-27 16:52:26.000000 mentat-ai-0.1.4/tests/codechange_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      146 2023-07-28 22:38:12.000000 mentat-ai-0.1.4/tests/config_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3805 2023-07-28 22:38:12.000000 mentat-ai-0.1.4/tests/conftest.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.4/tests/measure_api_speed.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.4/tests/record_benchmark.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-27 16:52:26.000000 mentat-ai-0.1.4/tests/system_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.4/tests/ui_test.py
```

### Comparing `mentat-ai-0.1.3/LICENSE` & `mentat-ai-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/README.md` & `mentat-ai-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 # ⚙️ Setup
 
 ## Install
 
 Before installing, it's suggested that you create a virtual environment to install it in:
 
 ```
+# Python 3.10 or higher is required
 python3 -m venv .venv
 source .venv/bin/activate
 ```
 
 Note that you'll have to have activated the virtual environment to run mentat if you install it there.
 
 There are then 3 install methods. The first two will just let you run it:
```

### Comparing `mentat-ai-0.1.3/mentat/app.py` & `mentat-ai-0.1.4/mentat/app.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/mentat/change_conflict_resolution.py` & `mentat-ai-0.1.4/mentat/change_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/mentat/code_change.py` & `mentat-ai-0.1.4/mentat/code_change.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/mentat/code_change_display.py` & `mentat-ai-0.1.4/mentat/code_change_display.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/mentat/code_file_manager.py` & `mentat-ai-0.1.4/mentat/code_file_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import glob
 import logging
 import math
 import mimetypes
 import os
 import subprocess
 from collections import defaultdict
 from pathlib import Path
@@ -171,14 +172,15 @@
             mimetypes.types_map.pop(file_type, None)
 
         for file_type in config.filetype_include_list():
             mimetypes.add_type("text/user-include-list", file_type)
         for file_type in config.filetype_exclude_list():
             mimetypes.types_map.pop(file_type, None)
 
+        self.config = config
         self.git_root = _get_shared_git_root_for_paths(paths)
         self._set_file_paths(paths)
         self.user_input_manager = user_input_manager
 
         if self.file_paths:
             cprint("Files included in context:", "green")
         else:
@@ -209,25 +211,40 @@
         self.file_paths = []
 
         for path in paths:
             path = Path(path)
             if path.is_file():
                 path_set.add(os.path.realpath(path))
             elif path.is_dir():
-                nonignored_files = set(
-                    filter(
+                non_git_ignored_files = set(
+                    # git returns / seperated paths even on windows, convert so we can remove
+                    # glob_excluded_files, which have windows paths on windows
+                    os.path.normpath(path)
+                    for path in filter(
                         lambda p: p != "",
                         subprocess.check_output(
                             # -c shows cached (regular) files, -o shows other (untracked/ new) files
                             ["git", "ls-files", "-c", "-o", "--exclude-standard"],
                             cwd=path,
                             text=True,
                         ).split("\n"),
                     )
                 )
+                glob_excluded_files = set(
+                    file
+                    for glob_path in self.config.file_exclude_glob_list()
+                    # If the user puts a / at the beginning, it will try to look in root directory
+                    for file in glob.glob(
+                        pathname=glob_path.lstrip("/"),
+                        root_dir=path,
+                        recursive=True,
+                    )
+                )
+                nonignored_files = non_git_ignored_files - glob_excluded_files
+
                 non_text_files = filter(
                     lambda f: not _is_file_text(
                         os.path.realpath(os.path.join(path, f))
                     ),
                     nonignored_files,
                 )
                 self.non_text_file_paths.extend(
```

### Comparing `mentat-ai-0.1.3/mentat/config_manager.py` & `mentat-ai-0.1.4/mentat/config_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,18 @@
 
     def filetype_include_list(self) -> list[str]:
         return self._get_key("filetype-include-list")
 
     def filetype_exclude_list(self) -> list[str]:
         return self._get_key("filetype-exclude-list")
 
+    def file_exclude_glob_list(self) -> list[str]:
+        return self._get_key("file-exclude-glob-list")
+
     def _get_key(self, key: str):
         if key in self.user_config:
             return self.user_config[key]
         elif key in self.default_config:
             return self.default_config[key]
         else:
-            logging.error(f"No value for config key {key} found")
+            logging.warning(f"No value for config key {key} found")
             return None
```

### Comparing `mentat-ai-0.1.3/mentat/conversation.py` & `mentat-ai-0.1.4/mentat/conversation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,21 @@
-import openai
-from termcolor import cprint
-
 from .code_change import CodeChange
 from .code_file_manager import CodeFileManager
 from .config_manager import ConfigManager
-from .llm_api import CostTracker, choose_model, count_tokens
+from .llm_api import CostTracker, check_model_availability, choose_model, count_tokens
 from .parsing import run_async_stream_and_parse_llm_response
 from .prompts import system_prompt
 
 
 class Conversation:
     def __init__(self, config: ConfigManager, cost_tracker: CostTracker):
         self.messages = []
         self.add_system_message(system_prompt)
-        self.allow_32k = config.allow_32k()
         self.cost_tracker = cost_tracker
-
-        if self.allow_32k:
-            # check if user actually has access to gpt-4-32k
-            available_models = [x["id"] for x in openai.Model.list()["data"]]
-            if "gpt-4-32k-0314" not in available_models:
-                cprint(
-                    (
-                        "You set ALLOW_32K to true, but your openAI API key doesn't"
-                        " have access to gpt-4-32k-0314. To remove this warning, set"
-                        " ALLOW_32K to false until you have access."
-                    ),
-                    "yellow",
-                )
-                self.allow_32k = False
+        self.allow_32k = check_model_availability(config.allow_32k())
 
     def add_system_message(self, message: str):
         self.messages.append({"role": "system", "content": message})
 
     def add_user_message(self, message: str):
         self.messages.append({"role": "user", "content": message})
```

### Comparing `mentat-ai-0.1.3/mentat/llm_api.py` & `mentat-ai-0.1.4/mentat/llm_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -53,14 +53,44 @@
     return response
 
 
 def count_tokens(message: str) -> int:
     return len(tiktoken.encoding_for_model("gpt-4").encode(message))
 
 
+def check_model_availability(allow_32k: bool) -> bool:
+    available_models = [x["id"] for x in openai.Model.list()["data"]]
+    if allow_32k:
+        # check if user has access to gpt-4-32k
+        if "gpt-4-32k-0314" not in available_models:
+            cprint(
+                (
+                    "You set ALLOW_32K to true, but your OpenAI API key doesn't"
+                    " have access to gpt-4-32k-0314. To remove this warning, set"
+                    " ALLOW_32K to false until you have access."
+                ),
+                "yellow",
+            )
+            allow_32k = False
+
+    if not allow_32k:
+        # check if user has access to gpt-4
+        if "gpt-4-0314" not in available_models:
+            cprint(
+                (
+                    "Sorry, but your OpenAI API key doesn't have access to gpt-4-0314,"
+                    " which is currently required to run Mentat."
+                ),
+                "red",
+            )
+            raise KeyboardInterrupt
+
+    return allow_32k
+
+
 def choose_model(messages: list[dict[str, str]], allow_32k) -> str:
     prompt_token_count = 0
     tokenizer = tiktoken.encoding_for_model("gpt-4")
     for message in messages:
         encoding = tokenizer.encode(message["content"])
         prompt_token_count += len(encoding)
     cprint(f"\nTotal token count: {prompt_token_count}", "cyan")
```

### Comparing `mentat-ai-0.1.3/mentat/logging_config.py` & `mentat-ai-0.1.4/mentat/logging_config.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/mentat/parsing.py` & `mentat-ai-0.1.4/mentat/parsing.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/mentat/prompts.py` & `mentat-ai-0.1.4/mentat/prompts.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/mentat/streaming_printer.py` & `mentat-ai-0.1.4/mentat/streaming_printer.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/mentat/user_input_manager.py` & `mentat-ai-0.1.4/mentat/user_input_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/mentat_ai.egg-info/SOURCES.txt` & `mentat-ai-0.1.4/mentat_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/mentat_ai.egg-info/requires.txt` & `mentat-ai-0.1.4/mentat_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/testbed/multifile_calculator/calculator.py` & `mentat-ai-0.1.4/testbed/multifile_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/tests/benchmark_test.py` & `mentat-ai-0.1.4/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/tests/codechange_test.py` & `mentat-ai-0.1.4/tests/codechange_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/tests/conftest.py` & `mentat-ai-0.1.4/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,17 @@
     mocker.patch.object(UserInputManager, "collect_user_input", new=mock_method)
 
     return mock_method
 
 
 @pytest.fixture
 def mock_setup_api_key(mocker):
-    return mocker.patch("mentat.app.setup_api_key")
+    mocker.patch("mentat.app.setup_api_key")
+    mocker.patch("mentat.conversation.check_model_availability")
+    return
 
 
 def add_permissions(func, path, exc_info):
     """
     Error handler for ``shutil.rmtree``.
 
     If the error is due to an access error (read only file)
@@ -87,15 +89,15 @@
         raise
 
 
 # Auto-used fixtures
 
 
 @pytest.fixture(autouse=True)
-def temp_testbed():
+def temp_testbed(monkeypatch):
     # create temporary copy of testbed, complete with git repo
     # realpath() resolves symlinks, required for paths to match on macOS
     temp_dir = os.path.realpath(tempfile.mkdtemp())
     temp_testbed = os.path.join(temp_dir, "testbed")
     shutil.copytree("testbed", temp_testbed)
     shutil.copy(".gitignore", temp_testbed)
     subprocess.run(
@@ -113,25 +115,23 @@
     subprocess.run(
         ["git", "commit", "-m", "add testbed"],
         cwd=temp_testbed,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
     )
 
-    yield temp_testbed
+    # necessary to undo chdir before calling rmtree, or it fails on windows
+    with monkeypatch.context() as m:
+        m.chdir(temp_testbed)
+        yield temp_testbed
 
     shutil.rmtree(temp_dir, onerror=add_permissions)
 
 
 @pytest.fixture(autouse=True)
-def change_cwd(temp_testbed, monkeypatch):
-    monkeypatch.chdir(temp_testbed)
-
-
-@pytest.fixture(autouse=True)
 def mock_sleep_time(mocker):
     mocker.patch.object(StreamingPrinter, "sleep_time", new=lambda self: 0)
 
 
 # Creating a prompt session in Github Actions on Windows throws an error
 # even though we don't use it, so we always have to mock the prompt session.
 @pytest.fixture(autouse=True)
```

### Comparing `mentat-ai-0.1.3/tests/measure_api_speed.py` & `mentat-ai-0.1.4/tests/measure_api_speed.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/tests/record_benchmark.py` & `mentat-ai-0.1.4/tests/record_benchmark.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/tests/system_test.py` & `mentat-ai-0.1.4/tests/system_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.3/tests/ui_test.py` & `mentat-ai-0.1.4/tests/ui_test.py`

 * *Files identical despite different names*

