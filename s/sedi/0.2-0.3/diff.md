# Comparing `tmp/sedi-0.2.tar.gz` & `tmp/sedi-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedi-0.2.tar", last modified: Sat Jul 29 11:22:03 2023, max compression
+gzip compressed data, was "sedi-0.3.tar", last modified: Sat Jul 29 11:35:35 2023, max compression
```

## Comparing `sedi-0.2.tar` & `sedi-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 11:22:03.931608 sedi-0.2/
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 11:22:03.931608 sedi-0.2/PKG-INFO
--rw-r--r--   0 aleksa    (1000) aleksa    (1000)     2478 2023-07-29 11:20:23.000000 sedi-0.2/sed.py
-drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 11:22:03.931608 sedi-0.2/sedi.egg-info/
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 11:22:03.000000 sedi-0.2/sedi.egg-info/PKG-INFO
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      158 2023-07-29 11:22:03.000000 sedi-0.2/sedi.egg-info/SOURCES.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)        1 2023-07-29 11:22:03.000000 sedi-0.2/sedi.egg-info/dependency_links.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       53 2023-07-29 11:22:03.000000 sedi-0.2/sedi.egg-info/entry_points.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)        4 2023-07-29 11:22:03.000000 sedi-0.2/sedi.egg-info/top_level.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       38 2023-07-29 11:22:03.931608 sedi-0.2/setup.cfg
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      329 2023-07-29 11:21:23.000000 sedi-0.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 11:35:35.406573 sedi-0.3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2023-07-29 11:35:35.406573 sedi-0.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2478 2023-07-29 11:35:26.000000 sedi-0.3/sed.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 11:35:35.406573 sedi-0.3/sedi.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2023-07-29 11:35:35.000000 sedi-0.3/sedi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      158 2023-07-29 11:35:35.000000 sedi-0.3/sedi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-29 11:35:35.000000 sedi-0.3/sedi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-07-29 11:35:35.000000 sedi-0.3/sedi.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-07-29 11:35:35.000000 sedi-0.3/sedi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-29 11:35:35.406573 sedi-0.3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2023-07-29 11:35:26.000000 sedi-0.3/setup.py
```

### Comparing `sedi-0.2/sed.py` & `sedi-0.3/sed.py`

 * *Files identical despite different names*

