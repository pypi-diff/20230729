# Comparing `tmp/sedi-0.6.tar.gz` & `tmp/sedi-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedi-0.6.tar", last modified: Sat Jul 29 13:26:04 2023, max compression
+gzip compressed data, was "sedi-0.7.tar", last modified: Sat Jul 29 13:40:17 2023, max compression
```

## Comparing `sedi-0.6.tar` & `sedi-0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 13:26:04.960028 sedi-0.6/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2023-07-29 13:26:04.960028 sedi-0.6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6383 2023-07-29 13:25:54.000000 sedi-0.6/provision.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2493 2023-07-29 13:25:54.000000 sedi-0.6/sed.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 13:26:04.960028 sedi-0.6/sedi.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2023-07-29 13:26:04.000000 sedi-0.6/sedi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      171 2023-07-29 13:26:04.000000 sedi-0.6/sedi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-29 13:26:04.000000 sedi-0.6/sedi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2023-07-29 13:26:04.000000 sedi-0.6/sedi.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2023-07-29 13:26:04.000000 sedi-0.6/sedi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-29 13:26:04.960028 sedi-0.6/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2023-07-29 13:25:54.000000 sedi-0.6/setup.py
+drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 13:40:17.897451 sedi-0.7/
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 13:40:17.897451 sedi-0.7/PKG-INFO
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)     6383 2023-07-29 13:12:19.000000 sedi-0.7/provision.py
+-rw-r--r--   0 aleksa    (1000) aleksa    (1000)     2493 2023-07-29 11:36:14.000000 sedi-0.7/sed.py
+drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 13:40:17.897451 sedi-0.7/sedi.egg-info/
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 13:40:17.000000 sedi-0.7/sedi.egg-info/PKG-INFO
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      171 2023-07-29 13:40:17.000000 sedi-0.7/sedi.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)        1 2023-07-29 13:40:17.000000 sedi-0.7/sedi.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       59 2023-07-29 13:40:17.000000 sedi-0.7/sedi.egg-info/entry_points.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       14 2023-07-29 13:40:17.000000 sedi-0.7/sedi.egg-info/top_level.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       38 2023-07-29 13:40:17.897451 sedi-0.7/setup.cfg
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      348 2023-07-29 13:40:16.000000 sedi-0.7/setup.py
```

### Comparing `sedi-0.6/provision.py` & `sedi-0.7/provision.py`

 * *Files identical despite different names*

### Comparing `sedi-0.6/sed.py` & `sedi-0.7/sed.py`

 * *Files identical despite different names*

