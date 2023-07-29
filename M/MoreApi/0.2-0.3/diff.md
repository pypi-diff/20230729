# Comparing `tmp/MoreApi-0.2.tar.gz` & `tmp/MoreApi-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MoreApi-0.2.tar", last modified: Sat Jul 29 06:35:35 2023, max compression
+gzip compressed data, was "MoreApi-0.3.tar", last modified: Sat Jul 29 06:47:10 2023, max compression
```

## Comparing `MoreApi-0.2.tar` & `MoreApi-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 06:35:35.618847 MoreApi-0.2/
--rw-r--r--   0 liulu      (501) staff       (20)    11357 2023-07-29 03:24:25.000000 MoreApi-0.2/LICENSE
-drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 06:35:35.615617 MoreApi-0.2/MoreAPI/
--rw-r--r--   0 liulu      (501) staff       (20)      916 2023-07-29 03:29:07.000000 MoreApi-0.2/MoreAPI/Auth.py
--rw-r--r--   0 liulu      (501) staff       (20)     2186 2023-07-29 03:29:07.000000 MoreApi-0.2/MoreAPI/DouYin.py
--rw-r--r--   0 liulu      (501) staff       (20)     1282 2023-07-29 06:03:08.000000 MoreApi-0.2/MoreAPI/KuWo.py
--rw-r--r--   0 liulu      (501) staff       (20)      898 2023-07-29 05:53:55.000000 MoreApi-0.2/MoreAPI/Video.py
--rw-r--r--   0 liulu      (501) staff       (20)     4143 2023-07-29 06:30:33.000000 MoreApi-0.2/MoreAPI/XHS.py
--rw-r--r--   0 liulu      (501) staff       (20)       36 2023-07-29 03:29:07.000000 MoreApi-0.2/MoreAPI/__init__.py
-drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 06:35:35.618029 MoreApi-0.2/MoreApi.egg-info/
--rw-r--r--   0 liulu      (501) staff       (20)     2447 2023-07-29 06:35:35.000000 MoreApi-0.2/MoreApi.egg-info/PKG-INFO
--rw-r--r--   0 liulu      (501) staff       (20)      282 2023-07-29 06:35:35.000000 MoreApi-0.2/MoreApi.egg-info/SOURCES.txt
--rw-r--r--   0 liulu      (501) staff       (20)        1 2023-07-29 06:35:35.000000 MoreApi-0.2/MoreApi.egg-info/dependency_links.txt
--rw-r--r--   0 liulu      (501) staff       (20)        9 2023-07-29 06:35:35.000000 MoreApi-0.2/MoreApi.egg-info/requires.txt
--rw-r--r--   0 liulu      (501) staff       (20)        8 2023-07-29 06:35:35.000000 MoreApi-0.2/MoreApi.egg-info/top_level.txt
--rw-r--r--   0 liulu      (501) staff       (20)     2447 2023-07-29 06:35:35.618575 MoreApi-0.2/PKG-INFO
--rw-r--r--   0 liulu      (501) staff       (20)     2105 2023-07-29 05:21:31.000000 MoreApi-0.2/README.md
--rw-r--r--   0 liulu      (501) staff       (20)       38 2023-07-29 06:35:35.618939 MoreApi-0.2/setup.cfg
--rw-r--r--   0 liulu      (501) staff       (20)      715 2023-07-29 06:31:25.000000 MoreApi-0.2/setup.py
+drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 06:47:10.132882 MoreApi-0.3/
+-rw-r--r--   0 liulu      (501) staff       (20)    11357 2023-07-29 03:24:25.000000 MoreApi-0.3/LICENSE
+drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 06:47:10.130728 MoreApi-0.3/MoreAPI/
+-rw-r--r--   0 liulu      (501) staff       (20)      916 2023-07-29 03:29:07.000000 MoreApi-0.3/MoreAPI/Auth.py
+-rw-r--r--   0 liulu      (501) staff       (20)     2186 2023-07-29 03:29:07.000000 MoreApi-0.3/MoreAPI/DouYin.py
+-rw-r--r--   0 liulu      (501) staff       (20)     1280 2023-07-29 06:46:28.000000 MoreApi-0.3/MoreAPI/KuWo.py
+-rw-r--r--   0 liulu      (501) staff       (20)      898 2023-07-29 05:53:55.000000 MoreApi-0.3/MoreAPI/Video.py
+-rw-r--r--   0 liulu      (501) staff       (20)     4143 2023-07-29 06:30:33.000000 MoreApi-0.3/MoreAPI/XHS.py
+-rw-r--r--   0 liulu      (501) staff       (20)      126 2023-07-29 06:46:10.000000 MoreApi-0.3/MoreAPI/__init__.py
+drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 06:47:10.132241 MoreApi-0.3/MoreApi.egg-info/
+-rw-r--r--   0 liulu      (501) staff       (20)     2488 2023-07-29 06:47:10.000000 MoreApi-0.3/MoreApi.egg-info/PKG-INFO
+-rw-r--r--   0 liulu      (501) staff       (20)      282 2023-07-29 06:47:10.000000 MoreApi-0.3/MoreApi.egg-info/SOURCES.txt
+-rw-r--r--   0 liulu      (501) staff       (20)        1 2023-07-29 06:47:10.000000 MoreApi-0.3/MoreApi.egg-info/dependency_links.txt
+-rw-r--r--   0 liulu      (501) staff       (20)        9 2023-07-29 06:47:10.000000 MoreApi-0.3/MoreApi.egg-info/requires.txt
+-rw-r--r--   0 liulu      (501) staff       (20)        8 2023-07-29 06:47:10.000000 MoreApi-0.3/MoreApi.egg-info/top_level.txt
+-rw-r--r--   0 liulu      (501) staff       (20)     2488 2023-07-29 06:47:10.132609 MoreApi-0.3/PKG-INFO
+-rw-r--r--   0 liulu      (501) staff       (20)     2146 2023-07-29 06:47:05.000000 MoreApi-0.3/README.md
+-rw-r--r--   0 liulu      (501) staff       (20)       38 2023-07-29 06:47:10.132963 MoreApi-0.3/setup.cfg
+-rw-r--r--   0 liulu      (501) staff       (20)      715 2023-07-29 06:47:05.000000 MoreApi-0.3/setup.py
```

### Comparing `MoreApi-0.2/LICENSE` & `MoreApi-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MoreApi-0.2/MoreAPI/Auth.py` & `MoreApi-0.3/MoreAPI/Auth.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.2/MoreAPI/DouYin.py` & `MoreApi-0.3/MoreAPI/DouYin.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.2/MoreAPI/KuWo.py` & `MoreApi-0.3/MoreAPI/KuWo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from MoreAPI.Auth import Auth
 
 
-class Video(Auth):
+class KuWo(Auth):
     def __init__(self, token: str):
         """
         初始化
         :param token: 登录用户的token
         """
         super().__init__(token)
         self.music_search_url = self.domain + "/api/kuwo/search/"
