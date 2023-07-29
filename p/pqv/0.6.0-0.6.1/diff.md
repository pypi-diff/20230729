# Comparing `tmp/pqv-0.6.0.tar.gz` & `tmp/pqv-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqv-0.6.0.tar", last modified: Sun Jun 25 21:21:43 2023, max compression
+gzip compressed data, was "pqv-0.6.1.tar", last modified: Sat Jul 29 09:11:40 2023, max compression
```

## Comparing `pqv-0.6.0.tar` & `pqv-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-06-25 21:21:43.804197 pqv-0.6.0/
--rw-r--r--   0 pieter     (501) staff       (20)     1066 2023-02-26 14:17:55.000000 pqv-0.6.0/LICENSE
--rw-r--r--   0 pieter     (501) staff       (20)      225 2023-06-25 21:21:43.803843 pqv-0.6.0/PKG-INFO
--rw-r--r--   0 pieter     (501) staff       (20)      102 2023-02-26 14:42:52.000000 pqv-0.6.0/README.md
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-06-25 21:21:43.801649 pqv-0.6.0/pqv/
--rw-r--r--   0 pieter     (501) staff       (20)        0 2023-02-26 14:09:31.000000 pqv-0.6.0/pqv/__init__.py
--rw-r--r--   0 pieter     (501) staff       (20)     5243 2023-06-25 21:19:56.000000 pqv-0.6.0/pqv/__main__.py
--rw-r--r--   0 pieter     (501) staff       (20)      165 2023-02-26 11:16:27.000000 pqv-0.6.0/pqv/style.css
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-06-25 21:21:43.803562 pqv-0.6.0/pqv.egg-info/
--rw-r--r--   0 pieter     (501) staff       (20)      225 2023-06-25 21:21:43.000000 pqv-0.6.0/pqv.egg-info/PKG-INFO
--rw-r--r--   0 pieter     (501) staff       (20)      236 2023-06-25 21:21:43.000000 pqv-0.6.0/pqv.egg-info/SOURCES.txt
--rw-r--r--   0 pieter     (501) staff       (20)        1 2023-06-25 21:21:43.000000 pqv-0.6.0/pqv.egg-info/dependency_links.txt
--rw-r--r--   0 pieter     (501) staff       (20)       42 2023-06-25 21:21:43.000000 pqv-0.6.0/pqv.egg-info/entry_points.txt
--rw-r--r--   0 pieter     (501) staff       (20)        1 2023-02-26 14:19:07.000000 pqv-0.6.0/pqv.egg-info/not-zip-safe
--rw-r--r--   0 pieter     (501) staff       (20)        4 2023-06-25 21:21:43.000000 pqv-0.6.0/pqv.egg-info/top_level.txt
--rw-r--r--   0 pieter     (501) staff       (20)       38 2023-06-25 21:21:43.804284 pqv-0.6.0/setup.cfg
--rw-r--r--   0 pieter     (501) staff       (20)      529 2023-06-25 21:20:39.000000 pqv-0.6.0/setup.py
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-07-29 09:11:40.746393 pqv-0.6.1/
+-rw-r--r--   0 pieter     (501) staff       (20)     1066 2023-02-26 14:17:55.000000 pqv-0.6.1/LICENSE
+-rw-r--r--   0 pieter     (501) staff       (20)      225 2023-07-29 09:11:40.746223 pqv-0.6.1/PKG-INFO
+-rw-r--r--   0 pieter     (501) staff       (20)      102 2023-02-26 14:42:52.000000 pqv-0.6.1/README.md
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-07-29 09:11:40.744315 pqv-0.6.1/pqv/
+-rw-r--r--   0 pieter     (501) staff       (20)        0 2023-02-26 14:09:31.000000 pqv-0.6.1/pqv/__init__.py
+-rw-r--r--   0 pieter     (501) staff       (20)     5243 2023-07-29 09:11:22.000000 pqv-0.6.1/pqv/__main__.py
+-rw-r--r--   0 pieter     (501) staff       (20)      165 2023-02-26 11:16:27.000000 pqv-0.6.1/pqv/style.css
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-07-29 09:11:40.745975 pqv-0.6.1/pqv.egg-info/
+-rw-r--r--   0 pieter     (501) staff       (20)      225 2023-07-29 09:11:40.000000 pqv-0.6.1/pqv.egg-info/PKG-INFO
+-rw-r--r--   0 pieter     (501) staff       (20)      262 2023-07-29 09:11:40.000000 pqv-0.6.1/pqv.egg-info/SOURCES.txt
+-rw-r--r--   0 pieter     (501) staff       (20)        1 2023-07-29 09:11:40.000000 pqv-0.6.1/pqv.egg-info/dependency_links.txt
+-rw-r--r--   0 pieter     (501) staff       (20)       42 2023-07-29 09:11:40.000000 pqv-0.6.1/pqv.egg-info/entry_points.txt
+-rw-r--r--   0 pieter     (501) staff       (20)        1 2023-02-26 14:19:07.000000 pqv-0.6.1/pqv.egg-info/not-zip-safe
+-rw-r--r--   0 pieter     (501) staff       (20)       26 2023-07-29 09:11:40.000000 pqv-0.6.1/pqv.egg-info/requires.txt
+-rw-r--r--   0 pieter     (501) staff       (20)        4 2023-07-29 09:11:40.000000 pqv-0.6.1/pqv.egg-info/top_level.txt
+-rw-r--r--   0 pieter     (501) staff       (20)       38 2023-07-29 09:11:40.746575 pqv-0.6.1/setup.cfg
+-rw-r--r--   0 pieter     (501) staff       (20)      616 2023-07-29 08:37:45.000000 pqv-0.6.1/setup.py
```

### Comparing `pqv-0.6.0/LICENSE` & `pqv-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pqv-0.6.0/pqv/__main__.py` & `pqv-0.6.1/pqv/__main__.py`

 * *Files identical despite different names*

