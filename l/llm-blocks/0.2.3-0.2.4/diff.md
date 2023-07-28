# Comparing `tmp/llm-blocks-0.2.3.tar.gz` & `tmp/llm-blocks-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-blocks-0.2.3.tar", last modified: Wed Jul 12 23:29:27 2023, max compression
+gzip compressed data, was "llm-blocks-0.2.4.tar", last modified: Fri Jul 28 23:46:04 2023, max compression
```

## Comparing `llm-blocks-0.2.3.tar` & `llm-blocks-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 23:29:27.789849 llm-blocks-0.2.3/
--rw-rw-rw-   0        0        0     2771 2023-07-12 23:29:27.788848 llm-blocks-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2327 2023-06-07 15:34:54.000000 llm-blocks-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 23:29:27.782613 llm-blocks-0.2.3/llm_blocks/
--rw-rw-rw-   0        0        0        0 2023-06-06 22:53:28.000000 llm-blocks-0.2.3/llm_blocks/__init__.py
--rw-rw-rw-   0        0        0     1620 2023-06-07 15:34:54.000000 llm-blocks-0.2.3/llm_blocks/chat_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:29:27.787852 llm-blocks-0.2.3/llm_blocks.egg-info/
--rw-rw-rw-   0        0        0     2771 2023-07-12 23:29:27.000000 llm-blocks-0.2.3/llm_blocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-12 23:29:27.000000 llm-blocks-0.2.3/llm_blocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 23:29:27.000000 llm-blocks-0.2.3/llm_blocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-12 23:29:27.000000 llm-blocks-0.2.3/llm_blocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-12 23:29:27.000000 llm-blocks-0.2.3/llm_blocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 23:29:27.789849 llm-blocks-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-07-12 23:29:10.000000 llm-blocks-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 23:46:04.535984 llm-blocks-0.2.4/
+-rw-rw-rw-   0        0        0     2771 2023-07-28 23:46:04.534527 llm-blocks-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2327 2023-06-07 15:34:54.000000 llm-blocks-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 23:46:04.523526 llm-blocks-0.2.4/llm_blocks/
+-rw-rw-rw-   0        0        0        0 2023-06-06 22:53:28.000000 llm-blocks-0.2.4/llm_blocks/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-07-28 23:44:09.000000 llm-blocks-0.2.4/llm_blocks/chat_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 23:46:04.533527 llm-blocks-0.2.4/llm_blocks.egg-info/
+-rw-rw-rw-   0        0        0     2771 2023-07-28 23:46:04.000000 llm-blocks-0.2.4/llm_blocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-28 23:46:04.000000 llm-blocks-0.2.4/llm_blocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 23:46:04.000000 llm-blocks-0.2.4/llm_blocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-28 23:46:04.000000 llm-blocks-0.2.4/llm_blocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-28 23:46:04.000000 llm-blocks-0.2.4/llm_blocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 23:46:04.535984 llm-blocks-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-07-28 23:45:55.000000 llm-blocks-0.2.4/setup.py
```

### Comparing `llm-blocks-0.2.3/PKG-INFO` & `llm-blocks-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-blocks
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple interface for creating and managing LLM chains
 Home-page: https://github.com/voynow/llm-blocks
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm-blocks-0.2.3/README.md` & `llm-blocks-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `llm-blocks-0.2.3/llm_blocks/chat_utils.py` & `llm-blocks-0.2.4/llm_blocks/chat_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,95 @@
-import dotenv
-from langchain.callbacks import get_openai_callback
 import os
-from langchain.chat_models import ChatOpenAI
-from langchain.prompts import PromptTemplate
-from langchain.chains import LLMChain
+import re
 import time
 
+import dotenv
+import openai
+from IPython.display import Markdown, clear_output, display
+
 dotenv.load_dotenv()
 OPENAI_API_KEY = os.getenv("OPENAI_API_KEY")
 if not OPENAI_API_KEY:
     raise ValueError(
         "OPENAI_API_KEY not found. Either create a .env file or set the environment variable."
     )
 
 
 class GenericChain:
     def __init__(
-        self, template: str, model_name: str = "gpt-3.5-turbo", temperature: float = 0.2
+        self,
+        template: str,
+        role: str = "user",
+        model_name: str = "gpt-3.5-turbo",
+        temperature: float = 0.2,
+        stream: bool = False,
     ):
-        llm = ChatOpenAI(
-            openai_api_key=OPENAI_API_KEY,
-            model_name=model_name,
-            temperature=temperature,
-        )
-        prompt = PromptTemplate.from_template(template)
-        self.chain = LLMChain(llm=llm, prompt=prompt)
+        """ 
+        Super simple interface for chat-like GPT completions
+
+        template (str): The template to use for the model
+        role (str, optional): The role of the user. Defaults to "user".
+        model_name (str, optional): The model name to use. Defaults to "gpt-3.5-turbo".
+        temperature (float, optional): The temperature to use. Defaults to 0.2.
+        stream (bool, optional): Whether to stream the output or not. Defaults to False.
+        """
+        self.template = template
+        self.input_variables = self.get_input_variables()
+        self.message = {"role": role, "content": None}
+        self.model_name = model_name
+        self.temperature = temperature
+        self.stream = stream
         self.logs = []
 
-    def __call__(self, *args, **kwargs):
-        inputs = {}
-        if args:
-            inputs = {
-                key: value
-                for key, value in zip(self.chain.prompt.input_variables, args)
-            }
-        if kwargs:
-            inputs.update(kwargs)
 
+    def get_input_variables(self) -> list:
+        """Get the input variables from the template"""
+        return re.findall(r"\{(\w+)\}", self.template)
+
+    def create_completion(self, inputs: dict) -> str:
+        """Create a GPT completion"""
+        self.message['content'] = self.template.format(**inputs)
+        response = openai.ChatCompletion.create(
+            model=self.model_name,
+            messages=[self.message],
+            temperature=self.temperature,
+            stream=self.stream,
+        )
+        return response
+
+    def stream_output(self, inputs) -> None:
+        """Get stream GPT completion - fun to watch"""
+        response = self.create_completion(inputs)
+        collected_content = ""
+        for chunk in response:
+            chunk_message = chunk['choices'][0]['delta']  
+            collected_content += chunk_message['content'] if 'content' in chunk_message else ''
+            clear_output(wait=True)
+            display(Markdown(collected_content))
+        return collected_content
+
+    def batch_output(self, inputs) -> None:
+        """Get batch GPT completion - not as fun to watch"""
         start_time = time.time()
-        with get_openai_callback() as cb:
-            response = self.chain(inputs)
+        response = self.create_completion(inputs).choices[0]["message"]["content"]
         response_time = time.time() - start_time
-
-        # Store logs in a list of dictionaries
-        log_entry = {
+        self.logs.append({
             "inputs": inputs,
-            "callback": cb,
             "response": response,
             "response_time": response_time,
-        }
-        self.logs.append(log_entry)
+        })
         return response
+
+    def __call__(self, *args, **kwargs) -> str:
+        """Call the model with the given inputs"""
+        inputs = {}
+        if args:
+            inputs = {key: value for key, value in zip(self.input_variables, args)}
+        if kwargs:
+            inputs.update(kwargs)
+
+        if self.stream:
+            return self.stream_output(inputs) 
+        return self.batch_output(inputs)
+            
+
+
```

### Comparing `llm-blocks-0.2.3/llm_blocks.egg-info/PKG-INFO` & `llm-blocks-0.2.4/llm_blocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-blocks
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple interface for creating and managing LLM chains
 Home-page: https://github.com/voynow/llm-blocks
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm-blocks-0.2.3/setup.py` & `llm-blocks-0.2.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="llm-blocks",
-    version="0.2.3",
+    version="0.2.4",
     author="Jamie Voynow",
     author_email="voynow99@gmail.com",
     description="Simple interface for creating and managing LLM chains",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/voynow/llm-blocks",
     packages=find_packages(),
@@ -20,10 +20,7 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
-
-# python setup.py sdist bdist_wheel
-# twine upload dist/*
```

