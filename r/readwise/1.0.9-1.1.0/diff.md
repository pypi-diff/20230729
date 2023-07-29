# Comparing `tmp/readwise-1.0.9.tar.gz` & `tmp/readwise-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readwise-1.0.9.tar", last modified: Mon Mar  6 22:43:28 2023, max compression
+gzip compressed data, was "readwise-1.1.0.tar", last modified: Sat Jul 29 19:58:26 2023, max compression
```

## Comparing `readwise-1.0.9.tar` & `readwise-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:43:28.967107 readwise-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-06 22:43:26.000000 readwise-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-03-06 22:43:28.967107 readwise-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-06 22:43:26.000000 readwise-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:43:28.967107 readwise-1.0.9/readwise/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-06 22:43:26.000000 readwise-1.0.9/readwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14514 2023-03-06 22:43:26.000000 readwise-1.0.9/readwise/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-06 22:43:26.000000 readwise-1.0.9/readwise/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:43:28.967107 readwise-1.0.9/readwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-03-06 22:43:28.000000 readwise-1.0.9/readwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-06 22:43:28.000000 readwise-1.0.9/readwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 22:43:28.000000 readwise-1.0.9/readwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-06 22:43:28.000000 readwise-1.0.9/readwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-06 22:43:28.000000 readwise-1.0.9/readwise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 22:43:28.967107 readwise-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-06 22:43:26.000000 readwise-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:58:26.276115 readwise-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-29 19:58:23.000000 readwise-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-29 19:58:26.276115 readwise-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-29 19:58:23.000000 readwise-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:58:26.276115 readwise-1.1.0/readwise/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-29 19:58:23.000000 readwise-1.1.0/readwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19325 2023-07-29 19:58:23.000000 readwise-1.1.0/readwise/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-29 19:58:23.000000 readwise-1.1.0/readwise/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:58:26.276115 readwise-1.1.0/readwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-29 19:58:26.000000 readwise-1.1.0/readwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-29 19:58:26.000000 readwise-1.1.0/readwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 19:58:26.000000 readwise-1.1.0/readwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 19:58:26.000000 readwise-1.1.0/readwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 19:58:26.000000 readwise-1.1.0/readwise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 19:58:26.276115 readwise-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-29 19:58:23.000000 readwise-1.1.0/setup.py
```

### Comparing `readwise-1.0.9/LICENSE` & `readwise-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readwise-1.0.9/PKG-INFO` & `readwise-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: readwise
-Version: 1.0.9
+Version: 1.1.0
 Summary: Readwise api client
 Home-page: https://github.com/rwxd/pyreadwise
 Author: rwxd
 Author-email: rwxd@pm.me
 License: MIT
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Module to use the Readwise API
 
 This module is a wrapper for the Readwise API.
@@ -20,15 +18,15 @@
 
 ## Installation
 
 ```bash
 pip install -U readwise
 ```
 
-## Quickstart
+## How to use
 
 ### Readwise API
 
 ```python
 from readwise import Readwise
 
 client = Readwise('token')
```

### Comparing `readwise-1.0.9/README.md` & `readwise-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Installation
 
 ```bash
 pip install -U readwise
 ```
 
-## Quickstart
+## How to use
 
 ### Readwise API
 
 ```python
 from readwise import Readwise
 
 client = Readwise('token')
```

### Comparing `readwise-1.0.9/readwise.egg-info/PKG-INFO` & `readwise-1.1.0/readwise.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: readwise
-Version: 1.0.9
+Version: 1.1.0
 Summary: Readwise api client
 Home-page: https://github.com/rwxd/pyreadwise
 Author: rwxd
 Author-email: rwxd@pm.me
 License: MIT
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Module to use the Readwise API
 
 This module is a wrapper for the Readwise API.
@@ -20,15 +18,15 @@
 
 ## Installation
 
 ```bash
 pip install -U readwise
 ```
 
-## Quickstart
+## How to use
 
 ### Readwise API
 
 ```python
 from readwise import Readwise
 
 client = Readwise('token')
```

### Comparing `readwise-1.0.9/setup.py` & `readwise-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,12 +28,10 @@
     author='rwxd',
     author_email='rwxd@pm.me',
     url='https://github.com/rwxd/pyreadwise',
     license='MIT',
     packages=['readwise'],
     install_requires=required,
     classifiers=[
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 )
```

