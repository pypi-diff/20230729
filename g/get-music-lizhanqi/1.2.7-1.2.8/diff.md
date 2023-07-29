# Comparing `tmp/get-music-lizhanqi-1.2.7.tar.gz` & `tmp/get-music-lizhanqi-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\???\Desktop\get_music\dist\.tmp-fe1sh4uw\get-music-lizhanqi-1.2.7.tar", last modified: Fri Jul 28 13:00:04 2023, max compression
+gzip compressed data, was "C:\Users\???\Desktop\get_music\dist\.tmp-ibl8a653\get-music-lizhanqi-1.2.8.tar", last modified: Sat Jul 29 10:45:32 2023, max compression
```

## Comparing `get-music-lizhanqi-1.2.7.tar` & `get-music-lizhanqi-1.2.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/
--rw-rw-rw-   0        0        0     1091 2022-04-09 10:07:52.000000 get-music-lizhanqi-1.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0     1759 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1345 2023-07-28 12:58:52.000000 get-music-lizhanqi-1.2.7/README.md
--rw-rw-rw-   0        0        0       86 2022-04-09 10:04:03.000000 get-music-lizhanqi-1.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      952 2023-07-28 12:56:58.000000 get-music-lizhanqi-1.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/tests/
-drwxrwxrwx   0        0        0        0 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/
--rw-rw-rw-   0        0        0      266 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/__init__.py
--rw-rw-rw-   0        0        0     3092 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/baidu.py
--rw-rw-rw-   0        0        0     1938 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/download.py
--rw-rw-rw-   0        0        0     2892 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/downloads.py
--rw-rw-rw-   0        0        0     3363 2023-07-28 12:50:20.000000 get-music-lizhanqi-1.2.7/tests/get_music/fivesing.py
--rw-rw-rw-   0        0        0    10519 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/get_music.py
--rw-rw-rw-   0        0        0    11919 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/gui.py
--rw-rw-rw-   0        0        0     2613 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/kg_one_playerlist.py
--rw-rw-rw-   0        0        0     2570 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/kg_playerlist.py
--rw-rw-rw-   0        0        0     5305 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/kugou.py
--rw-rw-rw-   0        0        0     3985 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/kuwo.py
--rw-rw-rw-   0        0        0     2685 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/kw_playerlist.py
--rw-rw-rw-   0        0        0     2861 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/migu.py
--rw-rw-rw-   0        0        0     3763 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/netease.py
--rw-rw-rw-   0        0        0     2090 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/oneting.py
--rw-rw-rw-   0        0        0     3306 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/playerlist.py
--rw-rw-rw-   0        0        0     4293 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/qq.py
--rw-rw-rw-   0        0        0     2534 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/qq_playerlist.py
--rw-rw-rw-   0        0        0     2569 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/singbz.py
--rw-rw-rw-   0        0        0     6826 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/top.py
--rw-rw-rw-   0        0        0     2214 2023-07-28 12:56:22.000000 get-music-lizhanqi-1.2.7/tests/get_music/ver.py
--rw-rw-rw-   0        0        0     3119 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/wy_playerlist.py
--rw-rw-rw-   0        0        0     3692 2023-07-24 00:44:04.000000 get-music-lizhanqi-1.2.7/tests/get_music/zhidao.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/tests/get_music_lizhanqi.egg-info/
--rw-rw-rw-   0        0        0     1759 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/tests/get_music_lizhanqi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/tests/get_music_lizhanqi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/tests/get_music_lizhanqi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/tests/get_music_lizhanqi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/tests/get_music_lizhanqi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-28 13:00:04.000000 get-music-lizhanqi-1.2.7/tests/get_music_lizhanqi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/
+-rw-rw-rw-   0        0        0     1091 2022-04-09 10:07:52.000000 get-music-lizhanqi-1.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     1660 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1246 2023-07-29 10:44:28.000000 get-music-lizhanqi-1.2.8/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-09 10:04:03.000000 get-music-lizhanqi-1.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      952 2023-07-29 10:44:53.000000 get-music-lizhanqi-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/
+drwxrwxrwx   0        0        0        0 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music/
+-rw-rw-rw-   0        0        0      266 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/__init__.py
+-rw-rw-rw-   0        0        0     3092 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/baidu.py
+-rw-rw-rw-   0        0        0     1938 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/download.py
+-rw-rw-rw-   0        0        0     2892 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/downloads.py
+-rw-rw-rw-   0        0        0     3363 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/fivesing.py
+-rw-rw-rw-   0        0        0    10519 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/get_music.py
+-rw-rw-rw-   0        0        0    11919 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/gui.py
+-rw-rw-rw-   0        0        0     2613 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/kg_one_playerlist.py
+-rw-rw-rw-   0        0        0     2570 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/kg_playerlist.py
+-rw-rw-rw-   0        0        0     5305 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/kugou.py
+-rw-rw-rw-   0        0        0     5575 2023-07-29 10:42:14.000000 get-music-lizhanqi-1.2.8/tests/get_music/kuwo.py
+-rw-rw-rw-   0        0        0     2685 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/kw_playerlist.py
+-rw-rw-rw-   0        0        0     2861 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/migu.py
+-rw-rw-rw-   0        0        0     3763 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/netease.py
+-rw-rw-rw-   0        0        0     2090 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/oneting.py
+-rw-rw-rw-   0        0        0     3306 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/playerlist.py
+-rw-rw-rw-   0        0        0     4293 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/qq.py
+-rw-rw-rw-   0        0        0     2534 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/qq_playerlist.py
+-rw-rw-rw-   0        0        0     2569 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/singbz.py
+-rw-rw-rw-   0        0        0     6826 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/top.py
+-rw-rw-rw-   0        0        0     2214 2023-07-29 10:43:41.000000 get-music-lizhanqi-1.2.8/tests/get_music/ver.py
+-rw-rw-rw-   0        0        0     3119 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/wy_playerlist.py
+-rw-rw-rw-   0        0        0     3692 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/zhidao.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/
+-rw-rw-rw-   0        0        0     1660 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/top_level.txt
```

### Comparing `get-music-lizhanqi-1.2.7/LICENSE.txt` & `get-music-lizhanqi-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/PKG-INFO` & `get-music-lizhanqi-1.2.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-music-lizhanqi
-Version: 1.2.7
+Version: 1.2.8
 Summary: 可以下载音乐的包哦
 Home-page: 
 Author: Li Zhan Qi
 Author-email: 3101978435@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 - 这是一个可以下载和搜索音乐的python命令行工具，支持，酷狗，酷我，百度，网易云，咪咕，qq音乐，5sing，欢迎前来学习的指点
 
 ## 使用方法
 - 长话短说**get-music -help**或**get-music-lizhanqi -help**打开帮助，帮助里面有全部命令的介绍，或者前往github地址:<https://github.com/lzq-hopego/get-music-lizhanqi>
 
 
 ## 更新记录
