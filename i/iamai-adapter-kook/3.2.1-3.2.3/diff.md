# Comparing `tmp/iamai_adapter_kook-3.2.1.tar.gz` & `tmp/iamai_adapter_kook-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_kook-3.2.1.tar", max compression
+gzip compressed data, was "iamai_adapter_kook-3.2.3.tar", max compression
```

## Comparing `iamai_adapter_kook-3.2.1.tar` & `iamai_adapter_kook-3.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34522 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/LICENSE
--rw-r--r--   0        0        0      239 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/README.md
--rw-r--r--   0        0        0    10236 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/iamai/adapter/kook/__init__.py
--rw-r--r--   0        0        0       64 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/iamai/adapter/kook/api/__init__.py
--rw-r--r--   0        0        0       25 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/iamai/adapter/kook/api/client.py
--rw-r--r--   0        0        0    12026 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/iamai/adapter/kook/api/client.pyi
--rw-r--r--   0        0        0     4149 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/iamai/adapter/kook/api/handle.py
--rw-r--r--   0        0        0    12569 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/iamai/adapter/kook/api/model.py
--rw-r--r--   0        0        0      834 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/iamai/adapter/kook/config.py
--rw-r--r--   0        0        0    22816 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/iamai/adapter/kook/event.py
--rw-r--r--   0        0        0     2113 2023-07-15 05:23:38.793804 iamai_adapter_kook-3.2.1/iamai/adapter/kook/exceptions.py
--rw-r--r--   0        0        0    14432 2023-07-15 05:23:38.797804 iamai_adapter_kook-3.2.1/iamai/adapter/kook/message.py
--rw-r--r--   0        0        0     1306 2023-07-15 05:23:38.797804 iamai_adapter_kook-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 iamai_adapter_kook-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/LICENSE
+-rw-r--r--   0        0        0      239 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/README.md
+-rw-r--r--   0        0        0    14584 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/iamai/adapter/kook/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/iamai/adapter/kook/api/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/iamai/adapter/kook/api/client.py
+-rw-r--r--   0        0        0    12026 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/iamai/adapter/kook/api/client.pyi
+-rw-r--r--   0        0        0     4149 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/iamai/adapter/kook/api/handle.py
+-rw-r--r--   0        0        0    12569 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/iamai/adapter/kook/api/model.py
+-rw-r--r--   0        0        0      872 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/iamai/adapter/kook/config.py
+-rw-r--r--   0        0        0    23161 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/iamai/adapter/kook/event.py
+-rw-r--r--   0        0        0     2113 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/iamai/adapter/kook/exceptions.py
+-rw-r--r--   0        0        0    14133 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/iamai/adapter/kook/message.py
+-rw-r--r--   0        0        0     1337 2023-07-29 04:29:08.914201 iamai_adapter_kook-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 iamai_adapter_kook-3.2.3/PKG-INFO
```

### Comparing `iamai_adapter_kook-3.2.1/LICENSE` & `iamai_adapter_kook-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iamai_adapter_kook-3.2.1/iamai/adapter/kook/api/client.pyi` & `iamai_adapter_kook-3.2.3/iamai/adapter/kook/api/client.pyi`

 * *Files identical despite different names*

### Comparing `iamai_adapter_kook-3.2.1/iamai/adapter/kook/api/handle.py` & `iamai_adapter_kook-3.2.3/iamai/adapter/kook/api/handle.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_kook-3.2.1/iamai/adapter/kook/api/model.py` & `iamai_adapter_kook-3.2.3/iamai/adapter/kook/api/model.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_kook-3.2.1/iamai/adapter/kook/config.py` & `iamai_adapter_kook-3.2.3/iamai/adapter/kook/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,7 +19,8 @@
     __config_name__ = "kook"
     adapter_type: Literal["ws", "wb"] = "ws"
     reconnect_interval: int = 3
     api_timeout: int = 1000
     access_token: str = ""
     compress: Literal[0, 1] = 0
     show_raw: bool = False
+    report_self_message: bool = False
```

### Comparing `iamai_adapter_kook-3.2.1/iamai/adapter/kook/event.py` & `iamai_adapter_kook-3.2.3/iamai/adapter/kook/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -514,15 +514,14 @@
     target_id: str
     """
     发送目的\n
     频道消息类时, 代表的是频道 channel_id\n
     如果 channel_type 为 GROUP 组播且 type 为 255 系统消息时，则代表服务器 guild_id"""
     author_id: Optional[str] = None
     content: str
-    message: str
     msg_id: str
     msg_timestamp: int
     nonce: str
     extra: Extra
     user_id: str
 
     post_type: str
@@ -535,26 +534,25 @@
 
     __event__ = "message"
 
     post_type: Literal["message"] = "message"
     message_type: str  # group private 其实是person
     sub_type: str
     event: EventMessage
