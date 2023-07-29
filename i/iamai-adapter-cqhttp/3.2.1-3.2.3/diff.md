# Comparing `tmp/iamai_adapter_cqhttp-3.2.1.tar.gz` & `tmp/iamai_adapter_cqhttp-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_cqhttp-3.2.1.tar", max compression
+gzip compressed data, was "iamai_adapter_cqhttp-3.2.3.tar", max compression
```

## Comparing `iamai_adapter_cqhttp-3.2.1.tar` & `iamai_adapter_cqhttp-3.2.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      246 2023-07-15 05:23:38.793804 iamai_adapter_cqhttp-3.2.1/README.md
--rw-r--r--   0        0        0     7995 2023-07-15 05:23:38.793804 iamai_adapter_cqhttp-3.2.1/iamai/adapter/cqhttp/__init__.py
--rw-r--r--   0        0        0      899 2023-07-15 05:23:38.793804 iamai_adapter_cqhttp-3.2.1/iamai/adapter/cqhttp/config.py
--rw-r--r--   0        0        0    14025 2023-07-15 05:23:38.793804 iamai_adapter_cqhttp-3.2.1/iamai/adapter/cqhttp/event.py
--rw-r--r--   0        0        0      656 2023-07-15 05:23:38.793804 iamai_adapter_cqhttp-3.2.1/iamai/adapter/cqhttp/exceptions.py
--rw-r--r--   0        0        0     7475 2023-07-15 05:23:38.793804 iamai_adapter_cqhttp-3.2.1/iamai/adapter/cqhttp/message.py
--rw-r--r--   0        0        0     1323 2023-07-15 05:23:38.793804 iamai_adapter_cqhttp-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1336 1970-01-01 00:00:00.000000 iamai_adapter_cqhttp-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-07-29 04:29:08.914201 iamai_adapter_cqhttp-3.2.3/LICENSE
+-rw-r--r--   0        0        0      246 2023-07-29 04:29:08.914201 iamai_adapter_cqhttp-3.2.3/README.md
+-rw-r--r--   0        0        0     7954 2023-07-29 04:29:08.914201 iamai_adapter_cqhttp-3.2.3/iamai/adapter/cqhttp/__init__.py
+-rw-r--r--   0        0        0      899 2023-07-29 04:29:08.914201 iamai_adapter_cqhttp-3.2.3/iamai/adapter/cqhttp/config.py
+-rw-r--r--   0        0        0    13961 2023-07-29 04:29:08.914201 iamai_adapter_cqhttp-3.2.3/iamai/adapter/cqhttp/event.py
+-rw-r--r--   0        0        0      656 2023-07-29 04:29:08.914201 iamai_adapter_cqhttp-3.2.3/iamai/adapter/cqhttp/exceptions.py
+-rw-r--r--   0        0        0     7452 2023-07-29 04:29:08.914201 iamai_adapter_cqhttp-3.2.3/iamai/adapter/cqhttp/message.py
+-rw-r--r--   0        0        0     1324 2023-07-29 04:29:08.914201 iamai_adapter_cqhttp-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 iamai_adapter_cqhttp-3.2.3/PKG-INFO
```

### Comparing `iamai_adapter_cqhttp-3.2.1/iamai/adapter/cqhttp/__init__.py` & `iamai_adapter_cqhttp-3.2.3/iamai/adapter/cqhttp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.url = self.config.url
         self.reconnect_interval = self.config.reconnect_interval
         self._api_response_cond = asyncio.Condition()
         await super().startup()
 
     async def reverse_ws_connection_hook(self):
         """反向 WebSocket 连接建立时的钩子函数。"""
-        logger.info(f"WebSocket connected!")
+        logger.info("WebSocket connected!")
         if self.config.access_token:
             if (
                 self.websocket.headers.get("Authorization", "")
                 != f"Bearer {self.config.access_token}"
             ):
                 await self.websocket.close()
 
