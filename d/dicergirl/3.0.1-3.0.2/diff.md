# Comparing `tmp/dicergirl-3.0.1.tar.gz` & `tmp/dicergirl-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicergirl-3.0.1.tar", last modified: Sat Jul 29 11:05:29 2023, max compression
+gzip compressed data, was "dicergirl-3.0.2.tar", last modified: Sat Jul 29 11:51:29 2023, max compression
```

## Comparing `dicergirl-3.0.1.tar` & `dicergirl-3.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 11:05:29.279598 dicergirl-3.0.1/
--rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.1/LICENSE
--rw-rw-rw-   0        0        0     5492 2023-07-29 11:05:29.279598 dicergirl-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4907 2023-07-29 08:14:02.000000 dicergirl-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 11:05:29.248553 dicergirl-3.0.1/dicergirl/
--rw-rw-rw-   0        0        0    18268 2023-07-29 10:51:25.000000 dicergirl-3.0.1/dicergirl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:05:29.279598 dicergirl-3.0.1/dicergirl/coc/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/coc/__init__.py
--rw-rw-rw-   0        0        0     4330 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/coc/coccards.py
--rw-rw-rw-   0        0        0     9097 2023-07-29 10:28:29.000000 dicergirl-3.0.1/dicergirl/coc/cocutils.py
--rw-rw-rw-   0        0        0     6020 2023-07-29 10:23:31.000000 dicergirl-3.0.1/dicergirl/coc/investigator.py
--rw-rw-rw-   0        0        0    16480 2023-07-29 10:29:57.000000 dicergirl-3.0.1/dicergirl/main.py
--rw-rw-rw-   0        0        0     3039 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/run.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:05:29.279598 dicergirl-3.0.1/dicergirl/scp/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/scp/__init__.py
--rw-rw-rw-   0        0        0     3275 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/scp/agent.py
--rw-rw-rw-   0        0        0     2810 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/scp/scpcards.py
--rw-rw-rw-   0        0        0     5151 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/scp/scputils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:05:29.279598 dicergirl-3.0.1/dicergirl/utils/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/utils/__init__.py
--rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/utils/chat.py
--rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/utils/decorators.py
--rw-rw-rw-   0        0        0     6471 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/utils/dicer.py
--rw-rw-rw-   0        0        0    16180 2023-07-29 07:34:15.000000 dicergirl-3.0.1/dicergirl/utils/handlers.py
--rw-rw-rw-   0        0        0    23138 2023-07-29 10:09:17.000000 dicergirl-3.0.1/dicergirl/utils/messages.py
--rw-rw-rw-   0        0        0      523 2023-07-29 10:56:34.000000 dicergirl-3.0.1/dicergirl/utils/settings.py
--rw-rw-rw-   0        0        0     4624 2023-07-29 11:03:23.000000 dicergirl-3.0.1/dicergirl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:05:29.267468 dicergirl-3.0.1/dicergirl.egg-info/
--rw-rw-rw-   0        0        0     5492 2023-07-29 11:05:29.000000 dicergirl-3.0.1/dicergirl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      672 2023-07-29 11:05:29.000000 dicergirl-3.0.1/dicergirl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:05:29.000000 dicergirl-3.0.1/dicergirl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-29 11:05:29.000000 dicergirl-3.0.1/dicergirl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 11:05:29.000000 dicergirl-3.0.1/dicergirl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 11:05:29.279598 dicergirl-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-07-29 10:54:48.000000 dicergirl-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:51:29.293415 dicergirl-3.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5492 2023-07-29 11:51:29.293415 dicergirl-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4907 2023-07-29 08:14:02.000000 dicergirl-3.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 11:51:29.277759 dicergirl-3.0.2/dicergirl/
+-rw-rw-rw-   0        0        0    18297 2023-07-29 11:49:48.000000 dicergirl-3.0.2/dicergirl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:51:29.293415 dicergirl-3.0.2/dicergirl/coc/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/coc/__init__.py
+-rw-rw-rw-   0        0        0     4330 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/coc/coccards.py
+-rw-rw-rw-   0        0        0     9097 2023-07-29 10:28:29.000000 dicergirl-3.0.2/dicergirl/coc/cocutils.py
+-rw-rw-rw-   0        0        0     6020 2023-07-29 10:23:31.000000 dicergirl-3.0.2/dicergirl/coc/investigator.py
+-rw-rw-rw-   0        0        0    16471 2023-07-29 11:31:10.000000 dicergirl-3.0.2/dicergirl/main.py
+-rw-rw-rw-   0        0        0     3081 2023-07-29 11:48:51.000000 dicergirl-3.0.2/dicergirl/run.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:51:29.293415 dicergirl-3.0.2/dicergirl/scp/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/scp/__init__.py
+-rw-rw-rw-   0        0        0     3275 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/scp/agent.py
+-rw-rw-rw-   0        0        0     2810 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/scp/scpcards.py
+-rw-rw-rw-   0        0        0     5151 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/scp/scputils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:51:29.293415 dicergirl-3.0.2/dicergirl/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/utils/__init__.py
+-rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/utils/chat.py
+-rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/utils/decorators.py
+-rw-rw-rw-   0        0        0     6471 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/utils/dicer.py
+-rw-rw-rw-   0        0        0    16180 2023-07-29 07:34:15.000000 dicergirl-3.0.2/dicergirl/utils/handlers.py
+-rw-rw-rw-   0        0        0    23138 2023-07-29 10:09:17.000000 dicergirl-3.0.2/dicergirl/utils/messages.py
+-rw-rw-rw-   0        0        0     1233 2023-07-29 11:46:42.000000 dicergirl-3.0.2/dicergirl/utils/settings.py
+-rw-rw-rw-   0        0        0     4809 2023-07-29 11:51:24.000000 dicergirl-3.0.2/dicergirl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:51:29.293415 dicergirl-3.0.2/dicergirl.egg-info/
+-rw-rw-rw-   0        0        0     5492 2023-07-29 11:51:29.000000 dicergirl-3.0.2/dicergirl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2023-07-29 11:51:29.000000 dicergirl-3.0.2/dicergirl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 11:51:29.000000 dicergirl-3.0.2/dicergirl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-29 11:51:29.000000 dicergirl-3.0.2/dicergirl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 11:51:29.000000 dicergirl-3.0.2/dicergirl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 11:51:29.293415 dicergirl-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-07-29 10:54:48.000000 dicergirl-3.0.2/setup.py
```

### Comparing `dicergirl-3.0.1/LICENSE` & `dicergirl-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/PKG-INFO` & `dicergirl-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.1
+Version: 3.0.2
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dicergirl-3.0.1/README.md` & `dicergirl-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/__init__.py` & `dicergirl-3.0.2/dicergirl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 DEBUG = False
 current_dir = Path(__file__).resolve().parent
 mode = "scp"
 
 try:
     driver = nonebot.get_driver()
