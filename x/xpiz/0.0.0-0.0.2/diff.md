# Comparing `tmp/xpiz-0.0.0.tar.gz` & `tmp/xpiz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpiz-0.0.0.tar", last modified: Fri Jul 28 17:04:22 2023, max compression
+gzip compressed data, was "xpiz-0.0.2.tar", last modified: Fri Jul 28 22:21:21 2023, max compression
```

## Comparing `xpiz-0.0.0.tar` & `xpiz-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:04:22.081842 xpiz-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 17:04:11.000000 xpiz-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-28 17:04:22.081842 xpiz-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 17:04:11.000000 xpiz-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:04:22.081842 xpiz-0.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3380 2023-07-28 17:04:11.000000 xpiz-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:04:22.081842 xpiz-0.0.0/xpiz/
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-28 17:04:11.000000 xpiz-0.0.0/xpiz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:04:22.081842 xpiz-0.0.0/xpiz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-28 17:04:22.000000 xpiz-0.0.0/xpiz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 17:04:22.000000 xpiz-0.0.0/xpiz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:04:22.000000 xpiz-0.0.0/xpiz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 17:04:22.000000 xpiz-0.0.0/xpiz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 17:04:22.000000 xpiz-0.0.0/xpiz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:21:21.976628 xpiz-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 22:21:09.000000 xpiz-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-28 22:21:21.976628 xpiz-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 22:21:09.000000 xpiz-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:21:21.976628 xpiz-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3380 2023-07-28 22:21:09.000000 xpiz-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:21:21.976628 xpiz-0.0.2/xpiz/
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-28 22:21:09.000000 xpiz-0.0.2/xpiz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:21:21.976628 xpiz-0.0.2/xpiz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-28 22:21:21.000000 xpiz-0.0.2/xpiz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 22:21:21.000000 xpiz-0.0.2/xpiz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:21:21.000000 xpiz-0.0.2/xpiz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 22:21:21.000000 xpiz-0.0.2/xpiz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 22:21:21.000000 xpiz-0.0.2/xpiz.egg-info/top_level.txt
```

### Comparing `xpiz-0.0.0/LICENSE` & `xpiz-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xpiz-0.0.0/setup.py` & `xpiz-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.0"
+VERSION = "0.0.2"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

### Comparing `xpiz-0.0.0/xpiz/__init__.py` & `xpiz-0.0.2/xpiz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os, sys, hashlib, zipfile, json, shutil
+from glob import glob as re
 
 """
 file=
 hash=$(file).sums
 default:: build
 size=2G
 build: hash split
```

