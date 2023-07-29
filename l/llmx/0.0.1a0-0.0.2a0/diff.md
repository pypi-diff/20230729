# Comparing `tmp/llmx-0.0.1a0.tar.gz` & `tmp/llmx-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmx-0.0.1a0.tar", last modified: Mon Jul 17 08:41:52 2023, max compression
+gzip compressed data, was "llmx-0.0.2a0.tar", last modified: Sat Jul 29 02:18:55 2023, max compression
```

## Comparing `llmx-0.0.1a0.tar` & `llmx-0.0.2a0.tar`

### file list

```diff
@@ -1,25 +1,34 @@
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-17 08:41:52.284628 llmx-0.0.1a0/
--rw-r--r--   0 victordibia   (501) staff       (20)     3124 2023-07-16 17:45:47.000000 llmx-0.0.1a0/.gitignore
--rw-r--r--   0 victordibia   (501) staff       (20)        0 2023-07-17 04:10:36.000000 llmx-0.0.1a0/MANIFEST.in
--rw-r--r--   0 victordibia   (501) staff       (20)     2741 2023-07-17 08:41:52.284421 llmx-0.0.1a0/PKG-INFO
--rw-r--r--   0 victordibia   (501) staff       (20)     2252 2023-07-16 17:47:24.000000 llmx-0.0.1a0/README.md
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-17 08:41:52.282209 llmx-0.0.1a0/llmx/
--rw-r--r--   0 victordibia   (501) staff       (20)       25 2023-07-11 18:55:26.000000 llmx-0.0.1a0/llmx/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)      710 2023-07-11 18:39:39.000000 llmx-0.0.1a0/llmx/datamodel.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-17 08:41:52.283728 llmx-0.0.1a0/llmx/generators/
--rw-r--r--   0 victordibia   (501) staff       (20)       19 2023-07-11 18:55:22.000000 llmx-0.0.1a0/llmx/generators/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)     9542 2023-07-11 19:01:03.000000 llmx-0.0.1a0/llmx/generators/text.py
--rw-r--r--   0 victordibia   (501) staff       (20)     1663 2023-07-11 18:26:14.000000 llmx-0.0.1a0/llmx/utils.py
--rw-r--r--   0 victordibia   (501) staff       (20)       18 2023-07-11 18:05:16.000000 llmx-0.0.1a0/llmx/version.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-17 08:41:52.283232 llmx-0.0.1a0/llmx.egg-info/
--rw-r--r--   0 victordibia   (501) staff       (20)     2741 2023-07-17 08:41:52.000000 llmx-0.0.1a0/llmx.egg-info/PKG-INFO
--rw-r--r--   0 victordibia   (501) staff       (20)      368 2023-07-17 08:41:52.000000 llmx-0.0.1a0/llmx.egg-info/SOURCES.txt
--rw-r--r--   0 victordibia   (501) staff       (20)        1 2023-07-17 08:41:52.000000 llmx-0.0.1a0/llmx.egg-info/dependency_links.txt
--rw-r--r--   0 victordibia   (501) staff       (20)       38 2023-07-17 08:41:52.000000 llmx-0.0.1a0/llmx.egg-info/entry_points.txt
--rw-r--r--   0 victordibia   (501) staff       (20)       35 2023-07-17 08:41:52.000000 llmx-0.0.1a0/llmx.egg-info/requires.txt
--rw-r--r--   0 victordibia   (501) staff       (20)        5 2023-07-17 08:41:52.000000 llmx-0.0.1a0/llmx.egg-info/top_level.txt
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-17 08:41:52.284035 llmx-0.0.1a0/notebooks/
--rw-r--r--   0 victordibia   (501) staff       (20)     3571 2023-07-17 08:40:12.000000 llmx-0.0.1a0/notebooks/tutorial.ipynb
--rw-r--r--   0 victordibia   (501) staff       (20)     1055 2023-07-17 08:39:02.000000 llmx-0.0.1a0/pyproject.toml
--rw-r--r--   0 victordibia   (501) staff       (20)       38 2023-07-17 08:41:52.284673 llmx-0.0.1a0/setup.cfg
--rw-r--r--   0 victordibia   (501) staff       (20)       36 2023-07-17 04:12:01.000000 llmx-0.0.1a0/setup.py
+drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.249914 llmx-0.0.2a0/
+-rw-r--r--   0 victordibia   (501) staff       (20)     3143 2023-07-28 03:18:55.000000 llmx-0.0.2a0/.gitignore
+-rw-r--r--   0 victordibia   (501) staff       (20)        0 2023-07-25 17:59:05.000000 llmx-0.0.2a0/MANIFEST.in
+-rw-r--r--   0 victordibia   (501) staff       (20)     3590 2023-07-29 02:18:55.249470 llmx-0.0.2a0/PKG-INFO
+-rw-r--r--   0 victordibia   (501) staff       (20)     3058 2023-07-29 02:15:52.000000 llmx-0.0.2a0/README.md
+drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.177791 llmx-0.0.2a0/llmx/
+-rw-r--r--   0 victordibia   (501) staff       (20)        0 2023-07-28 02:07:41.000000 llmx-0.0.2a0/llmx/__init__.py
+-rw-r--r--   0 victordibia   (501) staff       (20)     1322 2023-07-28 18:57:05.000000 llmx-0.0.2a0/llmx/datamodel.py
+drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.195789 llmx-0.0.2a0/llmx/generators/
+-rw-r--r--   0 victordibia   (501) staff       (20)       40 2023-07-28 16:35:42.000000 llmx-0.0.2a0/llmx/generators/__init__.py
+drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.234660 llmx-0.0.2a0/llmx/generators/text/
+-rw-r--r--   0 victordibia   (501) staff       (20)        0 2023-07-28 16:35:47.000000 llmx-0.0.2a0/llmx/generators/text/__init__.py
+-rw-r--r--   0 victordibia   (501) staff       (20)     1080 2023-07-28 18:43:55.000000 llmx-0.0.2a0/llmx/generators/text/base_textgen.py
+-rw-r--r--   0 victordibia   (501) staff       (20)     2777 2023-07-28 23:04:53.000000 llmx-0.0.2a0/llmx/generators/text/cohere_textgen.py
+-rw-r--r--   0 victordibia   (501) staff       (20)     8804 2023-07-29 02:14:05.000000 llmx-0.0.2a0/llmx/generators/text/hf_textgen.py
+-rw-r--r--   0 victordibia   (501) staff       (20)     2471 2023-07-28 18:44:52.000000 llmx-0.0.2a0/llmx/generators/text/openai_textgen.py
+-rw-r--r--   0 victordibia   (501) staff       (20)     2990 2023-07-28 22:08:12.000000 llmx-0.0.2a0/llmx/generators/text/palm_textgen.py
+-rw-r--r--   0 victordibia   (501) staff       (20)     1524 2023-07-28 23:03:28.000000 llmx-0.0.2a0/llmx/generators/text/textgen.py
+-rw-r--r--   0 victordibia   (501) staff       (20)     2269 2023-07-28 18:51:21.000000 llmx-0.0.2a0/llmx/utils.py
+-rw-r--r--   0 victordibia   (501) staff       (20)       37 2023-07-29 02:17:54.000000 llmx-0.0.2a0/llmx/version.py
+drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.192285 llmx-0.0.2a0/llmx.egg-info/
+-rw-r--r--   0 victordibia   (501) staff       (20)     3590 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/PKG-INFO
+-rw-r--r--   0 victordibia   (501) staff       (20)      621 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/SOURCES.txt
+-rw-r--r--   0 victordibia   (501) staff       (20)        1 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/dependency_links.txt
+-rw-r--r--   0 victordibia   (501) staff       (20)       38 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/entry_points.txt
+-rw-r--r--   0 victordibia   (501) staff       (20)      120 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/requires.txt
+-rw-r--r--   0 victordibia   (501) staff       (20)        5 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/top_level.txt
+drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.243005 llmx-0.0.2a0/notebooks/
+-rw-r--r--   0 victordibia   (501) staff       (20)     4324 2023-07-28 21:00:21.000000 llmx-0.0.2a0/notebooks/tutorial.ipynb
+-rw-r--r--   0 victordibia   (501) staff       (20)     1385 2023-07-28 20:56:36.000000 llmx-0.0.2a0/pyproject.toml
+-rw-r--r--   0 victordibia   (501) staff       (20)       38 2023-07-29 02:18:55.249998 llmx-0.0.2a0/setup.cfg
+-rw-r--r--   0 victordibia   (501) staff       (20)       36 2023-07-25 17:59:05.000000 llmx-0.0.2a0/setup.py
+drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.246690 llmx-0.0.2a0/tests/
+-rw-r--r--   0 victordibia   (501) staff       (20)     1597 2023-07-28 23:01:30.000000 llmx-0.0.2a0/tests/test_generators.py
```

### Comparing `llmx-0.0.1a0/.gitignore` & `llmx-0.0.2a0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .vscode
-pyllm/generators/cache
-Pyllm.egg-info
+llmx/generators/cache
+llmx.egg-info
+notebooks/test.ipynb
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `llmx-0.0.1a0/PKG-INFO` & `llmx-0.0.2a0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,84 @@
-Metadata-Version: 2.1
-Name: llmx
-Version: 0.0.1a0
-Summary: LLMX: A library for LLM Text Generation
-Author-email: Victor Dibia <victor.dibia@gmail.com>
-Project-URL: Homepage, https://github.com/victordibia/llmx
-Project-URL: Bug Tracker, https://github.com/victordibia/llmx/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+# LLMX - An API for Language Models
 
-# PYLLM
+[![PyPI version](https://badge.fury.io/py/llmx.svg)](https://badge.fury.io/py/llmx)
 
-A simple python package that provides a unified interface to several LLM providers - [OpenAI](https://platform.openai.com/docs/api-reference/authentication) (default), Palm, and local HuggingFace Models.
+A simple python package that provides a unified interface to several LLM providers [ OpenAI (default), PaLM, Cohere and local HuggingFace Models ].
 
 There is nothing special about this library, but some of the requirements I needed when I startec building this (that other libraries did not have):
 
-- Uses typed datamodels for model configuration: This makes it easier to build web apis (fast api) on top of this library. For example, the text generation config is a pydantic model.
+- **Unified Model Interface**: Single interface to create LLM text generators with support for **multiple LLM providers**.
 
 ```python
