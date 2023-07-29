# Comparing `tmp/mylibrarysina-1.1.6.tar.gz` & `tmp/mylibrarysina-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mylibrarysina-1.1.6.tar", last modified: Thu Jul 27 13:06:26 2023, max compression
+gzip compressed data, was "mylibrarysina-1.1.7.tar", last modified: Sat Jul 29 11:52:35 2023, max compression
```

## Comparing `mylibrarysina-1.1.6.tar` & `mylibrarysina-1.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-27 13:06:26.517391 mylibrarysina-1.1.6/
--rw-rw-r--   0 sina      (1000) sina      (1000)        0 2023-07-27 11:15:26.000000 mylibrarysina-1.1.6/LICENSE
--rw-rw-r--   0 sina      (1000) sina      (1000)      690 2023-07-27 13:06:26.517391 mylibrarysina-1.1.6/PKG-INFO
--rw-rw-r--   0 sina      (1000) sina      (1000)       21 2023-07-27 11:14:06.000000 mylibrarysina-1.1.6/README.md
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-27 13:06:26.517391 mylibrarysina-1.1.6/mylibrarysina.egg-info/
--rw-rw-r--   0 sina      (1000) sina      (1000)      690 2023-07-27 13:06:26.000000 mylibrarysina-1.1.6/mylibrarysina.egg-info/PKG-INFO
--rw-rw-r--   0 sina      (1000) sina      (1000)      174 2023-07-27 13:06:26.000000 mylibrarysina-1.1.6/mylibrarysina.egg-info/SOURCES.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-27 13:06:26.000000 mylibrarysina-1.1.6/mylibrarysina.egg-info/dependency_links.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-27 13:06:26.000000 mylibrarysina-1.1.6/mylibrarysina.egg-info/top_level.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)       38 2023-07-27 13:06:26.517391 mylibrarysina-1.1.6/setup.cfg
--rw-rw-r--   0 sina      (1000) sina      (1000)      742 2023-07-27 13:06:23.000000 mylibrarysina-1.1.6/setup.py
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-29 11:52:35.365054 mylibrarysina-1.1.7/
+-rw-rw-r--   0 sina      (1000) sina      (1000)        0 2023-07-29 11:49:01.000000 mylibrarysina-1.1.7/LICENSE
+-rw-rw-r--   0 sina      (1000) sina      (1000)      690 2023-07-29 11:52:35.365054 mylibrarysina-1.1.7/PKG-INFO
+-rw-rw-r--   0 sina      (1000) sina      (1000)       21 2023-07-29 11:49:01.000000 mylibrarysina-1.1.7/README.md
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-29 11:52:35.365054 mylibrarysina-1.1.7/mylibrarysina.egg-info/
+-rw-rw-r--   0 sina      (1000) sina      (1000)      690 2023-07-29 11:52:35.000000 mylibrarysina-1.1.7/mylibrarysina.egg-info/PKG-INFO
+-rw-rw-r--   0 sina      (1000) sina      (1000)      174 2023-07-29 11:52:35.000000 mylibrarysina-1.1.7/mylibrarysina.egg-info/SOURCES.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-29 11:52:35.000000 mylibrarysina-1.1.7/mylibrarysina.egg-info/dependency_links.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-29 11:52:35.000000 mylibrarysina-1.1.7/mylibrarysina.egg-info/top_level.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)       38 2023-07-29 11:52:35.365054 mylibrarysina-1.1.7/setup.cfg
+-rw-rw-r--   0 sina      (1000) sina      (1000)      742 2023-07-29 11:51:19.000000 mylibrarysina-1.1.7/setup.py
```

### Comparing `mylibrarysina-1.1.6/PKG-INFO` & `mylibrarysina-1.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mylibrarysina
-Version: 1.1.6
+Version: 1.1.7
 Summary: test
 Home-page: https://github.com/SinaSohrab
 Author: Sina
 Author-email: sinasohrab84@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mylibrarysina-1.1.6/mylibrarysina.egg-info/PKG-INFO` & `mylibrarysina-1.1.7/mylibrarysina.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mylibrarysina
-Version: 1.1.6
+Version: 1.1.7
 Summary: test
 Home-page: https://github.com/SinaSohrab
 Author: Sina
 Author-email: sinasohrab84@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mylibrarysina-1.1.6/setup.py` & `mylibrarysina-1.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='mylibrarysina',
-    version='1.1.6',
+    version='1.1.7',
     description='test',
     author='Sina',
     author_email='sinasohrab84@gmail.com',
     packages=[],
     install_requires=[],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

