# Comparing `tmp/swiftly-sys-0.0.8.tar.gz` & `tmp/swiftly-sys-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-sys-0.0.8.tar", last modified: Sat Jul 29 19:02:57 2023, max compression
+gzip compressed data, was "swiftly-sys-0.0.9.tar", last modified: Sat Jul 29 19:07:12 2023, max compression
```

## Comparing `swiftly-sys-0.0.8.tar` & `swiftly-sys-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.581618 swiftly-sys-0.0.8/
--rw-r--r--   0 brainspoof   (501) staff       (20)    11357 2023-07-29 09:32:23.000000 swiftly-sys-0.0.8/LICENCE
--rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 19:02:57.581471 swiftly-sys-0.0.8/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.577881 swiftly-sys-0.0.8/scripts/
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.579042 swiftly-sys-0.0.8/scripts/unix/
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.579565 swiftly-sys-0.0.8/scripts/unix/python/
--rw-r--r--   0 brainspoof   (501) staff       (20)       40 2023-07-29 18:59:50.000000 swiftly-sys-0.0.8/scripts/unix/python/swiftly-python-django.sh
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 18:59:15.000000 swiftly-sys-0.0.8/scripts/unix/python/swiftly-python.sh
--rwxr-xr-x   0 brainspoof   (501) staff       (20)       94 2023-07-29 19:02:25.000000 swiftly-sys-0.0.8/scripts/unix/swiftly
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580033 swiftly-sys-0.0.8/scripts/windows/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)        8 2023-07-29 16:25:58.000000 swiftly-sys-0.0.8/scripts/windows/swiftly.bat
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 19:02:57.581674 swiftly-sys-0.0.8/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      976 2023-07-29 19:02:35.000000 swiftly-sys-0.0.8/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580301 swiftly-sys-0.0.8/swiftly/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:12:56.000000 swiftly-sys-0.0.8/swiftly/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580401 swiftly-sys-0.0.8/swiftly/core/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:09.000000 swiftly-sys-0.0.8/swiftly/core/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580496 swiftly-sys-0.0.8/swiftly/runtime/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:17.000000 swiftly-sys-0.0.8/swiftly/runtime/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580585 swiftly-sys-0.0.8/swiftly/runtime/node/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:19.000000 swiftly-sys-0.0.8/swiftly/runtime/node/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580704 swiftly-sys-0.0.8/swiftly/runtime/python/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:23.000000 swiftly-sys-0.0.8/swiftly/runtime/python/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.581267 swiftly-sys-0.0.8/swiftly_sys.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 19:02:57.000000 swiftly-sys-0.0.8/swiftly_sys.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      540 2023-07-29 19:02:57.000000 swiftly-sys-0.0.8/swiftly_sys.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-29 19:02:57.000000 swiftly-sys-0.0.8/swiftly_sys.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        8 2023-07-29 19:02:57.000000 swiftly-sys-0.0.8/swiftly_sys.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.408031 swiftly-sys-0.0.9/
+-rw-r--r--   0 brainspoof   (501) staff       (20)    11357 2023-07-29 09:32:23.000000 swiftly-sys-0.0.9/LICENCE
+-rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 19:07:12.407892 swiftly-sys-0.0.9/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.404662 swiftly-sys-0.0.9/scripts/
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.405838 swiftly-sys-0.0.9/scripts/unix/
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.406329 swiftly-sys-0.0.9/scripts/unix/python/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       40 2023-07-29 18:59:50.000000 swiftly-sys-0.0.9/scripts/unix/python/swiftly-python-django.sh
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 18:59:15.000000 swiftly-sys-0.0.9/scripts/unix/python/swiftly-python.sh
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)       90 2023-07-29 19:04:14.000000 swiftly-sys-0.0.9/scripts/unix/swiftly
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.406586 swiftly-sys-0.0.9/scripts/windows/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)        8 2023-07-29 16:25:58.000000 swiftly-sys-0.0.9/scripts/windows/swiftly.bat
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 19:07:12.408085 swiftly-sys-0.0.9/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      976 2023-07-29 19:07:08.000000 swiftly-sys-0.0.9/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.406827 swiftly-sys-0.0.9/swiftly/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:12:56.000000 swiftly-sys-0.0.9/swiftly/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.406922 swiftly-sys-0.0.9/swiftly/core/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:09.000000 swiftly-sys-0.0.9/swiftly/core/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.407008 swiftly-sys-0.0.9/swiftly/runtime/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:17.000000 swiftly-sys-0.0.9/swiftly/runtime/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.407097 swiftly-sys-0.0.9/swiftly/runtime/node/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:19.000000 swiftly-sys-0.0.9/swiftly/runtime/node/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.407183 swiftly-sys-0.0.9/swiftly/runtime/python/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:23.000000 swiftly-sys-0.0.9/swiftly/runtime/python/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:07:12.407670 swiftly-sys-0.0.9/swiftly_sys.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 19:07:12.000000 swiftly-sys-0.0.9/swiftly_sys.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      540 2023-07-29 19:07:12.000000 swiftly-sys-0.0.9/swiftly_sys.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-29 19:07:12.000000 swiftly-sys-0.0.9/swiftly_sys.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        8 2023-07-29 19:07:12.000000 swiftly-sys-0.0.9/swiftly_sys.egg-info/top_level.txt
```

### Comparing `swiftly-sys-0.0.8/LICENCE` & `swiftly-sys-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `swiftly-sys-0.0.8/PKG-INFO` & `swiftly-sys-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftly-sys
-Version: 0.0.8
+Version: 0.0.9
 Summary: Do what you're good at; writing code. Swiftly handle the rest
 Home-page: https://github.com/brainspoof/swiftly-sys
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 License: Apache2
 Keywords: python project,project management,code management,project building,python project managment,organized project
 License-File: LICENCE
```

### Comparing `swiftly-sys-0.0.8/setup.py` & `swiftly-sys-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import glob
 import os
 
 scripts = [f for f in glob.glob('scripts/unix/**/*', recursive=True) + glob.glob('scripts/windows/**/*', recursive=True) if os.path.isfile(f)]
 
 setup(
     name='swiftly-sys',
-    version='0.0.8',
+    version='0.0.9',
     license='Apache2',
     packages=find_packages(),
     scripts=scripts,
     description = 'Do what you\'re good at; writing code. Swiftly handle the rest',
     long_description='''
     Swiftly let's you focus on building amazing products. Swiftly makes sure your entire code scales, while keeping the code so maintainable. No spaghetti code, ever!\n
     Read the docs at: https://docs.swiftly-sys.tech
```

### Comparing `swiftly-sys-0.0.8/swiftly_sys.egg-info/PKG-INFO` & `swiftly-sys-0.0.9/swiftly_sys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftly-sys
-Version: 0.0.8
+Version: 0.0.9
 Summary: Do what you're good at; writing code. Swiftly handle the rest
 Home-page: https://github.com/brainspoof/swiftly-sys
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 License: Apache2
 Keywords: python project,project management,code management,project building,python project managment,organized project
 License-File: LICENCE
```

### Comparing `swiftly-sys-0.0.8/swiftly_sys.egg-info/SOURCES.txt` & `swiftly-sys-0.0.9/swiftly_sys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

