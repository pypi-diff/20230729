# Comparing `tmp/nonechat-0.2.0.tar.gz` & `tmp/nonechat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonechat-0.2.0.tar", last modified: Mon Jul 17 01:21:04 2023, max compression
+gzip compressed data, was "nonechat-0.2.1.tar", last modified: Sat Jul 29 06:15:25 2023, max compression
```

## Comparing `nonechat-0.2.0.tar` & `nonechat-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      523 2023-07-17 01:20:32.519825 nonechat-0.2.0/README.md
--rw-r--r--   0        0        0      359 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/__init__.py
--rw-r--r--   0        0        0     3756 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/app.py
--rw-r--r--   0        0        0      674 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/backend.py
--rw-r--r--   0        0        0        0 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/__init__.py
--rw-r--r--   0        0        0      950 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/action.py
--rw-r--r--   0        0        0      913 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/chatroom/__init__.py
--rw-r--r--   0        0        0     2013 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/chatroom/history.py
--rw-r--r--   0        0        0     1418 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/chatroom/input.py
--rw-r--r--   0        0        0     4053 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/chatroom/message.py
--rw-r--r--   0        0        0     2396 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/chatroom/toolbar.py
--rw-r--r--   0        0        0       45 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/footer.py
--rw-r--r--   0        0        0     1184 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/header.py
--rw-r--r--   0        0        0     1508 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/log/__init__.py
--rw-r--r--   0        0        0     1561 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/components/log/toolbar.py
--rw-r--r--   0        0        0      582 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/info.py
--rw-r--r--   0        0        0     1143 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/log_redirect.py
--rw-r--r--   0        0        0     4132 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/message.py
--rw-r--r--   0        0        0       92 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/router/__init__.py
--rw-r--r--   0        0        0     1222 2023-07-17 01:20:32.519825 nonechat-0.2.0/nonechat/router/router.py
--rw-r--r--   0        0        0      690 2023-07-17 01:20:32.523825 nonechat-0.2.0/nonechat/setting.py
--rw-r--r--   0        0        0     2079 2023-07-17 01:20:32.523825 nonechat-0.2.0/nonechat/storage/__init__.py
--rw-r--r--   0        0        0      285 2023-07-17 01:20:32.523825 nonechat-0.2.0/nonechat/utils.py
--rw-r--r--   0        0        0     1905 2023-07-17 01:20:32.523825 nonechat-0.2.0/nonechat/views/horizontal.py
--rw-r--r--   0        0        0      700 2023-07-17 01:20:32.523825 nonechat-0.2.0/nonechat/views/log_view.py
--rw-r--r--   0        0        0     1303 2023-07-17 01:21:04.676749 nonechat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 nonechat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      523 2023-07-29 06:14:42.207416 nonechat-0.2.1/README.md
+-rw-r--r--   0        0        0      359 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/__init__.py
+-rw-r--r--   0        0        0     3756 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/app.py
+-rw-r--r--   0        0        0      674 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/backend.py
+-rw-r--r--   0        0        0        0 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/components/__init__.py
+-rw-r--r--   0        0        0      950 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/components/action.py
+-rw-r--r--   0        0        0      913 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/components/chatroom/__init__.py
+-rw-r--r--   0        0        0     2013 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/components/chatroom/history.py
+-rw-r--r--   0        0        0     1418 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/components/chatroom/input.py
+-rw-r--r--   0        0        0     4053 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/components/chatroom/message.py
+-rw-r--r--   0        0        0     2396 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/components/chatroom/toolbar.py
+-rw-r--r--   0        0        0       45 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/components/footer.py
+-rw-r--r--   0        0        0     1184 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/components/header.py
+-rw-r--r--   0        0        0     1508 2023-07-29 06:14:42.207416 nonechat-0.2.1/nonechat/components/log/__init__.py
+-rw-r--r--   0        0        0     1561 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/components/log/toolbar.py
+-rw-r--r--   0        0        0      582 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/info.py
+-rw-r--r--   0        0        0     1143 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/log_redirect.py
+-rw-r--r--   0        0        0     4138 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/message.py
+-rw-r--r--   0        0        0       92 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/router/__init__.py
+-rw-r--r--   0        0        0     1222 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/router/router.py
+-rw-r--r--   0        0        0      690 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/setting.py
+-rw-r--r--   0        0        0     2079 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/storage/__init__.py
+-rw-r--r--   0        0        0      285 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/utils.py
+-rw-r--r--   0        0        0     1905 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/views/horizontal.py
+-rw-r--r--   0        0        0      700 2023-07-29 06:14:42.211416 nonechat-0.2.1/nonechat/views/log_view.py
+-rw-r--r--   0        0        0     1394 2023-07-29 06:15:25.971492 nonechat-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 nonechat-0.2.1/PKG-INFO
```

### Comparing `nonechat-0.2.0/README.md` & `nonechat-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/app.py` & `nonechat-0.2.1/nonechat/app.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/backend.py` & `nonechat-0.2.1/nonechat/backend.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/components/action.py` & `nonechat-0.2.1/nonechat/components/action.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/components/chatroom/__init__.py` & `nonechat-0.2.1/nonechat/components/chatroom/__init__.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/components/chatroom/history.py` & `nonechat-0.2.1/nonechat/components/chatroom/history.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/components/chatroom/input.py` & `nonechat-0.2.1/nonechat/components/chatroom/input.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/components/chatroom/message.py` & `nonechat-0.2.1/nonechat/components/chatroom/message.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/components/chatroom/toolbar.py` & `nonechat-0.2.1/nonechat/components/chatroom/toolbar.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/components/header.py` & `nonechat-0.2.1/nonechat/components/header.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/components/log/__init__.py` & `nonechat-0.2.1/nonechat/components/log/__init__.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/components/log/toolbar.py` & `nonechat-0.2.1/nonechat/components/log/toolbar.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/info.py` & `nonechat-0.2.1/nonechat/info.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/log_redirect.py` & `nonechat-0.2.1/nonechat/log_redirect.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/message.py` & `nonechat-0.2.1/nonechat/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from dataclasses import field, asdict, dataclass
-from typing import Union, Iterator, Optional, Sequence, overload
+from typing import List, Union, Iterator, Optional, Sequence, overload
 
 from rich.style import Style
 from rich.segment import Segment
 from rich.emoji import EmojiVariant
 from rich.text import Text as RichText
 from rich.emoji import Emoji as RichEmoji
 from rich.markdown import Markdown as RichMarkdown
