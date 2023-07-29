# Comparing `tmp/MoreApi-0.1.tar.gz` & `tmp/MoreApi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MoreApi-0.1.tar", last modified: Sat Jul 29 05:48:06 2023, max compression
+gzip compressed data, was "MoreApi-0.2.tar", last modified: Sat Jul 29 06:35:35 2023, max compression
```

## Comparing `MoreApi-0.1.tar` & `MoreApi-0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 05:48:06.802706 MoreApi-0.1/
--rw-r--r--   0 liulu      (501) staff       (20)    11357 2023-07-29 03:24:25.000000 MoreApi-0.1/LICENSE
-drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 05:48:06.800286 MoreApi-0.1/MoreAPI/
--rw-r--r--   0 liulu      (501) staff       (20)      916 2023-07-29 03:29:07.000000 MoreApi-0.1/MoreAPI/Auth.py
--rw-r--r--   0 liulu      (501) staff       (20)     2186 2023-07-29 03:29:07.000000 MoreApi-0.1/MoreAPI/DouYin.py
--rw-r--r--   0 liulu      (501) staff       (20)       36 2023-07-29 03:29:07.000000 MoreApi-0.1/MoreAPI/__init__.py
-drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 05:48:06.801931 MoreApi-0.1/MoreApi.egg-info/
--rw-r--r--   0 liulu      (501) staff       (20)     2447 2023-07-29 05:48:06.000000 MoreApi-0.1/MoreApi.egg-info/PKG-INFO
--rw-r--r--   0 liulu      (501) staff       (20)      234 2023-07-29 05:48:06.000000 MoreApi-0.1/MoreApi.egg-info/SOURCES.txt
--rw-r--r--   0 liulu      (501) staff       (20)        1 2023-07-29 05:48:06.000000 MoreApi-0.1/MoreApi.egg-info/dependency_links.txt
--rw-r--r--   0 liulu      (501) staff       (20)        9 2023-07-29 05:48:06.000000 MoreApi-0.1/MoreApi.egg-info/requires.txt
--rw-r--r--   0 liulu      (501) staff       (20)        8 2023-07-29 05:48:06.000000 MoreApi-0.1/MoreApi.egg-info/top_level.txt
--rw-r--r--   0 liulu      (501) staff       (20)     2447 2023-07-29 05:48:06.802414 MoreApi-0.1/PKG-INFO
--rw-r--r--   0 liulu      (501) staff       (20)     2105 2023-07-29 05:21:31.000000 MoreApi-0.1/README.md
--rw-r--r--   0 liulu      (501) staff       (20)       38 2023-07-29 05:48:06.802817 MoreApi-0.1/setup.cfg
--rw-r--r--   0 liulu      (501) staff       (20)      715 2023-07-29 05:48:02.000000 MoreApi-0.1/setup.py
+drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 06:35:35.618847 MoreApi-0.2/
+-rw-r--r--   0 liulu      (501) staff       (20)    11357 2023-07-29 03:24:25.000000 MoreApi-0.2/LICENSE
+drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 06:35:35.615617 MoreApi-0.2/MoreAPI/
+-rw-r--r--   0 liulu      (501) staff       (20)      916 2023-07-29 03:29:07.000000 MoreApi-0.2/MoreAPI/Auth.py
+-rw-r--r--   0 liulu      (501) staff       (20)     2186 2023-07-29 03:29:07.000000 MoreApi-0.2/MoreAPI/DouYin.py
+-rw-r--r--   0 liulu      (501) staff       (20)     1282 2023-07-29 06:03:08.000000 MoreApi-0.2/MoreAPI/KuWo.py
+-rw-r--r--   0 liulu      (501) staff       (20)      898 2023-07-29 05:53:55.000000 MoreApi-0.2/MoreAPI/Video.py
+-rw-r--r--   0 liulu      (501) staff       (20)     4143 2023-07-29 06:30:33.000000 MoreApi-0.2/MoreAPI/XHS.py
+-rw-r--r--   0 liulu      (501) staff       (20)       36 2023-07-29 03:29:07.000000 MoreApi-0.2/MoreAPI/__init__.py
+drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-07-29 06:35:35.618029 MoreApi-0.2/MoreApi.egg-info/
+-rw-r--r--   0 liulu      (501) staff       (20)     2447 2023-07-29 06:35:35.000000 MoreApi-0.2/MoreApi.egg-info/PKG-INFO
+-rw-r--r--   0 liulu      (501) staff       (20)      282 2023-07-29 06:35:35.000000 MoreApi-0.2/MoreApi.egg-info/SOURCES.txt
+-rw-r--r--   0 liulu      (501) staff       (20)        1 2023-07-29 06:35:35.000000 MoreApi-0.2/MoreApi.egg-info/dependency_links.txt
+-rw-r--r--   0 liulu      (501) staff       (20)        9 2023-07-29 06:35:35.000000 MoreApi-0.2/MoreApi.egg-info/requires.txt
+-rw-r--r--   0 liulu      (501) staff       (20)        8 2023-07-29 06:35:35.000000 MoreApi-0.2/MoreApi.egg-info/top_level.txt
+-rw-r--r--   0 liulu      (501) staff       (20)     2447 2023-07-29 06:35:35.618575 MoreApi-0.2/PKG-INFO
+-rw-r--r--   0 liulu      (501) staff       (20)     2105 2023-07-29 05:21:31.000000 MoreApi-0.2/README.md
+-rw-r--r--   0 liulu      (501) staff       (20)       38 2023-07-29 06:35:35.618939 MoreApi-0.2/setup.cfg
+-rw-r--r--   0 liulu      (501) staff       (20)      715 2023-07-29 06:31:25.000000 MoreApi-0.2/setup.py
```

### Comparing `MoreApi-0.1/LICENSE` & `MoreApi-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MoreApi-0.1/MoreAPI/Auth.py` & `MoreApi-0.2/MoreAPI/Auth.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.1/MoreAPI/DouYin.py` & `MoreApi-0.2/MoreAPI/DouYin.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.1/MoreApi.egg-info/PKG-INFO` & `MoreApi-0.2/MoreApi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MoreApi
-Version: 0.1
+Version: 0.2
 Summary: MoreAPI是抖音/酷我/小红书/快手等各视频平台非官方的RESTful API平台。
 Home-page: https://github.com/liulu1550/MoreAPI.git
 Author: MoreCoding
 Author-email: wouldmissyou@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MoreApi-0.1/PKG-INFO` & `MoreApi-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MoreApi
-Version: 0.1
+Version: 0.2
 Summary: MoreAPI是抖音/酷我/小红书/快手等各视频平台非官方的RESTful API平台。
 Home-page: https://github.com/liulu1550/MoreAPI.git
 Author: MoreCoding
 Author-email: wouldmissyou@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MoreApi-0.1/README.md` & `MoreApi-0.2/README.md`

 * *Files identical despite different names*

### Comparing `MoreApi-0.1/setup.py` & `MoreApi-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import (setup, find_packages)
 
 setup(
 
     name="MoreApi",  # 包名
     author='MoreCoding',  #作者
-    version="0.1",  # 版本
+    version="0.2",  # 版本
     url='https://github.com/liulu1550/MoreAPI.git',  # github地址
     description='MoreAPI是抖音/酷我/小红书/快手等各视频平台非官方的RESTful API平台。',  #包的简述
     long_description=open('README.md', encoding='utf-8').read(),  # #包的详细介绍
     long_description_content_type="text/markdown",
     # 需要包含的子包列表
     packages=find_packages(),
     author_email='wouldmissyou@163.com',
```

