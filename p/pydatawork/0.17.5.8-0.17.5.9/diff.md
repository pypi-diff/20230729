# Comparing `tmp/pydatawork-0.17.5.8.tar.gz` & `tmp/pydatawork-0.17.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.5.8.tar", last modified: Sat Jul 29 16:09:45 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.5.9.tar", last modified: Sat Jul 29 16:12:22 2023, max compression
```

## Comparing `pydatawork-0.17.5.8.tar` & `pydatawork-0.17.5.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22366 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    17047 2023-07-29 16:07:37.000000 pydatawork-0.17.5.8/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22366 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    53428 2023-07-24 01:35:40.000000 pydatawork-0.17.5.8/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-29 16:09:45.000000 pydatawork-0.17.5.8/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-29 16:08:12.000000 pydatawork-0.17.5.8/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22368 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    17049 2023-07-29 16:11:28.000000 pydatawork-0.17.5.9/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22368 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    53428 2023-07-24 01:35:40.000000 pydatawork-0.17.5.9/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-29 16:12:22.000000 pydatawork-0.17.5.9/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-29 16:12:04.000000 pydatawork-0.17.5.9/setup.py
```

### Comparing `pydatawork-0.17.5.8/PKG-INFO` & `pydatawork-0.17.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.8
+Version: 0.17.5.9
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -16,15 +16,15 @@
         - basic functions
         - data processing
         - data analysis
         
         
         # roadmap
         
-        roadmap:
+        roadmap：
         https://trello.com/b/oGOjATiO/datawork-roadmap
         
         
         
         
         # pydatawork测试环境：python 3.7.2
```

### Comparing `pydatawork-0.17.5.8/README.md` & `pydatawork-0.17.5.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 - basic functions
 - data processing
 - data analysis
 
 
 # roadmap
 
-roadmap:
+roadmap：
 https://trello.com/b/oGOjATiO/datawork-roadmap
 
 
 
 
 # pydatawork测试环境：python 3.7.2
```

### Comparing `pydatawork-0.17.5.8/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.5.9/pydatawork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.8
+Version: 0.17.5.9
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -16,15 +16,15 @@
         - basic functions
         - data processing
         - data analysis
         
         
         # roadmap
         
-        roadmap:
+        roadmap：
         https://trello.com/b/oGOjATiO/datawork-roadmap
         
         
         
         
         # pydatawork测试环境：python 3.7.2
```

### Comparing `pydatawork-0.17.5.8/pydatawork.py` & `pydatawork-0.17.5.9/pydatawork.py`

 * *Files identical despite different names*

### Comparing `pydatawork-0.17.5.8/setup.py` & `pydatawork-0.17.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.5.8',
+    version='0.17.5.9',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

