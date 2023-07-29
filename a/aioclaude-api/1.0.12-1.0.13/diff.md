# Comparing `tmp/aioclaude-api-1.0.12.tar.gz` & `tmp/aioclaude-api-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioclaude-api-1.0.12.tar", last modified: Sat Jul 29 16:02:29 2023, max compression
+gzip compressed data, was "aioclaude-api-1.0.13.tar", last modified: Sat Jul 29 16:07:09 2023, max compression
```

## Comparing `aioclaude-api-1.0.12.tar` & `aioclaude-api-1.0.13.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 16:02:29.570364 aioclaude-api-1.0.12/
--rw-rw-rw-   0        0        0     1073 2023-07-29 14:51:37.000000 aioclaude-api-1.0.12/LICENSE
--rw-rw-rw-   0        0        0     5869 2023-07-29 16:02:29.567865 aioclaude-api-1.0.12/PKG-INFO
--rw-rw-rw-   0        0        0     4860 2023-07-29 15:43:54.000000 aioclaude-api-1.0.12/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 16:02:29.547212 aioclaude-api-1.0.12/aioclaude-api/
-drwxrwxrwx   0        0        0        0 2023-07-29 16:02:29.564857 aioclaude-api-1.0.12/aioclaude-api/aioclaude_api.egg-info/
--rw-rw-rw-   0        0        0     5869 2023-07-29 16:02:28.000000 aioclaude-api-1.0.12/aioclaude-api/aioclaude_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-07-29 16:02:29.000000 aioclaude-api-1.0.12/aioclaude-api/aioclaude_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 16:02:28.000000 aioclaude-api-1.0.12/aioclaude-api/aioclaude_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-29 16:02:28.000000 aioclaude-api-1.0.12/aioclaude-api/aioclaude_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-29 16:02:28.000000 aioclaude-api-1.0.12/aioclaude-api/aioclaude_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9890 2023-07-29 15:06:07.000000 aioclaude-api-1.0.12/aioclaude-api/claude_api.py
--rw-rw-rw-   0        0        0       42 2023-07-29 16:02:29.571366 aioclaude-api-1.0.12/setup.cfg
--rw-rw-rw-   0        0        0     1327 2023-07-29 15:46:07.000000 aioclaude-api-1.0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:07:09.099957 aioclaude-api-1.0.13/
+-rw-rw-rw-   0        0        0     1073 2023-07-29 14:51:37.000000 aioclaude-api-1.0.13/LICENSE
+-rw-rw-rw-   0        0        0     5869 2023-07-29 16:07:09.097409 aioclaude-api-1.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     4860 2023-07-29 15:43:54.000000 aioclaude-api-1.0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 16:07:09.072616 aioclaude-api-1.0.13/aioclaude-api/
+drwxrwxrwx   0        0        0        0 2023-07-29 16:07:09.093295 aioclaude-api-1.0.13/aioclaude-api/aioclaude_api.egg-info/
+-rw-rw-rw-   0        0        0     5869 2023-07-29 16:07:08.000000 aioclaude-api-1.0.13/aioclaude-api/aioclaude_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-29 16:07:08.000000 aioclaude-api-1.0.13/aioclaude-api/aioclaude_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:07:08.000000 aioclaude-api-1.0.13/aioclaude-api/aioclaude_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-29 16:07:08.000000 aioclaude-api-1.0.13/aioclaude-api/aioclaude_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-29 16:07:08.000000 aioclaude-api-1.0.13/aioclaude-api/aioclaude_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10296 2023-07-29 15:41:39.000000 aioclaude-api-1.0.13/aioclaude-api/aioclaude_api.py
+-rw-rw-rw-   0        0        0     9890 2023-07-29 15:06:07.000000 aioclaude-api-1.0.13/aioclaude-api/claude_api.py
+-rw-rw-rw-   0        0        0       42 2023-07-29 16:07:09.100810 aioclaude-api-1.0.13/setup.cfg
+-rw-rw-rw-   0        0        0     1330 2023-07-29 16:06:59.000000 aioclaude-api-1.0.13/setup.py
```

### Comparing `aioclaude-api-1.0.12/LICENSE` & `aioclaude-api-1.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `aioclaude-api-1.0.12/PKG-INFO` & `aioclaude-api-1.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioclaude-api
-Version: 1.0.12
+Version: 1.0.13
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/AmoreForever/Claude-API/
 Author: Hikamoru
 Author-email: me.thefarkhodov@gmail.com
 License: MIT
 Keywords: claude,ai,claude-ai,API,requests,chatbot,async,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aioclaude-api-1.0.12/README.md` & `aioclaude-api-1.0.13/README.md`

 * *Files identical despite different names*

### Comparing `aioclaude-api-1.0.12/aioclaude-api/aioclaude_api.egg-info/PKG-INFO` & `aioclaude-api-1.0.13/aioclaude-api/aioclaude_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioclaude-api
-Version: 1.0.12
+Version: 1.0.13
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/AmoreForever/Claude-API/
 Author: Hikamoru
 Author-email: me.thefarkhodov@gmail.com
 License: MIT
 Keywords: claude,ai,claude-ai,API,requests,chatbot,async,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aioclaude-api-1.0.12/aioclaude-api/claude_api.py` & `aioclaude-api-1.0.13/aioclaude-api/claude_api.py`

 * *Files identical despite different names*

### Comparing `aioclaude-api-1.0.12/setup.py` & `aioclaude-api-1.0.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 
 setup(
     name="aioclaude-api",
-    version="1.0.12",
+    version="1.0.13",
     author="Hikamoru",
     license="MIT",
     author_email="me.thefarkhodov@gmail.com",
     description="An unofficial API for Claude AI, allowing users to access and interact with Claude AII",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AmoreForever/Claude-API/",
@@ -23,15 +23,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     package_dir={"": "aioclaude-api"},
-    py_modules=["claude_api"],
+    py_modules=["aioclaude_api"],
     keywords=[
         "claude",
         "ai",
         "claude-ai",
         "API",
         "requests",
         "chatbot",
```

