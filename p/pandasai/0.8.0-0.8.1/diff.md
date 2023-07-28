# Comparing `tmp/pandasai-0.8.0.tar.gz` & `tmp/pandasai-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.8.0.tar", max compression
+gzip compressed data, was "pandasai-0.8.1.tar", max compression
```

## Comparing `pandasai-0.8.0.tar` & `pandasai-0.8.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1055 2023-07-27 19:15:30.960351 pandasai-0.8.0/LICENSE
--rw-r--r--   0        0        0     7853 2023-07-27 19:15:30.960351 pandasai-0.8.0/README.md
--rw-r--r--   0        0        0    27955 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/__init__.py
--rw-r--r--   0        0        0      155 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/callbacks/__init__.py
--rw-r--r--   0        0        0      519 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/callbacks/base.py
--rw-r--r--   0        0        0      583 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/callbacks/file.py
--rw-r--r--   0        0        0     1438 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     6404 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     3631 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/from_google_sheets.py
--rw-r--r--   0        0        0     1493 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3070 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     2454 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4289 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    12126 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      585 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     3130 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0     1230 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1578 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1261 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1380 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1256 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1983 2023-07-27 19:15:30.972351 pandasai-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9152 1970-01-01 00:00:00.000000 pandasai-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-28 23:36:48.651563 pandasai-0.8.1/LICENSE
+-rw-r--r--   0        0        0     7986 2023-07-28 23:36:48.651563 pandasai-0.8.1/README.md
+-rw-r--r--   0        0        0    28810 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/callbacks/__init__.py
+-rw-r--r--   0        0        0      519 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/callbacks/base.py
+-rw-r--r--   0        0        0      583 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/callbacks/file.py
+-rw-r--r--   0        0        0     1438 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     6404 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     3631 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/from_google_sheets.py
+-rw-r--r--   0        0        0     1493 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3070 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     2454 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4289 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    13023 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0      735 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      585 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     3130 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      739 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0     1230 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1578 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1261 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1380 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1256 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     2003 2023-07-28 23:36:48.663563 pandasai-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     9285 1970-01-01 00:00:00.000000 pandasai-0.8.1/PKG-INFO
```

### Comparing `pandasai-0.8.0/LICENSE` & `pandasai-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/README.md` & `pandasai-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # PandasAI 🐼
 
 [![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
 [![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
+[![Coverage](https://codecov.io/gh/gventuri/pandas-ai/branch/main/graph/badge.svg)](https://codecov.io/gh/gventuri/pandas-ai)
 [![Documentation Status](https://readthedocs.org/projects/pandas-ai/badge/?version=latest)](https://pandas-ai.readthedocs.io/en/latest/?badge=latest)
-[![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
+[![Discord](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
 [![Downloads](https://static.pepy.tech/badge/pandasai)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
 PandasAI is a Python library that adds Generative AI capabilities to [pandas](https://github.com/pandas-dev/pandas), the popular data analysis and manipulation tool. It is designed to be used in conjunction with pandas, and is not a replacement for it.
 
 <!-- Add images/pandas-ai.png -->
```

### Comparing `pandasai-0.8.0/pandasai/__init__.py` & `pandasai-0.8.1/pandasai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,16 +295,29 @@
             default_prompt=GenerateResponsePrompt,
             default_values=default_values,
         )
 
         return self._llm.call(generate_response_instruction, "")
 
     def _get_prompt(
-        self, key: str, default_prompt: Prompt, default_values: Dict = {}, df=None
-    ):
+        self,
+        key: str,
+        default_prompt: Type[Prompt],
+        default_values: Optional[dict] = None,
+        df=None,
+    ) -> tuple[Prompt, dict]:
+        if default_values is None:
+            default_values = {}
+
+        # prompt builtins are available to all prompts preceded by $
+        # e.g. $df.head(), $df.shape, $df.columns, etc.
+        prompt_builtins = {
+            "df": df,
+        }
+
         prompt = self._non_default_prompts.get(key)
 
         if prompt and isinstance(prompt, type):
             prompt = prompt(**default_values)
 
         if prompt:
             """Override all the variables with _ prefix with default variable values"""
@@ -314,15 +327,15 @@
 
             """Replace all variables with $ prefix with evaluated values"""
             prompt_text = prompt.text.split(" ")
             for i in range(len(prompt_text)):
                 word = prompt_text[i]
 
                 if word.startswith("$"):
-                    prompt_text[i] = str(eval(word[1:]))
+                    prompt_text[i] = str(eval(word[1:], prompt_builtins))
             prompt.text = " ".join(prompt_text)
 
             return prompt, prompt._args
 
         return default_prompt(**default_values), default_values
 
     def run(
@@ -381,15 +394,15 @@
                     (
                         multiple_dataframes_instruction,
                         multiple_dataframes_instruction_values,
                     ) = self._get_prompt(
                         "multiple_dataframes",
                         default_prompt=MultipleDataframesPrompt,
                         default_values=multiple_dataframes_default_values,
-                        df=heads,
+                        df=data_frame,
                     )
 
                     code = self._llm.generate_code(
                         multiple_dataframes_instruction,
                         prompt,
                     )
 
@@ -569,14 +582,32 @@
 
         return (
             isinstance(node, ast.Assign)
             and isinstance(node.targets[0], ast.Name)
             and re.match(r"df\d{0,2}$", node.targets[0].id)
         )
 
+    def _is_jailbreak(self, node: ast.stmt) -> bool:
+        """
+        Remove jailbreaks from the code to prevent malicious code execution.
+
+        Args:
+            node (object): ast.stmt
+
+        Returns (bool):
+        """
+
+        DANGEROUS_BUILTINS = ["__subclasses__", "__builtins__", "__import__"]
+
+        for child in ast.walk(node):
+            if isinstance(child, ast.Name) and child.id in DANGEROUS_BUILTINS:
+                return True
+
+        return False
+
     def _clean_code(self, code: str) -> str:
         """
         A method to clean the code to prevent malicious code execution
 
         Args:
             code(str): A python code
 
@@ -591,15 +622,15 @@
         # clear recent optional dependencies
         self._additional_dependencies = []
 
         for node in tree.body:
             if isinstance(node, (ast.Import, ast.ImportFrom)):
                 self._check_imports(node)
                 continue
-            if self._is_df_overwrite(node):
+            if self._is_df_overwrite(node) or self._is_jailbreak(node):
                 continue
             new_body.append(node)
 
         new_tree = ast.Module(body=new_body)
         return astor.to_source(new_tree, pretty_source=lambda x: "".join(x)).strip()
 
     def _get_environment(self) -> dict:
```

### Comparing `pandasai-0.8.0/pandasai/callbacks/base.py` & `pandasai-0.8.1/pandasai/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/callbacks/file.py` & `pandasai-0.8.1/pandasai/callbacks/file.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/constants.py` & `pandasai-0.8.1/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/exceptions.py` & `pandasai-0.8.1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/helpers/_optional.py` & `pandasai-0.8.1/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/helpers/anonymizer.py` & `pandasai-0.8.1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/helpers/cache.py` & `pandasai-0.8.1/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/helpers/from_excel.py` & `pandasai-0.8.1/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/helpers/from_google_sheets.py` & `pandasai-0.8.1/pandasai/helpers/from_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/helpers/notebook.py` & `pandasai-0.8.1/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/helpers/openai_info.py` & `pandasai-0.8.1/pandasai/helpers/openai_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/helpers/save_chart.py` & `pandasai-0.8.1/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/helpers/shortcuts.py` & `pandasai-0.8.1/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/llm/azure_openai.py` & `pandasai-0.8.1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/llm/base.py` & `pandasai-0.8.1/pandasai/llm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     class CustomLLM(BaseOpenAI):
 
         Custom Class Starts here!!
     ```
 """
 
+import os
 import ast
 import re
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Optional
 
 import openai
 import requests
@@ -276,14 +277,40 @@
     _api_url: str = "https://api-inference.huggingface.co/models/"
     _max_retries: int = 3
 
     @property
     def type(self) -> str:
         return "huggingface-llm"
 
+    def _setup(self, **kwargs):
+        """
+        Setup the HuggingFace LLM
+        Args:
+            **kwargs: ["api_token", "max_retries"]
+        """
+        self.api_token = (
+            kwargs.get("api_token") or os.getenv("HUGGINGFACE_API_KEY") or None
+        )
+        if self.api_token is None:
+            raise APIKeyNotFoundError("HuggingFace Hub API key is required")
+
+        # Since the huggingface API only returns few tokens at a time, we need to
+        # call the API multiple times to get all the tokens. This is the maximum
+        # number of retries we will do.
+        if kwargs.get("max_retries"):
+            self._max_retries = kwargs.get("max_retries")
+
+    def __init__(self, **kwargs):
+        """
+        __init__ method of HuggingFaceLLM Class
+        Args:
+            **kwargs: ["api_token", "max_retries"]
+        """
+        self._setup(**kwargs)
+
     def query(self, payload):
         """
         Query the HF API
         Args:
             payload: A JSON form payload
 
         Returns: Generated Response
```

### Comparing `pandasai-0.8.0/pandasai/llm/fake.py` & `pandasai-0.8.1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/llm/google_palm.py` & `pandasai-0.8.1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/llm/langchain.py` & `pandasai-0.8.1/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/llm/openai.py` & `pandasai-0.8.1/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/middlewares/base.py` & `pandasai-0.8.1/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/middlewares/charts.py` & `pandasai-0.8.1/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/middlewares/streamlit.py` & `pandasai-0.8.1/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/prompts/base.py` & `pandasai-0.8.1/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.8.1/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.8.1/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/prompts/generate_python_code.py` & `pandasai-0.8.1/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.8.1/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.0/pyproject.toml` & `pandasai-0.8.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.8.0"
+version = "0.8.1"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
@@ -24,14 +24,15 @@
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 ruff = "^0.0.220"
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 pytest-env = "^0.8.1"
 click = "^8.1.3"
+coverage = "^7.2.7"
 
 
 [tool.poetry.group.extras.dependencies]
 google-cloud-aiplatform = "^1.26.1"
 
 [tool.poetry.extras]
 google = ["google-generativeai"]
```

### Comparing `pandasai-0.8.0/PKG-INFO` & `pandasai-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.8.0
+Version: 0.8.1
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -28,16 +28,17 @@
 Description-Content-Type: text/markdown
 
 # PandasAI 🐼
 
 [![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
 [![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
+[![Coverage](https://codecov.io/gh/gventuri/pandas-ai/branch/main/graph/badge.svg)](https://codecov.io/gh/gventuri/pandas-ai)
 [![Documentation Status](https://readthedocs.org/projects/pandas-ai/badge/?version=latest)](https://pandas-ai.readthedocs.io/en/latest/?badge=latest)
-[![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
+[![Discord](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
 [![Downloads](https://static.pepy.tech/badge/pandasai)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
 PandasAI is a Python library that adds Generative AI capabilities to [pandas](https://github.com/pandas-dev/pandas), the popular data analysis and manipulation tool. It is designed to be used in conjunction with pandas, and is not a replacement for it.
 
 <!-- Add images/pandas-ai.png -->
```

