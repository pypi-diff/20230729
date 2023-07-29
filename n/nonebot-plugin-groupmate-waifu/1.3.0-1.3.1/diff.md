# Comparing `tmp/nonebot_plugin_groupmate_waifu-1.3.0.tar.gz` & `tmp/nonebot_plugin_groupmate_waifu-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.3.0.tar", last modified: Fri Jul 21 13:42:21 2023, max compression
+gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.3.1.tar", last modified: Sat Jul 29 06:13:02 2023, max compression
```

## Comparing `nonebot_plugin_groupmate_waifu-1.3.0.tar` & `nonebot_plugin_groupmate_waifu-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 13:42:21.307841 nonebot_plugin_groupmate_waifu-1.3.0/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      279 2023-07-21 13:42:21.306338 nonebot_plugin_groupmate_waifu-1.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 13:42:21.289662 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/
--rw-rw-rw-   0        0        0    21763 2023-07-21 13:35:00.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/__init__.py
--rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/config.py
--rw-rw-rw-   0        0        0     2015 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:42:21.302394 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-21 13:42:21.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-21 13:42:21.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 13:42:21.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-07-21 13:42:21.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-21 13:42:21.000000 nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 13:42:21.307841 nonebot_plugin_groupmate_waifu-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-07-21 13:42:16.000000 nonebot_plugin_groupmate_waifu-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 06:13:02.759354 nonebot_plugin_groupmate_waifu-1.3.1/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      279 2023-07-29 06:13:02.758854 nonebot_plugin_groupmate_waifu-1.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 06:13:02.746871 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/
+-rw-rw-rw-   0        0        0    21882 2023-07-29 06:10:31.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/config.py
+-rw-rw-rw-   0        0        0     2015 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 06:13:02.757353 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-29 06:13:02.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-29 06:13:02.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 06:13:02.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-29 06:13:02.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-29 06:13:02.000000 nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 06:13:02.759855 nonebot_plugin_groupmate_waifu-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-07-29 06:12:58.000000 nonebot_plugin_groupmate_waifu-1.3.1/setup.py
```

### Comparing `nonebot_plugin_groupmate_waifu-1.3.0/LICENSE` & `nonebot_plugin_groupmate_waifu-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/__init__.py` & `nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -286,17 +286,16 @@
         else:
             pass
 
     if not waifu_id:
         group_id = event.group_id
         member_list = await bot.get_group_member_list(group_id = group_id)
         lastmonth = event.time - last_sent_time_filter
-        id_list = {member['user_id'] for member in member_list if member["last_sent_time"] > lastmonth}
-        waifu_ids = id_list - set(rec.keys())
-        waifu_ids -= protect_set
+        rule_out = protect_set | set(rec.keys())
+        waifu_ids = [user_id for member in member_list if (user_id := member['user_id']) not in rule_out and member["last_sent_time"] > lastmonth]
         if waifu_ids:
             waifu_id = random.choice(list(waifu_ids))
         else:
             msg = "群友已经被娶光了、\n" + random.choice(no_waifu)
             await bot.send(event,msg,at_sender = True)
             return False
     state["waifu"] = waifu_id,tips
@@ -405,16 +404,16 @@
 waifu_list = on_command("查看群友卡池", aliases = {"群友卡池"}, priority = 90, block = True)
 
 @waifu_list.handle()
 async def _(bot:Bot, event: GroupMessageEvent):
     group_id = event.group_id
     member_list = await bot.get_group_member_list(group_id = group_id)
     lastmonth = event.time - last_sent_time_filter
-    waifu_ids = protect_list.get(group_id,set()) | set(record_CP.get(group_id).keys())
-    member_list = [member for member in member_list if member['user_id'] not in waifu_ids and member["last_sent_time"] > lastmonth]
+    rule_out = protect_list.get(group_id,set()) | set(record_CP.get(group_id).keys())
+    member_list = [member for member in member_list if member['user_id'] not in rule_out and member["last_sent_time"] > lastmonth]
     member_list.sort(key = lambda x:x["last_sent_time"] ,reverse = True)
     if member_list:
         msg ="卡池：\n——————————————\n"
         for member in member_list[:80]:
             msg += f"{member['card'] or member['nickname']}\n"
         await waifu_list.finish(MessageSegment.image(text_to_png(msg[:-1])))
     else:
@@ -459,63 +458,65 @@
         return False
     group_id = event.group_id
     user_id = event.user_id
     protect_set = protect_list.get(group_id,set())
     if user_id in protect_set:
         return False
     at = get_message_at(event.message)