@@ -114,17 +114,17 @@
         self, index: Union[int, slice]
     ) -> Union[Element, Sequence[Element]]:
         return self.content[index]
 
     def __len__(self) -> int:
         return len(self.content)
 
-    content: list[Element]
+    content: List[Element]
 
-    def __init__(self, elements: list[Element]):
+    def __init__(self, elements: List[Element]):
         """从传入的序列(可以是元组 tuple, 也可以是列表 list) 创建消息链.
         Args:
             elements (list[T]): 包含且仅包含消息元素的序列
         Returns:
             MessageChain: 以传入的序列作为所承载消息的消息链
         """
         self.content = elements
```

### Comparing `nonechat-0.2.0/nonechat/router/router.py` & `nonechat-0.2.1/nonechat/router/router.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/setting.py` & `nonechat-0.2.1/nonechat/setting.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/storage/__init__.py` & `nonechat-0.2.1/nonechat/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/views/horizontal.py` & `nonechat-0.2.1/nonechat/views/horizontal.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/nonechat/views/log_view.py` & `nonechat-0.2.1/nonechat/views/log_view.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.2.0/pyproject.toml` & `nonechat-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 dependencies = [
     "textual ~=0.29.0",
 ]
 requires-python = ">=3.8, <4.0"
 readme = "README.md"
 dynamic = []
-version = "0.2.0"
+version = "0.2.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/nonebot/nonechat"
 repository = "https://github.com/nonebot/nonechat"
@@ -74,12 +74,17 @@
 ignore = [
     "C901",
     "T201",
 ]
 line-length = 88
 target-version = "py38"
 
+[tool.pyright]
+pythonVersion = "3.8"
+pythonPlatform = "All"
+reportShadowedImports = false
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `nonechat-0.2.0/PKG-INFO` & `nonechat-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonechat
-Version: 0.2.0
+Version: 0.2.1
 Summary: Awesome chat console using Textual
 Home-page: https://github.com/nonebot/nonechat
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonebot/nonechat
 Project-URL: Repository, https://github.com/nonebot/nonechat
 Requires-Python: <4.0,>=3.8
```

