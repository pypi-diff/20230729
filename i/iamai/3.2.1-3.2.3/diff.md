# Comparing `tmp/iamai-3.2.1.tar.gz` & `tmp/iamai-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai-3.2.1.tar", max compression
+gzip compressed data, was "iamai-3.2.3.tar", max compression
```

## Comparing `iamai-3.2.1.tar` & `iamai-3.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-15 05:23:38.785804 iamai-3.2.1/LICENSE
--rw-r--r--   0        0        0     9810 2023-07-15 05:23:38.785804 iamai-3.2.1/README.md
--rw-r--r--   0        0        0      543 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/__init__.py
--rw-r--r--   0        0        0     4432 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/adapter/__init__.py
--rw-r--r--   0        0        0     1211 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/adapter/http_server_test_adapter.py
--rw-r--r--   0        0        0     1059 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/adapter/test.py
--rw-r--r--   0        0        0     7955 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/adapter/utils.py
--rw-r--r--   0        0        0    35504 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/bot.py
--rw-r--r--   0        0        0     1970 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/config.py
--rw-r--r--   0        0        0     1907 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/event.py
--rw-r--r--   0        0        0     1088 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/exceptions.py
--rw-r--r--   0        0        0      986 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/log.py
--rw-r--r--   0        0        0    13843 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/message.py
--rw-r--r--   0        0        0     3503 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/plugin.py
--rw-r--r--   0        0        0     1052 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/typing.py
--rw-r--r--   0        0        0     5529 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/utils.py
--rw-r--r--   0        0        0     2601 2023-07-15 05:23:38.797804 iamai-3.2.1/pyproject.toml
--rw-r--r--   0        0        0    11101 1970-01-01 00:00:00.000000 iamai-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-29 04:29:08.846200 iamai-3.2.3/LICENSE
+-rw-r--r--   0        0        0     9894 2023-07-29 04:29:08.850200 iamai-3.2.3/README.md
+-rw-r--r--   0        0        0      543 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/__init__.py
+-rw-r--r--   0        0        0     4393 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/adapter/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/adapter/http_server_test_adapter.py
+-rw-r--r--   0        0        0     1059 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/adapter/test.py
+-rw-r--r--   0        0        0     7954 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/adapter/utils.py
+-rw-r--r--   0        0        0    35504 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/bot.py
+-rw-r--r--   0        0        0     1970 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/config.py
+-rw-r--r--   0        0        0     1907 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/event.py
+-rw-r--r--   0        0        0     1088 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/exceptions.py
+-rw-r--r--   0        0        0      986 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/log.py
+-rw-r--r--   0        0        0    13746 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/message.py
+-rw-r--r--   0        0        0     3503 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/plugin.py
+-rw-r--r--   0        0        0     1052 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/typing.py
+-rw-r--r--   0        0        0     5506 2023-07-29 04:29:08.910201 iamai-3.2.3/iamai/utils.py
+-rw-r--r--   0        0        0     2937 2023-07-29 04:29:08.918201 iamai-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0    11319 1970-01-01 00:00:00.000000 iamai-3.2.3/PKG-INFO
```

### Comparing `iamai-3.2.1/LICENSE` & `iamai-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/README.md` & `iamai-3.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     <a href="https://www.kookapp.cn/">
       <img src="https://img.shields.io/badge/-%E5%BC%80%E9%BB%91%E5%95%A6Kook-83700?style=flat-square&logo=Discord&logoColor=white">
     </a>
     <!-- github -->
     <!-- <img src="https://img.shields.io/badge/-github-181717?style=flat-square&logo=github&logoColor=white"> -->
     <!-- discord -->
     <!-- <img src="https://img.shields.io/badge/-Discord-5865F2?style=flat-square&logo=Discord&logoColor=white"> -->
-    <!-- <br> -->
+    <br />
     <!-- bilibili live -->
-    <!-- <img src="https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-square&logo=Bilibili&logoColor=white"> -->
+    <img src="https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-square&logo=Bilibili&logoColor=white">
     <!-- mirai-api-http -->
     <img src="https://img.shields.io/badge/-Mirai%20api%20http%202.3+-00B8AA?style=flat-square">
     <!-- dingtalk -->
     <img src="https://img.shields.io/badge/-DingTalk-blue?style=flat-square">
     <!-- qqzone -->
     <!-- <img src="https://img.shields.io/badge/-QQ%20Zone-FECC00?style=flat-square&logo=Tencent QQ&logoColor=black"> -->
     <!-- <br> -->
