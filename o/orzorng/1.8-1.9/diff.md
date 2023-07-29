# Comparing `tmp/orzorng-1.8.tar.gz` & `tmp/orzorng-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orzorng-1.8.tar", last modified: Tue Feb 21 07:54:33 2023, max compression
+gzip compressed data, was "orzorng-1.9.tar", last modified: Wed Feb 22 07:54:41 2023, max compression
```

## Comparing `orzorng-1.8.tar` & `orzorng-1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-02-21 07:54:33.073228 orzorng-1.8/
--rw-r--r--   0 hugo       (501) staff       (20)     1051 2023-02-08 06:53:04.000000 orzorng-1.8/LICENSE.txt
--rw-r--r--   0 hugo       (501) staff       (20)       36 2023-02-08 09:07:55.000000 orzorng-1.8/MANIFEST.in
--rw-r--r--   0 hugo       (501) staff       (20)      615 2023-02-21 07:54:33.073367 orzorng-1.8/PKG-INFO
--rw-r--r--   0 hugo       (501) staff       (20)       23 2023-02-08 06:49:18.000000 orzorng-1.8/README.md
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-02-21 07:54:33.070083 orzorng-1.8/orzorng/
--rw-r--r--   0 hugo       (501) staff       (20)      327 2023-02-21 03:15:07.000000 orzorng-1.8/orzorng/__init__.py
--rw-r--r--   0 hugo       (501) staff       (20)      188 2023-02-15 02:51:57.000000 orzorng-1.8/orzorng/array.py
--rw-r--r--   0 hugo       (501) staff       (20)     1050 2023-02-21 03:15:07.000000 orzorng-1.8/orzorng/file.py
--rw-r--r--   0 hugo       (501) staff       (20)      240 2023-02-09 05:20:37.000000 orzorng-1.8/orzorng/folder.py
--rw-r--r--   0 hugo       (501) staff       (20)     1634 2023-02-21 07:54:11.000000 orzorng-1.8/orzorng/network.py
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-02-21 07:54:33.072464 orzorng-1.8/orzorng/res/
--rw-r--r--   0 hugo       (501) staff       (20)     1973 2023-02-18 10:01:13.000000 orzorng-1.8/orzorng/res/bans.data
--rw-r--r--   0 hugo       (501) staff       (20)      916 2023-02-15 03:06:34.000000 orzorng-1.8/orzorng/string.py
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-02-21 07:54:33.072015 orzorng-1.8/orzorng.egg-info/
--rw-r--r--   0 hugo       (501) staff       (20)      615 2023-02-21 07:54:32.000000 orzorng-1.8/orzorng.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (501) staff       (20)      336 2023-02-21 07:54:32.000000 orzorng-1.8/orzorng.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (501) staff       (20)        1 2023-02-21 07:54:32.000000 orzorng-1.8/orzorng.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (501) staff       (20)        9 2023-02-21 07:54:32.000000 orzorng-1.8/orzorng.egg-info/requires.txt
--rw-r--r--   0 hugo       (501) staff       (20)        8 2023-02-21 07:54:32.000000 orzorng-1.8/orzorng.egg-info/top_level.txt
--rw-r--r--   0 hugo       (501) staff       (20)       79 2023-02-21 07:54:33.074115 orzorng-1.8/setup.cfg
--rw-r--r--   0 hugo       (501) staff       (20)     1645 2023-02-21 07:54:25.000000 orzorng-1.8/setup.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-02-22 07:54:41.313277 orzorng-1.9/
+-rw-r--r--   0 hugo       (501) staff       (20)     1051 2023-02-08 06:53:04.000000 orzorng-1.9/LICENSE.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       36 2023-02-08 09:07:55.000000 orzorng-1.9/MANIFEST.in
+-rw-r--r--   0 hugo       (501) staff       (20)      615 2023-02-22 07:54:41.313501 orzorng-1.9/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)       23 2023-02-08 06:49:18.000000 orzorng-1.9/README.md
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-02-22 07:54:41.305904 orzorng-1.9/orzorng/
+-rw-r--r--   0 hugo       (501) staff       (20)      327 2023-02-21 03:15:07.000000 orzorng-1.9/orzorng/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)      188 2023-02-15 02:51:57.000000 orzorng-1.9/orzorng/array.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1050 2023-02-21 03:15:07.000000 orzorng-1.9/orzorng/file.py
+-rw-r--r--   0 hugo       (501) staff       (20)      240 2023-02-09 05:20:37.000000 orzorng-1.9/orzorng/folder.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1926 2023-02-22 07:54:06.000000 orzorng-1.9/orzorng/network.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-02-22 07:54:41.311956 orzorng-1.9/orzorng/res/
+-rw-r--r--   0 hugo       (501) staff       (20)     1973 2023-02-18 10:01:13.000000 orzorng-1.9/orzorng/res/bans.data
+-rw-r--r--   0 hugo       (501) staff       (20)      916 2023-02-15 03:06:34.000000 orzorng-1.9/orzorng/string.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-02-22 07:54:41.311579 orzorng-1.9/orzorng.egg-info/
+-rw-r--r--   0 hugo       (501) staff       (20)      615 2023-02-22 07:54:41.000000 orzorng-1.9/orzorng.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)      336 2023-02-22 07:54:41.000000 orzorng-1.9/orzorng.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (501) staff       (20)        1 2023-02-22 07:54:41.000000 orzorng-1.9/orzorng.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (501) staff       (20)        9 2023-02-22 07:54:41.000000 orzorng-1.9/orzorng.egg-info/requires.txt
+-rw-r--r--   0 hugo       (501) staff       (20)        8 2023-02-22 07:54:41.000000 orzorng-1.9/orzorng.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       79 2023-02-22 07:54:41.314359 orzorng-1.9/setup.cfg
+-rw-r--r--   0 hugo       (501) staff       (20)     1645 2023-02-22 07:54:06.000000 orzorng-1.9/setup.py
```

### Comparing `orzorng-1.8/LICENSE.txt` & `orzorng-1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `orzorng-1.8/PKG-INFO` & `orzorng-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orzorng
-Version: 1.8
+Version: 1.9
 Summary: learn to use
 Home-page: https://github.com/irnp/orzorng
 Author: hugo
 Author-email: orzorng@gmail.com
 License: MIT
 Keywords: orzorng,hugo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `orzorng-1.8/orzorng/file.py` & `orzorng-1.9/orzorng/file.py`

 * *Files identical despite different names*

### Comparing `orzorng-1.8/orzorng/network.py` & `orzorng-1.9/orzorng/network.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 # -*- coding: utf-8 -*-
 
 import os
 import time
 import requests
 
