# Comparing `tmp/gptw-0.4.2.tar.gz` & `tmp/gptw-0.4.3.tar.gz`

## Comparing `gptw-0.4.2.tar` & `gptw-0.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.4.2/gptw/__init__.py
--rw-r--r--   0        0        0     6748 2020-02-02 00:00:00.000000 gptw-0.4.2/gptw/gptw.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 gptw-0.4.2/gptw/prompts.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.4.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.4.2/LICENSE
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 gptw-0.4.2/README.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 gptw-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 gptw-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.4.3/gptw/__init__.py
+-rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 gptw-0.4.3/gptw/gptw.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 gptw-0.4.3/gptw/prompts.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.4.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 gptw-0.4.3/README.md
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 gptw-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 gptw-0.4.3/PKG-INFO
```

### Comparing `gptw-0.4.2/gptw/gptw.py` & `gptw-0.4.3/gptw/gptw.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,19 +97,21 @@
     with open(config_file, "w") as f:
         json.dump(cfg, f)
 
 
 CONFIG = None
 
 
-def get_config(key):
+def get_config(key, default_value=None):
     if not CONFIG:
         with open(config_file) as f:
             CFG = json.load(f)
     try:
+        if key not in CFG and default_value:
+            return default_value
         return CFG[key]
     except Exception:
         print("config not found, run `ww --config` to set it")
         sys.exit(1)
 
 
 def get_prompts():
@@ -139,60 +141,41 @@
     for chunk in client.send_message(bot_name, text, with_chat_break=True):
         pass
     # delete the 3 latest messages, including the chat break
     client.purge_conversation(bot_name, count=3)
     return chunk["text"]
 
 
-def ask_gpt_web(token, proxy, model, text):
-    os.environ["CHATGPT_BASE_URL"] = proxy
-    logging.debug("proxy:" + os.environ["CHATGPT_BASE_URL"])
-
-    from revChatGPT.V1 import Chatbot
-
-    chatbot = Chatbot(
-        config={
-            "access_token": token,
-            "paid": True,
-            "model": model,
-            "collect_analytics": False,
-        }
-    )
-    response = ""
-    for data in chatbot.ask(text):
-        response = data["message"]
-    return response
-
-
-def ask_azure_multi_pass(token, endpoint, depname, text):
+def ask_azure_multi_pass(repeat_cnt, token, endpoint, depname, text):
     msgs = [{"role": "user", "content": text}]
-    for _ in range(5):
+    for _ in range(repeat_cnt):
         resp = ask_azure(token, endpoint, depname, msgs)
         msgs.append({"role": "assistant", "content": resp})
-        msgs.append({"role": "user", "content": "a better one"})
+        msgs.append({"role": "user", "content": "retry, a better one please"})
         print(resp)
         print("")
     return ""
 
 
 def ask_azure(token, endpoint, depname, msgs):
     import openai
 
     logging.debug(f"!!!ask:{msgs}")
     openai.api_key = token
     openai.api_base = endpoint
     openai.api_type = "azure"
     openai.api_version = "2023-05-15"
     completion = openai.ChatCompletion.create(
-        engine=depname,
-        messages=msgs,
-        temperature=0.5,
+        engine=depname, messages=msgs, temperature=1.2, n=2
     )