+    set_package("nonebot2")
 except ValueError:
     utilless = True
 else:
     utilless = False
 
 if package == "nonebot2" and not utilless:
     from nonebot.rule import Rule
```

### Comparing `dicergirl-3.0.1/dicergirl/coc/coccards.py` & `dicergirl-3.0.2/dicergirl/coc/coccards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/coc/cocutils.py` & `dicergirl-3.0.2/dicergirl/coc/cocutils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/coc/investigator.py` & `dicergirl-3.0.2/dicergirl/coc/investigator.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/main.py` & `dicergirl-3.0.2/dicergirl/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 from scp.agent import Agent
 from coc.cocutils import sc, st, at, dam, en, rd0, ra, ti, li, rb, rp
 from coc.coccards import cards, cache_cards, sa_handler
 from scp.scpcards import scp_cards, scp_cache_cards
 from scp.scputils import sra, scp_dam, at as sat
 from utils.decorators import Commands
 from utils.messages import help_message, version
-from utils.utils import logger, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, get_handlers
+from utils.utils import logger, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, get_handlers, get_config
 from utils.handlers import scp_set_handler, scp_show_handler, scp_del_handler, set_handler, show_handler, del_handler
 from utils.chat import chat
 
 import botpy
 import logging
 import sys
 
 DEBUG = False
 current_dir = Path(__file__).resolve().parent
-config = read(current_dir / "config.yaml")
+config = get_config()
 mode = "scp"
 get_logger().setLevel(logging.CRITICAL)
 logger.remove()
 logger.add(
     sys.stdout,
     level = "INFO"
 )
```

### Comparing `dicergirl-3.0.1/dicergirl/run.py` & `dicergirl-3.0.2/dicergirl/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,15 @@
                     raise ValueError("监视线程未传入.")
             time.sleep(0.5)
     except KeyboardInterrupt:
         logger.info("用户要求结束任务, 程序退出.")
         sys.exit()
 
 def run():
+    sys.path.insert(0, str(current_dir))
     runpy.run_module(MODULE_TO_RELOAD, run_name="__main__", alter_sys=True)
  
 def main():
     freeze_support()
     try:
         monitor_folder(current_dir, target=run)
     except KeyboardInterrupt:
