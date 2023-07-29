# Comparing `tmp/fukkatsu-0.0.8.tar.gz` & `tmp/fukkatsu-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fukkatsu-0.0.8.tar", last modified: Fri Jun 23 00:15:05 2023, max compression
+gzip compressed data, was "fukkatsu-0.0.9.tar", last modified: Sat Jul 29 02:32:51 2023, max compression
```

## Comparing `fukkatsu-0.0.8.tar` & `fukkatsu-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.842525 fukkatsu-0.0.8/
--rw-rw-rw-   0        0        0     1387 2023-06-18 20:59:20.000000 fukkatsu-0.0.8/CHANGELOG.md
--rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    34713 2023-06-23 00:15:05.826902 fukkatsu-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    34072 2023-06-22 18:47:10.000000 fukkatsu-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.733149 fukkatsu-0.0.8/fukkatsu/
--rw-rw-rw-   0        0        0    14328 2023-06-23 00:04:08.000000 fukkatsu-0.0.8/fukkatsu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.780022 fukkatsu-0.0.8/fukkatsu/memory/
--rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.8/fukkatsu/memory/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.8/fukkatsu/memory/manage.py
--rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.8/fukkatsu/memory/short.py
-drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.795649 fukkatsu-0.0.8/fukkatsu/observer/
--rw-rw-rw-   0        0        0       40 2023-06-15 23:48:34.000000 fukkatsu-0.0.8/fukkatsu/observer/__init__.py
--rw-rw-rw-   0        0        0     1064 2023-06-21 22:36:45.000000 fukkatsu-0.0.8/fukkatsu/observer/tracker.py
-drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.811275 fukkatsu-0.0.8/fukkatsu/utils/
--rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.8/fukkatsu/utils/__init__.py
--rw-rw-rw-   0        0        0     4948 2023-06-21 01:01:09.000000 fukkatsu-0.0.8/fukkatsu/utils/helper.py
--rw-rw-rw-   0        0        0     4300 2023-06-23 00:04:08.000000 fukkatsu-0.0.8/fukkatsu/utils/medic.py
--rw-rw-rw-   0        0        0     3812 2023-06-21 00:15:16.000000 fukkatsu-0.0.8/fukkatsu/utils/prompt.py
-drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.764400 fukkatsu-0.0.8/fukkatsu.egg-info/
--rw-rw-rw-   0        0        0    34713 2023-06-23 00:15:05.000000 fukkatsu-0.0.8/fukkatsu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-06-23 00:15:05.000000 fukkatsu-0.0.8/fukkatsu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 00:15:05.000000 fukkatsu-0.0.8/fukkatsu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-23 00:15:05.000000 fukkatsu-0.0.8/fukkatsu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 00:15:05.000000 fukkatsu-0.0.8/fukkatsu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 00:15:05.842525 fukkatsu-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-06-20 23:55:09.000000 fukkatsu-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 02:32:51.839494 fukkatsu-0.0.9/
+-rw-rw-rw-   0        0        0     1610 2023-07-03 21:52:19.000000 fukkatsu-0.0.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    34713 2023-07-29 02:32:51.823845 fukkatsu-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    34072 2023-06-22 18:47:10.000000 fukkatsu-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 02:32:51.711568 fukkatsu-0.0.9/fukkatsu/
+-rw-rw-rw-   0        0        0    14493 2023-07-29 02:29:21.000000 fukkatsu-0.0.9/fukkatsu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 02:32:51.767684 fukkatsu-0.0.9/fukkatsu/memory/
+-rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.9/fukkatsu/memory/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.9/fukkatsu/memory/manage.py
+-rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.9/fukkatsu/memory/short.py
+drwxrwxrwx   0        0        0        0 2023-07-29 02:32:51.783684 fukkatsu-0.0.9/fukkatsu/observer/
+-rw-rw-rw-   0        0        0       40 2023-06-15 23:48:34.000000 fukkatsu-0.0.9/fukkatsu/observer/__init__.py
+-rw-rw-rw-   0        0        0     1064 2023-06-21 22:36:45.000000 fukkatsu-0.0.9/fukkatsu/observer/tracker.py
+drwxrwxrwx   0        0        0        0 2023-07-29 02:32:51.817327 fukkatsu-0.0.9/fukkatsu/utils/
+-rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.9/fukkatsu/utils/__init__.py
+-rw-rw-rw-   0        0        0     4948 2023-06-26 01:15:01.000000 fukkatsu-0.0.9/fukkatsu/utils/helper.py
+-rw-rw-rw-   0        0        0     4647 2023-07-29 02:29:21.000000 fukkatsu-0.0.9/fukkatsu/utils/medic.py
+-rw-rw-rw-   0        0        0     3812 2023-06-21 00:15:16.000000 fukkatsu-0.0.9/fukkatsu/utils/prompt.py
+drwxrwxrwx   0        0        0        0 2023-07-29 02:32:51.751684 fukkatsu-0.0.9/fukkatsu.egg-info/
+-rw-rw-rw-   0        0        0    34713 2023-07-29 02:32:51.000000 fukkatsu-0.0.9/fukkatsu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-07-29 02:32:51.000000 fukkatsu-0.0.9/fukkatsu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 02:32:51.000000 fukkatsu-0.0.9/fukkatsu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-29 02:32:51.000000 fukkatsu-0.0.9/fukkatsu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 02:32:51.000000 fukkatsu-0.0.9/fukkatsu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 02:32:51.839494 fukkatsu-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-06-26 23:22:33.000000 fukkatsu-0.0.9/setup.py
```

### Comparing `fukkatsu-0.0.8/CHANGELOG.md` & `fukkatsu-0.0.9/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -36,8 +36,20 @@
     - short-term-memory will now only save functions that executed successfully
 - live counter fix
     - removed unintended extra live
 - logging formatting enhanced + api call logging added
 
 ### 0.0.7
 
