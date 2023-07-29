# Comparing `tmp/iamai_adapter_mirai-3.2.1.tar.gz` & `tmp/iamai_adapter_mirai-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_mirai-3.2.1.tar", max compression
+gzip compressed data, was "iamai_adapter_mirai-3.2.3.tar", max compression
```

## Comparing `iamai_adapter_mirai-3.2.1.tar` & `iamai_adapter_mirai-3.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34522 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/LICENSE
--rw-r--r--   0        0        0      241 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/README.md
--rw-r--r--   0        0        0     9055 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/__init__.py
--rw-r--r--   0        0        0     1029 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/config.py
--rw-r--r--   0        0        0      562 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/__init__.py
--rw-r--r--   0        0        0      822 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/base.py
--rw-r--r--   0        0        0     1042 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/mate.py
--rw-r--r--   0        0        0     3650 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/message.py
--rw-r--r--   0        0        0     5492 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/notice.py
--rw-r--r--   0        0        0     4264 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/request.py
--rw-r--r--   0        0        0      644 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/exceptions.py
--rw-r--r--   0        0        0     4419 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/message.py
--rw-r--r--   0        0        0     1301 2023-07-15 05:23:38.797804 iamai_adapter_mirai-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 iamai_adapter_mirai-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/LICENSE
+-rw-r--r--   0        0        0      241 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/README.md
+-rw-r--r--   0        0        0     9038 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/__init__.py
+-rw-r--r--   0        0        0     1029 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/config.py
+-rw-r--r--   0        0        0      562 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/base.py
+-rw-r--r--   0        0        0     1042 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/mate.py
+-rw-r--r--   0        0        0     3650 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/message.py
+-rw-r--r--   0        0        0     5492 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/notice.py
+-rw-r--r--   0        0        0     4264 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/request.py
+-rw-r--r--   0        0        0      644 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/exceptions.py
+-rw-r--r--   0        0        0     4419 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/message.py
+-rw-r--r--   0        0        0     1302 2023-07-29 04:29:08.914201 iamai_adapter_mirai-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 iamai_adapter_mirai-3.2.3/PKG-INFO
```

### Comparing `iamai_adapter_mirai-3.2.1/LICENSE` & `iamai_adapter_mirai-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/__init__.py` & `iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.url = self.config.url
         self.reconnect_interval = self.config.reconnect_interval
         self._api_response_cond = asyncio.Condition()
         await super().startup()
 
     async def reverse_ws_connection_hook(self):
         """反向 WebSocket 连接建立时的钩子函数。"""
-        logger.info(f"WebSocket connected!")
+        logger.info("WebSocket connected!")
         asyncio.create_task(self.verify_identity())
 
     async def websocket_connect(self):
         """创建正向 WebSocket 连接。"""
         assert self.session is not None
         logger.info("Trying to verify identity and create connection...")
         async with self.session.ws_connect(
@@ -231,15 +231,15 @@
         Returns:
             API 响应。
 
         Raises:
             TypeError: message_type 非法。
             ...: 同 `call_api()` 方法。
         """
-        if message_type == "private" or message_type == "friend":
+        if message_type in ["private", "friend"]:
             return await self.sendFriendMessage(
                 target=target, messageChain=MiraiMessage(message_), quote=quote
             )
         elif message_type == "group":
             return await self.sendGroupMessage(
                 target=target, messageChain=MiraiMessage(message_), quote=quote
             )
```

### Comparing `iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/config.py` & `iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/config.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/__init__.py` & `iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/base.py` & `iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/base.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/mate.py` & `iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/mate.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/message.py` & `iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/message.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/notice.py` & `iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/notice.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/event/request.py` & `iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/event/request.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/exceptions.py` & `iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-3.2.1/iamai/adapter/mirai/message.py` & `iamai_adapter_mirai-3.2.3/iamai/adapter/mirai/message.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-3.2.1/pyproject.toml` & `iamai_adapter_mirai-3.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-mirai"
-version = "3.2.1"
+version = "3.2.3"
 description = "Mirai adapter for iamai."
 authors = ["简律纯 <i@jyunko.cn>"]
 license = "GPL-3.0 License"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
@@ -20,15 +20,15 @@
     "Topic :: Communications :: Chat",
 ]
 packages = [{ include = "iamai" }]
 exclude = ["iamai/__init__.py", "iamai/adapter/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-iamai = "^3.2"
+iamai = ">=3.2"
 
 [tool.poetry.dev-dependencies]
 iamai = { path = "../../", develop = true }
 
 [tool.pydantic-pycharm-plugin]
 ignore-init-method-arguments = true
```

### Comparing `iamai_adapter_mirai-3.2.1/PKG-INFO` & `iamai_adapter_mirai-3.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-mirai
-Version: 3.2.1
+Version: 3.2.3
 Summary: Mirai adapter for iamai.
 Home-page: https://retrofor.space/
 License: GPL-3.0 License
 Keywords: bot,chatbot,qq,qqbot,mirai
 Author: 简律纯
 Author-email: i@jyunko.cn
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
-Requires-Dist: iamai (>=3.2,<4.0)
+Requires-Dist: iamai (>=3.2)
 Project-URL: Documentation, https://iamai.retrofor.space/
 Project-URL: Repository, https://github.com/retrofor/iamai
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://docs.iamai.dev/"><img src="https://raw.githubusercontent.com/retrofor/iamai/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: iamai-adapter-mirai Version: 3.2.1 Summary: Mirai
+Metadata-Version: 2.1 Name: iamai-adapter-mirai Version: 3.2.3 Summary: Mirai
 adapter for iamai. Home-page: https://retrofor.space/ License: GPL-3.0 License
 Keywords: bot,chatbot,qq,qqbot,mirai Author: ç®å¾çº¯ Author-email:
 i@jyunko.cn Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Framework :: AsyncIO Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library Classifier: License :: OSI
 Approved :: MIT License Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Communications :: Chat Requires-Dist: iamai (>=3.2,<4.0) Project-URL:
+Topic :: Communications :: Chat Requires-Dist: iamai (>=3.2) Project-URL:
 Documentation, https://iamai.retrofor.space/ Project-URL: Repository, https://
 github.com/retrofor/iamai Description-Content-Type: text/markdown
               [logo] # iamai-Adapter-Mirai **Mirai åè®®éé**
```

