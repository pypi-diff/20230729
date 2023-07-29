# Comparing `tmp/swiftly-sys-0.0.7.tar.gz` & `tmp/swiftly-sys-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-sys-0.0.7.tar", last modified: Sat Jul 29 19:00:16 2023, max compression
+gzip compressed data, was "swiftly-sys-0.0.8.tar", last modified: Sat Jul 29 19:02:57 2023, max compression
```

## Comparing `swiftly-sys-0.0.7.tar` & `swiftly-sys-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.152734 swiftly-sys-0.0.7/
--rw-r--r--   0 brainspoof   (501) staff       (20)    11357 2023-07-29 09:32:23.000000 swiftly-sys-0.0.7/LICENCE
--rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 19:00:16.152601 swiftly-sys-0.0.7/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.149443 swiftly-sys-0.0.7/scripts/
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.150784 swiftly-sys-0.0.7/scripts/unix/
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.151148 swiftly-sys-0.0.7/scripts/unix/python/
--rw-r--r--   0 brainspoof   (501) staff       (20)       40 2023-07-29 18:59:50.000000 swiftly-sys-0.0.7/scripts/unix/python/swiftly.python.django.sh
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 18:59:15.000000 swiftly-sys-0.0.7/scripts/unix/python/swiftly.python.sh
--rwxr-xr-x   0 brainspoof   (501) staff       (20)       94 2023-07-29 19:00:02.000000 swiftly-sys-0.0.7/scripts/unix/swiftly
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.151396 swiftly-sys-0.0.7/scripts/windows/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)        8 2023-07-29 16:25:58.000000 swiftly-sys-0.0.7/scripts/windows/swiftly.bat
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 19:00:16.152780 swiftly-sys-0.0.7/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      976 2023-07-29 19:00:09.000000 swiftly-sys-0.0.7/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.151632 swiftly-sys-0.0.7/swiftly/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:12:56.000000 swiftly-sys-0.0.7/swiftly/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.151731 swiftly-sys-0.0.7/swiftly/core/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:09.000000 swiftly-sys-0.0.7/swiftly/core/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.151816 swiftly-sys-0.0.7/swiftly/runtime/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:17.000000 swiftly-sys-0.0.7/swiftly/runtime/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.151903 swiftly-sys-0.0.7/swiftly/runtime/node/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:19.000000 swiftly-sys-0.0.7/swiftly/runtime/node/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.151989 swiftly-sys-0.0.7/swiftly/runtime/python/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:23.000000 swiftly-sys-0.0.7/swiftly/runtime/python/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:00:16.152428 swiftly-sys-0.0.7/swiftly_sys.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 19:00:16.000000 swiftly-sys-0.0.7/swiftly_sys.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      540 2023-07-29 19:00:16.000000 swiftly-sys-0.0.7/swiftly_sys.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-29 19:00:16.000000 swiftly-sys-0.0.7/swiftly_sys.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        8 2023-07-29 19:00:16.000000 swiftly-sys-0.0.7/swiftly_sys.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.581618 swiftly-sys-0.0.8/
+-rw-r--r--   0 brainspoof   (501) staff       (20)    11357 2023-07-29 09:32:23.000000 swiftly-sys-0.0.8/LICENCE
+-rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 19:02:57.581471 swiftly-sys-0.0.8/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.577881 swiftly-sys-0.0.8/scripts/
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.579042 swiftly-sys-0.0.8/scripts/unix/
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.579565 swiftly-sys-0.0.8/scripts/unix/python/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       40 2023-07-29 18:59:50.000000 swiftly-sys-0.0.8/scripts/unix/python/swiftly-python-django.sh
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 18:59:15.000000 swiftly-sys-0.0.8/scripts/unix/python/swiftly-python.sh
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)       94 2023-07-29 19:02:25.000000 swiftly-sys-0.0.8/scripts/unix/swiftly
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580033 swiftly-sys-0.0.8/scripts/windows/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)        8 2023-07-29 16:25:58.000000 swiftly-sys-0.0.8/scripts/windows/swiftly.bat
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 19:02:57.581674 swiftly-sys-0.0.8/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      976 2023-07-29 19:02:35.000000 swiftly-sys-0.0.8/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580301 swiftly-sys-0.0.8/swiftly/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:12:56.000000 swiftly-sys-0.0.8/swiftly/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580401 swiftly-sys-0.0.8/swiftly/core/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:09.000000 swiftly-sys-0.0.8/swiftly/core/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580496 swiftly-sys-0.0.8/swiftly/runtime/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:17.000000 swiftly-sys-0.0.8/swiftly/runtime/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580585 swiftly-sys-0.0.8/swiftly/runtime/node/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:19.000000 swiftly-sys-0.0.8/swiftly/runtime/node/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.580704 swiftly-sys-0.0.8/swiftly/runtime/python/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:23.000000 swiftly-sys-0.0.8/swiftly/runtime/python/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 19:02:57.581267 swiftly-sys-0.0.8/swiftly_sys.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 19:02:57.000000 swiftly-sys-0.0.8/swiftly_sys.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      540 2023-07-29 19:02:57.000000 swiftly-sys-0.0.8/swiftly_sys.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-29 19:02:57.000000 swiftly-sys-0.0.8/swiftly_sys.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        8 2023-07-29 19:02:57.000000 swiftly-sys-0.0.8/swiftly_sys.egg-info/top_level.txt
```

### Comparing `swiftly-sys-0.0.7/LICENCE` & `swiftly-sys-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `swiftly-sys-0.0.7/PKG-INFO` & `swiftly-sys-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftly-sys
-Version: 0.0.7
+Version: 0.0.8
 Summary: Do what you're good at; writing code. Swiftly handle the rest
 Home-page: https://github.com/brainspoof/swiftly-sys
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 License: Apache2
 Keywords: python project,project management,code management,project building,python project managment,organized project
 License-File: LICENCE
```

