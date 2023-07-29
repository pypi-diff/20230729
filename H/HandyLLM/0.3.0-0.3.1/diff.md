# Comparing `tmp/HandyLLM-0.3.0.tar.gz` & `tmp/HandyLLM-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandyLLM-0.3.0.tar", last modified: Fri Jul 28 04:45:25 2023, max compression
+gzip compressed data, was "HandyLLM-0.3.1.tar", last modified: Sat Jul 29 07:09:42 2023, max compression
```

## Comparing `HandyLLM-0.3.0.tar` & `HandyLLM-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:45:25.206968 HandyLLM-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-28 04:45:25.206968 HandyLLM-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 04:45:25.206968 HandyLLM-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:45:25.202968 HandyLLM-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:45:25.202968 HandyLLM-0.3.0/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-28 04:45:25.000000 HandyLLM-0.3.0/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-28 04:45:25.000000 HandyLLM-0.3.0/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:45:25.000000 HandyLLM-0.3.0/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 04:45:25.000000 HandyLLM-0.3.0/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 04:45:25.000000 HandyLLM-0.3.0/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:45:25.206968 HandyLLM-0.3.0/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17200 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/src/handyllm/prompt_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/src/handyllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:45:25.206968 HandyLLM-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:09:42.501543 HandyLLM-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-29 07:09:42.501543 HandyLLM-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 07:09:42.501543 HandyLLM-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:09:42.497543 HandyLLM-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:09:42.497543 HandyLLM-0.3.1/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-29 07:09:42.000000 HandyLLM-0.3.1/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-29 07:09:42.000000 HandyLLM-0.3.1/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 07:09:42.000000 HandyLLM-0.3.1/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 07:09:42.000000 HandyLLM-0.3.1/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 07:09:42.000000 HandyLLM-0.3.1/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:09:42.497543 HandyLLM-0.3.1/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:09:42.501543 HandyLLM-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_stream.py
```

### Comparing `HandyLLM-0.3.0/PKG-INFO` & `HandyLLM-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.3.0
+Version: 0.3.1
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -37,17 +37,21 @@
 
 Example scripts are placed in [tests](./tests) folder.
 
 
 
 ## OpenAI API Request
 
+### Logs
+
+You can pass custom `logger` and `log_marks` (a string or a collection of strings) to `chat`/`completions` to get input and output logging.
+
 ### Timeout control
 
-This toolkit supports client-side `timeout` control, which OpenAI's official python package does not support yet:
+This toolkit supports client-side `timeout` control:
 
 ```python
 from handyllm import OpenAIAPI
 prompt = [{
     "role": "user",
     "content": "please tell me a joke"
     }]
@@ -142,26 +146,33 @@
 {
     "item1": "It is really a good day."
 }
 {
     "item2": "Indeed."
 }
 %output_format%
-%misc%
+%misc1%
+%misc2%
 ```
 
 ```python
 from handyllm import PromptConverter
 converter = PromptConverter()
 
 # chat can be used as the message parameter for OpenAI API
 chat = converter.rawfile2chat('prompt.txt')
 
 # variables wrapped in %s can be replaced at runtime
-new_chat = converter.chat_replace_variables(chat, {r'%misc%': 'Note: do not use any bad word.'})
+new_chat = converter.chat_replace_variables(
+    chat, 
+    {
+        r'%misc1%': 'Note1: do not use any bad word.',
+        r'%misc2%': 'Note2: be optimistic.',
+    }
+)
 ```
 
 ### Substitute
 
 `PromptConverter` can also substitute placeholder variables like `%output_format%` stored in text files to make multiple prompts modular. A substitute map `substitute.txt` looks like this:
 
 ```
```

### Comparing `HandyLLM-0.3.0/README.md` & `HandyLLM-0.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -24,17 +24,21 @@
 
 Example scripts are placed in [tests](./tests) folder.
 
 
 
 ## OpenAI API Request
 
+### Logs
+
+You can pass custom `logger` and `log_marks` (a string or a collection of strings) to `chat`/`completions` to get input and output logging.
+
 ### Timeout control
 
