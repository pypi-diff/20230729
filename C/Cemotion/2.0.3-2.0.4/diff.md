# Comparing `tmp/Cemotion-2.0.3.tar.gz` & `tmp/Cemotion-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cemotion-2.0.3.tar", last modified: Sun Apr  2 12:05:50 2023, max compression
+gzip compressed data, was "Cemotion-2.0.4.tar", last modified: Sat Jul 29 09:37:39 2023, max compression
```

## Comparing `Cemotion-2.0.3.tar` & `Cemotion-2.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 DTC        (501) staff       (20)        0 2023-04-02 12:05:50.173592 Cemotion-2.0.3/
-drwxr-xr-x   0 DTC        (501) staff       (20)        0 2023-04-02 12:05:50.172516 Cemotion-2.0.3/Cemotion.egg-info/
--rw-r--r--   0 DTC        (501) staff       (20)     3212 2023-04-02 12:05:50.000000 Cemotion-2.0.3/Cemotion.egg-info/PKG-INFO
--rw-r--r--   0 DTC        (501) staff       (20)      243 2023-04-02 12:05:50.000000 Cemotion-2.0.3/Cemotion.egg-info/SOURCES.txt
--rw-r--r--   0 DTC        (501) staff       (20)        1 2023-04-02 12:05:50.000000 Cemotion-2.0.3/Cemotion.egg-info/dependency_links.txt
--rw-r--r--   0 DTC        (501) staff       (20)       92 2023-04-02 12:05:50.000000 Cemotion-2.0.3/Cemotion.egg-info/requires.txt
--rw-r--r--   0 DTC        (501) staff       (20)        9 2023-04-02 12:05:50.000000 Cemotion-2.0.3/Cemotion.egg-info/top_level.txt
--rw-r--r--   0 DTC        (501) staff       (20)     1066 2023-04-01 15:38:55.000000 Cemotion-2.0.3/LICENSE
--rw-r--r--   0 DTC        (501) staff       (20)     3212 2023-04-02 12:05:50.173456 Cemotion-2.0.3/PKG-INFO
--rw-r--r--   0 DTC        (501) staff       (20)     2853 2023-04-02 12:01:28.000000 Cemotion-2.0.3/README.md
-drwxr-xr-x   0 DTC        (501) staff       (20)        0 2023-04-02 12:05:50.173059 Cemotion-2.0.3/cemotion/
--rw-r--r--   0 DTC        (501) staff       (20)       65 2023-04-01 15:38:55.000000 Cemotion-2.0.3/cemotion/__init__.py
--rw-r--r--   0 DTC        (501) staff       (20)     3782 2023-04-02 12:04:12.000000 Cemotion-2.0.3/cemotion/app.py
--rw-r--r--   0 DTC        (501) staff       (20)     1673 2023-04-02 09:50:25.000000 Cemotion-2.0.3/cemotion/download.py
--rw-r--r--   0 DTC        (501) staff       (20)       38 2023-04-02 12:05:50.173638 Cemotion-2.0.3/setup.cfg
--rw-r--r--   0 DTC        (501) staff       (20)      764 2023-04-02 12:04:39.000000 Cemotion-2.0.3/setup.py
+drwxr-xr-x   0 DTC        (501) staff       (20)        0 2023-07-29 09:37:39.757357 Cemotion-2.0.4/
+drwxr-xr-x   0 DTC        (501) staff       (20)        0 2023-07-29 09:37:39.756164 Cemotion-2.0.4/Cemotion.egg-info/
+-rw-r--r--   0 DTC        (501) staff       (20)     3212 2023-07-29 09:37:39.000000 Cemotion-2.0.4/Cemotion.egg-info/PKG-INFO
+-rw-r--r--   0 DTC        (501) staff       (20)      243 2023-07-29 09:37:39.000000 Cemotion-2.0.4/Cemotion.egg-info/SOURCES.txt
+-rw-r--r--   0 DTC        (501) staff       (20)        1 2023-07-29 09:37:39.000000 Cemotion-2.0.4/Cemotion.egg-info/dependency_links.txt
+-rw-r--r--   0 DTC        (501) staff       (20)       92 2023-07-29 09:37:39.000000 Cemotion-2.0.4/Cemotion.egg-info/requires.txt
+-rw-r--r--   0 DTC        (501) staff       (20)        9 2023-07-29 09:37:39.000000 Cemotion-2.0.4/Cemotion.egg-info/top_level.txt
+-rw-r--r--   0 DTC        (501) staff       (20)     1066 2023-04-01 15:38:55.000000 Cemotion-2.0.4/LICENSE
+-rw-r--r--   0 DTC        (501) staff       (20)     3212 2023-07-29 09:37:39.757204 Cemotion-2.0.4/PKG-INFO
+-rw-r--r--   0 DTC        (501) staff       (20)     2853 2023-04-02 12:01:28.000000 Cemotion-2.0.4/README.md
+drwxr-xr-x   0 DTC        (501) staff       (20)        0 2023-07-29 09:37:39.756869 Cemotion-2.0.4/cemotion/
+-rw-r--r--   0 DTC        (501) staff       (20)       65 2023-04-01 15:38:55.000000 Cemotion-2.0.4/cemotion/__init__.py
+-rw-r--r--   0 DTC        (501) staff       (20)     3782 2023-04-02 12:04:12.000000 Cemotion-2.0.4/cemotion/app.py
+-rw-r--r--   0 DTC        (501) staff       (20)     1673 2023-04-02 09:50:25.000000 Cemotion-2.0.4/cemotion/download.py
+-rw-r--r--   0 DTC        (501) staff       (20)       38 2023-07-29 09:37:39.757414 Cemotion-2.0.4/setup.cfg
+-rw-r--r--   0 DTC        (501) staff       (20)      764 2023-07-29 09:37:32.000000 Cemotion-2.0.4/setup.py
```

### Comparing `Cemotion-2.0.3/Cemotion.egg-info/PKG-INFO` & `Cemotion-2.0.4/Cemotion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cemotion
-Version: 2.0.3
+Version: 2.0.4
 Summary: 基于NLP的中文情感倾向分析库
 Author: Cyberbolt
 Author-email: 735245473@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `Cemotion-2.0.3/LICENSE` & `Cemotion-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Cemotion-2.0.3/PKG-INFO` & `Cemotion-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cemotion
-Version: 2.0.3
+Version: 2.0.4
 Summary: 基于NLP的中文情感倾向分析库
 Author: Cyberbolt
 Author-email: 735245473@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `Cemotion-2.0.3/README.md` & `Cemotion-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Cemotion-2.0.3/cemotion/app.py` & `Cemotion-2.0.4/cemotion/app.py`

 * *Files identical despite different names*

### Comparing `Cemotion-2.0.3/cemotion/download.py` & `Cemotion-2.0.4/cemotion/download.py`

 * *Files identical despite different names*