-    message: KookMessage
 
     def __repr__(self) -> str:
-        return f'Event<{self.type}>: "{self.message}"'
+        return f'Event<{self.type}>: "{self.content}"'
 
     def get_plain_text(self) -> str:
         """获取消息的纯文本内容。
 
         Returns:
             消息的纯文本内容。
         """
-        return self.message.get_plain_text()  # type: ignore
+        return self.content.get_plain_text()  # type: ignore
 
     async def reply(self, msg: "T_KookMSG") -> Dict[str, Any]:
         """回复消息。
 
         Args:
             msg: 回复消息的内容，同 `call_api()` 方法。
 
@@ -566,22 +564,32 @@
 
 class PrivateMessageEvent(MessageEvent):
     """私聊消息"""
 
     __event__ = "message.private"
     message_type: Literal["private"]
 
+    async def reply(self, msg: "T_KookMSG") -> Dict[str, Any]:
+        return await self.adapter.call_api(
+            api="direct-message/create", target_id=self.author_id, content=msg
+        )
+
 
 class ChannelMessageEvent(MessageEvent):
     """公共频道消息"""
 
     __event__ = "message.group"
     message_type: Literal["group"]
     group_id: str
 
+    async def reply(self, msg: "T_KookMSG") -> Dict[str, Any]:
+        return await self.adapter.call_api(
+            "message/create", target_id=self.target_id, content=msg
+        )
+
 
 # Notice Events
 class NoticeEvent(KookEvent):
     """通知事件"""
 
     __event__ = "notice"
     post_type: Literal["notice"]
@@ -869,15 +877,15 @@
     __event__ = "notice.message_btn_click"
     notice_type: Literal["message_btn_click"]
     user_id: str
     group_id: int
 
 
 # Meta Events
-class MetaEvent(KookEvent):
+class MetaEvent(OriginEvent):
     """元事件"""
 
     __event__ = "meta_event"
     post_type: Literal["meta_event"]
     meta_event_type: str
 
 
@@ -897,15 +905,15 @@
     sub_type: str
 
 
 # 事件类映射
 _kook_events = {
     model.__event__: model
     for model in globals().values()
-    if inspect.isclass(model) and issubclass(model, KookEvent)
+    if inspect.isclass(model) and issubclass(model, OriginEvent)
 }
 
 
 def get_event_class(
     post_type: str, event_type: str, sub_type: Optional[str] = None
 ) -> Type[T_KookEvent]:  # type: ignore
     """根据接收到的消息类型返回对应的事件类。
