# Comparing `tmp/t265-0.1.3.tar.gz` & `tmp/t265-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t265-0.1.3.tar", last modified: Tue Jul 18 01:32:23 2023, max compression
+gzip compressed data, was "t265-0.1.4.tar", last modified: Sat Jul 29 04:52:41 2023, max compression
```

## Comparing `t265-0.1.3.tar` & `t265-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-18 01:32:23.037089 t265-0.1.3/
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       25 2023-07-18 00:54:55.000000 t265-0.1.3/MANIFEST.in
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-18 01:32:23.037089 t265-0.1.3/PKG-INFO
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-18 01:21:38.000000 t265-0.1.3/requirements.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       38 2023-07-18 01:32:23.037089 t265-0.1.3/setup.cfg
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     1008 2023-07-18 01:29:33.000000 t265-0.1.3/setup.py
-drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-18 01:32:23.037089 t265-0.1.3/t265/
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     2560 2023-07-18 01:17:25.000000 t265-0.1.3/t265/Tracking.py
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       31 2023-07-18 00:54:55.000000 t265-0.1.3/t265/__init__.py
-drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-18 01:32:23.037089 t265-0.1.3/t265.egg-info/
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-18 01:32:23.000000 t265-0.1.3/t265.egg-info/PKG-INFO
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      210 2023-07-18 01:32:23.000000 t265-0.1.3/t265.egg-info/SOURCES.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        1 2023-07-18 01:32:23.000000 t265-0.1.3/t265.egg-info/dependency_links.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-18 01:32:23.000000 t265-0.1.3/t265.egg-info/requires.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        5 2023-07-18 01:32:23.000000 t265-0.1.3/t265.egg-info/top_level.txt
+drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 04:52:41.373495 t265-0.1.4/
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       25 2023-07-18 00:54:55.000000 t265-0.1.4/MANIFEST.in
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-29 04:52:41.373495 t265-0.1.4/PKG-INFO
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-18 01:21:38.000000 t265-0.1.4/requirements.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       38 2023-07-29 04:52:41.373495 t265-0.1.4/setup.cfg
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     1008 2023-07-29 04:50:35.000000 t265-0.1.4/setup.py
+drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 04:52:41.373495 t265-0.1.4/t265/
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     3931 2023-07-29 04:42:31.000000 t265-0.1.4/t265/Tracking.py
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       31 2023-07-18 00:54:55.000000 t265-0.1.4/t265/__init__.py
+drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 04:52:41.373495 t265-0.1.4/t265.egg-info/
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-29 04:52:41.000000 t265-0.1.4/t265.egg-info/PKG-INFO
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      210 2023-07-29 04:52:41.000000 t265-0.1.4/t265.egg-info/SOURCES.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        1 2023-07-29 04:52:41.000000 t265-0.1.4/t265.egg-info/dependency_links.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-29 04:52:41.000000 t265-0.1.4/t265.egg-info/requires.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        5 2023-07-29 04:52:41.000000 t265-0.1.4/t265.egg-info/top_level.txt
```

### Comparing `t265-0.1.3/PKG-INFO` & `t265-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t265
-Version: 0.1.3
+Version: 0.1.4
 Summary: t265 Tracking camera API wrapper
 Author: Yusuke Tanaka
 License: LGPLv3
 Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework
 Classifier: Intended Audience :: Developers
```

### Comparing `t265-0.1.3/setup.py` & `t265-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name='t265',
-    version='0.1.3',
+    version='0.1.4',
     description='t265 Tracking camera API wrapper',
     author='Yusuke Tanaka',
     license='LGPLv3',
     project_urls={'GitHub':'https://github.com/Suke0811/Localization_T265'},
     packages=find_packages(include=['t265', 't265.*']),
     install_requires=requirements,
     classifiers=[
```

### Comparing `t265-0.1.3/t265.egg-info/PKG-INFO` & `t265-0.1.4/t265.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t265
-Version: 0.1.3
+Version: 0.1.4
 Summary: t265 Tracking camera API wrapper
 Author: Yusuke Tanaka
 License: LGPLv3
 Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework
 Classifier: Intended Audience :: Developers
```

