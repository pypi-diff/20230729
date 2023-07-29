# Comparing `tmp/CipherProgram-0.0.2.tar.gz` & `tmp/CipherProgram-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CipherProgram-0.0.2.tar", last modified: Fri Jul 28 20:57:24 2023, max compression
+gzip compressed data, was "CipherProgram-0.0.3.tar", last modified: Sat Jul 29 11:17:33 2023, max compression
```

## Comparing `CipherProgram-0.0.2.tar` & `CipherProgram-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-28 20:57:24.466413 CipherProgram-0.0.2/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-28 20:57:24.466413 CipherProgram-0.0.2/Cipher/
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-07-28 20:46:04.000000 CipherProgram-0.0.2/Cipher/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      627 2023-07-28 20:56:20.000000 CipherProgram-0.0.2/Cipher/main.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-28 20:57:24.466413 CipherProgram-0.0.2/CipherProgram.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)      482 2023-07-28 20:57:24.000000 CipherProgram-0.0.2/CipherProgram.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      208 2023-07-28 20:57:24.000000 CipherProgram-0.0.2/CipherProgram.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-07-28 20:57:24.000000 CipherProgram-0.0.2/CipherProgram.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        7 2023-07-28 20:57:24.000000 CipherProgram-0.0.2/CipherProgram.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1363 2023-07-28 20:08:20.000000 CipherProgram-0.0.2/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)      482 2023-07-28 20:57:24.466413 CipherProgram-0.0.2/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)       95 2023-07-28 20:43:44.000000 CipherProgram-0.0.2/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-07-28 20:57:24.466413 CipherProgram-0.0.2/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1256 2023-07-28 20:56:26.000000 CipherProgram-0.0.2/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-29 11:17:33.707654 CipherProgram-0.0.3/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-29 11:17:33.703657 CipherProgram-0.0.3/Cipher/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-07-28 20:46:04.000000 CipherProgram-0.0.3/Cipher/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      627 2023-07-28 20:56:20.000000 CipherProgram-0.0.3/Cipher/main.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-29 11:17:33.707654 CipherProgram-0.0.3/CipherProgram.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      815 2023-07-29 11:17:33.000000 CipherProgram-0.0.3/CipherProgram.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      208 2023-07-29 11:17:33.000000 CipherProgram-0.0.3/CipherProgram.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-07-29 11:17:33.000000 CipherProgram-0.0.3/CipherProgram.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        7 2023-07-29 11:17:33.000000 CipherProgram-0.0.3/CipherProgram.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1363 2023-07-28 20:08:20.000000 CipherProgram-0.0.3/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      815 2023-07-29 11:17:33.707654 CipherProgram-0.0.3/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      428 2023-07-28 21:07:49.000000 CipherProgram-0.0.3/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-07-29 11:17:33.707654 CipherProgram-0.0.3/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1256 2023-07-29 11:17:30.000000 CipherProgram-0.0.3/setup.py
```

### Comparing `CipherProgram-0.0.2/Cipher/main.py` & `CipherProgram-0.0.3/Cipher/main.py`

 * *Files identical despite different names*

### Comparing `CipherProgram-0.0.2/LICENSE` & `CipherProgram-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CipherProgram-0.0.2/setup.py` & `CipherProgram-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="CipherProgram",
 
     # version of the module
-    version="0.0.2",
+    version="0.0.3",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Cipher.git',
 
     # your Email address
```