```

### Comparing `iamai_adapter_kook-3.2.1/iamai/adapter/kook/exceptions.py` & `iamai_adapter_kook-3.2.3/iamai/adapter/kook/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_kook-3.2.1/iamai/adapter/kook/message.py` & `iamai_adapter_kook-3.2.3/iamai/adapter/kook/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Kook 适配器消息。"""
+
 import json
 from io import StringIO
 from dataclasses import dataclass
 from typing_extensions import override, deprecated
 from typing import Any, Dict, Type, Tuple, Union, Mapping, Iterable, Optional, cast
 
 from iamai.message import Message, MessageSegment
@@ -27,18 +28,15 @@
     "video": 3,
     "file": 4,
     "audio": 8,
     "kmarkdown": 9,
     "card": 10,
 }
 
-rev_msg_type_map = {}
-for msg_type, code in msg_type_map.items():
-    rev_msg_type_map[code] = msg_type
-
+rev_msg_type_map = {code: msg_type for msg_type, code in msg_type_map.items()}
 # 根据协议消息段类型显示消息段内容
 segment_text = {
     "text": "[文字]",
     "image": "[图片]",
     "video": "[视频]",
     "file": "[文件]",
     "audio": "[音频]",
@@ -99,15 +97,15 @@
     def conduct(
         self, other: Union[str, "KookMessageSegment", Iterable["KookMessageSegment"]]
     ) -> "KookMessageSegment":
         """
         连接两个或多个 MessageSegment，必须为纯文本段或 KMarkdown 段
         """
 
-        if isinstance(other, str) or isinstance(other, KookMessageSegment):
+        if isinstance(other, (str, KookMessageSegment)):
             other = [other]  # type: ignore
         msg = KookMessage([self, *other])
         msg.reduce()  # type: ignore
 
         if len(msg) != 1:
             raise UnsupportedMessageOperation("必须为纯文本段或 KMarkdown 段")
         else:
@@ -329,17 +327,17 @@
     message: Message
 
     def serialize(self, for_send: bool = True) -> Tuple[int, str]:
         if len(self.message) != 1:
             self.message = self.message.copy()
             self.message.reduce()  # type: ignore
 
-            if len(self.message) != 1:
-                # 转化为卡片消息发送
-                return MessageSerializer(KookMessage(_convert_to_card_message(self.message))).serialize()  # type: ignore
+        if len(self.message) != 1:
+            # 转化为卡片消息发送
+            return MessageSerializer(KookMessage(_convert_to_card_message(self.message))).serialize()  # type: ignore
 
         msg_type = self.message[0].type
         msg_type_code = msg_type_map[msg_type]
         # bot 发送消息只支持"text", "kmarkdown", "card"
         # 经测试还支持"image", "video", "file"
         if msg_type in ("text", "kmarkdown", "card"):
             return msg_type_code, self.message[0].data["content"]
@@ -383,23 +381,19 @@
         elif self.type == "kmarkdown":
             content = self.data["content"]
             raw_content = self.data["kmarkdown"]["raw_content"]
 
             # raw_content默认strip掉首尾空格，但是开黑啦本体的聊天界面中不会strip，所以这里还原了
             unescaped = unescape_kmarkdown(content)
             is_plain_text = unescaped.strip() == raw_content
-            if is_plain_text:
-                raw_content = unescaped
-
-            # 如果是KMarkdown消息是纯文本，直接构造纯文本消息
-            # 目的是让on_command等依赖__str__的规则能够在消息存在转义字符时正常工作
-            if is_plain_text:
-                return KookMessage(KookMessageSegment.text(raw_content))
-            else:
+            if not is_plain_text:
                 return KookMessage(KookMessageSegment.KMarkdown(content, raw_content))
+            raw_content = unescaped
+
+            return KookMessage(KookMessageSegment.text(raw_content))
         elif self.type == "card":
             return KookMessage(KookMessageSegment.Card(self.data["content"]))
         else:
             return KookMessage(KookMessageSegment(self.type, self.data))
 
 
 def escape_kmarkdown(content: str):
```

### Comparing `iamai_adapter_kook-3.2.1/pyproject.toml` & `iamai_adapter_kook-3.2.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-kook"
-version = "3.2.1"
+version = "3.2.3"
 description = "Kook adapter for iamai."
 authors = ["简律纯 <i@jyunko.cn>"]
 license = "GPL-3.0 License"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
@@ -20,15 +20,16 @@
     "Topic :: Communications :: Chat",
 ]
 packages = [{ include = "iamai" }]
 exclude = ["iamai/__init__.py", "iamai/adapter/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-iamai = "^3.2"
+iamai = ">=3.2"
+typing-extensions = ">=4.7.0"
 
 [tool.poetry.dev-dependencies]
 iamai = { path = "../../", develop = true }
 
 [tool.pydantic-pycharm-plugin]
 ignore-init-method-arguments = true
```

### Comparing `iamai_adapter_kook-3.2.1/PKG-INFO` & `iamai_adapter_kook-3.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-kook
-Version: 3.2.1
+Version: 3.2.3
 Summary: Kook adapter for iamai.
 Home-page: https://retrofor.space/
 License: GPL-3.0 License
 Keywords: bot,chatbot,kook,kookbot,kaiheila
 Author: 简律纯
 Author-email: i@jyunko.cn
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
-Requires-Dist: iamai (>=3.2,<4.0)
+Requires-Dist: iamai (>=3.2)
+Requires-Dist: typing-extensions (>=4.7.0)
 Project-URL: Documentation, https://iamai.retrofor.space/
 Project-URL: Repository, https://github.com/retrofor/iamai
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://docs.iamai.dev/"><img src="https://raw.githubusercontent.com/retrofor/iamai/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: iamai-adapter-kook Version: 3.2.1 Summary: Kook
+Metadata-Version: 2.1 Name: iamai-adapter-kook Version: 3.2.3 Summary: Kook
 adapter for iamai. Home-page: https://retrofor.space/ License: GPL-3.0 License
 Keywords: bot,chatbot,kook,kookbot,kaiheila Author: ç®å¾çº¯ Author-email:
 i@jyunko.cn Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Framework :: AsyncIO Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library Classifier: License :: OSI
 Approved :: MIT License Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Communications :: Chat Requires-Dist: iamai (>=3.2,<4.0) Project-URL:
-Documentation, https://iamai.retrofor.space/ Project-URL: Repository, https://
-github.com/retrofor/iamai Description-Content-Type: text/markdown
+Topic :: Communications :: Chat Requires-Dist: iamai (>=3.2) Requires-Dist:
+typing-extensions (>=4.7.0) Project-URL: Documentation, https://
+iamai.retrofor.space/ Project-URL: Repository, https://github.com/retrofor/
+iamai Description-Content-Type: text/markdown
                [logo] # iamai-Adapter-Kook **Kook åè®®éé**
```

