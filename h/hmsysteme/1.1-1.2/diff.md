# Comparing `tmp/hmsysteme-1.1.tar.gz` & `tmp/hmsysteme-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmsysteme-1.1.tar", last modified: Sat Jul 29 15:15:28 2023, max compression
+gzip compressed data, was "hmsysteme-1.2.tar", last modified: Sat Jul 29 15:56:02 2023, max compression
```

## Comparing `hmsysteme-1.1.tar` & `hmsysteme-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 stan      (1000) stan      (1001)        0 2023-07-29 15:15:28.851346 hmsysteme-1.1/
--rw-r--r--   0 stan      (1000) stan      (1001)      256 2023-07-29 15:15:28.851346 hmsysteme-1.1/PKG-INFO
--rw-r--r--   0 stan      (1000) stan      (1001)        6 2020-10-10 10:35:32.000000 hmsysteme-1.1/README.md
-drwxr-xr-x   0 stan      (1000) stan      (1001)        0 2023-07-29 15:15:28.851346 hmsysteme-1.1/hmsysteme/
--rw-r--r--   0 stan      (1000) stan      (1001)       25 2020-10-10 13:26:28.000000 hmsysteme-1.1/hmsysteme/__init__.py
--rw-r--r--   0 stan      (1000) stan      (1001)     5439 2023-07-29 15:04:32.000000 hmsysteme-1.1/hmsysteme/functions.py
-drwxr-xr-x   0 stan      (1000) stan      (1001)        0 2023-07-29 15:15:28.851346 hmsysteme-1.1/hmsysteme.egg-info/
--rw-r--r--   0 stan      (1000) stan      (1001)      256 2023-07-29 15:15:28.000000 hmsysteme-1.1/hmsysteme.egg-info/PKG-INFO
--rw-r--r--   0 stan      (1000) stan      (1001)      269 2023-07-29 15:15:28.000000 hmsysteme-1.1/hmsysteme.egg-info/SOURCES.txt
--rw-r--r--   0 stan      (1000) stan      (1001)        1 2023-07-29 15:15:28.000000 hmsysteme-1.1/hmsysteme.egg-info/dependency_links.txt
--rw-r--r--   0 stan      (1000) stan      (1001)        1 2020-10-10 11:17:30.000000 hmsysteme-1.1/hmsysteme.egg-info/not-zip-safe
--rw-r--r--   0 stan      (1000) stan      (1001)       39 2023-07-29 15:15:28.000000 hmsysteme-1.1/hmsysteme.egg-info/requires.txt
--rw-r--r--   0 stan      (1000) stan      (1001)       10 2023-07-29 15:15:28.000000 hmsysteme-1.1/hmsysteme.egg-info/top_level.txt
--rw-r--r--   0 stan      (1000) stan      (1001)       79 2023-07-29 15:15:28.851346 hmsysteme-1.1/setup.cfg
--rw-r--r--   0 stan      (1000) stan      (1001)      399 2023-07-29 15:09:41.000000 hmsysteme-1.1/setup.py
+drwxr-xr-x   0 stan      (1000) stan      (1001)        0 2023-07-29 15:56:02.829958 hmsysteme-1.2/
+-rw-r--r--   0 stan      (1000) stan      (1001)      256 2023-07-29 15:56:02.829958 hmsysteme-1.2/PKG-INFO
+-rw-r--r--   0 stan      (1000) stan      (1001)        6 2020-10-10 10:35:32.000000 hmsysteme-1.2/README.md
+drwxr-xr-x   0 stan      (1000) stan      (1001)        0 2023-07-29 15:56:02.829958 hmsysteme-1.2/hmsysteme/
+-rw-r--r--   0 stan      (1000) stan      (1001)       25 2020-10-10 13:26:28.000000 hmsysteme-1.2/hmsysteme/__init__.py
+-rw-r--r--   0 stan      (1000) stan      (1001)     5439 2023-07-29 15:04:32.000000 hmsysteme-1.2/hmsysteme/functions.py
+drwxr-xr-x   0 stan      (1000) stan      (1001)        0 2023-07-29 15:56:02.829958 hmsysteme-1.2/hmsysteme.egg-info/
+-rw-r--r--   0 stan      (1000) stan      (1001)      256 2023-07-29 15:56:02.000000 hmsysteme-1.2/hmsysteme.egg-info/PKG-INFO
+-rw-r--r--   0 stan      (1000) stan      (1001)      269 2023-07-29 15:56:02.000000 hmsysteme-1.2/hmsysteme.egg-info/SOURCES.txt
+-rw-r--r--   0 stan      (1000) stan      (1001)        1 2023-07-29 15:56:02.000000 hmsysteme-1.2/hmsysteme.egg-info/dependency_links.txt
+-rw-r--r--   0 stan      (1000) stan      (1001)        1 2020-10-10 11:17:30.000000 hmsysteme-1.2/hmsysteme.egg-info/not-zip-safe
+-rw-r--r--   0 stan      (1000) stan      (1001)       39 2023-07-29 15:56:02.000000 hmsysteme-1.2/hmsysteme.egg-info/requires.txt
+-rw-r--r--   0 stan      (1000) stan      (1001)       10 2023-07-29 15:56:02.000000 hmsysteme-1.2/hmsysteme.egg-info/top_level.txt
+-rw-r--r--   0 stan      (1000) stan      (1001)       79 2023-07-29 15:56:02.829958 hmsysteme-1.2/setup.cfg
+-rw-r--r--   0 stan      (1000) stan      (1001)      399 2023-07-29 15:55:38.000000 hmsysteme-1.2/setup.py
```

### Comparing `hmsysteme-1.1/hmsysteme/functions.py` & `hmsysteme-1.2/hmsysteme/functions.py`

 * *Files identical despite different names*