-- 2023-07-28 完成v1.2.7版本,修复5sing翻唱原唱使用中文名字搜索无返回值的问题(编码问题)，修复有时无法直接返回值的问题(超时问题)
+- 2023-07-29 完成v1.2.8版本,修复酷我音乐接口失效的错误。
 
 
 
 
 ## THE END
 - 本脚本仅支持学习使用，如有发现有任何商业用途，一经发现您将受到法律责任。
 - 本程序使用的接口全部来源于网络，切不可有任何商业用途，或我程序中有涉及你公司利益的，你可以联系我，我会及时删除源代码，并不再更新。
```

### Comparing `get-music-lizhanqi-1.2.7/README.md` & `get-music-lizhanqi-1.2.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 - 这是一个可以下载和搜索音乐的python命令行工具，支持，酷狗，酷我，百度，网易云，咪咕，qq音乐，5sing，欢迎前来学习的指点
 
 ## 使用方法
 - 长话短说**get-music -help**或**get-music-lizhanqi -help**打开帮助，帮助里面有全部命令的介绍，或者前往github地址:<https://github.com/lzq-hopego/get-music-lizhanqi>
 
 
 ## 更新记录
-- 2023-07-28 完成v1.2.7版本,修复5sing翻唱原唱使用中文名字搜索无返回值的问题(编码问题)，修复有时无法直接返回值的问题(超时问题)
+- 2023-07-29 完成v1.2.8版本,修复酷我音乐接口失效的错误。
 
 
 
 
 ## THE END
 - 本脚本仅支持学习使用，如有发现有任何商业用途，一经发现您将受到法律责任。
 - 本程序使用的接口全部来源于网络，切不可有任何商业用途，或我程序中有涉及你公司利益的，你可以联系我，我会及时删除源代码，并不再更新。
```

### Comparing `get-music-lizhanqi-1.2.7/setup.py` & `get-music-lizhanqi-1.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="get-music-lizhanqi",
-    version="1.2.7",
+    version="1.2.8",
     author="Li Zhan Qi",
     author_email="3101978435@qq.com",
     description="可以下载音乐的包哦",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
