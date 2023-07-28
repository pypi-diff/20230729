# Comparing `tmp/ohnlptk-xlang-python-0.0.3.tar.gz` & `tmp/ohnlptk-xlang-python-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohnlptk-xlang-python-0.0.3.tar", last modified: Wed Jul 26 15:20:14 2023, max compression
+gzip compressed data, was "ohnlptk-xlang-python-1.0.0.tar", last modified: Fri Jul 28 22:25:09 2023, max compression
```

## Comparing `ohnlptk-xlang-python-0.0.3.tar` & `ohnlptk-xlang-python-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/ohnlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/ohnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/backbone_module_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 15:20:14.000000 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 15:20:14.000000 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:20:14.000000 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 15:20:14.000000 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 15:20:14.000000 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:25:09.784550 ohnlptk-xlang-python-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 22:25:07.000000 ohnlptk-xlang-python-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-28 22:25:09.784550 ohnlptk-xlang-python-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-28 22:25:07.000000 ohnlptk-xlang-python-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:25:09.780550 ohnlptk-xlang-python-1.0.0/ohnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:25:07.000000 ohnlptk-xlang-python-1.0.0/ohnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:25:09.780550 ohnlptk-xlang-python-1.0.0/ohnlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:25:07.000000 ohnlptk-xlang-python-1.0.0/ohnlp/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:25:09.780550 ohnlptk-xlang-python-1.0.0/ohnlp/toolkit/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:25:07.000000 ohnlptk-xlang-python-1.0.0/ohnlp/toolkit/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-28 22:25:07.000000 ohnlptk-xlang-python-1.0.0/ohnlp/toolkit/backbone/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-28 22:25:07.000000 ohnlptk-xlang-python-1.0.0/ohnlp/toolkit/backbone/backbone_module_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:25:09.784550 ohnlptk-xlang-python-1.0.0/ohnlptk_xlang_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-28 22:25:09.000000 ohnlptk-xlang-python-1.0.0/ohnlptk_xlang_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-28 22:25:09.000000 ohnlptk-xlang-python-1.0.0/ohnlptk_xlang_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:25:09.000000 ohnlptk-xlang-python-1.0.0/ohnlptk_xlang_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 22:25:09.000000 ohnlptk-xlang-python-1.0.0/ohnlptk_xlang_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 22:25:09.000000 ohnlptk-xlang-python-1.0.0/ohnlptk_xlang_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:25:09.784550 ohnlptk-xlang-python-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-28 22:25:07.000000 ohnlptk-xlang-python-1.0.0/setup.py
```

### Comparing `ohnlptk-xlang-python-0.0.3/LICENSE` & `ohnlptk-xlang-python-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ohnlptk-xlang-python-0.0.3/README.md` & `ohnlptk-xlang-python-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/api.py` & `ohnlptk-xlang-python-1.0.0/ohnlp/toolkit/backbone/api.py`

 * *Files identical despite different names*

### Comparing `ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/backbone_module_launcher.py` & `ohnlptk-xlang-python-1.0.0/ohnlp/toolkit/backbone/backbone_module_launcher.py`

 * *Files identical despite different names*

