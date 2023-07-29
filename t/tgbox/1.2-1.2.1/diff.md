# Comparing `tmp/tgbox-1.2.tar.gz` & `tmp/tgbox-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgbox-1.2.tar", last modified: Mon May 22 20:45:52 2023, max compression
+gzip compressed data, was "tgbox-1.2.1.tar", last modified: Sat Jul 29 07:47:51 2023, max compression
```

## Comparing `tgbox-1.2.tar` & `tgbox-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 20:45:52.798249 tgbox-1.2/
--rw-r--r--   0 non       (1000) non       (1000)       32 2023-05-13 15:05:38.000000 tgbox-1.2/MANIFEST.in
--rw-r--r--   0 non       (1000) non       (1000)     7710 2023-05-22 20:45:52.798249 tgbox-1.2/PKG-INFO
--rw-r--r--   0 non       (1000) non       (1000)     5723 2023-05-13 15:05:38.000000 tgbox-1.2/README.rst
--rw-r--r--   0 non       (1000) non       (1000)       38 2023-05-22 20:45:52.798249 tgbox-1.2/setup.cfg
--rw-r--r--   0 non       (1000) non       (1000)     2134 2023-05-22 20:43:54.000000 tgbox-1.2/setup.py
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 20:45:52.790248 tgbox-1.2/tgbox/
--rw-r--r--   0 non       (1000) non       (1000)     1428 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/__init__.py
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 20:45:52.794248 tgbox-1.2/tgbox/api/
--rw-r--r--   0 non       (1000) non       (1000)       78 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/api/__init__.py
--rw-r--r--   0 non       (1000) non       (1000)     9285 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/api/db.py
--rw-r--r--   0 non       (1000) non       (1000)   104193 2023-05-21 15:40:55.000000 tgbox-1.2/tgbox/api/local.py
--rw-r--r--   0 non       (1000) non       (1000)    79976 2023-05-21 15:43:36.000000 tgbox-1.2/tgbox/api/remote.py
--rw-r--r--   0 non       (1000) non       (1000)    20759 2023-05-14 15:15:11.000000 tgbox-1.2/tgbox/api/utils.py
--rw-r--r--   0 non       (1000) non       (1000)     6266 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/crypto.py
--rw-r--r--   0 non       (1000) non       (1000)     3744 2023-05-21 15:21:29.000000 tgbox-1.2/tgbox/defaults.py
--rw-r--r--   0 non       (1000) non       (1000)     2097 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/errors.py
--rw-r--r--   0 non       (1000) non       (1000)    14575 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/fastelethon.py
--rw-r--r--   0 non       (1000) non       (1000)    19962 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/keys.py
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 20:45:52.794248 tgbox-1.2/tgbox/other/
--rw-r--r--   0 non       (1000) non       (1000)    13796 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/other/tgbox_logo.png
--rw-r--r--   0 non       (1000) non       (1000)    13116 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/other/words.txt
--rw-r--r--   0 non       (1000) non       (1000)    19278 2023-05-22 18:58:07.000000 tgbox-1.2/tgbox/tools.py
--rw-r--r--   0 non       (1000) non       (1000)       16 2023-05-22 19:12:12.000000 tgbox-1.2/tgbox/version.py
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 20:45:52.794248 tgbox-1.2/tgbox.egg-info/
--rw-r--r--   0 non       (1000) non       (1000)     7710 2023-05-22 20:45:52.000000 tgbox-1.2/tgbox.egg-info/PKG-INFO
--rw-r--r--   0 non       (1000) non       (1000)      455 2023-05-22 20:45:52.000000 tgbox-1.2/tgbox.egg-info/SOURCES.txt
--rw-r--r--   0 non       (1000) non       (1000)        1 2023-05-22 20:45:52.000000 tgbox-1.2/tgbox.egg-info/dependency_links.txt
--rw-r--r--   0 non       (1000) non       (1000)      172 2023-05-22 20:45:52.000000 tgbox-1.2/tgbox.egg-info/requires.txt
--rw-r--r--   0 non       (1000) non       (1000)        6 2023-05-22 20:45:52.000000 tgbox-1.2/tgbox.egg-info/top_level.txt
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-07-29 07:47:51.006202 tgbox-1.2.1/
+-rw-r--r--   0 non       (1000) non       (1000)       32 2023-06-06 14:07:12.000000 tgbox-1.2.1/MANIFEST.in
+-rw-r--r--   0 non       (1000) non       (1000)     7714 2023-07-29 07:47:51.006202 tgbox-1.2.1/PKG-INFO
+-rw-r--r--   0 non       (1000) non       (1000)     5723 2023-06-06 14:07:12.000000 tgbox-1.2.1/README.rst
+-rw-r--r--   0 non       (1000) non       (1000)       38 2023-07-29 07:47:51.006202 tgbox-1.2.1/setup.cfg
+-rw-r--r--   0 non       (1000) non       (1000)     2134 2023-07-29 07:27:27.000000 tgbox-1.2.1/setup.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-07-29 07:47:50.982200 tgbox-1.2.1/tgbox/
+-rw-r--r--   0 non       (1000) non       (1000)     1428 2023-06-06 14:07:10.000000 tgbox-1.2.1/tgbox/__init__.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-07-29 07:47:50.998201 tgbox-1.2.1/tgbox/api/
+-rw-r--r--   0 non       (1000) non       (1000)       78 2023-06-06 14:07:11.000000 tgbox-1.2.1/tgbox/api/__init__.py
+-rw-r--r--   0 non       (1000) non       (1000)     9285 2023-07-29 07:26:18.000000 tgbox-1.2.1/tgbox/api/db.py
+-rw-r--r--   0 non       (1000) non       (1000)   104193 2023-07-29 07:26:18.000000 tgbox-1.2.1/tgbox/api/local.py
+-rw-r--r--   0 non       (1000) non       (1000)    79976 2023-07-29 07:26:18.000000 tgbox-1.2.1/tgbox/api/remote.py
+-rw-r--r--   0 non       (1000) non       (1000)    20759 2023-07-29 07:26:18.000000 tgbox-1.2.1/tgbox/api/utils.py
+-rw-r--r--   0 non       (1000) non       (1000)     6266 2023-07-29 07:26:18.000000 tgbox-1.2.1/tgbox/crypto.py
+-rw-r--r--   0 non       (1000) non       (1000)     3744 2023-07-29 07:26:18.000000 tgbox-1.2.1/tgbox/defaults.py
+-rw-r--r--   0 non       (1000) non       (1000)     2097 2023-06-06 14:07:10.000000 tgbox-1.2.1/tgbox/errors.py
+-rw-r--r--   0 non       (1000) non       (1000)    14575 2023-06-06 14:07:10.000000 tgbox-1.2.1/tgbox/fastelethon.py
+-rw-r--r--   0 non       (1000) non       (1000)    19962 2023-07-29 07:26:18.000000 tgbox-1.2.1/tgbox/keys.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-07-29 07:47:51.002202 tgbox-1.2.1/tgbox/other/
+-rw-r--r--   0 non       (1000) non       (1000)    13796 2023-06-06 14:07:10.000000 tgbox-1.2.1/tgbox/other/tgbox_logo.png
+-rw-r--r--   0 non       (1000) non       (1000)    13116 2023-06-06 14:07:10.000000 tgbox-1.2.1/tgbox/other/words.txt
+-rw-r--r--   0 non       (1000) non       (1000)    19278 2023-07-29 07:26:18.000000 tgbox-1.2.1/tgbox/tools.py
+-rw-r--r--   0 non       (1000) non       (1000)       18 2023-07-29 07:37:16.000000 tgbox-1.2.1/tgbox/version.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-07-29 07:47:50.982200 tgbox-1.2.1/tgbox.egg-info/
+-rw-r--r--   0 non       (1000) non       (1000)     7714 2023-07-29 07:47:50.000000 tgbox-1.2.1/tgbox.egg-info/PKG-INFO
+-rw-r--r--   0 non       (1000) non       (1000)      455 2023-07-29 07:47:50.000000 tgbox-1.2.1/tgbox.egg-info/SOURCES.txt
+-rw-r--r--   0 non       (1000) non       (1000)        1 2023-07-29 07:47:50.000000 tgbox-1.2.1/tgbox.egg-info/dependency_links.txt
+-rw-r--r--   0 non       (1000) non       (1000)      172 2023-07-29 07:47:50.000000 tgbox-1.2.1/tgbox.egg-info/requires.txt
+-rw-r--r--   0 non       (1000) non       (1000)        6 2023-07-29 07:47:50.000000 tgbox-1.2.1/tgbox.egg-info/top_level.txt
```

### Comparing `tgbox-1.2/PKG-INFO` & `tgbox-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tgbox
-Version: 1.2
+Version: 1.2.1
 Summary: Encrypted cloud storage API based on a Telegram API
 Home-page: https://github.com/NonProjects/tgbox
 Author: NonProjects
 Author-email: thenonproton@pm.me
 License: LGPL-2.1
