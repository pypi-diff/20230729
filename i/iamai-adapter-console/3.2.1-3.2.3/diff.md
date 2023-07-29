# Comparing `tmp/iamai_adapter_console-3.2.1.tar.gz` & `tmp/iamai_adapter_console-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_console-3.2.1.tar", max compression
+gzip compressed data, was "iamai_adapter_console-3.2.3.tar", max compression
```

## Comparing `iamai_adapter_console-3.2.1.tar` & `iamai_adapter_console-3.2.3.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0      245 2023-07-15 05:23:38.793804 iamai_adapter_console-3.2.1/README.md
--rw-r--r--   0        0        0     1041 2023-07-15 05:23:38.793804 iamai_adapter_console-3.2.1/iamai/adapter/console/__init__.py
--rw-r--r--   0        0        0      283 2023-07-15 05:23:38.793804 iamai_adapter_console-3.2.1/iamai/adapter/console/config.py
--rw-r--r--   0        0        0      932 2023-07-15 05:23:38.793804 iamai_adapter_console-3.2.1/iamai/adapter/console/event.py
--rw-r--r--   0        0        0     1299 2023-07-15 05:23:38.793804 iamai_adapter_console-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 iamai_adapter_console-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-07-29 04:29:08.914201 iamai_adapter_console-3.2.3/LICENSE
+-rw-r--r--   0        0        0      245 2023-07-29 04:29:08.914201 iamai_adapter_console-3.2.3/README.md
+-rw-r--r--   0        0        0      951 2023-07-29 04:29:08.914201 iamai_adapter_console-3.2.3/iamai/adapter/console/__init__.py
+-rw-r--r--   0        0        0      283 2023-07-29 04:29:08.914201 iamai_adapter_console-3.2.3/iamai/adapter/console/config.py
+-rw-r--r--   0        0        0     2500 2023-07-29 04:29:08.914201 iamai_adapter_console-3.2.3/iamai/adapter/console/event.py
+-rw-r--r--   0        0        0      678 2023-07-29 04:29:08.914201 iamai_adapter_console-3.2.3/iamai/adapter/console/message.py
+-rw-r--r--   0        0        0     1300 2023-07-29 04:29:08.914201 iamai_adapter_console-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 iamai_adapter_console-3.2.3/PKG-INFO
```

### Comparing `iamai_adapter_console-3.2.1/iamai/adapter/console/__init__.py` & `iamai_adapter_console-3.2.3/iamai/adapter/console/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,28 +3,21 @@
 """
 from asyncio import Condition
 
 from iamai.event import Event
 from iamai.adapter import Adapter
 
 from .config import Config
+from .event import ConsoleEvent
 
+__all__ = ["ConsoleAdapter"]
 
-class ConsoleEvent(Event["ConsoleAdapter"]):
-    """测试适配器事件。
 
-    Attributes:
-        message: 消息内容。
-    """
-
-    message: str
-
-
-class ConsoleAdapter(Adapter[ConsoleEvent, None]):
-    """测试适配器。"""
+class ConsoleAdapter(Adapter[ConsoleEvent, Config]):
+    """Console适配器。"""
 
     name: str = "console"
     _msg: str = ""
     _cond: Condition
     Config = Config
 
     async def startup(self):
```

### Comparing `iamai_adapter_console-3.2.1/pyproject.toml` & `iamai_adapter_console-3.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-console"
-version = "3.2.1"
+version = "3.2.3"
 description = "Console adapter for iamai."
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

### Comparing `iamai_adapter_console-3.2.1/PKG-INFO` & `iamai_adapter_console-3.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-console
-Version: 3.2.1
+Version: 3.2.3
 Summary: Console adapter for iamai.
 Home-page: https://retrofor.space/
 License: GPL-3.0 License
 Keywords: bot,chatbot,console,Chat
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
-Metadata-Version: 2.1 Name: iamai-adapter-console Version: 3.2.1 Summary:
+Metadata-Version: 2.1 Name: iamai-adapter-console Version: 3.2.3 Summary:
 Console adapter for iamai. Home-page: https://retrofor.space/ License: GPL-3.0
 License Keywords: bot,chatbot,console,Chat Author: ç®å¾çº¯ Author-email:
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
             [logo] # iamai-Adapter-Console **console åè®®éé**
```

