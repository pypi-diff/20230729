# Comparing `tmp/freeGPT-1.2.5.tar.gz` & `tmp/freeGPT-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.2.5.tar", last modified: Wed Jul 26 20:12:54 2023, max compression
+gzip compressed data, was "freeGPT-1.2.6.tar", last modified: Sat Jul 29 09:16:31 2023, max compression
```

## Comparing `freeGPT-1.2.5.tar` & `freeGPT-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 20:12:54.009432 freeGPT-1.2.5/
--rw-rw-rw-   0        0        0    18092 2023-07-26 19:50:03.000000 freeGPT-1.2.5/LICENSE
--rw-rw-rw-   0        0        0     4463 2023-07-26 20:12:54.002432 freeGPT-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3154 2023-07-26 19:50:03.000000 freeGPT-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 20:12:53.981433 freeGPT-1.2.5/freeGPT/
--rw-rw-rw-   0        0        0      164 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/alpaca_7b.py
--rw-rw-rw-   0        0        0     2697 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/gpt3.py
--rw-rw-rw-   0        0        0     4715 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/gpt4.py
--rw-rw-rw-   0        0        0      614 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/pollinations.py
--rw-rw-rw-   0        0        0     3351 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/prodia.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:12:53.999431 freeGPT-1.2.5/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     4463 2023-07-26 20:12:53.000000 freeGPT-1.2.5/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-07-26 20:12:53.000000 freeGPT-1.2.5/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 20:12:53.000000 freeGPT-1.2.5/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 20:12:53.000000 freeGPT-1.2.5/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 20:12:53.000000 freeGPT-1.2.5/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 20:12:54.009432 freeGPT-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1663 2023-07-26 19:50:03.000000 freeGPT-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:16:31.424970 freeGPT-1.2.6/
+-rw-rw-rw-   0        0        0    18092 2023-07-29 09:15:34.000000 freeGPT-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0     4387 2023-07-29 09:16:31.424970 freeGPT-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3078 2023-07-29 09:15:34.000000 freeGPT-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 09:16:31.408969 freeGPT-1.2.6/freeGPT/
+-rw-rw-rw-   0        0        0      164 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/alpaca_7b.py
+-rw-rw-rw-   0        0        0     2697 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/gpt3.py
+-rw-rw-rw-   0        0        0     2495 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/gpt4.py
+-rw-rw-rw-   0        0        0      738 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/pollinations.py
+-rw-rw-rw-   0        0        0     3530 2023-07-29 09:15:34.000000 freeGPT-1.2.6/freeGPT/prodia.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:16:31.424970 freeGPT-1.2.6/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     4387 2023-07-29 09:16:31.000000 freeGPT-1.2.6/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-07-29 09:16:31.000000 freeGPT-1.2.6/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 09:16:31.000000 freeGPT-1.2.6/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-29 09:16:31.000000 freeGPT-1.2.6/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 09:16:31.000000 freeGPT-1.2.6/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 09:16:31.424970 freeGPT-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1663 2023-07-29 09:15:34.000000 freeGPT-1.2.6/setup.py
```

### Comparing `freeGPT-1.2.5/LICENSE` & `freeGPT-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.5/PKG-INFO` & `freeGPT-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.5
+Version: 1.2.6
 Summary: freeGPT provides free access to GPT3, GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
 Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt,ai
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-#### Sorry, The freeGPT bot is in 100 servers and I can't verify it ATM. Please join my [Discord server](https://discord.gg/XH6pUGkwRr) if you wish to use it.
+##### The freeGPT bot has been verified, invite it [here](https://dsc.gg/freegpt)!
 
 [![PyPI](https://img.shields.io/pypi/v/freeGPT)](https://pypi.org/project/freeGPT)
 [![Downloads](https://static.pepy.tech/badge/freeGPT)](https://pypi.org/project/freeGPT)
 [![Status](https://img.shields.io/pypi/status/freeGPT)](https://pypi.org/project/freeGPT)
 
 # freeGPT
```

### Comparing `freeGPT-1.2.5/README.md` & `freeGPT-1.2.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#### Sorry, The freeGPT bot is in 100 servers and I can't verify it ATM. Please join my [Discord server](https://discord.gg/XH6pUGkwRr) if you wish to use it.
+##### The freeGPT bot has been verified, invite it [here](https://dsc.gg/freegpt)!
 
 [![PyPI](https://img.shields.io/pypi/v/freeGPT)](https://pypi.org/project/freeGPT)
 [![Downloads](https://static.pepy.tech/badge/freeGPT)](https://pypi.org/project/freeGPT)
 [![Status](https://img.shields.io/pypi/status/freeGPT)](https://pypi.org/project/freeGPT)
 
 # freeGPT
```

### Comparing `freeGPT-1.2.5/freeGPT/alpaca_7b.py` & `freeGPT-1.2.6/freeGPT/alpaca_7b.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.5/freeGPT/gpt3.py` & `freeGPT-1.2.6/freeGPT/gpt3.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.5/freeGPT/prodia.py` & `freeGPT-1.2.6/freeGPT/prodia.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,28 +36,30 @@
             "sec-ch-ua-platform": '"Linux"',
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-site",
             "sec-gpc": "1",
             "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.79 Safari/537.36",
         }
-
-        async with ClientSession() as session:
-            async with session.get(
-                "https://api.prodia.com/generate",
-                params=params,
-                headers=headers,
-                timeout=45,
-            ) as resp:
-                data = await resp.json()
-                job_id = data["job"]
-                while True:
-                    async with session.get(
-                        f"https://api.prodia.com/job/{job_id}", headers=headers
-                    ) as resp:
-                        json = await resp.json()
-                        if json["status"] == "succeeded":
-                            async with session.get(
-                                f"https://images.prodia.xyz/{job_id}.png?download=1",
-                                headers=headers,
-                            ) as resp:
-                                return await resp.content.read()
+        try:
+            async with ClientSession() as session:
+                async with session.get(
+                    "https://api.prodia.com/generate",
+                    params=params,
+                    headers=headers,
+                    timeout=45,
+                ) as resp:
+                    data = await resp.json()
+                    job_id = data["job"]
+                    while True:
+                        async with session.get(
+                            f"https://api.prodia.com/job/{job_id}", headers=headers
+                        ) as resp:
+                            json = await resp.json()
+                            if json["status"] == "succeeded":
+                                async with session.get(
+                                    f"https://images.prodia.xyz/{job_id}.png?download=1",
+                                    headers=headers,
+                                ) as resp:
+                                    return await resp.content.read()
+        except Exception:
+            raise Exception("Unable to fetch the response.")
```

### Comparing `freeGPT-1.2.5/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.2.6/freeGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.5
+Version: 1.2.6
 Summary: freeGPT provides free access to GPT3, GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
 Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt,ai
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-#### Sorry, The freeGPT bot is in 100 servers and I can't verify it ATM. Please join my [Discord server](https://discord.gg/XH6pUGkwRr) if you wish to use it.
+##### The freeGPT bot has been verified, invite it [here](https://dsc.gg/freegpt)!
 
 [![PyPI](https://img.shields.io/pypi/v/freeGPT)](https://pypi.org/project/freeGPT)
 [![Downloads](https://static.pepy.tech/badge/freeGPT)](https://pypi.org/project/freeGPT)
 [![Status](https://img.shields.io/pypi/status/freeGPT)](https://pypi.org/project/freeGPT)
 
 # freeGPT
```

### Comparing `freeGPT-1.2.5/setup.py` & `freeGPT-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.2.5",
+    version="1.2.6",
     description="freeGPT provides free access to GPT3, GPT4 and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv2",
     keywords=[
```