-This toolkit supports client-side `timeout` control, which OpenAI's official python package does not support yet:
+This toolkit supports client-side `timeout` control:
 
 ```python
 from handyllm import OpenAIAPI
 prompt = [{
     "role": "user",
     "content": "please tell me a joke"
     }]
@@ -129,26 +133,33 @@
 {
     "item1": "It is really a good day."
 }
 {
     "item2": "Indeed."
 }
 %output_format%
-%misc%
+%misc1%
+%misc2%
 ```
 
 ```python
 from handyllm import PromptConverter
 converter = PromptConverter()
 
 # chat can be used as the message parameter for OpenAI API
 chat = converter.rawfile2chat('prompt.txt')
 
 # variables wrapped in %s can be replaced at runtime
-new_chat = converter.chat_replace_variables(chat, {r'%misc%': 'Note: do not use any bad word.'})
+new_chat = converter.chat_replace_variables(
+    chat, 
+    {
+        r'%misc1%': 'Note1: do not use any bad word.',
+        r'%misc2%': 'Note2: be optimistic.',
+    }
+)
 ```
 
 ### Substitute
 
 `PromptConverter` can also substitute placeholder variables like `%output_format%` stored in text files to make multiple prompts modular. A substitute map `substitute.txt` looks like this:
 
 ```
```

### Comparing `HandyLLM-0.3.0/pyproject.toml` & `HandyLLM-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `HandyLLM-0.3.0/src/HandyLLM.egg-info/PKG-INFO` & `HandyLLM-0.3.1/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.3.0
+Version: 0.3.1
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -37,17 +37,21 @@
 
 Example scripts are placed in [tests](./tests) folder.
 
 
 
 ## OpenAI API Request
 
+### Logs
+
+You can pass custom `logger` and `log_marks` (a string or a collection of strings) to `chat`/`completions` to get input and output logging.
+
 ### Timeout control
 
-This toolkit supports client-side `timeout` control, which OpenAI's official python package does not support yet:
+This toolkit supports client-side `timeout` control:
 
 ```python
 from handyllm import OpenAIAPI
 prompt = [{
     "role": "user",
     "content": "please tell me a joke"
     }]
@@ -142,26 +146,33 @@
 {
     "item1": "It is really a good day."
 }
 {
     "item2": "Indeed."
 }
 %output_format%
-%misc%
+%misc1%
+%misc2%
 ```
 
 ```python
 from handyllm import PromptConverter
 converter = PromptConverter()
 
 # chat can be used as the message parameter for OpenAI API
 chat = converter.rawfile2chat('prompt.txt')
 
 # variables wrapped in %s can be replaced at runtime
-new_chat = converter.chat_replace_variables(chat, {r'%misc%': 'Note: do not use any bad word.'})
+new_chat = converter.chat_replace_variables(
+    chat, 
+    {
+        r'%misc1%': 'Note1: do not use any bad word.',
+        r'%misc2%': 'Note2: be optimistic.',
+    }
+)
 ```
 
 ### Substitute
 
 `PromptConverter` can also substitute placeholder variables like `%output_format%` stored in text files to make multiple prompts modular. A substitute map `substitute.txt` looks like this:
 
 ```
```

### Comparing `HandyLLM-0.3.0/src/HandyLLM.egg-info/SOURCES.txt` & `HandyLLM-0.3.1/src/HandyLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.0/src/handyllm/endpoint_manager.py` & `HandyLLM-0.3.1/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.0/src/handyllm/openai_api.py` & `HandyLLM-0.3.1/src/handyllm/openai_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import time
 import requests
 import logging
 import json
 import copy
 
 from .prompt_converter import PromptConverter
+from . import utils
 
 module_logger = logging.getLogger(__name__)
 
 class OpenAIAPI:
     
     base_url = "https://api.openai.com/v1"
     
@@ -141,15 +142,19 @@
     @staticmethod
     def chat(model, messages, timeout=None, endpoint_manager=None, logger=None, log_marks=[], **kwargs):
         request_url = '/chat/completions'
 
         if logger is not None and 'messages' in kwargs:
             arguments = copy.deepcopy(kwargs)
             arguments.pop('messages', None)
-            input_lines = [str(item) for item in log_marks]
+            # check if log_marks is iterable
+            if utils.isiterable(log_marks):
+                input_lines = [str(item) for item in log_marks]
+            else:
+                input_lines = [str(log_marks)]
             input_lines.append(json.dumps(arguments, indent=2, ensure_ascii=False))
             input_lines.append(" INPUT START ".center(50, '-'))
             input_lines.append(OpenAIAPI.converter.chat2raw(kwargs['messages']))
             input_lines.append(" INPUT END ".center(50, '-')+"\n")
             input_str = "\n".join(input_lines)
         
         start_time = time.time()