```

### Comparing `dicergirl-3.0.1/dicergirl/scp/agent.py` & `dicergirl-3.0.2/dicergirl/scp/agent.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/scp/scpcards.py` & `dicergirl-3.0.2/dicergirl/scp/scpcards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/scp/scputils.py` & `dicergirl-3.0.2/dicergirl/scp/scputils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/utils/chat.py` & `dicergirl-3.0.2/dicergirl/utils/chat.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/utils/decorators.py` & `dicergirl-3.0.2/dicergirl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/utils/dicer.py` & `dicergirl-3.0.2/dicergirl/utils/dicer.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/utils/handlers.py` & `dicergirl-3.0.2/dicergirl/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/utils/messages.py` & `dicergirl-3.0.2/dicergirl/utils/messages.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/dicergirl/utils/utils.py` & `dicergirl-3.0.2/dicergirl/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 from loguru import logger
 from typing import Union
 
 try:
     from utils.decorators import translate_punctuation
-    from utils.settings import package
+    from utils.settings import package, setconfig, getconfig
 except ImportError:
     from .decorators import translate_punctuation
-    from .settings import package
+    from .settings import package, setconfig, getconfig
 
 if package == "nonebot2":
     from nonebot.adapters.onebot.v11 import MessageEvent, GroupMessageEvent
     class Message:
         pass
 elif package == "qqguild":
     from botpy.message import Message
@@ -21,29 +21,28 @@
         pass
 
 import json
 import os
 import uuid
 import re
 import inspect
-import yaml
 
 current_dir = Path(__file__).resolve().parent
 dicer_girl_dir = Path.home() / ".dicergirl"
 data_dir = dicer_girl_dir / "data"
 _coc_cachepath = data_dir / "coc_cards.json"
 _scp_cachepath = data_dir / "scp_cards.json"
 _super_user = data_dir / "super_user.json"
 _log = logger
 su_uuid = (str(uuid.uuid1()) + str(uuid.uuid4())).replace("-", "")
-version = "3.0.1"
+version = "3.0.2"
 
 def init():
     if not dicer_girl_dir.exists():
-        _log.info("Dicer Girl 数据文件夹未建立, 建立它.")
+        _log.info("Dicer Girl 文件夹未建立, 建立它.")
         dicer_girl_dir.mkdir()
     if not data_dir.exists():
         _log.info("Dicer Girl 数据文件夹未建立, 建立它.")
         data_dir.mkdir()
     if not os.path.exists(_coc_cachepath):
         _log.info("[cocdicer] COC存储文件未建立, 建立它.")
         with open(_coc_cachepath, "w", encoding="utf-8") as f:
@@ -53,14 +52,20 @@
         with open(_scp_cachepath, "w", encoding="utf-8") as f:
             f.write("{}")
     if not os.path.exists(_super_user):
         _log.info("[cocdicer] 超级用户存储文件未建立, 建立它.")
         with open(_super_user, "w", encoding="utf-8") as f:
             f.write("{}")
 
+def set_config(appid, token):
+    return setconfig(appid, token, path=dicer_girl_dir, filename="config.yaml")
+
+def get_config() -> dict:
+    return getconfig(path=dicer_girl_dir, filename="config.yaml")
+
 def format_msg(message, begin=None):
     msg = format_str(message, begin=begin).split(" ")
     outer = []
     for m in msg:
         m = re.split(r'(\d+)|([a-zA-Z]+)|([\u4e00-\u9fa5]+)', m)
         m = list(filter(None, m))
         outer += m
@@ -80,16 +85,15 @@
             for b in begin:
                 msg = msg.replace(b, "").lstrip(" ")
         else:
             msg = msg.replace(begin, "").lstrip(" ")
     _log.debug(msg)
     return msg
 
-def get_handlers(main, target="Commands"):
-    TARGET_DECORATOR = target
+def get_handlers(main):
     commands_functions = []
 
     for _, obj in vars(main).items():
         if inspect.isfunction(obj) and hasattr(obj, '__annotations__'):
             annotations = obj.__annotations__
             if annotations.get('message') is Message:
                 commands_functions.append(obj)
```

### Comparing `dicergirl-3.0.1/dicergirl.egg-info/PKG-INFO` & `dicergirl-3.0.2/dicergirl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.1
+Version: 3.0.2
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dicergirl-3.0.1/dicergirl.egg-info/SOURCES.txt` & `dicergirl-3.0.2/dicergirl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.1/setup.py` & `dicergirl-3.0.2/setup.py`

 * *Files identical despite different names*

