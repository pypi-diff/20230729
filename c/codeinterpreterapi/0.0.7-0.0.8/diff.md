# Comparing `tmp/codeinterpreterapi-0.0.7.tar.gz` & `tmp/codeinterpreterapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeinterpreterapi-0.0.7.tar", max compression
+gzip compressed data, was "codeinterpreterapi-0.0.8.tar", max compression
```

## Comparing `codeinterpreterapi-0.0.7.tar` & `codeinterpreterapi-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.7/LICENSE
--rw-r--r--   0        0        0     4364 2023-07-27 12:56:18.816462 codeinterpreterapi-0.0.7/README.md
--rw-r--r--   0        0        0      104 2023-07-27 17:09:11.503788 codeinterpreterapi-0.0.7/codeinterpreterapi/__init__.py
--rw-r--r--   0        0        0      929 2023-07-27 17:09:11.504081 codeinterpreterapi-0.0.7/codeinterpreterapi/callbacks.py
--rw-r--r--   0        0        0        0 2023-07-27 17:09:11.504186 codeinterpreterapi-0.0.7/codeinterpreterapi/chains/__init__.py
--rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.7/codeinterpreterapi/chains/functions_agent.py
--rw-r--r--   0        0        0     1578 2023-07-27 17:09:11.504417 codeinterpreterapi-0.0.7/codeinterpreterapi/chains/modifications_check.py
--rw-r--r--   0        0        0      977 2023-07-27 17:09:11.504941 codeinterpreterapi-0.0.7/codeinterpreterapi/chains/remove_download_link.py
--rw-r--r--   0        0        0      390 2023-07-17 19:38:21.218647 codeinterpreterapi-0.0.7/codeinterpreterapi/config.py
--rw-r--r--   0        0        0      225 2023-07-17 11:27:36.915415 codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/__init__.py
--rw-r--r--   0        0        0     1379 2023-07-17 11:23:07.801403 codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/modifications_check.py
--rw-r--r--   0        0        0      959 2023-07-17 11:26:26.313924 codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/remove_dl_link.py
--rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/system_message.py
--rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.7/codeinterpreterapi/schema/__init__.py
--rw-r--r--   0        0        0     2385 2023-07-27 12:56:18.814797 codeinterpreterapi-0.0.7/codeinterpreterapi/schema/file.py
--rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.7/codeinterpreterapi/schema/input.py
--rw-r--r--   0        0        0      629 2023-07-14 17:11:05.960810 codeinterpreterapi-0.0.7/codeinterpreterapi/schema/response.py
--rw-r--r--   0        0        0     8266 2023-07-27 17:11:47.122779 codeinterpreterapi-0.0.7/codeinterpreterapi/session.py
--rw-r--r--   0        0        0      686 2023-07-27 17:16:10.970203 codeinterpreterapi-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5259 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4364 2023-07-29 19:51:57.281872 codeinterpreterapi-0.0.8/README.md
+-rw-r--r--   0        0        0      104 2023-07-29 19:51:57.279068 codeinterpreterapi-0.0.8/codeinterpreterapi/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-29 19:51:57.279769 codeinterpreterapi-0.0.8/codeinterpreterapi/callbacks.py
+-rw-r--r--   0        0        0        0 2023-07-29 19:51:57.277704 codeinterpreterapi-0.0.8/codeinterpreterapi/chains/__init__.py
+-rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.8/codeinterpreterapi/chains/functions_agent.py
+-rw-r--r--   0        0        0     1578 2023-07-29 19:51:57.279319 codeinterpreterapi-0.0.8/codeinterpreterapi/chains/modifications_check.py
+-rw-r--r--   0        0        0      977 2023-07-29 19:51:57.279378 codeinterpreterapi-0.0.8/codeinterpreterapi/chains/remove_download_link.py
+-rw-r--r--   0        0        0      390 2023-07-17 19:38:21.218647 codeinterpreterapi-0.0.8/codeinterpreterapi/config.py
+-rw-r--r--   0        0        0      225 2023-07-29 19:51:57.279480 codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/__init__.py
+-rw-r--r--   0        0        0     1379 2023-07-29 19:51:57.279579 codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/modifications_check.py
+-rw-r--r--   0        0        0      959 2023-07-17 11:26:26.313924 codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/remove_dl_link.py
+-rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/system_message.py
+-rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.8/codeinterpreterapi/schema/__init__.py
+-rw-r--r--   0        0        0     2385 2023-07-27 12:56:18.814797 codeinterpreterapi-0.0.8/codeinterpreterapi/schema/file.py
+-rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.8/codeinterpreterapi/schema/input.py
+-rw-r--r--   0        0        0      629 2023-07-29 19:51:57.279665 codeinterpreterapi-0.0.8/codeinterpreterapi/schema/response.py
+-rw-r--r--   0        0        0     8266 2023-07-29 19:51:57.279122 codeinterpreterapi-0.0.8/codeinterpreterapi/session.py
+-rw-r--r--   0        0        0      681 2023-07-29 19:58:48.997254 codeinterpreterapi-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.8/PKG-INFO
```

### Comparing `codeinterpreterapi-0.0.7/LICENSE` & `codeinterpreterapi-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/README.md` & `codeinterpreterapi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/codeinterpreterapi/callbacks.py` & `codeinterpreterapi-0.0.8/codeinterpreterapi/callbacks.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/codeinterpreterapi/chains/functions_agent.py` & `codeinterpreterapi-0.0.8/codeinterpreterapi/chains/functions_agent.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/codeinterpreterapi/chains/modifications_check.py` & `codeinterpreterapi-0.0.8/codeinterpreterapi/chains/modifications_check.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/codeinterpreterapi/chains/remove_download_link.py` & `codeinterpreterapi-0.0.8/codeinterpreterapi/chains/remove_download_link.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/modifications_check.py` & `codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/modifications_check.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/remove_dl_link.py` & `codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/remove_dl_link.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/system_message.py` & `codeinterpreterapi-0.0.8/codeinterpreterapi/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/codeinterpreterapi/schema/file.py` & `codeinterpreterapi-0.0.8/codeinterpreterapi/schema/file.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/codeinterpreterapi/schema/response.py` & `codeinterpreterapi-0.0.8/codeinterpreterapi/schema/response.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/codeinterpreterapi/session.py` & `codeinterpreterapi-0.0.8/codeinterpreterapi/session.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.7/pyproject.toml` & `codeinterpreterapi-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "codeinterpreterapi"
-version = "0.0.7"
+version = "0.0.8"
 description = "CodeInterpreterAPI is an unofficial and open source python interface for the ChatGPT CodeInterpreter."
-authors = ["Shroominic <pleurae-berets.0u@icloud.com>"]
+authors = ["Shroominic <contact@shroominic.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 python-dotenv = "^1.0.0"
 openai = "^0.27.8"
 langchain = "^0.0.232"
-codeboxapi = "^0.0.9"
+codeboxapi = "^0.0.11"
 
 [tool.poetry.extras]
 image_support = ["Pillow"]
 streamlit_support = ["streamlit"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
```

### Comparing `codeinterpreterapi-0.0.7/PKG-INFO` & `codeinterpreterapi-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: codeinterpreterapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: CodeInterpreterAPI is an unofficial and open source python interface for the ChatGPT CodeInterpreter.
 License: MIT
 Author: Shroominic
-Author-email: pleurae-berets.0u@icloud.com
+Author-email: contact@shroominic.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: image-support
 Provides-Extra: streamlit-support
-Requires-Dist: codeboxapi (>=0.0.9,<0.0.10)
+Requires-Dist: codeboxapi (>=0.0.11,<0.0.12)
 Requires-Dist: langchain (>=0.0.232,<0.0.233)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Code Interpreter API
```