@@ -195,15 +200,19 @@
     @staticmethod
     def completions(model, prompt, timeout=None, endpoint_manager=None, logger=None, log_marks=[], **kwargs):
         request_url = '/completions'
 
         if logger is not None and 'prompt' in kwargs:
             arguments = copy.deepcopy(kwargs)
             arguments.pop('prompt', None)
-            input_lines = [str(item) for item in log_marks]
+            # check if log_marks is iterable
+            if utils.isiterable(log_marks):
+                input_lines = [str(item) for item in log_marks]
+            else:
+                input_lines = [str(log_marks)]
             input_lines.append(json.dumps(arguments, indent=2, ensure_ascii=False))
             input_lines.append(" INPUT START ".center(50, '-'))
             input_lines.append(kwargs['prompt'])
             input_lines.append(" INPUT END ".center(50, '-')+"\n")
             input_str = "\n".join(input_lines)
         
         start_time = time.time()
```

### Comparing `HandyLLM-0.3.0/src/handyllm/prompt_converter.py` & `HandyLLM-0.3.1/src/handyllm/prompt_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,14 @@
                 for var, value in variable_map.items():
                     if var in message['content']:
                         message['content'] = message['content'].replace(var, value)
             return chat
         else:
             new_chat = []
             for message in chat:
+                new_message = {"role": message['role'], "content": message['content']}
                 for var, value in variable_map.items():
-                    if var in message['content']:
-                        new_message = {"role": message['role'], "content": message['content'].replace(var, value)}
-                    else:
-                        new_message = {"role": message['role'], "content": message['content']}
+                    if var in new_message['content']:
+                        new_message['content'] = new_message['content'].replace(var, value)
                 new_chat.append(new_message)
             return new_chat
```

### Comparing `HandyLLM-0.3.0/src/handyllm/utils.py` & `HandyLLM-0.3.1/src/handyllm/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 from urllib.parse import urlparse
 import os
 import time
+import collections.abc
 
 
 def get_filename_from_url(download_url):
     # Parse the URL.
     parsed_url = urlparse(download_url)
     # The last part of the path is usually the filename.
     filename = os.path.basename(parsed_url.path)
@@ -19,7 +20,12 @@
             filename = 'download_' + time.strftime("%Y%m%d_%H%M%S")
         file_path = os.path.abspath(os.path.join(dir, filename))
     # Open the file in binary mode and write to it.
     with open(file_path, "wb") as file:
         file.write(response.content)
     return file_path
 
+def isiterable(arg):
+    return (
+        isinstance(arg, collections.abc.Iterable) 
+        and not isinstance(arg, str)
+    )
```

### Comparing `HandyLLM-0.3.0/tests/test_completions.py` & `HandyLLM-0.3.1/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.0/tests/test_embedding.py` & `HandyLLM-0.3.1/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.0/tests/test_files.py` & `HandyLLM-0.3.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.0/tests/test_images.py` & `HandyLLM-0.3.1/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.0/tests/test_models.py` & `HandyLLM-0.3.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.0/tests/test_moderation.py` & `HandyLLM-0.3.1/tests/test_moderation.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.0/tests/test_prompt.py` & `HandyLLM-0.3.1/tests/test_prompt.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,13 +2,21 @@
 from handyllm import PromptConverter
 converter = PromptConverter()
 
 converter.read_substitute_content('substitute.txt')  # read substitute map
 
 # chat can be used as the message parameter for OpenAI API
 chat = converter.rawfile2chat('prompt.txt')  # variables are substituted according to map
-print(json.dumps(chat, indent=2))
-print()
+# print(json.dumps(chat, indent=2))
+print(converter.chat2raw(chat))
+print('-----')
 
 # variables wrapped in %s can be replaced at runtime
-new_chat = converter.chat_replace_variables(chat, {r'%misc%': 'Note: do not use any bad word.'})
-print(json.dumps(new_chat, indent=2))
+new_chat = converter.chat_replace_variables(
+    chat, 
+    {
+        r'%misc1%': 'Note1: do not use any bad word.',
+        r'%misc2%': 'Note2: be optimistic.',
+    }
+)
+# print(json.dumps(new_chat, indent=2))
+print(converter.chat2raw(new_chat))
```

### Comparing `HandyLLM-0.3.0/tests/test_stream.py` & `HandyLLM-0.3.1/tests/test_stream.py`

 * *Files identical despite different names*

