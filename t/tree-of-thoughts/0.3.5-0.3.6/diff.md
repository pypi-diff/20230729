# Comparing `tmp/tree-of-thoughts-0.3.5.tar.gz` & `tmp/tree-of-thoughts-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.3.5.tar", last modified: Sat Jul 29 19:03:42 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.3.6.tar", last modified: Sat Jul 29 19:10:48 2023, max compression
```

## Comparing `tree-of-thoughts-0.3.5.tar` & `tree-of-thoughts-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:42.836820 tree-of-thoughts-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-29 19:03:42.836820 tree-of-thoughts-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 19:03:42.836820 tree-of-thoughts-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:42.832820 tree-of-thoughts-0.3.5/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/abstract_language_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/guidance_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/huggingface_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/langchain_tot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/openai_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/text_generation_web_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:42.836820 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-29 19:03:42.000000 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-29 19:03:42.000000 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 19:03:42.000000 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 19:03:42.000000 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 19:03:42.000000 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:10:48.837896 tree-of-thoughts-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 19:10:35.000000 tree-of-thoughts-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-29 19:10:48.837896 tree-of-thoughts-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-07-29 19:10:35.000000 tree-of-thoughts-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 19:10:48.837896 tree-of-thoughts-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:10:48.837896 tree-of-thoughts-0.3.6/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/tree_of_thoughts/langchain_tot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:10:48.837896 tree-of-thoughts-0.3.6/tree_of_thoughts/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/tree_of_thoughts/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/tree_of_thoughts/models/abstract_language_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/tree_of_thoughts/models/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/tree_of_thoughts/models/guidance_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/tree_of_thoughts/models/huggingface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/tree_of_thoughts/models/openai_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/tree_of_thoughts/text_generation_web_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-07-29 19:10:36.000000 tree-of-thoughts-0.3.6/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:10:48.837896 tree-of-thoughts-0.3.6/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-29 19:10:48.000000 tree-of-thoughts-0.3.6/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-29 19:10:48.000000 tree-of-thoughts-0.3.6/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 19:10:48.000000 tree-of-thoughts-0.3.6/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 19:10:48.000000 tree-of-thoughts-0.3.6/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 19:10:48.000000 tree-of-thoughts-0.3.6/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.3.5/LICENSE` & `tree-of-thoughts-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.5/PKG-INFO` & `tree-of-thoughts-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.3.5
+Version: 0.3.6
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.3.5/README.md` & `tree-of-thoughts-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.5/setup.py` & `tree-of-thoughts-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.3.5',
+  version = '0.3.6',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.3.5/tree_of_thoughts/guidance_model.py` & `tree-of-thoughts-0.3.6/tree_of_thoughts/models/guidance_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import guidance
-from tree_of_thoughts.abstract_language_model import AbstractLanguageModel
+from tree_of_thoughts.models.abstract_language_model import AbstractLanguageModel
 import time
 import os
 import openai
 
 
 class GuidanceLanguageModel(AbstractLanguageModel):
     def __init__(self, model, strategy="cot", evaluation_strategy="value", enable_ReAct_prompting=False):
```

### Comparing `tree-of-thoughts-0.3.5/tree_of_thoughts/huggingface_model.py` & `tree-of-thoughts-0.3.6/tree_of_thoughts/models/huggingface_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from transformers import pipeline
-from tree_of_thoughts.abstract_language_model import AbstractLanguageModel
+from tree_of_thoughts.models.abstract_language_model import AbstractLanguageModel
 
 
 class HuggingLanguageModel(AbstractLanguageModel):
     def __init__(self, model_name, model_tokenizer=None, verbose=False):
         self.model = AutoModelForCausalLM.from_pretrained(model_name)
         self.tokenizer = AutoTokenizer.from_pretrained(model_tokenizer or model_name)
         self.verbose = verbose
```

### Comparing `tree-of-thoughts-0.3.5/tree_of_thoughts/langchain_tot.py` & `tree-of-thoughts-0.3.6/tree_of_thoughts/langchain_tot.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.5/tree_of_thoughts/openai_models.py` & `tree-of-thoughts-0.3.6/tree_of_thoughts/models/openai_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import openai
 import time
-from  tree_of_thoughts.abstract_language_model import AbstractLanguageModel
+from  tree_of_thoughts.models.abstract_language_model import AbstractLanguageModel
 import concurrent.futures
 import logging 
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
```

### Comparing `tree-of-thoughts-0.3.5/tree_of_thoughts/text_generation_web_ui.py` & `tree-of-thoughts-0.3.6/tree_of_thoughts/text_generation_web_ui.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.5/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.3.6/tree_of_thoughts/treeofthoughts.py`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.3.6/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.3.5
+Version: 0.3.6
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

