# Comparing `tmp/mcqq-tool-0.0.9.tar.gz` & `tmp/mcqq-tool-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq-tool-0.0.9.tar", last modified: Wed Jul 19 13:29:36 2023, max compression
+gzip compressed data, was "mcqq-tool-0.1.0.tar", last modified: Sat Jul 29 06:52:38 2023, max compression
```

## Comparing `mcqq-tool-0.0.9.tar` & `mcqq-tool-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:29:36.315772 mcqq-tool-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-19 13:29:36.315772 mcqq-tool-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:29:36.311771 mcqq-tool-0.0.9/mcqq_tool/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:29:36.311771 mcqq-tool-0.0.9/mcqq_tool/model/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/model/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/model/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/model/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/model/spigot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:29:36.311771 mcqq-tool-0.0.9/mcqq_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-19 13:29:36.000000 mcqq-tool-0.0.9/mcqq_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-19 13:29:36.000000 mcqq-tool-0.0.9/mcqq_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:29:36.000000 mcqq-tool-0.0.9/mcqq_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-19 13:29:36.000000 mcqq-tool-0.0.9/mcqq_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 13:29:36.000000 mcqq-tool-0.0.9/mcqq_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 13:29:36.315772 mcqq-tool-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:38.043194 mcqq-tool-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-29 06:52:38.043194 mcqq-tool-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:38.039194 mcqq-tool-0.1.0/mcqq_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:38.043194 mcqq-tool-0.1.0/mcqq_tool/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/model/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/model/forge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/model/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/model/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/model/spigot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/mcqq_tool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:38.039194 mcqq-tool-0.1.0/mcqq_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-29 06:52:37.000000 mcqq-tool-0.1.0/mcqq_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-29 06:52:37.000000 mcqq-tool-0.1.0/mcqq_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 06:52:37.000000 mcqq-tool-0.1.0/mcqq_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-29 06:52:37.000000 mcqq-tool-0.1.0/mcqq_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 06:52:37.000000 mcqq-tool-0.1.0/mcqq_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 06:52:38.043194 mcqq-tool-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-29 06:52:27.000000 mcqq-tool-0.1.0/setup.py
```

### Comparing `mcqq-tool-0.0.9/LICENSE` & `mcqq-tool-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.9/PKG-INFO` & `mcqq-tool-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 0.0.9
+Version: 0.1.0
 Summary: MC_QQ 工具包
 Home-page: https://github.com/17TheWord/mcqq-tool
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mcqq-tool-0.0.9/mcqq_tool/common.py` & `mcqq-tool-0.1.0/mcqq_tool/common.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.9/mcqq_tool/config.py` & `mcqq-tool-0.1.0/mcqq_tool/config.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.9/mcqq_tool/model/__init__.py` & `mcqq-tool-0.1.0/mcqq_tool/model/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from .basemodel import BaseEvent, BaseChatEvent, BaseDeathEvent, BaseJoinEvent, BaseQuitEvent
+from .forge import ForgePlayerLoggedInEvent, ForgePlayerLoggedOutEvent, ForgeServerChatEvent, ForgePlayerRespawnEvent
 from .minecraft import MinecraftPlayerChatEvent, MinecraftPlayerJoinEvent, MinecraftPlayerQuitEvent
 from .spigot import AsyncPlayerChatEvent, PlayerDeathEvent, PlayerJoinEvent, PlayerQuitEvent
 
 event_dict = {
     # 原版
     "MinecraftPlayerJoinEvent": MinecraftPlayerJoinEvent,
     "MinecraftPlayerQuitEvent": MinecraftPlayerQuitEvent,
     "MinecraftPlayerChatEvent": MinecraftPlayerChatEvent,
     # Spigot
     "AsyncPlayerChatEvent": AsyncPlayerChatEvent,
     "PlayerDeathEvent": PlayerDeathEvent,
     "PlayerJoinEvent": PlayerJoinEvent,
     "PlayerQuitEvent": PlayerQuitEvent,
+    # Forge
+    "ForgeServerChatEvent": ForgeServerChatEvent,
+    "ForgePlayerLoggedInEvent": ForgePlayerLoggedInEvent,
+    "ForgePlayerLoggedOutEvent": ForgePlayerLoggedOutEvent,
+    "ForgePlayerRespawnEvent": ForgePlayerRespawnEvent,
 }
```

### Comparing `mcqq-tool-0.0.9/mcqq_tool/model/basemodel.py` & `mcqq-tool-0.1.0/mcqq_tool/model/basemodel.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.9/mcqq_tool/model/minecraft.py` & `mcqq-tool-0.1.0/mcqq_tool/model/minecraft.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.9/mcqq_tool/model/spigot.py` & `mcqq-tool-0.1.0/mcqq_tool/model/spigot.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.9/mcqq_tool/utils.py` & `mcqq-tool-0.1.0/mcqq_tool/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,16 @@
                         back_msg = await client.rcon.send_cmd(cmd)
                         await bot.send(event=event, message=f"服务器返回：{back_msg[0]}")
                         logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client.server_name}] 的消息 \"{cmd}\"")
                     except ClientNotConnectedError as e:
                         logger.error(f"[MC_QQ_Rcon]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：{e}")
                         await remove_client(client.server_name)
                 elif client.websocket:
-                    await bot.send(event=event, message="该服务器不支持Rcon，无法执行该命令")
+                    cmd_list = {"message": [{"msgType": "command", "msgData": cmd}]}
+                    await client.websocket.send_text(str(cmd_list))
                 else:
                     logger.error(f"[MC_QQ]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：该客户端没有连接")
                     await remove_client(client.server_name)
 
 
 async def _get_clients(event: Union[GroupMessageEvent, GuildMessageEvent]) -> List[Client]:
     """
```

### Comparing `mcqq-tool-0.0.9/mcqq_tool.egg-info/PKG-INFO` & `mcqq-tool-0.1.0/mcqq_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 0.0.9
+Version: 0.1.0
 Summary: MC_QQ 工具包
 Home-page: https://github.com/17TheWord/mcqq-tool
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mcqq-tool-0.0.9/setup.py` & `mcqq-tool-0.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="mcqq-tool",
-    version="0.0.9",
+    version="0.1.0",
     author="17TheWord",
     author_email="17theword@gmail.com",
     description="MC_QQ 工具包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/17TheWord/mcqq-tool",
     packages=setuptools.find_packages(),
```

