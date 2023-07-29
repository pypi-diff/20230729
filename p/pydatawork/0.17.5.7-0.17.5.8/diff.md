# Comparing `tmp/pydatawork-0.17.5.7.tar.gz` & `tmp/pydatawork-0.17.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.5.7.tar", last modified: Thu Jul 20 18:19:07 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.5.8.tar", last modified: Sat Jul 29 16:09:45 2023, max compression
```

## Comparing `pydatawork-0.17.5.7.tar` & `pydatawork-0.17.5.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16977 2023-07-08 15:03:51.000000 pydatawork-0.17.5.7/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    53278 2023-07-20 18:16:53.000000 pydatawork-0.17.5.7/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-20 18:17:43.000000 pydatawork-0.17.5.7/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22366 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    17047 2023-07-29 16:07:37.000000 pydatawork-0.17.5.8/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22366 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    53428 2023-07-24 01:35:40.000000 pydatawork-0.17.5.8/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-29 16:08:12.000000 pydatawork-0.17.5.8/setup.py
```

### Comparing `pydatawork-0.17.5.7/PKG-INFO` & `pydatawork-0.17.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.7
+Version: 0.17.5.8
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -14,14 +14,21 @@
         
         pydatawork content summary：Mon Jul 3 21:52:47 CST 2023
         - basic functions
         - data processing
         - data analysis
         
         
+        # roadmap
+        
+        roadmap:
+        https://trello.com/b/oGOjATiO/datawork-roadmap
+        
+        
+        
         
         # pydatawork测试环境：python 3.7.2
         
         pydatawork中所用到的库：
         
         ```python
         import os
```

### Comparing `pydatawork-0.17.5.7/README.md` & `pydatawork-0.17.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 
 pydatawork content summary：Mon Jul 3 21:52:47 CST 2023
 - basic functions
 - data processing
 - data analysis
 
 
+# roadmap
+
+roadmap:
+https://trello.com/b/oGOjATiO/datawork-roadmap
+
+
+
 
 # pydatawork测试环境：python 3.7.2
 
 pydatawork中所用到的库：
 
 ```python
 import os
```

### Comparing `pydatawork-0.17.5.7/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.5.8/pydatawork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.7
+Version: 0.17.5.8
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -14,14 +14,21 @@
         
         pydatawork content summary：Mon Jul 3 21:52:47 CST 2023
         - basic functions
         - data processing
         - data analysis
         
         
+        # roadmap
+        
+        roadmap:
+        https://trello.com/b/oGOjATiO/datawork-roadmap
+        
+        
+        
         
         # pydatawork测试环境：python 3.7.2
         
         pydatawork中所用到的库：
         
         ```python
         import os
```

### Comparing `pydatawork-0.17.5.7/pydatawork.py` & `pydatawork-0.17.5.8/pydatawork.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,20 @@
 #     print("\n1.pydatawork的官方文档中提供了函数说明和一些示例，或许对你有用。\npydatawork官方文档：https://pypi.org/project/pydatawork/")
 #     print("\n2.如果你有好的想法或建议，欢迎给我反馈。\n我的邮箱是: zhouqiling.bjfu@foxmail.com")
 #     print("\n3.也可以描述你的需求，给pydatawork提出功能建议。\npydatawork功能建议收集表：https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ")
 #     print("\n")
 
 
 def hello_jkzhou(): # 为什么要定义主函数？ @知识卡片
+    """
+    功能：pydatawork官方文档：交互式页面，练习页面，获取联系方式。
+
+    参数：无需输入参数。
+    """
+    
     # 先定义需要用到的函数
     def menu():
         print("\n==pydatawork官方文档==")
         print("1.basic functions") # 基础函数索引
         print("2.data processing") # 数据处理函数索引
         print("3.data analysis") # 数据分析函数索引
         print("4.查找") # 根据用户输入的关键词，提示对方用哪个函数
```

### Comparing `pydatawork-0.17.5.7/setup.py` & `pydatawork-0.17.5.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.5.7',
+    version='0.17.5.8',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