@@ -123,14 +123,17 @@
 
 iamai itself is just a chatbot framework and additional protocol adapters are required to support specific protocols. You can use pip to install the protocol adapter:
 
 ```py
 pip install iamai-adapter-cqhttp
 pip install iamai-adapter-mirai
 pip install iamai-adapter-dingtalk
+pip install iamai-adapter-console
+pip install iamai-adapter-bililive
+pip install iamai-adapter-kook
 ```
 
 ## ❗ Usage
 
 firstly, you need to load an adapter.
 
 ```python
@@ -184,15 +187,15 @@
 ```
 
 ## 👀 See the docs
 
 > choices below.
 
 - [https://iamai.retrofor.space](https://iamai.retrofor.space) _(recommend)_
-- [retrofor.github.io/iamai](https://retrofor.github.io/iamai)
+- [https://iamai-asi.vercel.app](https://iamai-asi.vercel.app)
 
 ## ✨ Project Activity
 
 ![Alt](https://repobeats.axiom.co/api/embed/cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg "Repobeats analytics image")
 
 ## 👨‍🚀 Contributors
```

#### html2text {}

```diff
@@ -4,19 +4,20 @@
                       ç®ä½ä¸­æ ã«ã»ãã íêµ­ì´
             Cross-platform robot framework, mainly used for ML/DL.
                              [Website] [Website]
                                [pypi] [python]
      [https://results.pre-commit.ci/badge/github/retrofor/iamai/main.svg]
                          [Codacy_Badge] [Codacy Badge]
   [onebotv11] [https://img.shields.io/badge/-%E5%BC%80%E9%BB%91%E5%95%A6Kook-
-    83700?style=flat-square&logo=Discord&logoColor=white]         [https://
-  img.shields.io/badge/-Mirai%20api%20http%202.3+-00B8AA?style=flat-square]
-[https://img.shields.io/badge/-DingTalk-blue?style=flat-square]         [https:
-       //img.shields.io/badge/-Console-4EAA25?style=flat-square&logo=GNU
-                           bash&logoColor=white]
+          83700?style=flat-square&logo=Discord&logoColor=white]
+        [https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-
+    square&logo=Bilibili&logoColor=white]  [https://img.shields.io/badge/-
+ Mirai%20api%20http%202.3+-00B8AA?style=flat-square]  [https://img.shields.io/
+badge/-DingTalk-blue?style=flat-square]         [https://img.shields.io/badge/-
+      Console-4EAA25?style=flat-square&logo=GNU bash&logoColor=white]
   [https://img.shields.io/github/forks/retrofor/iamai?style=social] [https://
            img.shields.io/github/stars/retrofor/iamai?style=social]
 [https://img.shields.io/github/watchers/retrofor/iamai?style=social] [https://
         img.shields.io/github/search/retrofor/iamai/goto?style=social]
 [https://img.shields.io/github/repo-size/retrofor/iamai?style=social] [https://
        img.shields.io/github/languages/top/retrofor/iamai?style=social]
 ## ð Introduction A Cross-platform robot framework, mainly used for machine
@@ -35,43 +36,44 @@
 ## â¬ï¸ Install ### FrameWork - STABLE VERSION ```sh pip install iamai ``` or
 you can also install for TEST. - TEST VERSION ```sh git clone https://
 github.com/retrofor/iamai.git cd iamai poetry install --no-dev # æ¨è pip
 install . # ä¸æ¨è ``` ### Adapters iamai itself is just a chatbot framework
 and additional protocol adapters are required to support specific protocols.
 You can use pip to install the protocol adapter: ```py pip install iamai-
 adapter-cqhttp pip install iamai-adapter-mirai pip install iamai-adapter-
-dingtalk ``` ## â Usage firstly, you need to load an adapter. ```python from
-iamai import Bot bot = Bot() bot.load_adapters("iamai.adapter.cqhttp") bot.run
-() ``` then, you need load the transformer and use your models. ### transformer
-(Use from the ð¤/transformers library) ```python from transformers import
-AutoModelWithLMHead, AutoTokenizer # load models model =
-AutoModelWithLMHead.from_pretrained("gpt2") # load tokenizer tokenizer =
-AutoTokenizer.from_pretrained("gpt2") # transfor the text to token input_ids =
-tokenizer.encode("Hello, my name is IamAI!", add_special_tokens=True) # input
-the token to the models outputs = model.generate(input_ids) # get the text
-generated generated_text = tokenizer.decode(outputs[0]) ``` You can use pre-
-built optimizers to speed up the model inference process, or you can write your
-own optimizer. However, it's important to note that the transformer model
-optimizer is a special type of optimizer that is designed specifically for
-optimizing parameters in transformer models, thereby improving their
-performance. To write a transformer model optimizer, you need to have an
-understanding of how optimizers work and be familiar with the structure of
-transformer models. The principle of optimizers can be referred to in the paper
-["Attention Is All You Need"](https://arxiv.org/abs/1706.03762), and the
-structure of transformer models can be referred to in the paper ["Transformer:
-A Novel Neural Network Architecture for Language Understanding"](https://
-ai.googleblog.com/2017/08/transformer-novel-neural-network.html?m=1). The
-implementation of optimizers can be referred to in the [AdamW optimizer](https:
-//huggingface.co/transformers/v3.0.2/main_classes/optimizer_schedules.html) in
-the Hugging Face Transformers library. ### Use the Inference API ```python
-import requests API_URL = "https://api-inference.huggingface.co/models/xxx/
-xxxxx" headers = {"Authorization": "Bearer
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"} def query(payload): response =
+dingtalk pip install iamai-adapter-console pip install iamai-adapter-bililive
+pip install iamai-adapter-kook ``` ## â Usage firstly, you need to load an
+adapter. ```python from iamai import Bot bot = Bot() bot.load_adapters
+("iamai.adapter.cqhttp") bot.run() ``` then, you need load the transformer and
+use your models. ### transformer(Use from the ð¤/transformers library)
+```python from transformers import AutoModelWithLMHead, AutoTokenizer # load
+models model = AutoModelWithLMHead.from_pretrained("gpt2") # load tokenizer
+tokenizer = AutoTokenizer.from_pretrained("gpt2") # transfor the text to token
+input_ids = tokenizer.encode("Hello, my name is IamAI!",
+add_special_tokens=True) # input the token to the models outputs =
+model.generate(input_ids) # get the text generated generated_text =
+tokenizer.decode(outputs[0]) ``` You can use pre-built optimizers to speed up
+the model inference process, or you can write your own optimizer. However, it's
+important to note that the transformer model optimizer is a special type of
+optimizer that is designed specifically for optimizing parameters in
+transformer models, thereby improving their performance. To write a transformer
+model optimizer, you need to have an understanding of how optimizers work and
+be familiar with the structure of transformer models. The principle of
+optimizers can be referred to in the paper ["Attention Is All You Need"](https:
+//arxiv.org/abs/1706.03762), and the structure of transformer models can be
+referred to in the paper ["Transformer: A Novel Neural Network Architecture for
+Language Understanding"](https://ai.googleblog.com/2017/08/transformer-novel-
+neural-network.html?m=1). The implementation of optimizers can be referred to
+in the [AdamW optimizer](https://huggingface.co/transformers/v3.0.2/
+main_classes/optimizer_schedules.html) in the Hugging Face Transformers
+library. ### Use the Inference API ```python import requests API_URL = "https:/
+/api-inference.huggingface.co/models/xxx/xxxxx" headers = {"Authorization":
+"Bearer xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"} def query(payload): response =
 requests.post(API_URL, headers=headers, json=payload) return response.json()
 output = query({ "inputs": "xxx", }) ``` ## ð See the docs > choices below.
 - [https://iamai.retrofor.space](https://iamai.retrofor.space) _(recommend)_ -
-[retrofor.github.io/iamai](https://retrofor.github.io/iamai) ## â¨ Project
+[https://iamai-asi.vercel.app](https://iamai-asi.vercel.app) ## â¨ Project
 Activity ![Alt](https://repobeats.axiom.co/api/embed/
 cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg "Repobeats analytics image") ##
 ð¨âð Contributors [https://contrib.rocks/image?repo=retrofor/iamai] ##
 ð License [MIT](https://github.com/retrofor/iamai/blob/main/LICENSE) Â©
 2023-PRESENT [ç®å¾çº¯](https://github.com/HsiangNianian)
```

### Comparing `iamai-3.2.1/iamai/__init__.py` & `iamai-3.2.3/iamai/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/iamai/adapter/__init__.py` & `iamai-3.2.3/iamai/adapter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,17 +110,15 @@
 
         Raises:
             GetEventTimeout: 超过最大事件数或超时。
         """
 
         def func_wrapper(_func):
             async def _wrapper(_event: T_Event):
-                if _event.adapter is not self:
-                    return False
-                return await _func(_event)
+                return False if _event.adapter is not self else await _func(_event)
 
             return _wrapper
 
         if func is None:
             func = sync_func_wrapper(lambda x: True)
         elif not asyncio.iscoroutinefunction(func):
             func = sync_func_wrapper(func)
```

### Comparing `iamai-3.2.1/iamai/adapter/http_server_test_adapter.py` & `iamai-3.2.3/iamai/adapter/http_server_test_adapter.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/iamai/adapter/test.py` & `iamai-3.2.3/iamai/adapter/test.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/iamai/adapter/utils.py` & `iamai-3.2.3/iamai/adapter/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         await self.websocket.prepare(request)
         await self.reverse_ws_connection_hook()
         await self.handle_websocket()
         return self.websocket
 
     async def reverse_ws_connection_hook(self):
         """反向 WebSocket 连接建立时的钩子函数。"""
-        logger.info(f"WebSocket connected!")
+        logger.info("WebSocket connected!")
 
     async def websocket_connect(self):
         """创建正向 WebSocket 连接。"""
         logger.info("Tying to connect to WebSocket server...")
         async with self.session.ws_connect(
             f"ws://{self.host}:{self.port}{self.url}"
         ) as self.websocket:
```

### Comparing `iamai-3.2.1/iamai/bot.py` & `iamai-3.2.3/iamai/bot.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/iamai/config.py` & `iamai-3.2.3/iamai/config.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/iamai/event.py` & `iamai-3.2.3/iamai/event.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/iamai/exceptions.py` & `iamai-3.2.3/iamai/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/iamai/log.py` & `iamai-3.2.3/iamai/log.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/iamai/message.py` & `iamai-3.2.3/iamai/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,15 @@
             yield msg
         elif isinstance(msg, Mapping):
             yield self._mapping_to_message_segment(msg)
         elif isinstance(msg, str):
             yield self._str_to_message_segment(msg)
         elif isinstance(msg, Iterable):
             for seg in msg:
-                for i in self._construct(seg):
-                    yield i
+                yield from self._construct(seg)
 
     def _mapping_to_message_segment(self, msg: Mapping) -> T_MessageSegment:
         """用于将 Mapping 转换为 MessageSegment，如有需要，子类可重写此方法以更改对 Mapping 的默认行为。
 
         Args:
             msg: 要解析为 MessageSegment 的数据。
 
@@ -113,15 +112,15 @@
 
         Returns:
             由 str 转换的 MessageSegment。
         """
         raise NotImplementedError
 
     def __repr__(self) -> str:
-        return "Message:[{}]".format(",".join(map(lambda x: repr(x), self)))
+        return f'Message:[{",".join(map(lambda x: repr(x), self))}]'
 
     def __str__(self) -> str:
         return "".join(map(lambda x: str(x), self))
 
     def __contains__(self, item) -> bool:
         if isinstance(item, str):
             return item in str(self)
@@ -199,17 +198,15 @@
 
         Returns:
             检查结果。
         """
         if isinstance(prefix, str):
             return str(self).startswith(prefix, start, end)
         elif isinstance(prefix, self._message_segment_class):
-            if len(self) == 0:
-                return False
-            return self[0] == prefix
+            return False if len(self) == 0 else self[0] == prefix
         raise TypeError(
             f"first arg must be str or {self._message_segment_class}，not {type(prefix)}"
         )
 
     def endswith(
         self, suffix: Union[str, T_MessageSegment], start=None, end=None
     ) -> bool:
@@ -226,17 +223,15 @@
 
         Returns:
             检查结果。
         """
         if isinstance(suffix, str):
             return str(self).endswith(suffix, start, end)
         elif isinstance(suffix, self._message_segment_class):
-            if len(self) == 0:
-                return False
-            return self[-1] == suffix
+            return False if len(self) == 0 else self[-1] == suffix
         raise TypeError(
             f"first arg must be str or {self._message_segment_class}，not {type(suffix)}"
         )
 
     def replace(
         self,
         old: Union[str, T_MessageSegment],
```

### Comparing `iamai-3.2.1/iamai/plugin.py` & `iamai-3.2.3/iamai/plugin.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/iamai/typing.py` & `iamai-3.2.3/iamai/typing.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2.1/iamai/utils.py` & `iamai-3.2.3/iamai/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,17 +142,15 @@
     return classes
 
 
 class DataclassEncoder(json.JSONEncoder):
     """用于解析 MessageSegment 的 JSONEncoder 类。"""
 
     def default(self, o):
-        if dataclasses.is_dataclass(o):
-            return o.as_dict()
-        return super().default(o)
+        return o.as_dict() if dataclasses.is_dataclass(o) else super().default(o)
 
 
 def samefile(path1: str, path2: str) -> bool:
     """一个 `os.path.samefile` 的简单包装。
 
     Args:
         path1: 路径1。
```

### Comparing `iamai-3.2.1/pyproject.toml` & `iamai-3.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,74 @@
 [tool.poetry]
 name = "iamai"
-version = "3.2.1"
+version = "3.2.3"
 description = "bot framework."
 authors = ["简律纯 <i@jyunko.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
-keywords = ["bot", "qq", "qqbot", "mirai", "coolq", "kook", "go-cqhttp", "dingtalk", "console"]
+keywords = [
+  "bot",
+  "qq",
+  "qqbot",
+  "mirai",
+  "coolq",
+  "kook",
+  "go-cqhttp",
+  "dingtalk",
+  "console",
+  "apscheduler",
+  "bilibili",
+  "bilibili-live",
+]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Library",
   "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3"
+  "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 tomli = { version = "^2.0.0", python = "<3.11" }
 pydantic = "^1.10.0"
 aiohttp = "^3.8.0"
 loguru = ">=0.6,<0.8"
-typing-extensions = "^4.4.0"
+pyyaml = "^6.0"
+typing-extensions = ">=4.7.0"
 
 [tool.poetry.group.dev.dependencies]
 watchfiles = "^0.18.0"
 sophia-doc = "^0.1.0"
+iamai-adapter-bililive = { path = "./packages/iamai-adapter-bililive", develop = true }
 iamai-adapter-console = { path = "./packages/iamai-adapter-console", develop = true }
 iamai-adapter-kook = { path = "./packages/iamai-adapter-kook", develop = true }
 iamai-adapter-cqhttp = { path = "./packages/iamai-adapter-cqhttp", develop = true }
 iamai-adapter-dingtalk = { path = "./packages/iamai-adapter-dingtalk", develop = true }
 iamai-adapter-apscheduler = { path = "./packages/iamai-adapter-apscheduler", develop = true }
 black = "^23.1.0"
 isort = "^5.12.0"
 pre-commit = "^3.1.0"
 pre-commit-hooks = "^4.4.0"
 
 [tool.poetry.extras]
 kook = ["iamai-adapter-kook"]
+mirai = ["iamai-adapter-mirai"]
 cqhttp = ["iamai-adapter-cqhttp"]
+console = ["iamai-adapter-console"]
+bililive = ["iamai-adapter-bililive"]
 dingtalk = ["iamai-adapter-dingtalk"]
 apscheduler = ["iamai-adapter-apscheduler"]
 hot_reload = ["watchfiles"]
 all = [
+  "iamai-adapter-mirai",
+  "iamai-adapter-bililive",
   "iamai-adapter-console",
   "iamai-adapter-kook",
   "iamai-adapter-cqhttp",
   "iamai-adapter-dingtalk",
   "iamai-adapter-apscheduler",
   "watchfiles",
 ]
```

### Comparing `iamai-3.2.1/PKG-INFO` & `iamai-3.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: iamai
-Version: 3.2.1
+Version: 3.2.3
 Summary: bot framework.
 Home-page: https://retrofor.space/
 License: MIT
-Keywords: bot,qq,qqbot,mirai,coolq,kook,go-cqhttp,dingtalk,console
+Keywords: bot,qq,qqbot,mirai,coolq,kook,go-cqhttp,dingtalk,console,apscheduler,bilibili,bilibili-live
 Author: 简律纯
 Author-email: i@jyunko.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: License :: OSI Approved :: MIT License
@@ -16,23 +16,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: apscheduler
+Provides-Extra: bililive
+Provides-Extra: console
 Provides-Extra: cqhttp
 Provides-Extra: dingtalk
 Provides-Extra: hot-reload
 Provides-Extra: kook
+Provides-Extra: mirai
 Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
 Requires-Dist: loguru (>=0.6,<0.8)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tomli (>=2.0.0,<3.0.0) ; python_version < "3.11"
-Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.7.0)
 Project-URL: Documentation, https://iamai.retrofor.space/
 Project-URL: Repository, https://github.com/retrofor/iamai
 Description-Content-Type: text/markdown
 
 <p align="center"><img width="128" src="https://iamai.retrofor.space/retro.png"></p>
 <h1 align="center">
   iamai
@@ -79,17 +83,17 @@
     <a href="https://www.kookapp.cn/">
       <img src="https://img.shields.io/badge/-%E5%BC%80%E9%BB%91%E5%95%A6Kook-83700?style=flat-square&logo=Discord&logoColor=white">
     </a>
     <!-- github -->
     <!-- <img src="https://img.shields.io/badge/-github-181717?style=flat-square&logo=github&logoColor=white"> -->
     <!-- discord -->
     <!-- <img src="https://img.shields.io/badge/-Discord-5865F2?style=flat-square&logo=Discord&logoColor=white"> -->
-    <!-- <br> -->
+    <br />
     <!-- bilibili live -->
-    <!-- <img src="https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-square&logo=Bilibili&logoColor=white"> -->
+    <img src="https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-square&logo=Bilibili&logoColor=white">
     <!-- mirai-api-http -->
     <img src="https://img.shields.io/badge/-Mirai%20api%20http%202.3+-00B8AA?style=flat-square">
     <!-- dingtalk -->
     <img src="https://img.shields.io/badge/-DingTalk-blue?style=flat-square">
     <!-- qqzone -->
     <!-- <img src="https://img.shields.io/badge/-QQ%20Zone-FECC00?style=flat-square&logo=Tencent QQ&logoColor=black"> -->
     <!-- <br> -->
@@ -158,14 +162,17 @@
 
 iamai itself is just a chatbot framework and additional protocol adapters are required to support specific protocols. You can use pip to install the protocol adapter:
 
 ```py
 pip install iamai-adapter-cqhttp
 pip install iamai-adapter-mirai
 pip install iamai-adapter-dingtalk
+pip install iamai-adapter-console
+pip install iamai-adapter-bililive
+pip install iamai-adapter-kook
 ```
 
 ## ❗ Usage
 
 firstly, you need to load an adapter.
 
 ```python
@@ -219,15 +226,15 @@
 ```
 
 ## 👀 See the docs
 
 > choices below.
 
 - [https://iamai.retrofor.space](https://iamai.retrofor.space) _(recommend)_
-- [retrofor.github.io/iamai](https://retrofor.github.io/iamai)
+- [https://iamai-asi.vercel.app](https://iamai-asi.vercel.app)
 
 ## ✨ Project Activity
 
 ![Alt](https://repobeats.axiom.co/api/embed/cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg "Repobeats analytics image")
 
 ## 👨‍🚀 Contributors
```

#### html2text {}

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 2.1 Name: iamai Version: 3.2.1 Summary: bot framework. Home-
+Metadata-Version: 2.1 Name: iamai Version: 3.2.3 Summary: bot framework. Home-
 page: https://retrofor.space/ License: MIT Keywords:
-bot,qq,qqbot,mirai,coolq,kook,go-cqhttp,dingtalk,console Author: ç®å¾çº¯
+bot,qq,qqbot,mirai,coolq,kook,go-
+cqhttp,dingtalk,console,apscheduler,bilibili,bilibili-live Author: ç®å¾çº¯
 Author-email: i@jyunko.cn Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: apscheduler
-Provides-Extra: cqhttp Provides-Extra: dingtalk Provides-Extra: hot-reload
-Provides-Extra: kook Requires-Dist: aiohttp (>=3.8.0,<4.0.0) Requires-Dist:
+Provides-Extra: bililive Provides-Extra: console Provides-Extra: cqhttp
+Provides-Extra: dingtalk Provides-Extra: hot-reload Provides-Extra: kook
+Provides-Extra: mirai Requires-Dist: aiohttp (>=3.8.0,<4.0.0) Requires-Dist:
 loguru (>=0.6,<0.8) Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist:
-tomli (>=2.0.0,<3.0.0) ; python_version < "3.11" Requires-Dist: typing-
-extensions (>=4.4.0,<5.0.0) Project-URL: Documentation, https://
-iamai.retrofor.space/ Project-URL: Repository, https://github.com/retrofor/
-iamai Description-Content-Type: text/markdown
+pyyaml (>=6.0,<7.0) Requires-Dist: tomli (>=2.0.0,<3.0.0) ; python_version <
+"3.11" Requires-Dist: typing-extensions (>=4.7.0) Project-URL: Documentation,
+https://iamai.retrofor.space/ Project-URL: Repository, https://github.com/
+retrofor/iamai Description-Content-Type: text/markdown
                    [https://iamai.retrofor.space/retro.png]
                               ****** iamai ******
                                [Discord] [QQç¾¤]
                       ç®ä½ä¸­æ ã«ã»ãã íêµ­ì´
             Cross-platform robot framework, mainly used for ML/DL.
                              [Website] [Website]
                                [pypi] [python]
      [https://results.pre-commit.ci/badge/github/retrofor/iamai/main.svg]
                          [Codacy_Badge] [Codacy Badge]
   [onebotv11] [https://img.shields.io/badge/-%E5%BC%80%E9%BB%91%E5%95%A6Kook-
-    83700?style=flat-square&logo=Discord&logoColor=white]         [https://
-  img.shields.io/badge/-Mirai%20api%20http%202.3+-00B8AA?style=flat-square]
-[https://img.shields.io/badge/-DingTalk-blue?style=flat-square]         [https:
-       //img.shields.io/badge/-Console-4EAA25?style=flat-square&logo=GNU
-                           bash&logoColor=white]
+          83700?style=flat-square&logo=Discord&logoColor=white]
+        [https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-
+    square&logo=Bilibili&logoColor=white]  [https://img.shields.io/badge/-
+ Mirai%20api%20http%202.3+-00B8AA?style=flat-square]  [https://img.shields.io/
+badge/-DingTalk-blue?style=flat-square]         [https://img.shields.io/badge/-
+      Console-4EAA25?style=flat-square&logo=GNU bash&logoColor=white]
   [https://img.shields.io/github/forks/retrofor/iamai?style=social] [https://
            img.shields.io/github/stars/retrofor/iamai?style=social]
 [https://img.shields.io/github/watchers/retrofor/iamai?style=social] [https://
         img.shields.io/github/search/retrofor/iamai/goto?style=social]
 [https://img.shields.io/github/repo-size/retrofor/iamai?style=social] [https://
        img.shields.io/github/languages/top/retrofor/iamai?style=social]
 ## ð Introduction A Cross-platform robot framework, mainly used for machine
@@ -53,43 +56,44 @@
 ## â¬ï¸ Install ### FrameWork - STABLE VERSION ```sh pip install iamai ``` or
 you can also install for TEST. - TEST VERSION ```sh git clone https://
 github.com/retrofor/iamai.git cd iamai poetry install --no-dev # æ¨è pip
 install . # ä¸æ¨è ``` ### Adapters iamai itself is just a chatbot framework
 and additional protocol adapters are required to support specific protocols.
 You can use pip to install the protocol adapter: ```py pip install iamai-
 adapter-cqhttp pip install iamai-adapter-mirai pip install iamai-adapter-
-dingtalk ``` ## â Usage firstly, you need to load an adapter. ```python from
-iamai import Bot bot = Bot() bot.load_adapters("iamai.adapter.cqhttp") bot.run
-() ``` then, you need load the transformer and use your models. ### transformer
-(Use from the ð¤/transformers library) ```python from transformers import
-AutoModelWithLMHead, AutoTokenizer # load models model =
-AutoModelWithLMHead.from_pretrained("gpt2") # load tokenizer tokenizer =
-AutoTokenizer.from_pretrained("gpt2") # transfor the text to token input_ids =
-tokenizer.encode("Hello, my name is IamAI!", add_special_tokens=True) # input
-the token to the models outputs = model.generate(input_ids) # get the text
-generated generated_text = tokenizer.decode(outputs[0]) ``` You can use pre-
-built optimizers to speed up the model inference process, or you can write your
-own optimizer. However, it's important to note that the transformer model
-optimizer is a special type of optimizer that is designed specifically for
-optimizing parameters in transformer models, thereby improving their
-performance. To write a transformer model optimizer, you need to have an
-understanding of how optimizers work and be familiar with the structure of
-transformer models. The principle of optimizers can be referred to in the paper
-["Attention Is All You Need"](https://arxiv.org/abs/1706.03762), and the
-structure of transformer models can be referred to in the paper ["Transformer:
-A Novel Neural Network Architecture for Language Understanding"](https://
-ai.googleblog.com/2017/08/transformer-novel-neural-network.html?m=1). The
-implementation of optimizers can be referred to in the [AdamW optimizer](https:
-//huggingface.co/transformers/v3.0.2/main_classes/optimizer_schedules.html) in
-the Hugging Face Transformers library. ### Use the Inference API ```python
-import requests API_URL = "https://api-inference.huggingface.co/models/xxx/
-xxxxx" headers = {"Authorization": "Bearer
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"} def query(payload): response =
+dingtalk pip install iamai-adapter-console pip install iamai-adapter-bililive
+pip install iamai-adapter-kook ``` ## â Usage firstly, you need to load an
+adapter. ```python from iamai import Bot bot = Bot() bot.load_adapters
+("iamai.adapter.cqhttp") bot.run() ``` then, you need load the transformer and
+use your models. ### transformer(Use from the ð¤/transformers library)
+```python from transformers import AutoModelWithLMHead, AutoTokenizer # load
+models model = AutoModelWithLMHead.from_pretrained("gpt2") # load tokenizer
+tokenizer = AutoTokenizer.from_pretrained("gpt2") # transfor the text to token
+input_ids = tokenizer.encode("Hello, my name is IamAI!",
+add_special_tokens=True) # input the token to the models outputs =
+model.generate(input_ids) # get the text generated generated_text =
+tokenizer.decode(outputs[0]) ``` You can use pre-built optimizers to speed up
+the model inference process, or you can write your own optimizer. However, it's
+important to note that the transformer model optimizer is a special type of
+optimizer that is designed specifically for optimizing parameters in
+transformer models, thereby improving their performance. To write a transformer
+model optimizer, you need to have an understanding of how optimizers work and
+be familiar with the structure of transformer models. The principle of
+optimizers can be referred to in the paper ["Attention Is All You Need"](https:
+//arxiv.org/abs/1706.03762), and the structure of transformer models can be
+referred to in the paper ["Transformer: A Novel Neural Network Architecture for
+Language Understanding"](https://ai.googleblog.com/2017/08/transformer-novel-
+neural-network.html?m=1). The implementation of optimizers can be referred to
+in the [AdamW optimizer](https://huggingface.co/transformers/v3.0.2/
+main_classes/optimizer_schedules.html) in the Hugging Face Transformers
+library. ### Use the Inference API ```python import requests API_URL = "https:/
+/api-inference.huggingface.co/models/xxx/xxxxx" headers = {"Authorization":
+"Bearer xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"} def query(payload): response =
 requests.post(API_URL, headers=headers, json=payload) return response.json()
 output = query({ "inputs": "xxx", }) ``` ## ð See the docs > choices below.
 - [https://iamai.retrofor.space](https://iamai.retrofor.space) _(recommend)_ -
-[retrofor.github.io/iamai](https://retrofor.github.io/iamai) ## â¨ Project
+[https://iamai-asi.vercel.app](https://iamai-asi.vercel.app) ## â¨ Project
 Activity ![Alt](https://repobeats.axiom.co/api/embed/
 cc9b8bded331c406e68cc0c7c294ef04122d6da2.svg "Repobeats analytics image") ##
 ð¨âð Contributors [https://contrib.rocks/image?repo=retrofor/iamai] ##
 ð License [MIT](https://github.com/retrofor/iamai/blob/main/LICENSE) Â©
 2023-PRESENT [ç®å¾çº¯](https://github.com/HsiangNianian)
```

