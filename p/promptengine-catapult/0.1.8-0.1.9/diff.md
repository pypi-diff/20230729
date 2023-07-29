# Comparing `tmp/promptengine_catapult-0.1.8.tar.gz` & `tmp/promptengine_catapult-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptengine_catapult-0.1.8.tar", last modified: Sat Jul 29 18:13:28 2023, max compression
+gzip compressed data, was "promptengine_catapult-0.1.9.tar", last modified: Sat Jul 29 20:02:21 2023, max compression
```

## Comparing `promptengine_catapult-0.1.8.tar` & `promptengine_catapult-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 18:13:28.954076 promptengine_catapult-0.1.8/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-07-29 04:57:06.000000 promptengine_catapult-0.1.8/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 18:13:28.954076 promptengine_catapult-0.1.8/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.8/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 18:13:28.954076 promptengine_catapult-0.1.8/promptengine_catapult/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.8/promptengine_catapult/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.8/promptengine_catapult/config.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8356 2023-07-29 18:13:10.000000 promptengine_catapult-0.1.8/promptengine_catapult/prompt_engine.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      832 2023-07-29 07:58:05.000000 promptengine_catapult-0.1.8/promptengine_catapult/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 18:13:28.954076 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 18:13:28.000000 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      396 2023-07-29 18:13:28.000000 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-07-29 18:13:28.000000 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-07-29 18:13:28.000000 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-07-29 18:13:28.000000 promptengine_catapult-0.1.8/promptengine_catapult.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-07-29 18:13:28.958076 promptengine_catapult-0.1.8/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-07-29 18:13:17.000000 promptengine_catapult-0.1.8/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 20:02:21.124287 promptengine_catapult-0.1.9/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-07-29 04:57:06.000000 promptengine_catapult-0.1.9/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 20:02:21.124287 promptengine_catapult-0.1.9/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.9/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 20:02:21.120287 promptengine_catapult-0.1.9/promptengine_catapult/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.9/promptengine_catapult/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-07-29 07:14:51.000000 promptengine_catapult-0.1.9/promptengine_catapult/config.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8455 2023-07-29 19:58:22.000000 promptengine_catapult-0.1.9/promptengine_catapult/prompt_engine.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      832 2023-07-29 07:58:05.000000 promptengine_catapult-0.1.9/promptengine_catapult/utils.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-29 20:02:21.120287 promptengine_catapult-0.1.9/promptengine_catapult.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-07-29 20:02:21.000000 promptengine_catapult-0.1.9/promptengine_catapult.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      396 2023-07-29 20:02:21.000000 promptengine_catapult-0.1.9/promptengine_catapult.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-07-29 20:02:21.000000 promptengine_catapult-0.1.9/promptengine_catapult.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-07-29 20:02:21.000000 promptengine_catapult-0.1.9/promptengine_catapult.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-07-29 20:02:21.000000 promptengine_catapult-0.1.9/promptengine_catapult.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-07-29 20:02:21.124287 promptengine_catapult-0.1.9/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-07-29 20:02:01.000000 promptengine_catapult-0.1.9/setup.py
```

### Comparing `promptengine_catapult-0.1.8/LICENSE` & `promptengine_catapult-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.8/PKG-INFO` & `promptengine_catapult-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine_catapult
-Version: 0.1.8
+Version: 0.1.9
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.1.8/README.md` & `promptengine_catapult-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.8/promptengine_catapult/config.py` & `promptengine_catapult-0.1.9/promptengine_catapult/config.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.8/promptengine_catapult/prompt_engine.py` & `promptengine_catapult-0.1.9/promptengine_catapult/prompt_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,13 +220,15 @@
         # Extract the rating value and feedback text
         Overall_Rating = rating_line.split(': ')[1]
         Overall_Feedback = feedback_line.split(': ')[1]
         
         return {
             'system_message': system_message,
             'Overall Rating': Overall_Rating,
-            'Overall Feedback' : Overall_Feedback
+            'Overall Feedback' : Overall_Feedback,
+            'Questions':questions_answered,
+            'Answers':answers[:min_convo]            
         }
 
 
 # TO Do:
 # redis timeout
```

### Comparing `promptengine_catapult-0.1.8/promptengine_catapult/utils.py` & `promptengine_catapult-0.1.9/promptengine_catapult/utils.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.1.8/promptengine_catapult.egg-info/PKG-INFO` & `promptengine_catapult-0.1.9/promptengine_catapult.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine-catapult
-Version: 0.1.8
+Version: 0.1.9
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.1.8/setup.py` & `promptengine_catapult-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 DESCRIPTION = "PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model."
 LONG_DESCRIPTION = """
 PromptEngine is a Python library that provides an interface for conducting interview sessions using OpenAI's ChatGPT model. It allows you to interact with the AI assistant to simulate interview conversations and generate responses based on candidate input.
 """
 
 # Setting up
 setup(
```

