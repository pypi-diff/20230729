# Comparing `tmp/pymkpsxiso-0.1.3.tar.gz` & `tmp/pymkpsxiso-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymkpsxiso-0.1.3.tar", last modified: Sat Apr 29 05:12:10 2023, max compression
+gzip compressed data, was "pymkpsxiso-0.1.4.tar", last modified: Sat Jul 29 17:51:26 2023, max compression
```

## Comparing `pymkpsxiso-0.1.3.tar` & `pymkpsxiso-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.081299 pymkpsxiso-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-29 05:11:47.000000 pymkpsxiso-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-29 05:11:47.000000 pymkpsxiso-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-29 05:12:10.081299 pymkpsxiso-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-29 05:11:47.000000 pymkpsxiso-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.065299 pymkpsxiso-0.1.3/mkpsxiso/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.069299 pymkpsxiso-0.1.3/mkpsxiso/ThreadPool/
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-29 05:11:52.000000 pymkpsxiso-0.1.3/mkpsxiso/ThreadPool/ThreadPool.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.069299 pymkpsxiso-0.1.3/mkpsxiso/miniaudio/
--rw-r--r--   0 runner    (1001) docker     (123)  3083782 2023-04-29 05:11:57.000000 pymkpsxiso-0.1.3/mkpsxiso/miniaudio/miniaudio.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.065299 pymkpsxiso-0.1.3/mkpsxiso/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.073299 pymkpsxiso-0.1.3/mkpsxiso/src/dumpsxiso/
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/dumpsxiso/cdreader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/dumpsxiso/cdreader.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.077299 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/cdwriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/cdwriter.h
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/edcecc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/edcecc.h
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/global.h
--rw-r--r--   0 runner    (1001) docker     (123)    29623 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/iso.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/iso.h
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/miniaudio_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/miniaudio_pcm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.077299 pymkpsxiso-0.1.3/mkpsxiso/src/shared/
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/cd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/common.h
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/fs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/fs.h
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/listview.h
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/mmappedfile.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/mmappedfile.h
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/platform.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/platform.h
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/xa.h
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-29 05:11:48.000000 pymkpsxiso-0.1.3/mkpsxiso/src/shared/xml.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.077299 pymkpsxiso-0.1.3/mkpsxiso/tinyxml2/
--rwxr-xr-x   0 runner    (1001) docker     (123)    77745 2023-04-29 05:11:58.000000 pymkpsxiso-0.1.3/mkpsxiso/tinyxml2/tinyxml2.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    73727 2023-04-29 05:11:58.000000 pymkpsxiso-0.1.3/mkpsxiso/tinyxml2/tinyxml2.h
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-29 05:11:47.000000 pymkpsxiso-0.1.3/pymkpsxiso.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:12:10.081299 pymkpsxiso-0.1.3/pymkpsxiso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-29 05:12:10.000000 pymkpsxiso-0.1.3/pymkpsxiso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-29 05:12:10.000000 pymkpsxiso-0.1.3/pymkpsxiso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 05:12:10.000000 pymkpsxiso-0.1.3/pymkpsxiso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 05:12:10.000000 pymkpsxiso-0.1.3/pymkpsxiso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 05:12:10.081299 pymkpsxiso-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-29 05:11:47.000000 pymkpsxiso-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:26.954895 pymkpsxiso-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 17:51:04.000000 pymkpsxiso-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-29 17:51:04.000000 pymkpsxiso-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-29 17:51:26.954895 pymkpsxiso-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-29 17:51:04.000000 pymkpsxiso-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:26.942895 pymkpsxiso-0.1.4/mkpsxiso/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:26.942895 pymkpsxiso-0.1.4/mkpsxiso/ThreadPool/
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-29 17:51:09.000000 pymkpsxiso-0.1.4/mkpsxiso/ThreadPool/ThreadPool.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:26.942895 pymkpsxiso-0.1.4/mkpsxiso/miniaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)  3083782 2023-07-29 17:51:14.000000 pymkpsxiso-0.1.4/mkpsxiso/miniaudio/miniaudio.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:26.942895 pymkpsxiso-0.1.4/mkpsxiso/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:26.946895 pymkpsxiso-0.1.4/mkpsxiso/src/dumpsxiso/
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/dumpsxiso/cdreader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/dumpsxiso/cdreader.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:26.950894 pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/cdwriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/cdwriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/edcecc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/edcecc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/global.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29623 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/iso.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/iso.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/miniaudio_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/miniaudio_pcm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:26.950894 pymkpsxiso-0.1.4/mkpsxiso/src/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/cd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/fs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/fs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/listview.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/mmappedfile.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/mmappedfile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/platform.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/platform.h
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/xa.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-29 17:51:05.000000 pymkpsxiso-0.1.4/mkpsxiso/src/shared/xml.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:26.950894 pymkpsxiso-0.1.4/mkpsxiso/tinyxml2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77745 2023-07-29 17:51:15.000000 pymkpsxiso-0.1.4/mkpsxiso/tinyxml2/tinyxml2.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    73727 2023-07-29 17:51:15.000000 pymkpsxiso-0.1.4/mkpsxiso/tinyxml2/tinyxml2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-29 17:51:04.000000 pymkpsxiso-0.1.4/pymkpsxiso.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:26.954895 pymkpsxiso-0.1.4/pymkpsxiso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-29 17:51:26.000000 pymkpsxiso-0.1.4/pymkpsxiso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-29 17:51:26.000000 pymkpsxiso-0.1.4/pymkpsxiso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:51:26.000000 pymkpsxiso-0.1.4/pymkpsxiso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 17:51:26.000000 pymkpsxiso-0.1.4/pymkpsxiso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 17:51:26.954895 pymkpsxiso-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-29 17:51:04.000000 pymkpsxiso-0.1.4/setup.py
```

### Comparing `pymkpsxiso-0.1.3/LICENSE` & `pymkpsxiso-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/PKG-INFO` & `pymkpsxiso-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymkpsxiso
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python interface for mkpsxiso.
 Home-page: https://github.com/Illidanz/pymkpsxiso
 Author: Illidan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/ThreadPool/ThreadPool.h` & `pymkpsxiso-0.1.4/mkpsxiso/ThreadPool/ThreadPool.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/miniaudio/miniaudio.h` & `pymkpsxiso-0.1.4/mkpsxiso/miniaudio/miniaudio.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/dumpsxiso/cdreader.cpp` & `pymkpsxiso-0.1.4/mkpsxiso/src/dumpsxiso/cdreader.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/dumpsxiso/cdreader.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/dumpsxiso/cdreader.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/cdwriter.cpp` & `pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/cdwriter.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/cdwriter.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/cdwriter.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/edcecc.cpp` & `pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/edcecc.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/edcecc.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/edcecc.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/iso.cpp` & `pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/iso.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/iso.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/iso.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/miniaudio_helpers.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/miniaudio_helpers.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/mkpsxiso/miniaudio_pcm.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/mkpsxiso/miniaudio_pcm.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/cd.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/cd.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/common.cpp` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/common.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/common.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/common.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/fs.cpp` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/fs.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/fs.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/fs.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/listview.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/listview.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/mmappedfile.cpp` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/mmappedfile.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/mmappedfile.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/mmappedfile.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/platform.cpp` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/platform.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/platform.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/platform.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/xa.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/xa.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/src/shared/xml.h` & `pymkpsxiso-0.1.4/mkpsxiso/src/shared/xml.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/tinyxml2/tinyxml2.cpp` & `pymkpsxiso-0.1.4/mkpsxiso/tinyxml2/tinyxml2.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/mkpsxiso/tinyxml2/tinyxml2.h` & `pymkpsxiso-0.1.4/mkpsxiso/tinyxml2/tinyxml2.h`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/pymkpsxiso.cpp` & `pymkpsxiso-0.1.4/pymkpsxiso.cpp`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/pymkpsxiso.egg-info/PKG-INFO` & `pymkpsxiso-0.1.4/pymkpsxiso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymkpsxiso
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python interface for mkpsxiso.
 Home-page: https://github.com/Illidanz/pymkpsxiso
 Author: Illidan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pymkpsxiso-0.1.3/pymkpsxiso.egg-info/SOURCES.txt` & `pymkpsxiso-0.1.4/pymkpsxiso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymkpsxiso-0.1.3/setup.py` & `pymkpsxiso-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 for dir in INCLUDES:
     for file in os.listdir(dir):
         if file.endswith(".cpp") and "xmltest" not in file and "example" not in file and "main.cpp" not in file:
             sources.append(dir + "/" + file)
 
 def main():
     setup(name="pymkpsxiso",
-          version="0.1.3",
+          version="0.1.4",
           author="Illidan",
           description="Python interface for mkpsxiso.",
           long_description=long_description,
           long_description_content_type="text/markdown",
           url="https://github.com/Illidanz/pymkpsxiso",
           classifiers=[
               "Programming Language :: Python :: 3",
```

