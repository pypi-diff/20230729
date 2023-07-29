# Comparing `tmp/promptengine_catapult-0.1.2.tar.gz` & `tmp/promptengine_catapult-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptengine_catapult-0.1.2.tar", last modified: Sat Jul 29 07:20:00 2023, max compression
+gzip compressed data, was "promptengine_catapult-0.1.3.tar", last modified: Sat Jul 29 07:52:54 2023, max compression
```

## Comparing `promptengine_catapult-0.1.2.tar` & `promptengine_catapult-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 07:20:00.619855 promptengine_catapult-0.1.2/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-07-29 04:57:06.000000 promptengine_catapult-0.1.2/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 07:20:00.619855 promptengine_catapult-0.1.2/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.2/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 07:20:00.619855 promptengine_catapult-0.1.2/promptengine_catapult/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.2/promptengine_catapult/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.2/promptengine_catapult/config.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6457 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.2/promptengine_catapult/prompt_engine.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      805 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.2/promptengine_catapult/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 07:20:00.619855 promptengine_catapult-0.1.2/promptengine_catapult.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 07:20:00.000000 promptengine_catapult-0.1.2/promptengine_catapult.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      396 2023-07-29 07:20:00.000000 promptengine_catapult-0.1.2/promptengine_catapult.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-07-29 07:20:00.000000 promptengine_catapult-0.1.2/promptengine_catapult.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-07-29 07:20:00.000000 promptengine_catapult-0.1.2/promptengine_catapult.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-07-29 07:20:00.000000 promptengine_catapult-0.1.2/promptengine_catapult.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-07-29 07:20:00.623855 promptengine_catapult-0.1.2/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-07-29 07:15:46.000000 promptengine_catapult-0.1.2/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 07:52:54.406177 promptengine_catapult-0.1.3/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-07-29 04:57:06.000000 promptengine_catapult-0.1.3/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 07:52:54.406177 promptengine_catapult-0.1.3/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.3/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 07:52:54.406177 promptengine_catapult-0.1.3/promptengine_catapult/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.3/promptengine_catapult/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.3/promptengine_catapult/config.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6499 2023-07-29 07:52:03.000000 promptengine_catapult-0.1.3/promptengine_catapult/prompt_engine.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      805 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.3/promptengine_catapult/utils.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 07:52:54.406177 promptengine_catapult-0.1.3/promptengine_catapult.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 07:52:54.000000 promptengine_catapult-0.1.3/promptengine_catapult.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      396 2023-07-29 07:52:54.000000 promptengine_catapult-0.1.3/promptengine_catapult.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-07-29 07:52:54.000000 promptengine_catapult-0.1.3/promptengine_catapult.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-07-29 07:52:54.000000 promptengine_catapult-0.1.3/promptengine_catapult.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-07-29 07:52:54.000000 promptengine_catapult-0.1.3/promptengine_catapult.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-07-29 07:52:54.406177 promptengine_catapult-0.1.3/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-07-29 07:52:34.000000 promptengine_catapult-0.1.3/setup.py
```

### Comparing `promptengine_catapult-0.1.2/LICENSE` & `promptengine_catapult-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.2/PKG-INFO` & `promptengine_catapult-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine_catapult
-Version: 0.1.2
+Version: 0.1.3
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.1.2/README.md` & `promptengine_catapult-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.2/promptengine_catapult/config.py` & `promptengine_catapult-0.1.3/promptengine_catapult/config.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.2/promptengine_catapult/prompt_engine.py` & `promptengine_catapult-0.1.3/promptengine_catapult/prompt_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 os.chdir(os.path.dirname(os.path.abspath(__file__)))
 import openai
 import redis
 import json
 import tiktoken
 import requests
-import config
+#import config
+from promptengine_catapult import config
 from promptengine_catapult.utils import *
 import logging
 
 from dotenv import load_dotenv
 import io
 import openai
 from pydub import AudioSegment
```

### Comparing `promptengine_catapult-0.1.2/promptengine_catapult/utils.py` & `promptengine_catapult-0.1.3/promptengine_catapult/utils.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.2/promptengine_catapult.egg-info/PKG-INFO` & `promptengine_catapult-0.1.3/promptengine_catapult.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine-catapult
-Version: 0.1.2
+Version: 0.1.3
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.1.2/setup.py` & `promptengine_catapult-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 DESCRIPTION = "PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model."
 LONG_DESCRIPTION = """
 PromptEngine is a Python library that provides an interface for conducting interview sessions using OpenAI's ChatGPT model. It allows you to interact with the AI assistant to simulate interview conversations and generate responses based on candidate input.
 """
 
 # Setting up
 setup(
```