+requests_api_err_num = 0
 
-def request_api(local_sql, action, data, timeout=120):
+
+def request_api(local_sql, action, data, timeout=120, req_err_func=None):
+    global requests_api_err_num
     try:
         res = requests.post(local_sql, dict({'action': action}, **data), timeout=timeout)
         # print('ok request_api', action, res.text)
         print('ok request_api', action)
+        requests_api_err_num = 0
         return res
     except Exception as get_err:
         print('err request_api', local_sql, action, get_err)
         time.sleep(1)
+        requests_api_err_num += 1
+
+        if requests_api_err_num > 3:
+            if req_err_func != None:
+                req_err_func()
+                requests_api_err_num = 0
+
         return request_api(local_sql, action, data, timeout)
 
 
 change_ip_time = 0
 
 
 def change_ip():
```

### Comparing `orzorng-1.8/orzorng/res/bans.data` & `orzorng-1.9/orzorng/res/bans.data`

 * *Files identical despite different names*

### Comparing `orzorng-1.8/orzorng/string.py` & `orzorng-1.9/orzorng/string.py`

 * *Files identical despite different names*

### Comparing `orzorng-1.8/orzorng.egg-info/PKG-INFO` & `orzorng-1.9/orzorng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orzorng
-Version: 1.8
+Version: 1.9
 Summary: learn to use
 Home-page: https://github.com/irnp/orzorng
 Author: hugo
 Author-email: orzorng@gmail.com
 License: MIT
 Keywords: orzorng,hugo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `orzorng-1.8/setup.py` & `orzorng-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name='orzorng',  # How you named your package folder (MyLib)
     packages=['orzorng'],  # Chose the same as "name"
     include_package_data=True,
     # exclude_package_date={'': ['.gitignore']},
     # zip_safe=False,
-    version='1.8',  # Start with a small number and increase it with every change you make
+    version='1.9',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='learn to use',  # Give a short description about your library
     author='hugo',  # Type in your name
     author_email='orzorng@gmail.com',  # Type in your E-Mail
     url='https://github.com/irnp/orzorng',  # Provide either the link to your github or to your website
     # download_url='',  # I explain this later on
     keywords=['orzorng', 'hugo'],  # Keywords that define your package best
```

