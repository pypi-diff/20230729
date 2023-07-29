# Comparing `tmp/mentat-ai-0.1.5.tar.gz` & `tmp/mentat-ai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentat-ai-0.1.5.tar", last modified: Sat Jul 29 00:15:10 2023, max compression
+gzip compressed data, was "mentat-ai-0.1.6.tar", last modified: Sat Jul 29 00:41:39 2023, max compression
```

## Comparing `mentat-ai-0.1.5.tar` & `mentat-ai-0.1.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:15:10.000872 mentat-ai-0.1.5/
--rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.5/LICENSE
--rw-r--r--   0 biobootloader   (501) staff       (20)      148 2023-07-29 00:15:10.000757 mentat-ai-0.1.5/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)     2997 2023-07-28 22:38:12.000000 mentat-ai-0.1.5/README.md
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:15:09.997491 mentat-ai-0.1.5/mentat/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.5/mentat/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      342 2023-07-28 22:38:12.000000 mentat-ai-0.1.5/mentat/__main__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     6025 2023-07-28 22:38:06.000000 mentat-ai-0.1.5/mentat/app.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.5/mentat/change_conflict_resolution.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.5/mentat/code_change.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.5/mentat/code_change_display.py
--rw-r--r--   0 biobootloader   (501) staff       (20)    14002 2023-07-28 23:48:43.000000 mentat-ai-0.1.5/mentat/code_file_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1645 2023-07-28 23:48:43.000000 mentat-ai-0.1.5/mentat/config_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1728 2023-07-28 22:38:12.000000 mentat-ai-0.1.5/mentat/conversation.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      359 2023-07-28 23:48:43.000000 mentat-ai-0.1.5/mentat/default_config.json
--rw-r--r--   0 biobootloader   (501) staff       (20)     4821 2023-07-28 22:38:12.000000 mentat-ai-0.1.5/mentat/llm_api.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.5/mentat/logging_config.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-27 16:52:26.000000 mentat-ai-0.1.5/mentat/parsing.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.5/mentat/prompts.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.5/mentat/streaming_printer.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.5/mentat/user_input_manager.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:15:09.998146 mentat-ai-0.1.5/mentat_ai.egg-info/
--rw-r--r--   0 biobootloader   (501) staff       (20)      148 2023-07-29 00:15:09.000000 mentat-ai-0.1.5/mentat_ai.egg-info/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)      997 2023-07-29 00:15:09.000000 mentat-ai-0.1.5/mentat_ai.egg-info/SOURCES.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-29 00:15:09.000000 mentat-ai-0.1.5/mentat_ai.egg-info/dependency_links.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-29 00:15:09.000000 mentat-ai-0.1.5/mentat_ai.egg-info/entry_points.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)      765 2023-07-29 00:15:09.000000 mentat-ai-0.1.5/mentat_ai.egg-info/requires.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-29 00:15:09.000000 mentat-ai-0.1.5/mentat_ai.egg-info/top_level.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.5/pyproject.toml
--rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-29 00:15:10.000904 mentat-ai-0.1.5/setup.cfg
--rw-r--r--   0 biobootloader   (501) staff       (20)      558 2023-07-29 00:14:28.000000 mentat-ai-0.1.5/setup.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:15:09.998239 mentat-ai-0.1.5/testbed/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.5/testbed/__init__.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:15:09.998798 mentat-ai-0.1.5/testbed/multifile_calculator/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.5/testbed/multifile_calculator/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.5/testbed/multifile_calculator/calculator.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.5/testbed/multifile_calculator/operations.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:15:10.000599 mentat-ai-0.1.5/tests/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.5/tests/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.5/tests/benchmark_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3872 2023-07-28 23:48:43.000000 mentat-ai-0.1.5/tests/code_file_manager_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     7507 2023-07-27 16:52:26.000000 mentat-ai-0.1.5/tests/codechange_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      146 2023-07-28 22:38:12.000000 mentat-ai-0.1.5/tests/config_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3805 2023-07-28 22:38:12.000000 mentat-ai-0.1.5/tests/conftest.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.5/tests/measure_api_speed.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.5/tests/record_benchmark.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-27 16:52:26.000000 mentat-ai-0.1.5/tests/system_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.5/tests/ui_test.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.362030 mentat-ai-0.1.6/
+-rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.6/LICENSE
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3324 2023-07-29 00:41:39.361927 mentat-ai-0.1.6/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3114 2023-07-29 00:20:59.000000 mentat-ai-0.1.6/README.md
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.358661 mentat-ai-0.1.6/mentat/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.6/mentat/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      342 2023-07-28 22:38:12.000000 mentat-ai-0.1.6/mentat/__main__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     6025 2023-07-28 22:38:06.000000 mentat-ai-0.1.6/mentat/app.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.6/mentat/change_conflict_resolution.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.6/mentat/code_change.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.6/mentat/code_change_display.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)    14002 2023-07-28 23:48:43.000000 mentat-ai-0.1.6/mentat/code_file_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1645 2023-07-28 23:48:43.000000 mentat-ai-0.1.6/mentat/config_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1728 2023-07-28 22:38:12.000000 mentat-ai-0.1.6/mentat/conversation.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      359 2023-07-28 23:48:43.000000 mentat-ai-0.1.6/mentat/default_config.json
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4821 2023-07-28 22:38:12.000000 mentat-ai-0.1.6/mentat/llm_api.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.6/mentat/logging_config.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-27 16:52:26.000000 mentat-ai-0.1.6/mentat/parsing.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.6/mentat/prompts.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.6/mentat/streaming_printer.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.6/mentat/user_input_manager.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.359331 mentat-ai-0.1.6/mentat_ai.egg-info/
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3324 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)      997 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/entry_points.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)      765 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/requires.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/top_level.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.6/pyproject.toml
+-rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-29 00:41:39.362059 mentat-ai-0.1.6/setup.cfg
+-rw-r--r--   0 biobootloader   (501) staff       (20)      853 2023-07-29 00:41:11.000000 mentat-ai-0.1.6/setup.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.359432 mentat-ai-0.1.6/testbed/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.6/testbed/__init__.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.359794 mentat-ai-0.1.6/testbed/multifile_calculator/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.6/testbed/multifile_calculator/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.6/testbed/multifile_calculator/calculator.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.6/testbed/multifile_calculator/operations.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.361755 mentat-ai-0.1.6/tests/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.6/tests/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.6/tests/benchmark_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3872 2023-07-28 23:48:43.000000 mentat-ai-0.1.6/tests/code_file_manager_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7507 2023-07-27 16:52:26.000000 mentat-ai-0.1.6/tests/codechange_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      146 2023-07-28 22:38:12.000000 mentat-ai-0.1.6/tests/config_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3805 2023-07-28 22:38:12.000000 mentat-ai-0.1.6/tests/conftest.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.6/tests/measure_api_speed.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.6/tests/record_benchmark.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-27 16:52:26.000000 mentat-ai-0.1.6/tests/system_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.6/tests/ui_test.py
```

### Comparing `mentat-ai-0.1.5/LICENSE` & `mentat-ai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/README.md` & `mentat-ai-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [![Twitter Follow](https://img.shields.io/twitter/follow/bio_bootloader?style=social)](https://twitter.com/bio_bootloader)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/XbPdxAMJte?style=flat)](https://discord.gg/zbvd9qx9Pb)
 [![Stable Version](https://img.shields.io/pypi/v/mentat-ai?color=blue)](https://pypi.org/project/mentat-ai/)
+[![License](https://img.shields.io/pypi/l/mentat-ai.svg)](https://github.com/biobootloader/mentat/blob/main/LICENSE)
 
 # 🧙‍♂️ Mentat ⚡
 
 > _It is by will alone I set my mind in motion_
 > 
 > The Mentat Mantra
```

### Comparing `mentat-ai-0.1.5/mentat/app.py` & `mentat-ai-0.1.6/mentat/app.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/change_conflict_resolution.py` & `mentat-ai-0.1.6/mentat/change_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/code_change.py` & `mentat-ai-0.1.6/mentat/code_change.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/code_change_display.py` & `mentat-ai-0.1.6/mentat/code_change_display.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/code_file_manager.py` & `mentat-ai-0.1.6/mentat/code_file_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/config_manager.py` & `mentat-ai-0.1.6/mentat/config_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/conversation.py` & `mentat-ai-0.1.6/mentat/conversation.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/llm_api.py` & `mentat-ai-0.1.6/mentat/llm_api.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/logging_config.py` & `mentat-ai-0.1.6/mentat/logging_config.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/parsing.py` & `mentat-ai-0.1.6/mentat/parsing.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/prompts.py` & `mentat-ai-0.1.6/mentat/prompts.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/streaming_printer.py` & `mentat-ai-0.1.6/mentat/streaming_printer.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat/user_input_manager.py` & `mentat-ai-0.1.6/mentat/user_input_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat_ai.egg-info/SOURCES.txt` & `mentat-ai-0.1.6/mentat_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/mentat_ai.egg-info/requires.txt` & `mentat-ai-0.1.6/mentat_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/testbed/multifile_calculator/calculator.py` & `mentat-ai-0.1.6/testbed/multifile_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/tests/benchmark_test.py` & `mentat-ai-0.1.6/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/tests/code_file_manager_test.py` & `mentat-ai-0.1.6/tests/code_file_manager_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/tests/codechange_test.py` & `mentat-ai-0.1.6/tests/codechange_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/tests/conftest.py` & `mentat-ai-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/tests/measure_api_speed.py` & `mentat-ai-0.1.6/tests/measure_api_speed.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/tests/record_benchmark.py` & `mentat-ai-0.1.6/tests/record_benchmark.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/tests/system_test.py` & `mentat-ai-0.1.6/tests/system_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.5/tests/ui_test.py` & `mentat-ai-0.1.6/tests/ui_test.py`

 * *Files identical despite different names*

