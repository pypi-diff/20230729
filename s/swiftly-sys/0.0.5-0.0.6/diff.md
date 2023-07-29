# Comparing `tmp/swiftly-sys-0.0.5.tar.gz` & `tmp/swiftly-sys-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-sys-0.0.5.tar", last modified: Sat Jul 29 16:38:32 2023, max compression
+gzip compressed data, was "swiftly-sys-0.0.6.tar", last modified: Sat Jul 29 18:47:28 2023, max compression
```

## Comparing `swiftly-sys-0.0.5.tar` & `swiftly-sys-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 16:38:32.762110 swiftly-sys-0.0.5/
--rw-r--r--   0 brainspoof   (501) staff       (20)    11357 2023-07-29 09:32:23.000000 swiftly-sys-0.0.5/LICENCE
--rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 16:38:32.761963 swiftly-sys-0.0.5/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 16:38:32.760358 swiftly-sys-0.0.5/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)      760 2023-07-29 12:26:12.000000 swiftly-sys-0.0.5/scripts/swiftly
--rwxr-xr-x   0 brainspoof   (501) staff       (20)        8 2023-07-29 16:25:58.000000 swiftly-sys-0.0.5/scripts/swiftly.bat
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 16:38:32.762161 swiftly-sys-0.0.5/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      845 2023-07-29 16:35:32.000000 swiftly-sys-0.0.5/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 16:38:32.760639 swiftly-sys-0.0.5/swiftly/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:12:56.000000 swiftly-sys-0.0.5/swiftly/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 16:38:32.760735 swiftly-sys-0.0.5/swiftly/core/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:09.000000 swiftly-sys-0.0.5/swiftly/core/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 16:38:32.760833 swiftly-sys-0.0.5/swiftly/runtime/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:17.000000 swiftly-sys-0.0.5/swiftly/runtime/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 16:38:32.760929 swiftly-sys-0.0.5/swiftly/runtime/node/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:19.000000 swiftly-sys-0.0.5/swiftly/runtime/node/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 16:38:32.761110 swiftly-sys-0.0.5/swiftly/runtime/python/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:23.000000 swiftly-sys-0.0.5/swiftly/runtime/python/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      198 2023-07-29 12:18:07.000000 swiftly-sys-0.0.5/swiftly/runtime/python/run.sh
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 16:38:32.761768 swiftly-sys-0.0.5/swiftly_sys.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 16:38:32.000000 swiftly-sys-0.0.5/swiftly_sys.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      363 2023-07-29 16:38:32.000000 swiftly-sys-0.0.5/swiftly_sys.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-29 16:38:32.000000 swiftly-sys-0.0.5/swiftly_sys.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        8 2023-07-29 16:38:32.000000 swiftly-sys-0.0.5/swiftly_sys.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.696726 swiftly-sys-0.0.6/
+-rw-r--r--   0 brainspoof   (501) staff       (20)    11357 2023-07-29 09:32:23.000000 swiftly-sys-0.0.6/LICENCE
+-rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 18:47:28.696591 swiftly-sys-0.0.6/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.693301 swiftly-sys-0.0.6/scripts/
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.694478 swiftly-sys-0.0.6/scripts/unix/
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.694716 swiftly-sys-0.0.6/scripts/unix/python/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-29 18:38:14.000000 swiftly-sys-0.0.6/scripts/unix/python/swiftly.python.sh
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)       59 2023-07-29 18:38:43.000000 swiftly-sys-0.0.6/scripts/unix/swiftly
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.694976 swiftly-sys-0.0.6/scripts/windows/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)        8 2023-07-29 16:25:58.000000 swiftly-sys-0.0.6/scripts/windows/swiftly.bat
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 18:47:28.696775 swiftly-sys-0.0.6/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      976 2023-07-29 18:47:22.000000 swiftly-sys-0.0.6/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.695286 swiftly-sys-0.0.6/swiftly/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:12:56.000000 swiftly-sys-0.0.6/swiftly/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.695409 swiftly-sys-0.0.6/swiftly/core/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:09.000000 swiftly-sys-0.0.6/swiftly/core/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.695551 swiftly-sys-0.0.6/swiftly/runtime/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:17.000000 swiftly-sys-0.0.6/swiftly/runtime/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.695705 swiftly-sys-0.0.6/swiftly/runtime/node/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:19.000000 swiftly-sys-0.0.6/swiftly/runtime/node/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.695840 swiftly-sys-0.0.6/swiftly/runtime/python/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:23.000000 swiftly-sys-0.0.6/swiftly/runtime/python/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 18:47:28.696399 swiftly-sys-0.0.6/swiftly_sys.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 18:47:28.000000 swiftly-sys-0.0.6/swiftly_sys.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      495 2023-07-29 18:47:28.000000 swiftly-sys-0.0.6/swiftly_sys.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-29 18:47:28.000000 swiftly-sys-0.0.6/swiftly_sys.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        8 2023-07-29 18:47:28.000000 swiftly-sys-0.0.6/swiftly_sys.egg-info/top_level.txt
```

### Comparing `swiftly-sys-0.0.5/LICENCE` & `swiftly-sys-0.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `swiftly-sys-0.0.5/PKG-INFO` & `swiftly-sys-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftly-sys
-Version: 0.0.5
+Version: 0.0.6
 Summary: Do what you're good at; writing code. Swiftly handle the rest
 Home-page: https://github.com/brainspoof/swiftly-sys
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 License: Apache2
 Keywords: python project,project management,code management,project building,python project managment,organized project
 License-File: LICENCE
```

### Comparing `swiftly-sys-0.0.5/setup.py` & `swiftly-sys-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from setuptools import setup, find_packages
+import glob
+import os
+
+scripts = [f for f in glob.glob('scripts/unix/**/*', recursive=True) + glob.glob('scripts/windows/**/*', recursive=True) if os.path.isfile(f)]
 
 setup(
     name='swiftly-sys',
-    version='0.0.5',
+    version='0.0.6',
     license='Apache2',
     packages=find_packages(),
-    scripts=['scripts/swiftly', 'scripts/swiftly.bat'],
+    scripts=scripts,
     description = 'Do what you\'re good at; writing code. Swiftly handle the rest',
     long_description='''
     Swiftly let's you focus on building amazing products. Swiftly makes sure your entire code scales, while keeping the code so maintainable. No spaghetti code, ever!\n
     Read the docs at: https://docs.swiftly-sys.tech
     ''',
     author = 'Shubham Gupta',
     author_email = 'shubhastro2@gmail.com',
```

### Comparing `swiftly-sys-0.0.5/swiftly_sys.egg-info/PKG-INFO` & `swiftly-sys-0.0.6/swiftly_sys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftly-sys
-Version: 0.0.5
+Version: 0.0.6
 Summary: Do what you're good at; writing code. Swiftly handle the rest
 Home-page: https://github.com/brainspoof/swiftly-sys
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 License: Apache2
 Keywords: python project,project management,code management,project building,python project managment,organized project
 License-File: LICENCE
```