```

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/baidu.py` & `get-music-lizhanqi-1.2.8/tests/get_music/baidu.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/download.py` & `get-music-lizhanqi-1.2.8/tests/get_music/download.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/downloads.py` & `get-music-lizhanqi-1.2.8/tests/get_music/downloads.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/fivesing.py` & `get-music-lizhanqi-1.2.8/tests/get_music/fivesing.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/get_music.py` & `get-music-lizhanqi-1.2.8/tests/get_music/get_music.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/gui.py` & `get-music-lizhanqi-1.2.8/tests/get_music/gui.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/kg_one_playerlist.py` & `get-music-lizhanqi-1.2.8/tests/get_music/kg_one_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/kg_playerlist.py` & `get-music-lizhanqi-1.2.8/tests/get_music/kg_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/kugou.py` & `get-music-lizhanqi-1.2.8/tests/get_music/kugou.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/kw_playerlist.py` & `get-music-lizhanqi-1.2.8/tests/get_music/kw_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/migu.py` & `get-music-lizhanqi-1.2.8/tests/get_music/migu.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/netease.py` & `get-music-lizhanqi-1.2.8/tests/get_music/netease.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/oneting.py` & `get-music-lizhanqi-1.2.8/tests/get_music/oneting.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/playerlist.py` & `get-music-lizhanqi-1.2.8/tests/get_music/playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/qq.py` & `get-music-lizhanqi-1.2.8/tests/get_music/qq.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/qq_playerlist.py` & `get-music-lizhanqi-1.2.8/tests/get_music/qq_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/singbz.py` & `get-music-lizhanqi-1.2.8/tests/get_music/singbz.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/top.py` & `get-music-lizhanqi-1.2.8/tests/get_music/top.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/ver.py` & `get-music-lizhanqi-1.2.8/tests/get_music/ver.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                 url = 'http://api.ip33.com/ip/search?s='                     
                 d = requests.get(url,timeout=1).json()                                                       
                 console.print('\n[b green]信息二:本机外网ip地址为:[b red]{}[/]，归属:[b red]{}[/]'.format(d['ip'],d['area']))
             except:
                 console.print("\n[b red]ip地址信息查二询失败！")
             return
     
-    version = '1.2.7'
+    version = '1.2.8'
     console.print("[green]当前版本:"+"v"+version)
     url = 'https://pypi.org/project/get-music-lizhanqi/#history'
     try:
         with console.status("[b green]检查最新版中..."):
             html = requests.get(url,timeout = 5)
             txt = html.text
             crad = re.findall(r' <a class="card release__card" href="/project/get-music-lizhanqi/(.*?)/">',txt,re.S)
```

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/wy_playerlist.py` & `get-music-lizhanqi-1.2.8/tests/get_music/wy_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music/zhidao.py` & `get-music-lizhanqi-1.2.8/tests/get_music/zhidao.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music_lizhanqi.egg-info/PKG-INFO` & `get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-music-lizhanqi
-Version: 1.2.7
+Version: 1.2.8
 Summary: 可以下载音乐的包哦
 Home-page: 
 Author: Li Zhan Qi
 Author-email: 3101978435@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 - 这是一个可以下载和搜索音乐的python命令行工具，支持，酷狗，酷我，百度，网易云，咪咕，qq音乐，5sing，欢迎前来学习的指点
 
 ## 使用方法
 - 长话短说**get-music -help**或**get-music-lizhanqi -help**打开帮助，帮助里面有全部命令的介绍，或者前往github地址:<https://github.com/lzq-hopego/get-music-lizhanqi>
 
 
 ## 更新记录
-- 2023-07-28 完成v1.2.7版本,修复5sing翻唱原唱使用中文名字搜索无返回值的问题(编码问题)，修复有时无法直接返回值的问题(超时问题)
+- 2023-07-29 完成v1.2.8版本,修复酷我音乐接口失效的错误。
 
 
 
 
 ## THE END
 - 本脚本仅支持学习使用，如有发现有任何商业用途，一经发现您将受到法律责任。
 - 本程序使用的接口全部来源于网络，切不可有任何商业用途，或我程序中有涉及你公司利益的，你可以联系我，我会及时删除源代码，并不再更新。
```

### Comparing `get-music-lizhanqi-1.2.7/tests/get_music_lizhanqi.egg-info/SOURCES.txt` & `get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