-- fix of "Attempt `x` to reanimate" logging message
+- fix of "Attempt `x` to reanimate" logging message
+
+
+### 0.0.8
+
+- new `stalk` decorator
+- increased unittest coverage
+- provided more examples in documentation
+
+### 0.0.9
+
+- improved testing
+- `reset_openai_key` added to overwrite openai key set by env variable
```

### Comparing `fukkatsu-0.0.8/LICENSE` & `fukkatsu-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.8/PKG-INFO` & `fukkatsu-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fukkatsu-0.0.8/README.md` & `fukkatsu-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.8/fukkatsu/__init__.py` & `fukkatsu-0.0.9/fukkatsu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 import copy
 import functools
 import traceback
 
 from fukkatsu.memory import SHORT_TERM_MEMORY
 from fukkatsu.observer.tracker import track
 from fukkatsu.utils import (check_and_install_libraries, extract_imports,
                             extract_text_between_pipes,
                             insert_string_after_colon, remove_trace_lines,
                             remove_wrapper_name, rename_function,
                             return_input_arguments, return_source_code,
                             sampler)
-from fukkatsu.utils.medic import defibrillate, enhance, stalker, twin
+from fukkatsu.utils.medic import (defibrillate, enhance, overwrite_openai_key,
+                                  set_openai_key, stalker, twin)
+
+set_openai_key()
+
+
+def reset_openai_key(key: str):
+    overwrite_openai_key(key)
 
 
 def resurrect(
     lives: int = 1,
     additional_req: str = "",
     allow_installs: bool = False,
     active_twin: bool = False,
@@ -265,15 +272,15 @@
 
         return wrapper
 
     return _mutate
 
 
 def stalk(
-    likelihood: float = 1,
+    likelihood: float = 1.0,
     additional_req: str = "",
     allow_installs: bool = False,
     active_twin: bool = False,
     llm: dict = {"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"},
     temperature: dict = {"primary": 0.1, "secondary": 0.1},
 ):
     def _stalk(func):
```

### Comparing `fukkatsu-0.0.8/fukkatsu/memory/manage.py` & `fukkatsu-0.0.9/fukkatsu/memory/manage.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.8/fukkatsu/observer/tracker.py` & `fukkatsu-0.0.9/fukkatsu/observer/tracker.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.8/fukkatsu/utils/helper.py` & `fukkatsu-0.0.9/fukkatsu/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.8/fukkatsu/utils/medic.py` & `fukkatsu-0.0.9/fukkatsu/utils/medic.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,20 +5,31 @@
 from fukkatsu.observer.tracker import track
 from fukkatsu.utils.prompt import (ADDITIONAL, CONTEXT, CONTEXT_MUTATE,
                                    CONTEXT_STALKER, CONTEXT_TWIN,
                                    OUTPUT_CONSTRAINTS,
                                    OUTPUT_CONSTRAINTS_MUTATE,
                                    OUTPUT_CONSTRAINTS_TWIN)
 
-try:
-    openai.api_key = os.environ.get("OPENAI_API_KEY")
-    print("OPENAI_API_KEY found in environment variables.")
-except:
-    print("OPENAI_API_KEY not found in environment variables.")
-    raise Exception("OPENAI_API_KEY not found in environment variables.")
+
+def set_openai_key():
+    track.warning("Setting OPENAI_API_KEY")
+    try:
+        openai.api_key = os.environ.get("OPENAI_API_KEY")
+        track.warning("OPENAI_API_KEY found in environment variables.")
+    except:
+        track.error("OPENAI_API_KEY not found in environment variables.")
+
+
+def overwrite_openai_key(key: str):
+    if type(key) != str:
+        track.error("Invalid Key format. OPENAI_API_KEY not overwritten.")
+        raise Exception("Invalid Key format. OPENAI_API_KEY not overwritten.")
+    else:
+        openai.api_key = key
+        track.warning("OPENAI_API_KEY overwritten.")
 
 
 def defibrillate(
     inputs: str,
     faulty_function: str,
     error_trace: str,
     model: str,
```

### Comparing `fukkatsu-0.0.8/fukkatsu/utils/prompt.py` & `fukkatsu-0.0.9/fukkatsu/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.8/fukkatsu.egg-info/PKG-INFO` & `fukkatsu-0.0.9/fukkatsu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fukkatsu-0.0.8/setup.py` & `fukkatsu-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/fukkatsu",
     description="A python library for runtime LLM supported code corrections.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="fukkatsu",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(include=["fukkatsu", "fukkatsu.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
         "openai >= 0.27.5, <= 0.28",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
```

