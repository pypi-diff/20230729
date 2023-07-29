# Comparing `tmp/iamai_adapter_dingtalk-3.2.1.tar.gz` & `tmp/iamai_adapter_dingtalk-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_dingtalk-3.2.1.tar", max compression
+gzip compressed data, was "iamai_adapter_dingtalk-3.2.3.tar", max compression
```

## Comparing `iamai_adapter_dingtalk-3.2.1.tar` & `iamai_adapter_dingtalk-3.2.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      247 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/README.md
--rw-r--r--   0        0        0     5440 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/__init__.py
--rw-r--r--   0        0        0      590 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/config.py
--rw-r--r--   0        0        0     2363 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/event.py
--rw-r--r--   0        0        0      387 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/exceptions.py
--rw-r--r--   0        0        0     3200 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/message.py
--rw-r--r--   0        0        0     1294 2023-07-15 05:23:38.793804 iamai_adapter_dingtalk-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 iamai_adapter_dingtalk-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-07-29 04:29:08.914201 iamai_adapter_dingtalk-3.2.3/LICENSE
+-rw-r--r--   0        0        0      247 2023-07-29 04:29:08.914201 iamai_adapter_dingtalk-3.2.3/README.md
+-rw-r--r--   0        0        0     5382 2023-07-29 04:29:08.914201 iamai_adapter_dingtalk-3.2.3/iamai/adapter/dingtalk/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-29 04:29:08.914201 iamai_adapter_dingtalk-3.2.3/iamai/adapter/dingtalk/config.py
+-rw-r--r--   0        0        0     2363 2023-07-29 04:29:08.914201 iamai_adapter_dingtalk-3.2.3/iamai/adapter/dingtalk/event.py
+-rw-r--r--   0        0        0      387 2023-07-29 04:29:08.914201 iamai_adapter_dingtalk-3.2.3/iamai/adapter/dingtalk/exceptions.py
+-rw-r--r--   0        0        0     3118 2023-07-29 04:29:08.914201 iamai_adapter_dingtalk-3.2.3/iamai/adapter/dingtalk/message.py
+-rw-r--r--   0        0        0     1295 2023-07-29 04:29:08.914201 iamai_adapter_dingtalk-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 iamai_adapter_dingtalk-3.2.3/PKG-INFO
```

### Comparing `iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/__init__.py` & `iamai_adapter_dingtalk-3.2.3/iamai/adapter/dingtalk/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     async def handler(self, request: web.Request):
         """处理 aiohttp 服务器的接收。
 
         Args:
             request: aiohttp 服务器的 Request 对象。
         """
         if "timestamp" not in request.headers or "sign" not in request.headers:
-            logger.error(f"Illegal http header, incomplete http header")
+            logger.error("Illegal http header, incomplete http header")
         elif abs(int(request.headers["timestamp"]) - time.time() * 1000) > 3600000:
             logger.error(
                 f'Illegal http header, timestamp: {request.headers["timestamp"]}'
             )
         elif request.headers["sign"] != self.get_sign(request.headers["timestamp"]):
             logger.error(f'Illegal http header, sign: {request.headers["sign"]}')
         else:
@@ -92,15 +92,15 @@
             timestamp: 时间戳。
 
         Returns:
             签名。
         """
         hmac_code = hmac.new(
             self.config.app_secret.encode("utf-8"),
-            "{}\n{}".format(timestamp, self.config.app_secret).encode("utf-8"),
+            f"{timestamp}\n{self.config.app_secret}".encode("utf-8"),
             digestmod=hashlib.sha256,
         ).digest()
         return base64.b64encode(hmac_code).decode("utf-8")
 
     async def send(
         self,
         webhook: str,
@@ -133,17 +133,15 @@
         else:
             raise TypeError(
                 f"msg must be str, Dict or DingTalkMessage, not {type(msg)!r}"
             )
 
         if at is not None:
             if isinstance(at, DingTalkMessage):
-                if at.type == "at":
-                    pass
-                else:
+                if at.type != "at":
                     raise ValueError(f'at.type must be "at", not {at.type}')
             elif isinstance(at, dict):
                 at = DingTalkMessage.raw(at)
             else:
                 raise TypeError(f"at must be Dict or DingTalkMessage, not {type(at)!r}")
 
         if conversation_type == "1":
```

### Comparing `iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/config.py` & `iamai_adapter_dingtalk-3.2.3/iamai/adapter/dingtalk/config.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/event.py` & `iamai_adapter_dingtalk-3.2.3/iamai/adapter/dingtalk/event.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_dingtalk-3.2.1/iamai/adapter/dingtalk/message.py` & `iamai_adapter_dingtalk-3.2.3/iamai/adapter/dingtalk/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,23 @@
     """DingTalk 消息"""
 
     @property
     def _message_class(self) -> None:
         return None
 
     def __str__(self):
-        if self.type == "text":
-            return self.data["content"]
-        else:
-            return super().__str__()
+        return self.data["content"] if self.type == "text" else super().__str__()
 
     def as_dict(self) -> Dict[str, Dict[str, Any]]:
         """返回符合钉钉消息标准的消息字段字典。
 
         Returns:
             符合钉钉消息标准的消息字段字典。
         """
-        if self.type == "raw":
-            return self.data
-        else:
-            return {self.type: self.data}
+        return self.data if self.type == "raw" else {self.type: self.data}
 
     @classmethod
     def raw(cls, data: Dict[str, Any]) -> "DingTalkMessage":
         """DingTalk 原始消息"""
         return cls(type="raw", data=data)
 
     @classmethod
```

### Comparing `iamai_adapter_dingtalk-3.2.1/pyproject.toml` & `iamai_adapter_dingtalk-3.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-dingtalk"
-version = "3.2.1"
+version = "3.2.3"
 description = "DingTalk adapter for iamai."
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

### Comparing `iamai_adapter_dingtalk-3.2.1/PKG-INFO` & `iamai_adapter_dingtalk-3.2.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-dingtalk
-Version: 3.2.1
+Version: 3.2.3
 Summary: DingTalk adapter for iamai.
 Home-page: https://retrofor.space/
 License: GPL-3.0 License
 Keywords: bot,chatbot,dingtalk
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
-Metadata-Version: 2.1 Name: iamai-adapter-dingtalk Version: 3.2.1 Summary:
+Metadata-Version: 2.1 Name: iamai-adapter-dingtalk Version: 3.2.3 Summary:
 DingTalk adapter for iamai. Home-page: https://retrofor.space/ License: GPL-3.0
 License Keywords: bot,chatbot,dingtalk Author: ç®å¾çº¯ Author-email:
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
            [logo] # iamai-Adapter-Dingtalk **Dingtalk åè®®éé**
```

