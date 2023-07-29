# Comparing `tmp/multilogue-0.0.5.tar.gz` & `tmp/multilogue-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multilogue-0.0.5.tar", last modified: Sat Jul 29 19:44:18 2023, max compression
+gzip compressed data, was "multilogue-0.0.6.tar", last modified: Sat Jul 29 21:10:56 2023, max compression
```

## Comparing `multilogue-0.0.5.tar` & `multilogue-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.5/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-07-29 19:44:18.175396 multilogue-0.0.5/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       55 2023-07-02 15:37:04.000000 multilogue-0.0.5/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      689 2023-07-29 19:11:37.000000 multilogue-0.0.5/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-29 19:44:18.175396 multilogue-0.0.5/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/src/multilogue/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-07-29 19:20:27.000000 multilogue-0.0.5/src/multilogue/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1244 2023-07-27 12:09:50.000000 multilogue-0.0.5/src/multilogue/entities.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-07-27 00:36:41.000000 multilogue-0.0.5/src/multilogue/participants.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/src/multilogue/utilities/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      246 2023-07-29 19:42:30.000000 multilogue-0.0.5/src/multilogue/utilities/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1336 2023-07-29 19:42:30.000000 multilogue-0.0.5/src/multilogue/utilities/chatgpt.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/src/multilogue.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-07-29 19:44:18.000000 multilogue-0.0.5/src/multilogue.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      402 2023-07-29 19:44:18.000000 multilogue-0.0.5/src/multilogue.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-29 19:44:18.000000 multilogue-0.0.5/src/multilogue.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       17 2023-07-29 19:44:18.000000 multilogue-0.0.5/src/multilogue.egg-info/requires.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-07-29 19:44:18.000000 multilogue-0.0.5/src/multilogue.egg-info/top_level.txt
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 19:44:18.175396 multilogue-0.0.5/tests/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      345 2023-07-27 12:09:50.000000 multilogue-0.0.5/tests/test_entities.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.955251 multilogue-0.0.6/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.6/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-07-29 21:10:56.955251 multilogue-0.0.6/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       55 2023-07-02 15:37:04.000000 multilogue-0.0.6/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      689 2023-07-29 20:15:07.000000 multilogue-0.0.6/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-29 21:10:56.955251 multilogue-0.0.6/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.951251 multilogue-0.0.6/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.951251 multilogue-0.0.6/src/multilogue/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-07-29 19:20:27.000000 multilogue-0.0.6/src/multilogue/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1244 2023-07-27 12:09:50.000000 multilogue-0.0.6/src/multilogue/entities.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-07-27 00:36:41.000000 multilogue-0.0.6/src/multilogue/participants.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.951251 multilogue-0.0.6/src/multilogue/utilities/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      246 2023-07-29 19:42:30.000000 multilogue-0.0.6/src/multilogue/utilities/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1762 2023-07-29 21:09:58.000000 multilogue-0.0.6/src/multilogue/utilities/chatgpt.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.951251 multilogue-0.0.6/src/multilogue.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-07-29 21:10:56.000000 multilogue-0.0.6/src/multilogue.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      402 2023-07-29 21:10:56.000000 multilogue-0.0.6/src/multilogue.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-29 21:10:56.000000 multilogue-0.0.6/src/multilogue.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       17 2023-07-29 21:10:56.000000 multilogue-0.0.6/src/multilogue.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-07-29 21:10:56.000000 multilogue-0.0.6/src/multilogue.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.951251 multilogue-0.0.6/tests/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      345 2023-07-27 12:09:50.000000 multilogue-0.0.6/tests/test_entities.py
```

### Comparing `multilogue-0.0.5/LICENSE` & `multilogue-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.5/PKG-INFO` & `multilogue-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilogue
-Version: 0.0.5
+Version: 0.0.6
 Summary: Multilogue
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/multilogue
 Project-URL: Bug Tracker, https://github.com/multilogue/multilogue/issues
 Keywords: multilogue,multilectic,conversation,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multilogue-0.0.5/pyproject.toml` & `multilogue-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "multilogue"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Multilogue"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `multilogue-0.0.5/src/multilogue/entities.py` & `multilogue-0.0.6/src/multilogue/entities.py`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.5/src/multilogue/utilities/chatgpt.py` & `multilogue-0.0.6/src/multilogue/utilities/chatgpt.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,28 +13,44 @@
 
 organization    = environ.get("OPENAI_ORGANIZATION")
 api_base        = environ.get("OPENAI_API_BASE", "https://api.openai.com/v1")
 api_type        = environ.get("OPENAI_API_TYPE", "open_ai")
 default_model   = environ.get("OPENAI_DEFAULT_MODEL", "gpt-3.5-turbo-0613")
 
 
-def answer(messages, functions=None, function_call=None, model=default_model):
+def answer( messages,
+            functions=None,
+            function_call=None,
+            model=default_model,
+            **kwargs):
+
+    """A simple requests call to ChatGPT.
+        kwargs:
+            temperature     = 0 to 1.0
+            top_p           = 0.0 to 1.0
+            n               = 1 to ...
+            frequency_penalty = -2.0 to 2.0
+            presence_penalty = -2.0 to 2.0
+            max_tokens      = number of tokens
+    """
     headers = {
         "Content-Type": "application/json",
         "Authorization": "Bearer " + api_key,
+        "Organization": organization
     }
-    json_data = {"model": model, "messages": messages}
+    json_data = {"model": model, "messages": messages} | kwargs
     if functions is not None:
         json_data.update({"functions": functions})
     if function_call is not None:
         json_data.update({"function_call": function_call})
     try:
         response = requests.post(
             f"{api_base}/chat/completions",
             headers=headers,
             json=json_data,
         )
+
         return response
     except Exception as e:
         print("Unable to generate ChatCompletion response")
         print(f"Exception: {e}")
         return e
```

### Comparing `multilogue-0.0.5/src/multilogue.egg-info/PKG-INFO` & `multilogue-0.0.6/src/multilogue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilogue
-Version: 0.0.5
+Version: 0.0.6
 Summary: Multilogue
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/multilogue
 Project-URL: Bug Tracker, https://github.com/multilogue/multilogue/issues
 Keywords: multilogue,multilectic,conversation,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

