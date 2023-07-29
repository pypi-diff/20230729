# Comparing `tmp/nonebot_plugin_aujob-0.1.0.tar.gz` & `tmp/nonebot_plugin_aujob-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aujob-0.1.0.tar", last modified: Sat Jul 29 02:42:50 2023, max compression
+gzip compressed data, was "nonebot_plugin_aujob-0.1.1.tar", last modified: Sat Jul 29 09:04:49 2023, max compression
```

## Comparing `nonebot_plugin_aujob-0.1.0.tar` & `nonebot_plugin_aujob-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 02:42:50.197320 nonebot_plugin_aujob-0.1.0/
--rw-rw-rw-   0        0        0      511 2023-07-29 02:42:50.197320 nonebot_plugin_aujob-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 02:42:50.182321 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob/
--rw-rw-rw-   0        0        0     1741 2023-07-29 02:41:43.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob/__init__.py
--rw-rw-rw-   0        0        0    11199 2023-07-29 02:41:44.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 02:42:50.194320 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/
--rw-rw-rw-   0        0        0      511 2023-07-29 02:42:50.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-29 02:42:50.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 02:42:50.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-29 02:42:50.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-29 02:42:50.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      698 2023-07-29 02:42:21.000000 nonebot_plugin_aujob-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 02:42:50.198319 nonebot_plugin_aujob-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 09:04:49.669662 nonebot_plugin_aujob-0.1.1/
+-rw-rw-rw-   0        0        0      511 2023-07-29 09:04:49.666661 nonebot_plugin_aujob-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 09:04:49.648658 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob/
+-rw-rw-rw-   0        0        0     1734 2023-07-29 09:04:02.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob/__init__.py
+-rw-rw-rw-   0        0        0    11199 2023-07-29 02:41:44.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:04:49.663661 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-07-29 09:04:49.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-29 09:04:49.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 09:04:49.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-29 09:04:49.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-29 09:04:49.000000 nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2023-07-29 09:04:33.000000 nonebot_plugin_aujob-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 09:04:49.669662 nonebot_plugin_aujob-0.1.1/setup.cfg
```

### Comparing `nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob/__init__.py` & `nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 __plugin_meta__ = PluginMetadata(
     name="Among US中的TOH模组职业介绍",
     description="查询TOH模组里职业的玩法描述",
     usage="发送/auhelp 查看插件帮助信息",
     type="application",
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
     homepage="https://github.com/qwqZYLqwq/nonebot-plugin-aujob",
-    # 发布必填。
-    supported_adapters={"~onebot.v11"},
+    # 发布必填
+
+
+    #supported_adapters={"null"},
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 
 
 matcher_character = on_startswith(".t ", ignorecase=True, priority=10, block=True)
```

### Comparing `nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob/utils.py` & `nonebot_plugin_aujob-0.1.1/nonebot_plugin_aujob/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_aujob-0.1.0/pyproject.toml` & `nonebot_plugin_aujob-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nonebot_plugin_aujob"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="qwqZYLqwq", email="3422471182@qq.com" },
 ]
 description = "A nonebot plugin"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