### Comparing `swiftly-sys-0.0.7/setup.py` & `swiftly-sys-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import glob
 import os
 
 scripts = [f for f in glob.glob('scripts/unix/**/*', recursive=True) + glob.glob('scripts/windows/**/*', recursive=True) if os.path.isfile(f)]
 
 setup(
     name='swiftly-sys',
-    version='0.0.7',
+    version='0.0.8',
     license='Apache2',
     packages=find_packages(),
     scripts=scripts,
     description = 'Do what you\'re good at; writing code. Swiftly handle the rest',
     long_description='''
     Swiftly let's you focus on building amazing products. Swiftly makes sure your entire code scales, while keeping the code so maintainable. No spaghetti code, ever!\n
     Read the docs at: https://docs.swiftly-sys.tech
```

### Comparing `swiftly-sys-0.0.7/swiftly_sys.egg-info/PKG-INFO` & `swiftly-sys-0.0.8/swiftly_sys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftly-sys
-Version: 0.0.7
+Version: 0.0.8
 Summary: Do what you're good at; writing code. Swiftly handle the rest
 Home-page: https://github.com/brainspoof/swiftly-sys
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 License: Apache2
 Keywords: python project,project management,code management,project building,python project managment,organized project
 License-File: LICENCE
```

### Comparing `swiftly-sys-0.0.7/swiftly_sys.egg-info/SOURCES.txt` & `swiftly-sys-0.0.8/swiftly_sys.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENCE
 setup.py
 scripts/unix
 scripts/windows
 scripts/unix/node
 scripts/unix/python
 scripts/unix/swiftly
-scripts/unix/python/swiftly.python.django.sh
-scripts/unix/python/swiftly.python.sh
+scripts/unix/python/swiftly-python-django.sh
+scripts/unix/python/swiftly-python.sh
 scripts/windows/node
 scripts/windows/python
 scripts/windows/swiftly.bat
 swiftly/__init__.py
 swiftly/core/__init__.py
 swiftly/runtime/__init__.py
 swiftly/runtime/node/__init__.py
```