@@ -34,11 +34,11 @@
                               params={"rid": rid})
         return result.json()
 
 
 if __name__ == '__main__':
     token = "62cauRzwo9nL2vK8DgtY9bCJ4nnsvYYvDROeodJIONJntkrrwVODh16z2myRnW2c"
 
-    moreapi = Video(token)
+    moreapi = KuWo(token)
 
     t = moreapi.get_music_data("440623")
     print(t)
```

### Comparing `MoreApi-0.2/MoreAPI/Video.py` & `MoreApi-0.3/MoreAPI/Video.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.2/MoreAPI/XHS.py` & `MoreApi-0.3/MoreAPI/XHS.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.2/MoreApi.egg-info/PKG-INFO` & `MoreApi-0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: MoreApi
-Version: 0.2
-Summary: MoreAPI是抖音/酷我/小红书/快手等各视频平台非官方的RESTful API平台。
-Home-page: https://github.com/liulu1550/MoreAPI.git
-Author: MoreCoding
-Author-email: wouldmissyou@163.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Description/简介
 
 `MoreAPI`是抖音/酷我/小红书/各视频平台非官方的RESTful API平台。
 
 `MoreAPI`提供的API只能获取公开数据，即任何人都可以通过浏览器及APP等访问相关服务以获取它们。
 
 如果您有任何建议或者需求，请联系站长，更多的功能正在开发中，敬请期待！