@@ -114,15 +114,15 @@
         """
         post_type = msg.get("post_type")
 
         # message_sent 自身消息处理
         if post_type == "message_sent":
             event_type = msg.get("message_type")
         else:
-            event_type = msg.get(post_type + "_type")
+            event_type = msg.get(f"{post_type}_type")
 
         sub_type = msg.get("sub_type", None)
         event_class = get_event_class(post_type, event_type, sub_type)
 
         cqhttp_event = event_class(adapter=self, **msg)
 
         if cqhttp_event.post_type == "meta_event":
@@ -132,17 +132,15 @@
                 and cqhttp_event.sub_type == "connect"
             ):
                 logger.success(
                     f"WebSocket connection "
                     f"from CQHTTP Bot {msg.get('self_id')} accepted!"
                 )
             elif cqhttp_event.meta_event_type == "heartbeat":
-                if cqhttp_event.status.good and cqhttp_event.status.online:
-                    pass
-                else:
+                if not cqhttp_event.status.good or not cqhttp_event.status.online:
                     logger.error(
                         f"CQHTTP Bot status is not good: {cqhttp_event.status.dict()}"
                     )
         else:
             await self.handle_event(cqhttp_event)
 
     async def call_api(self, api: str, **params) -> Dict[str, Any]:
```

### Comparing `iamai_adapter_cqhttp-3.2.1/iamai/adapter/cqhttp/config.py` & `iamai_adapter_cqhttp-3.2.3/iamai/adapter/cqhttp/config.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_cqhttp-3.2.1/iamai/adapter/cqhttp/event.py` & `iamai_adapter_cqhttp-3.2.3/iamai/adapter/cqhttp/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,18 +84,15 @@
     self_id: int
     self_tiny_id: Optional[str]
     post_type: Literal["message", "message_sent", "notice", "request", "meta_event"]
 
     @property
     def to_me(self) -> bool:
         """当前事件的 user_id 是否等于 self_id 或 self_tiny_id。"""
-        return (
-            getattr(self, "user_id") == self.self_id
-            or getattr(self, "user_id") == self.self_tiny_id
-        )
+        return getattr(self, "user_id") in [self.self_id, self.self_tiny_id]
 
 
 class MessageEvent(CQHTTPEvent):
     """消息事件"""
 
     __event__ = "message"
     post_type: Literal["message"]
```

### Comparing `iamai_adapter_cqhttp-3.2.1/iamai/adapter/cqhttp/exceptions.py` & `iamai_adapter_cqhttp-3.2.3/iamai/adapter/cqhttp/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_cqhttp-3.2.1/iamai/adapter/cqhttp/message.py` & `iamai_adapter_cqhttp-3.2.3/iamai/adapter/cqhttp/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,15 @@
     """CQHTTP 消息字段。"""
 
     @property
     def _message_class(self) -> Type["CQHTTPMessage"]:
         return CQHTTPMessage
 
     def __str__(self) -> str:
-        if self.type == "text":
-            return self.data.get("text", "")
-        return self.get_cqcode()
+        return self.data.get("text", "") if self.type == "text" else self.get_cqcode()
 
     def get_cqcode(self) -> str:
         """
         Returns:
             此消息字段的 CQ 码形式。
         """
         if self.type == "text":
```

### Comparing `iamai_adapter_cqhttp-3.2.1/pyproject.toml` & `iamai_adapter_cqhttp-3.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-cqhttp"
-version = "3.2.1"
+version = "3.2.3"
 description = "OneBot(go-cqhttp) adapter for iamai."
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

### Comparing `iamai_adapter_cqhttp-3.2.1/PKG-INFO` & `iamai_adapter_cqhttp-3.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-cqhttp
-Version: 3.2.1
+Version: 3.2.3
 Summary: OneBot(go-cqhttp) adapter for iamai.
 Home-page: https://retrofor.space/
 License: GPL-3.0 License
 Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq
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
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: iamai-adapter-cqhttp Version: 3.2.1 Summary: OneBot
+Metadata-Version: 2.1 Name: iamai-adapter-cqhttp Version: 3.2.3 Summary: OneBot
 (go-cqhttp) adapter for iamai. Home-page: https://retrofor.space/ License: GPL-
 3.0 License Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq Author: ç®å¾çº¯
 Author-email: i@jyunko.cn Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework ::
 Robot Framework Classifier: Framework :: Robot Framework :: Library Classifier:
 License :: OSI Approved :: MIT License Classifier: License :: Other/Proprietary
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Communications :: Chat Requires-Dist: iamai (>=3.2,<4.0)
+Classifier: Topic :: Communications :: Chat Requires-Dist: iamai (>=3.2)
 Project-URL: Documentation, https://iamai.retrofor.space/ Project-URL:
 Repository, https://github.com/retrofor/iamai Description-Content-Type: text/
 markdown
            [logo] # iamai-Adapter-CQHTTP **go-cqhttp åè®®éé**
```