-    at = at[0] if at else None
-    if at in protect_set:
-        return False
     yinpa_id = None
     tips = "你的涩涩对象是、"
-    protect_set = protect_list.get(group_id,set())
     if at:
+        at = at[0]
+        if at in protect_set:
+            return False
         if at == user_id:
             msg = f"恭喜你涩到了你自己！" + MessageSegment.image(file = await user_img(user_id))
             await bot.send(event,msg,at_sender = True)
             return False
-        elif at == record_CP[group_id].get(user_id,0):
-            if 0 < random.randint(1,100) <= yinpa_CP:
+        X = random.randint(1,100)
+        if at == record_CP.get(group_id,{}).get(user_id,0):
+            if 0 < X <= yinpa_CP:
+                yinpa_id = at
                 tips = "恭喜你涩到了你的老婆！"
             else:
                 await bot.send(event,"你的老婆拒绝和你涩涩！",at_sender = True)
                 return False
-        X = random.randint(1,100)
-        if 0 < X <= yinpa_HE:
+        elif 0 < X <= yinpa_HE:
             yinpa_id = at
-            tips = "恭喜你涩到了群友！" + tips
+            tips = "恭喜你涩到了群友！"
         elif yinpa_HE < X <= yinpa_BE:
             yinpa_id = user_id
     if not yinpa_id:
-
         member_list = await bot.get_group_member_list(group_id = group_id)
         lastmonth = event.time - last_sent_time_filter
-        yinpa_ids = {member['user_id'] for member in member_list if member["last_sent_time"] > lastmonth} - protect_set
-        if not yinpa_ids:
-            return False
+        yinpa_ids = [user_id for member in member_list if (user_id := member['user_id']) not in protect_set and member["last_sent_time"] > lastmonth]
+        if yinpa_ids:
+            yinpa_id = random.choice(yinpa_ids)
         else:
-            yinpa_id = random.choice(list(yinpa_ids))
+            return False
     state["yinpa"] = yinpa_id,tips
     return True
 
 yinpa = on_message(rule = yinpa_rule, priority = 90, block = True)
 
 @yinpa.handle()
 async def _(bot:Bot, event: GroupMessageEvent, state:T_State):
     group_id = event.group_id
     user_id = event.user_id
-    yinpa_id,tips = state["yinpa"]
-    member = await bot.get_group_member_info(group_id = group_id, user_id = yinpa_id)
-    msg = tips + MessageSegment.image(file = await user_img(yinpa_id)) + f"『{(member['card'] or member['nickname'])}』！"
-    record_yinpa1[user_id] = record_yinpa1.get(user_id,0) + 1
-    save(record_yinpa1_file,record_yinpa1)
-    record_yinpa2[user_id] = record_yinpa2.get(yinpa_id,0) + 1
-    save(record_yinpa2_file,record_yinpa2)
-    await yinpa.finish(msg, at_sender=True)
+    yinpa_id, tips = state["yinpa"]
+    if yinpa_id == user_id:
+        await yinpa.finish("不可以涩涩！", at_sender = True)
+    else:
+        record_yinpa1[user_id] = record_yinpa1.get(user_id,0) + 1
+        save(record_yinpa1_file,record_yinpa1)
+        record_yinpa2[user_id] = record_yinpa2.get(yinpa_id,0) + 1
+        save(record_yinpa2_file,record_yinpa2)
+        member = await bot.get_group_member_info(group_id = group_id, user_id = yinpa_id)
+        msg = tips + MessageSegment.image(file = await user_img(yinpa_id)) + f"『{(member['card'] or member['nickname'])}』！"
+        await yinpa.finish(msg, at_sender=True)
 
 # 查看涩涩记录
 
 yinpa_list = on_command("涩涩记录",aliases = {"色色记录"}, priority = 90, block = True)
 
 @yinpa_list.handle()
 async def _(bot:Bot, event: GroupMessageEvent):
```

### Comparing `nonebot_plugin_groupmate_waifu-1.3.0/nonebot_plugin_groupmate_waifu/utils.py` & `nonebot_plugin_groupmate_waifu-1.3.1/nonebot_plugin_groupmate_waifu/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.3.0/setup.py` & `nonebot_plugin_groupmate_waifu-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_groupmate_waifu',
-version='1.3.0',
+version='1.3.1',
 description='娶群友',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_groupmate_waifu"]),
```

