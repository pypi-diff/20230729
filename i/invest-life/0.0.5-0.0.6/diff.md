# Comparing `tmp/invest_life-0.0.5.tar.gz` & `tmp/invest_life-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest_life-0.0.5.tar", last modified: Thu Jul 27 09:30:39 2023, max compression
+gzip compressed data, was "invest_life-0.0.6.tar", last modified: Sat Jul 29 01:34:42 2023, max compression
```

## Comparing `invest_life-0.0.5.tar` & `invest_life-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 09:30:39.291898 invest_life-0.0.5/
--rw-r--r--   0 mac        (501) staff       (20)     1073 2023-07-25 13:12:51.000000 invest_life-0.0.5/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-27 09:30:39.291588 invest_life-0.0.5/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      159 2023-07-25 13:12:33.000000 invest_life-0.0.5/README.md
--rw-r--r--   0 mac        (501) staff       (20)      459 2023-07-27 09:30:21.000000 invest_life-0.0.5/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-27 09:30:39.291995 invest_life-0.0.5/setup.cfg
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 09:30:39.288093 invest_life-0.0.5/src/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-25 13:00:59.000000 invest_life-0.0.5/src/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 09:30:39.290208 invest_life-0.0.5/src/invest_life.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-27 09:30:39.000000 invest_life-0.0.5/src/invest_life.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      236 2023-07-27 09:30:39.000000 invest_life-0.0.5/src/invest_life.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-27 09:30:39.000000 invest_life-0.0.5/src/invest_life.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       20 2023-07-27 09:30:39.000000 invest_life-0.0.5/src/invest_life.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)   221418 2023-07-27 09:30:14.000000 invest_life-0.0.5/src/investlife.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 09:30:39.290622 invest_life-0.0.5/tests/
--rw-r--r--   0 mac        (501) staff       (20)       24 2023-07-25 14:03:29.000000 invest_life-0.0.5/tests/test.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 01:34:42.604053 invest_life-0.0.6/
+-rw-r--r--   0 mac        (501) staff       (20)     1073 2023-07-25 13:12:51.000000 invest_life-0.0.6/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-29 01:34:42.603713 invest_life-0.0.6/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      159 2023-07-25 13:12:33.000000 invest_life-0.0.6/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      459 2023-07-29 01:34:17.000000 invest_life-0.0.6/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-29 01:34:42.604158 invest_life-0.0.6/setup.cfg
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 01:34:42.597116 invest_life-0.0.6/src/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-25 13:00:59.000000 invest_life-0.0.6/src/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 01:34:42.601979 invest_life-0.0.6/src/invest_life.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-29 01:34:42.000000 invest_life-0.0.6/src/invest_life.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      236 2023-07-29 01:34:42.000000 invest_life-0.0.6/src/invest_life.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-29 01:34:42.000000 invest_life-0.0.6/src/invest_life.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       20 2023-07-29 01:34:42.000000 invest_life-0.0.6/src/invest_life.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)   221415 2023-07-27 09:37:40.000000 invest_life-0.0.6/src/investlife.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 01:34:42.602543 invest_life-0.0.6/tests/
+-rw-r--r--   0 mac        (501) staff       (20)       24 2023-07-25 14:03:29.000000 invest_life-0.0.6/tests/test.py
```

### Comparing `invest_life-0.0.5/LICENSE` & `invest_life-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `invest_life-0.0.5/PKG-INFO` & `invest_life-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest_life
-Version: 0.0.5
+Version: 0.0.6
 Summary: a package from investor
 Author-email: kelvin <wwwhhitzxt@163.com>
 Project-URL: Homepage, https://investlife.cn/
 Project-URL: Bug Tracker, https://investlife.cn/info/author.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `invest_life-0.0.5/src/invest_life.egg-info/PKG-INFO` & `invest_life-0.0.6/src/invest_life.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-life
-Version: 0.0.5
+Version: 0.0.6
 Summary: a package from investor
 Author-email: kelvin <wwwhhitzxt@163.com>
 Project-URL: Homepage, https://investlife.cn/
 Project-URL: Bug Tracker, https://investlife.cn/info/author.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `invest_life-0.0.5/src/investlife.py` & `invest_life-0.0.6/src/investlife.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # url
 base_url = 'https://investlife.cn/data/'
 
 # token
 g_token = None
 
 # 设置token
-def set_token(user_token):
+def set_token(token = None):
     global g_token
-    g_token = user_token
+    g_token = token
 
 def get_stock_list(listed_state = None, fields = None):
     """
     记录A股上市、退市股票交易代码、股票名称、上市状态等信息；
 
     输入参数：
     :param str listed_state : 上市状态
```

