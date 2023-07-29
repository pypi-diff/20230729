# Comparing `tmp/csidimageprocessing-0.0.1.tar.gz` & `tmp/csidimageprocessing-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csidimageprocessing-0.0.1.tar", last modified: Sat Jul 29 16:07:54 2023, max compression
+gzip compressed data, was "csidimageprocessing-0.0.2.tar", last modified: Sat Jul 29 16:36:06 2023, max compression
```

## Comparing `csidimageprocessing-0.0.1.tar` & `csidimageprocessing-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 siddharthach   (501) staff       (20)        0 2023-07-29 16:07:54.658308 csidimageprocessing-0.0.1/
--rw-r--r--   0 siddharthach   (501) staff       (20)     1075 2023-07-29 16:00:36.000000 csidimageprocessing-0.0.1/LICENSE
--rw-r--r--   0 siddharthach   (501) staff       (20)      619 2023-07-29 16:07:54.658193 csidimageprocessing-0.0.1/PKG-INFO
--rw-r--r--   0 siddharthach   (501) staff       (20)       37 2023-07-29 16:01:27.000000 csidimageprocessing-0.0.1/README.txt
-drwxr-xr-x   0 siddharthach   (501) staff       (20)        0 2023-07-29 16:07:54.658005 csidimageprocessing-0.0.1/csidimageprocessing.egg-info/
--rw-r--r--   0 siddharthach   (501) staff       (20)      619 2023-07-29 16:07:54.000000 csidimageprocessing-0.0.1/csidimageprocessing.egg-info/PKG-INFO
--rw-r--r--   0 siddharthach   (501) staff       (20)      241 2023-07-29 16:07:54.000000 csidimageprocessing-0.0.1/csidimageprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 siddharthach   (501) staff       (20)        1 2023-07-29 16:07:54.000000 csidimageprocessing-0.0.1/csidimageprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 siddharthach   (501) staff       (20)       31 2023-07-29 16:07:54.000000 csidimageprocessing-0.0.1/csidimageprocessing.egg-info/requires.txt
--rw-r--r--   0 siddharthach   (501) staff       (20)        1 2023-07-29 16:07:54.000000 csidimageprocessing-0.0.1/csidimageprocessing.egg-info/top_level.txt
--rw-r--r--   0 siddharthach   (501) staff       (20)       38 2023-07-29 16:07:54.658348 csidimageprocessing-0.0.1/setup.cfg
--rw-r--r--   0 siddharthach   (501) staff       (20)      730 2023-07-29 16:02:30.000000 csidimageprocessing-0.0.1/setup.py
+drwxr-xr-x   0 siddharthach   (501) staff       (20)        0 2023-07-29 16:36:06.517171 csidimageprocessing-0.0.2/
+-rw-r--r--   0 siddharthach   (501) staff       (20)       77 2023-07-29 16:03:13.000000 csidimageprocessing-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 siddharthach   (501) staff       (20)     1075 2023-07-29 16:00:36.000000 csidimageprocessing-0.0.2/LICENSE
+-rw-r--r--   0 siddharthach   (501) staff       (20)       25 2023-07-29 16:32:49.000000 csidimageprocessing-0.0.2/MANIFEST.in
+-rw-r--r--   0 siddharthach   (501) staff       (20)      619 2023-07-29 16:36:06.517048 csidimageprocessing-0.0.2/PKG-INFO
+-rw-r--r--   0 siddharthach   (501) staff       (20)       37 2023-07-29 16:01:27.000000 csidimageprocessing-0.0.2/README.txt
+-rw-r--r--   0 siddharthach   (501) staff       (20)     2528 2023-07-29 16:13:47.000000 csidimageprocessing-0.0.2/__init__.py
+drwxr-xr-x   0 siddharthach   (501) staff       (20)        0 2023-07-29 16:36:06.516864 csidimageprocessing-0.0.2/csidimageprocessing.egg-info/
+-rw-r--r--   0 siddharthach   (501) staff       (20)      619 2023-07-29 16:36:06.000000 csidimageprocessing-0.0.2/csidimageprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 siddharthach   (501) staff       (20)      279 2023-07-29 16:36:06.000000 csidimageprocessing-0.0.2/csidimageprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 siddharthach   (501) staff       (20)        1 2023-07-29 16:36:06.000000 csidimageprocessing-0.0.2/csidimageprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 siddharthach   (501) staff       (20)       31 2023-07-29 16:36:06.000000 csidimageprocessing-0.0.2/csidimageprocessing.egg-info/requires.txt
+-rw-r--r--   0 siddharthach   (501) staff       (20)        1 2023-07-29 16:36:06.000000 csidimageprocessing-0.0.2/csidimageprocessing.egg-info/top_level.txt
+-rw-r--r--   0 siddharthach   (501) staff       (20)       38 2023-07-29 16:36:06.517215 csidimageprocessing-0.0.2/setup.cfg
+-rw-r--r--   0 siddharthach   (501) staff       (20)      730 2023-07-29 16:35:43.000000 csidimageprocessing-0.0.2/setup.py
```

### Comparing `csidimageprocessing-0.0.1/LICENSE` & `csidimageprocessing-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csidimageprocessing-0.0.1/PKG-INFO` & `csidimageprocessing-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csidimageprocessing
-Version: 0.0.1
+Version: 0.0.2
 Summary: A  basic image segentation package
 Home-page: 
 Author: Siddhartha
 Author-email: chappidisiddhartha59736@gmail.com
 License: MIT
 Keywords: image
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `csidimageprocessing-0.0.1/csidimageprocessing.egg-info/PKG-INFO` & `csidimageprocessing-0.0.2/csidimageprocessing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csidimageprocessing
-Version: 0.0.1
+Version: 0.0.2
 Summary: A  basic image segentation package
 Home-page: 
 Author: Siddhartha
 Author-email: chappidisiddhartha59736@gmail.com
 License: MIT
 Keywords: image
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `csidimageprocessing-0.0.1/setup.py` & `csidimageprocessing-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='csidimageprocessing',
-  version='0.0.1',
+  version='0.0.2',
   description='A  basic image segentation package',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Siddhartha',
   author_email='chappidisiddhartha59736@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

