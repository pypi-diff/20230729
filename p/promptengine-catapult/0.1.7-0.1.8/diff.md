# Comparing `tmp/promptengine_catapult-0.1.7.tar.gz` & `tmp/promptengine_catapult-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptengine_catapult-0.1.7.tar", last modified: Sat Jul 29 18:07:22 2023, max compression
+gzip compressed data, was "promptengine_catapult-0.1.8.tar", last modified: Sat Jul 29 18:13:28 2023, max compression
```

## Comparing `promptengine_catapult-0.1.7.tar` & `promptengine_catapult-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 18:07:22.218140 promptengine_catapult-0.1.7/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-07-29 04:57:06.000000 promptengine_catapult-0.1.7/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 18:07:22.218140 promptengine_catapult-0.1.7/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.7/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 18:07:22.218140 promptengine_catapult-0.1.7/promptengine_catapult/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.7/promptengine_catapult/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.7/promptengine_catapult/config.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8275 2023-07-29 18:06:50.000000 promptengine_catapult-0.1.7/promptengine_catapult/prompt_engine.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      832 2023-07-29 07:58:05.000000 promptengine_catapult-0.1.7/promptengine_catapult/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 18:07:22.218140 promptengine_catapult-0.1.7/promptengine_catapult.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 18:07:22.000000 promptengine_catapult-0.1.7/promptengine_catapult.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      396 2023-07-29 18:07:22.000000 promptengine_catapult-0.1.7/promptengine_catapult.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-07-29 18:07:22.000000 promptengine_catapult-0.1.7/promptengine_catapult.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-07-29 18:07:22.000000 promptengine_catapult-0.1.7/promptengine_catapult.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-07-29 18:07:22.000000 promptengine_catapult-0.1.7/promptengine_catapult.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-07-29 18:07:22.218140 promptengine_catapult-0.1.7/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-07-29 18:07:17.000000 promptengine_catapult-0.1.7/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 18:13:28.954076 promptengine_catapult-0.1.8/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-07-29 04:57:06.000000 promptengine_catapult-0.1.8/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 18:13:28.954076 promptengine_catapult-0.1.8/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.8/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 18:13:28.954076 promptengine_catapult-0.1.8/promptengine_catapult/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.8/promptengine_catapult/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.8/promptengine_catapult/config.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8356 2023-07-29 18:13:10.000000 promptengine_catapult-0.1.8/promptengine_catapult/prompt_engine.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      832 2023-07-29 07:58:05.000000 promptengine_catapult-0.1.8/promptengine_catapult/utils.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 18:13:28.954076 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 18:13:28.000000 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      396 2023-07-29 18:13:28.000000 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-07-29 18:13:28.000000 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-07-29 18:13:28.000000 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-07-29 18:13:28.000000 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-07-29 18:13:28.958076 promptengine_catapult-0.1.8/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-07-29 18:13:17.000000 promptengine_catapult-0.1.8/setup.py
```

### Comparing `promptengine_catapult-0.1.7/LICENSE` & `promptengine_catapult-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.7/PKG-INFO` & `promptengine_catapult-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine_catapult
-Version: 0.1.7
+Version: 0.1.8
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.1.7/README.md` & `promptengine_catapult-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.7/promptengine_catapult/config.py` & `promptengine_catapult-0.1.8/promptengine_catapult/config.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.7/promptengine_catapult/prompt_engine.py` & `promptengine_catapult-0.1.8/promptengine_catapult/prompt_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import logging
 
 from dotenv import load_dotenv
 import io
 import openai
 from pydub import AudioSegment
 from pydub.playback import play
+import pandas as pd
 
 
 # setting logging
 logging.basicConfig(
     level=(logging.DEBUG if os.getenv("LOG_MODE") == "DEBUG" else logging.INFO)
 )
 
@@ -188,18 +189,19 @@
         messages.append({"role": "system", "content": system_msg})
 
         questions = self.redis_prompt.lrange(interview_id+'_questions', 0, - 1)
         answers = self.redis_prompt.lrange(interview_id+'_answers', 0, - 1)
         questions=questions[::-1]
         answers=answers[::-1]
 
-        questions_answered=questions[:len(answers)]
+        min_convo=min(len(answers), len(questions))
+        questions_answered=questions[:min_convo]
         
         df=pd.DataFrame({'Questions':questions_answered,
-                        'Answers':answers})
+                        'Answers':answers[:min_convo]})
         
         result1=df.to_dict('index')
         
         messages.append({"role": "user", "content": str(result1)})
 
         response = openai.ChatCompletion.create(
             model=model_used,
```

### Comparing `promptengine_catapult-0.1.7/promptengine_catapult/utils.py` & `promptengine_catapult-0.1.8/promptengine_catapult/utils.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.7/promptengine_catapult.egg-info/PKG-INFO` & `promptengine_catapult-0.1.8/promptengine_catapult.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine-catapult
-Version: 0.1.7
+Version: 0.1.8
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.1.7/setup.py` & `promptengine_catapult-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 DESCRIPTION = "PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model."
 LONG_DESCRIPTION = """
 PromptEngine is a Python library that provides an interface for conducting interview sessions using OpenAI's ChatGPT model. It allows you to interact with the AI assistant to simulate interview conversations and generate responses based on candidate input.
 """
 
 # Setting up
 setup(
```