@@ -48,18 +37,23 @@
 
 #### 注册账号
 
 注册地址  [http://doc.moreapi.wouldmissyou.com/api-97366881](http://doc.moreapi.wouldmissyou.com/api-97366881)
 
 #### 调用示例
 
+安装
+```shell
+pip install MoreApi
+```
+
 ```python
-import moreapi
+import MoreApi
 
 if __name__ == '__main__':
     token = "您账号的token"  # 注册账号后登录获取token
-    douyin_api = moreapi.DouYin(token)  # 抖音接口
+    douyin_api = MoreApi.DouYin(token)  # 抖音接口
     video_data = douyin_api.get_video_data("7258926046223797544")  # 调用获取抖音单一视频信息API
     print(video_data)
 ```
 
-文档地址：[http://doc.moreapi.wouldmissyou.com/](http://doc.moreapi.wouldmissyou.com/)
+文档地址：[http://doc.moreapi.wouldmissyou.com/](http://doc.moreapi.wouldmissyou.com/)
```

### Comparing `MoreApi-0.2/PKG-INFO` & `MoreApi-0.3/MoreApi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MoreApi
-Version: 0.2
+Version: 0.3
 Summary: MoreAPI是抖音/酷我/小红书/快手等各视频平台非官方的RESTful API平台。
 Home-page: https://github.com/liulu1550/MoreAPI.git
 Author: MoreCoding
 Author-email: wouldmissyou@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -48,18 +48,23 @@
 
 #### 注册账号
 
 注册地址  [http://doc.moreapi.wouldmissyou.com/api-97366881](http://doc.moreapi.wouldmissyou.com/api-97366881)
 
 #### 调用示例
 
+安装
+```shell
+pip install MoreApi
+```
+
 ```python
-import moreapi
+import MoreApi
 
 if __name__ == '__main__':
     token = "您账号的token"  # 注册账号后登录获取token
-    douyin_api = moreapi.DouYin(token)  # 抖音接口
+    douyin_api = MoreApi.DouYin(token)  # 抖音接口
     video_data = douyin_api.get_video_data("7258926046223797544")  # 调用获取抖音单一视频信息API
     print(video_data)
 ```
 
 文档地址：[http://doc.moreapi.wouldmissyou.com/](http://doc.moreapi.wouldmissyou.com/)
```

### Comparing `MoreApi-0.2/README.md` & `MoreApi-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: MoreApi
+Version: 0.3
+Summary: MoreAPI是抖音/酷我/小红书/快手等各视频平台非官方的RESTful API平台。
+Home-page: https://github.com/liulu1550/MoreAPI.git
+Author: MoreCoding
+Author-email: wouldmissyou@163.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Description/简介
 
 `MoreAPI`是抖音/酷我/小红书/各视频平台非官方的RESTful API平台。
 
 `MoreAPI`提供的API只能获取公开数据，即任何人都可以通过浏览器及APP等访问相关服务以获取它们。
 
 如果您有任何建议或者需求，请联系站长，更多的功能正在开发中，敬请期待！
@@ -37,18 +48,23 @@
 
 #### 注册账号
 
 注册地址  [http://doc.moreapi.wouldmissyou.com/api-97366881](http://doc.moreapi.wouldmissyou.com/api-97366881)
 
 #### 调用示例
 
+安装
+```shell
+pip install MoreApi
+```
+
 ```python
-import moreapi
+import MoreApi
 
 if __name__ == '__main__':
     token = "您账号的token"  # 注册账号后登录获取token
-    douyin_api = moreapi.DouYin(token)  # 抖音接口
+    douyin_api = MoreApi.DouYin(token)  # 抖音接口
     video_data = douyin_api.get_video_data("7258926046223797544")  # 调用获取抖音单一视频信息API
     print(video_data)
 ```
 
-文档地址：[http://doc.moreapi.wouldmissyou.com/](http://doc.moreapi.wouldmissyou.com/)
+文档地址：[http://doc.moreapi.wouldmissyou.com/](http://doc.moreapi.wouldmissyou.com/)
```

### Comparing `MoreApi-0.2/setup.py` & `MoreApi-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import (setup, find_packages)
 
 setup(
 
     name="MoreApi",  # 包名
     author='MoreCoding',  #作者
-    version="0.2",  # 版本
+    version="0.3",  # 版本
     url='https://github.com/liulu1550/MoreAPI.git',  # github地址
     description='MoreAPI是抖音/酷我/小红书/快手等各视频平台非官方的RESTful API平台。',  #包的简述
     long_description=open('README.md', encoding='utf-8').read(),  # #包的详细介绍
     long_description_content_type="text/markdown",
     # 需要包含的子包列表
     packages=find_packages(),
     author_email='wouldmissyou@163.com',
```