-Download-URL: https://github.com/NonProjects/tgbox/archive/refs/tags/v1.2.tar.gz
+Download-URL: https://github.com/NonProjects/tgbox/archive/refs/tags/v1.2.1.tar.gz
 Description: TGBOX: encrypted cloud storage based on Telegram
         ================================================
         .. epigraph::
                 | This repository contains a set of classes and functions used to manage TGBOX.
                 | Try the `tgbox-cli <https://github.com/NotStatilko/tgbox-cli>`__  if you're interested in working implementation!
         
         .. code-block:: python
```

### Comparing `tgbox-1.2/README.rst` & `tgbox-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/setup.py` & `tgbox-1.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     package_data = {
         'tgbox': ['tgbox/other'],
     },
     include_package_data = True,
 
     install_requires = [
         'aiosqlite==0.18.0',
-        'telethon==1.28.2',
+        'telethon==1.29.2',
         'ecdsa==0.18.0',
         'filetype==1.2.0',
         'pysocks==1.7.1'
     ],
     keywords = [
         'Telegram', 'Cloud-Storage', 'Cloud',
         'API', 'Asyncio', 'Non-official'
```

### Comparing `tgbox-1.2/tgbox/__init__.py` & `tgbox-1.2.1/tgbox/__init__.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/api/db.py` & `tgbox-1.2.1/tgbox/api/db.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/api/local.py` & `tgbox-1.2.1/tgbox/api/local.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/api/remote.py` & `tgbox-1.2.1/tgbox/api/remote.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/api/utils.py` & `tgbox-1.2.1/tgbox/api/utils.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/crypto.py` & `tgbox-1.2.1/tgbox/crypto.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/defaults.py` & `tgbox-1.2.1/tgbox/defaults.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/errors.py` & `tgbox-1.2.1/tgbox/errors.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/fastelethon.py` & `tgbox-1.2.1/tgbox/fastelethon.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/keys.py` & `tgbox-1.2.1/tgbox/keys.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/other/tgbox_logo.png` & `tgbox-1.2.1/tgbox/other/tgbox_logo.png`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/other/words.txt` & `tgbox-1.2.1/tgbox/other/words.txt`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox/tools.py` & `tgbox-1.2.1/tgbox/tools.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.2/tgbox.egg-info/PKG-INFO` & `tgbox-1.2.1/tgbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tgbox
-Version: 1.2
+Version: 1.2.1
 Summary: Encrypted cloud storage API based on a Telegram API
 Home-page: https://github.com/NonProjects/tgbox
 Author: NonProjects
 Author-email: thenonproton@pm.me
 License: LGPL-2.1
-Download-URL: https://github.com/NonProjects/tgbox/archive/refs/tags/v1.2.tar.gz
+Download-URL: https://github.com/NonProjects/tgbox/archive/refs/tags/v1.2.1.tar.gz
 Description: TGBOX: encrypted cloud storage based on Telegram
         ================================================
         .. epigraph::
                 | This repository contains a set of classes and functions used to manage TGBOX.
                 | Try the `tgbox-cli <https://github.com/NotStatilko/tgbox-cli>`__  if you're interested in working implementation!
         
         .. code-block:: python
```

