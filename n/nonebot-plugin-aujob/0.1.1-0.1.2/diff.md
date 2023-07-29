# Comparing `tmp/nonebot_plugin_aujob-0.1.1.tar.gz` & `tmp/nonebot_plugin_aujob-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aujob-0.1.1.tar", last modified: Sat Jul 29 09:04:49 2023, max compression
+gzip compressed data, was "nonebot_plugin_aujob-0.1.2.tar", last modified: Sat Jul 29 12:12:20 2023, max compression
```

## Comparing `nonebot_plugin_aujob-0.1.1.tar` & `nonebot_plugin_aujob-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 09:04:49.669662 nonebot_plugin_aujob-0.1.1/
--rw-rw-rw-   0        0        0      511 2023-07-29 09:04:49.666661 nonebot_plugin_aujob-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 09:04:49.648658 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob/
--rw-rw-rw-   0        0        0     1734 2023-07-29 09:04:02.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob/__init__.py
--rw-rw-rw-   0        0        0    11199 2023-07-29 02:41:44.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:04:49.663661 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/
--rw-rw-rw-   0        0        0      511 2023-07-29 09:04:49.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-29 09:04:49.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 09:04:49.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-29 09:04:49.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-29 09:04:49.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      698 2023-07-29 09:04:33.000000 nonebot_plugin_aujob-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 09:04:49.669662 nonebot_plugin_aujob-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 12:12:20.309430 nonebot_plugin_aujob-0.1.2/
+-rw-rw-rw-   0        0        0      511 2023-07-29 12:12:20.307429 nonebot_plugin_aujob-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 12:12:20.275414 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob/
+-rw-rw-rw-   0        0        0     1709 2023-07-29 12:11:37.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob/__init__.py
+-rw-rw-rw-   0        0        0    11199 2023-07-29 02:41:44.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:12:20.305412 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-07-29 12:12:19.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-29 12:12:20.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 12:12:19.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-29 12:12:19.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-29 12:12:19.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2023-07-29 12:11:53.000000 nonebot_plugin_aujob-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 12:12:20.310430 nonebot_plugin_aujob-0.1.2/setup.cfg
```

### Comparing `nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob/__init__.py` & `nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from nonebot.internal.matcher import Matcher
 from nonebot.plugin import PluginMetadata
 from nonebot import on_startswith
-from nonebot.adapters.onebot.v11 import MessageEvent
+from nonebot.adapters import Event
 
 from .utils import dict_character, dict_else
 
 __plugin_meta__ = PluginMetadata(
     name="Among US中的TOH模组职业介绍",
     description="查询TOH模组里职业的玩法描述",
     usage="发送/auhelp 查看插件帮助信息",
@@ -21,15 +21,15 @@
 )
 
 
 matcher_character = on_startswith(".t ", ignorecase=True, priority=10, block=True)
 
 
 @matcher_character.handle()
-async def _(matcher: Matcher, event: MessageEvent):
+async def _(matcher: Matcher, event: Event):
     """角色资料菜单"""
     plain_text = event.get_message().extract_plain_text().strip()
     plain_text = plain_text.replace(".t ", "")
     if plain_text in dict_character:
         msg = dict_character[plain_text]
     else:
         msg = "命令或职业不存在，请发送\n/auhelp\n查看全部的职业名称"
```

### Comparing `nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob/utils.py` & `nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_aujob-0.1.1/pyproject.toml` & `nonebot_plugin_aujob-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nonebot_plugin_aujob"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="qwqZYLqwq", email="3422471182@qq.com" },
 ]
 description = "A nonebot plugin"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