-config = TextGenerationConfig(
-    model="gpt-3.5-turbo-0301",
-    n=1,
-    temperature=0.5,
-    max_tokens=100,
-    top_p=1.0,
-    top_k=50,
-    frequency_penalty=0.0,
-    presence_penalty=0.0,
-)
+
+openai_generator = TextGenerator(provider="openai")
+palm_generator = TextGenerator(provider="google") # or palm
+cohere_generator = TextGenerator(provider="cohere") # or palm
+hf_generator = TextGenerator(provider="huggingface") # run locally
 ```
 
-- Unified Interface: Switch between LLM providers with a single line of code. Standardizes on the OpenAI ChatML format. For example, the standard prompt sent a model is formatted as an array of objects, where each object has a role (`system`, `user`, or `assistant`) and content of the form.
+- **Unified Messaging Interface**. Standardizes on the OpenAI ChatML format. For example, the standard prompt sent a model is formatted as an array of objects, where each object has a role (`system`, `user`, or `assistant`) and content of the form. A single request is list one only one message (e.g., write code to plot a cosine wave signal). A conversation is a list of messages e.g. write code for x, update the axis to y, etc. For all models.
 
 ```python
-
 messages = [
     {"role": "user", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
-    {"role": "user", "content": "What is  gravity?"},
+    {"role": "user", "content": "What is  gravity?"}
 ]
 ```
 
-Are there other libraries that do things like this really well? Yes! I'd recommend looking at guidance.
+- **Good Utils (e.g., Caching etc)**: E.g. being able to use caching for faster responses. General policy is that cache is used if config (including messages) is the same. If you want to force a new response, set `use_cache=False` in the `generate` call.
+
+```python
+response = gen.generate(config=config, use_cache=True)
+```
+
+Are there other libraries that do things like this really well? Yes! I'd recommend looking at [guidance](https://github.com/microsoft/guidance) which does a lot more. Interested in optimized inference? Try somthing like [vllm](https://github.com/vllm-project/vllm).
 
 ## Installation
 
 Install from pypi. Please use python3.9 or higher.
 
 ```bash
-pip install pyllm
+pip install llmx
 ```
 
 Install in development mode
 
 ```bash
 git clone
-cd pyllm
+cd llmx
 pip install -e .
 ```
 
 Note that you may want to use the latest version of pip to install this package.
 `python3 -m pip install --upgrade pip`
 
 ## Usage
 
+Set your api keys first
+
+```bash
+export OPENAI_API_KEY=<your key>
+export PALM_API_KEY=<your key>
+export COHERE_API_KEY=<your key>
+```
+
 ```python
-from pyllm import OpenAITextGenerator, TextGenerationConfig
+from llmx.generators.text.textgen import TextGenerator
+from llmx.datamodel import TextGenerationConfig
 
-gen = OpenAITextGenerator()
-config = TextGenerationConfig(
-    model="gpt-3.5-turbo-0301",
-    messages=[
+gen = TextGenerator(provider="openai")
+config = TextGenerationConfig(messages=[
         {"role": "user", "content": "What is the height of the Eiffel Tower?"},
-    ],
-    n=1,
-    temperature=0.5,
-    max_tokens=100,
-    top_p=1.0,
-    top_k=50,
-    frequency_penalty=0.0,
-    presence_penalty=0.0,
-)
+    ])
 response = gen.generate(config=config, use_cache=False)
 print(response.text)
 # [{'role': 'assistant', 'content': 'The height of the Eiffel Tower is 324 meters (1,063 feet).'}]
 ```
+
+## Current Work
+
+- Supported models
+  - [x] OpenAI
+  - [x] PaLM
+  - [x] Cohere
+  - [ ] HuggingFace (local)
```

### Comparing `llmx-0.0.1a0/llmx/utils.py` & `llmx-0.0.2a0/llmx/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,67 @@
-
+from dataclasses import asdict
 import logging
 import json
-from typing import Any 
+from typing import Any
 import tiktoken
 from diskcache import Cache
 import hashlib
+import os
+import platform
 
 logger = logging.getLogger(__name__)
 
+
 def num_tokens_from_messages(messages, model="gpt-3.5-turbo-0301"):
     """Returns the number of tokens used by a list of messages."""
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError:
         encoding = tiktoken.get_encoding("cl100k_base")
-    if model == "gpt-3.5-turbo-0301":  # note: future models may deviate from this
+    if (
+        model == "gpt-3.5-turbo-0301" or True
+    ):  # note: future models may deviate from this
         num_tokens = 0
         for message in messages:
-            num_tokens += 4  # every message follows <im_start>{role/name}\n{content}<im_end>\n
+            if not isinstance(message, dict):
+                message = asdict(message)
+
+            num_tokens += (
+                4  # every message follows <im_start>{role/name}\n{content}<im_end>\n
+            )
+
             for key, value in message.items():
                 num_tokens += len(encoding.encode(value))
                 if key == "name":  # if there's a name, the role is omitted
                     num_tokens += -1  # role is always required and always 1 token
         num_tokens += 2  # every reply is primed with <im_start>assistant
         return num_tokens
-    else:
-        raise NotImplementedError(
-            f"""num_tokens_from_messages() is not presently implemented for model {model}.""")
 
 
 def cache_request(cache: Cache, params: dict, values: dict | None = None) -> Any:
     # Generate a unique key for the request
 
     key = hashlib.md5(json.dumps(params, sort_keys=True).encode("utf-8")).hexdigest()
     # Check if the request is cached
     if key in cache and values is None:
-        print("retrieving from cache")
+        # print("retrieving from cache")
         return cache[key]
 
     # Cache the provided values and return them
     if values:
-        print("saving to cache")
+        # print("saving to cache")
         cache[key] = values
-    return values
+    return values
+
+
+def get_user_cache_dir(app_name: str) -> str:
+    system = platform.system()
+    if system == "Windows":
+        cache_path = os.path.join(os.getenv("LOCALAPPDATA"), app_name, "Cache")
+    elif system == "Darwin":
+        cache_path = os.path.join(os.path.expanduser("~/Library/Caches"), app_name)
+    else:  # Linux and other UNIX-like systems
+        cache_path = os.path.join(
+            os.getenv("XDG_CACHE_HOME", os.path.expanduser("~/.cache")), app_name
+        )
+    os.makedirs(cache_path, exist_ok=True)
+    return cache_path
```

