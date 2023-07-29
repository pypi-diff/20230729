# Comparing `tmp/swiftly-sys-0.0.1.tar.gz` & `tmp/swiftly-sys-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-sys-0.0.1.tar", last modified: Sat Jul 29 12:29:18 2023, max compression
+gzip compressed data, was "swiftly-sys-0.0.2.tar", last modified: Sat Jul 29 15:52:49 2023, max compression
```

## Comparing `swiftly-sys-0.0.1.tar` & `swiftly-sys-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:29:18.339985 swiftly-sys-0.0.1/
--rw-r--r--   0 brainspoof   (501) staff       (20)    11357 2023-07-29 09:32:23.000000 swiftly-sys-0.0.1/LICENCE
--rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 12:29:18.339854 swiftly-sys-0.0.1/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:29:18.338621 swiftly-sys-0.0.1/scripts/
--rw-r--r--   0 brainspoof   (501) staff       (20)      760 2023-07-29 12:26:12.000000 swiftly-sys-0.0.1/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 12:29:18.340033 swiftly-sys-0.0.1/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      822 2023-07-29 12:05:55.000000 swiftly-sys-0.0.1/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:29:18.338869 swiftly-sys-0.0.1/swiftly/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:12:56.000000 swiftly-sys-0.0.1/swiftly/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:29:18.338958 swiftly-sys-0.0.1/swiftly/core/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:09.000000 swiftly-sys-0.0.1/swiftly/core/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:29:18.339045 swiftly-sys-0.0.1/swiftly/runtime/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:17.000000 swiftly-sys-0.0.1/swiftly/runtime/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:29:18.339132 swiftly-sys-0.0.1/swiftly/runtime/node/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:19.000000 swiftly-sys-0.0.1/swiftly/runtime/node/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:29:18.339220 swiftly-sys-0.0.1/swiftly/runtime/python/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:23.000000 swiftly-sys-0.0.1/swiftly/runtime/python/__init__.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:29:18.339664 swiftly-sys-0.0.1/swiftly_sys.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 12:29:18.000000 swiftly-sys-0.0.1/swiftly_sys.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      313 2023-07-29 12:29:18.000000 swiftly-sys-0.0.1/swiftly_sys.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-29 12:29:18.000000 swiftly-sys-0.0.1/swiftly_sys.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        8 2023-07-29 12:29:18.000000 swiftly-sys-0.0.1/swiftly_sys.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 15:52:49.839194 swiftly-sys-0.0.2/
+-rw-r--r--   0 brainspoof   (501) staff       (20)    11357 2023-07-29 09:32:23.000000 swiftly-sys-0.0.2/LICENCE
+-rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 15:52:49.839068 swiftly-sys-0.0.2/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 15:52:49.837968 swiftly-sys-0.0.2/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)      760 2023-07-29 12:26:12.000000 swiftly-sys-0.0.2/scripts/swiftly
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:06:56.000000 swiftly-sys-0.0.2/scripts/swiftly.bat
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-29 15:52:49.839245 swiftly-sys-0.0.2/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      845 2023-07-29 15:51:02.000000 swiftly-sys-0.0.2/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 15:52:49.838059 swiftly-sys-0.0.2/swiftly/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:12:56.000000 swiftly-sys-0.0.2/swiftly/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 15:52:49.838153 swiftly-sys-0.0.2/swiftly/core/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:09.000000 swiftly-sys-0.0.2/swiftly/core/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 15:52:49.838240 swiftly-sys-0.0.2/swiftly/runtime/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:17.000000 swiftly-sys-0.0.2/swiftly/runtime/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 15:52:49.838327 swiftly-sys-0.0.2/swiftly/runtime/node/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:19.000000 swiftly-sys-0.0.2/swiftly/runtime/node/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 15:52:49.838427 swiftly-sys-0.0.2/swiftly/runtime/python/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-29 12:13:23.000000 swiftly-sys-0.0.2/swiftly/runtime/python/__init__.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-29 15:52:49.838882 swiftly-sys-0.0.2/swiftly_sys.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)      623 2023-07-29 15:52:49.000000 swiftly-sys-0.0.2/swiftly_sys.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      333 2023-07-29 15:52:49.000000 swiftly-sys-0.0.2/swiftly_sys.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-29 15:52:49.000000 swiftly-sys-0.0.2/swiftly_sys.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        8 2023-07-29 15:52:49.000000 swiftly-sys-0.0.2/swiftly_sys.egg-info/top_level.txt
```

### Comparing `swiftly-sys-0.0.1/LICENCE` & `swiftly-sys-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `swiftly-sys-0.0.1/PKG-INFO` & `swiftly-sys-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftly-sys
-Version: 0.0.1
+Version: 0.0.2
 Summary: Do what you're good at; writing code. Swiftly handle the rest
 Home-page: https://github.com/brainspoof/swiftly-sys
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 License: Apache2
 Keywords: python project,project management,code management,project building,python project managment,organized project
 License-File: LICENCE
```

### Comparing `swiftly-sys-0.0.1/scripts/swiftly` & `swiftly-sys-0.0.2/scripts/swiftly`

 * *Files identical despite different names*

### Comparing `swiftly-sys-0.0.1/setup.py` & `swiftly-sys-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='swiftly-sys',
-    version='0.0.1',
+    version='0.0.2',
     license='Apache2',
     packages=find_packages(),
-    scripts=['scripts/swiftly'],
+    scripts=['scripts/swiftly', 'scripts/swiftly.bat'],
     description = 'Do what you\'re good at; writing code. Swiftly handle the rest',
     long_description='''
     Swiftly let's you focus on building amazing products. Swiftly makes sure your entire code scales, while keeping the code so maintainable. No spaghetti code, ever!\n
     Read the docs at: https://docs.swiftly-sys.tech
     ''',
     author = 'Shubham Gupta',
     author_email = 'shubhastro2@gmail.com',
```

### Comparing `swiftly-sys-0.0.1/swiftly_sys.egg-info/PKG-INFO` & `swiftly-sys-0.0.2/swiftly_sys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftly-sys
-Version: 0.0.1
+Version: 0.0.2
 Summary: Do what you're good at; writing code. Swiftly handle the rest
 Home-page: https://github.com/brainspoof/swiftly-sys
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 License: Apache2
 Keywords: python project,project management,code management,project building,python project managment,organized project
 License-File: LICENCE
```