-    resp = str(completion.choices[0].message.content).strip()
-    logging.debug(f"!!!resp:{resp}")
+    ret = str(completion.choices[0].message.content).strip()
+
+    for x in completion.choices[1:]:
+        print(str(x.message.content).strip())
+    logging.debug(f"!!!resp:{ret}")
     return str(completion.choices[0].message.content).strip()
 
 
 def list_commands(prompts):
     print(f'{"cmd":<{3}} | {"meaning":<{30}} | {"example"}')
     for pmt in prompts:
         print(
@@ -240,19 +223,14 @@
         token = get_config("openai-token")
         print(ask_gpt(token, model, msg))
     if get_config("provider") == "poe":
         logging.debug("use poe")
         token = get_config("poe-token")
         bot_name = get_config("poe-bot-name")
         print(ask_poe(token, bot_name, msg))
-    if get_config("provider") == "gpt-web":
-        logging.debug("use gpt-web")
-        token = get_config("gpt-web-token")
-        proxy = get_config("gpt-web-proxy")
-        model = get_config("gpt-web-model")
-        print(ask_gpt_web(token, proxy, model, msg))
     if get_config("provider") == "azure":
         logging.debug("use azure")
         token = get_config("azure-token")
         endpoint = get_config("azure-endpoint")
         depname = get_config("azure-depname")
-        print(ask_azure_multi_pass(token, endpoint, depname, msg))
+        repeat_cnt = int(get_config("azure-repeat-cnt", 3))
+        print(ask_azure_multi_pass(repeat_cnt, token, endpoint, depname, msg))
```

### Comparing `gptw-0.4.2/gptw/prompts.json` & `gptw-0.4.3/gptw/prompts.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'cmds'": "{'e': {'prompt': 'Please translate the following sentence into English. Please only "*

 * *           "output the translated content and do not output any other irrelevant content'}}"}*

```diff
@@ -19,15 +19,15 @@
             "_comment": "Dictionary",
             "example": "ww dic dictionary",
             "prompt": "Please provide the definitions of the following English words, including both English and Chinese explanations, an example sentence in English, and the correct pronunciation. Please also correct any spelling errors in the words. Please refrain from providing any additional output beyond the definitions."
         },
         "e": {
             "_comment": "Translate into English",
             "example": "ww e \u4f60\u597d",
-            "prompt": "Please rephrase the text delimited by triple backticks into natural-sounding English, adhering to native speaker conventions. Limit your response to the translation only."
+            "prompt": "Please translate the following sentence into English. Please only output the translated content and do not output any other irrelevant content"
         },
         "p": {
             "_comment": "Polish sentence",
             "example": "ww p hwo are you",
             "prompt": "Please review the sentence below for grammar, tense, word choice, and phrasing issues. Edit the sentence to make it sound natural and align with native speaker conventions. Provide a brief explanation for any changes made."
         },
         "r": {
```

### Comparing `gptw-0.4.2/.gitignore` & `gptw-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gptw-0.4.2/LICENSE` & `gptw-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gptw-0.4.2/README.md` & `gptw-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `gptw-0.4.2/pyproject.toml` & `gptw-0.4.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,53 +2,45 @@
 build-backend = "hatchling.build"
 requires = ["hatchling>=1.12.2", "hatch-vcs>=0.3"]
 
 [project]
 name = "gptw"
 dynamic = ["version"]
 description = "The ChatGPT command-line wrapper simplifies the execution of predetermined tasks through ChatGPT."
-authors = [
-  {email = "xinydev@gmail.com"},
-  {name = "Xin Yang"}
-]
-homepage="https://github.com/xinydev/gptW"
+authors = [{ email = "xinydev@gmail.com" }, { name = "Xin Yang" }]
+homepage = "https://github.com/xinydev/gptW"
 readme.file = "README.md"
 readme.content-type = "text/markdown"
-keywords = ["ChatGPT", "Command Line", "English Translation","English Polishing"]
+keywords = [
+  "ChatGPT",
+  "Command Line",
+  "English Translation",
+  "English Polishing",
+]
 license = "Apache-2.0"
 requires-python = ">=3.7.1"
-dependencies = [
-  "argparse>=1.4.0",
-  "openai>=0.27.0",
-  "poe-api>=0.3.1",
-  "revChatGPT>=5.0.3"
-]
-optional-dependencies.testing = [
-  "coverage==5.5",
-  "pytest==7.1.3",
-]
+dependencies = ["argparse>=1.4.0", "openai>=0.27.0", "poe-api>=0.3.1"]
+optional-dependencies.testing = ["coverage==5.5", "pytest==7.1.3"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Natural Language :: English",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 [project.scripts]
-gptw="gptw.gptw:main"
-ww="gptw.gptw:main"
+gptw = "gptw.gptw:main"
+ww = "gptw.gptw:main"
 
 [tool.setuptools.dynamic]
-version = {attr = "gptw.__version__"}
+version = { attr = "gptw.__version__" }
 
 [tool.hatch.version]
 path = "gptw/__init__.py"
 
 [tool.hatch.build]
-include = [
-  "gptw/*",
-]
+include = ["gptw/*"]
```

### Comparing `gptw-0.4.2/PKG-INFO` & `gptw-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptw
-Version: 0.4.2
+Version: 0.4.3
 Summary: The ChatGPT command-line wrapper simplifies the execution of predetermined tasks through ChatGPT.
 Author: Xin Yang
 Author-email: xinydev@gmail.com
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: ChatGPT,Command Line,English Polishing,English Translation
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7.1
 Requires-Dist: argparse>=1.4.0
 Requires-Dist: openai>=0.27.0
 Requires-Dist: poe-api>=0.3.1
-Requires-Dist: revchatgpt>=5.0.3
 Provides-Extra: testing
 Requires-Dist: coverage==5.5; extra == 'testing'
 Requires-Dist: pytest==7.1.3; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # GPT Simplify Your Daily Workflow (gptW)
```

