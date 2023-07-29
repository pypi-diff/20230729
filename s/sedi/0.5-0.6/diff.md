# Comparing `tmp/sedi-0.5.tar.gz` & `tmp/sedi-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedi-0.5.tar", last modified: Sat Jul 29 13:15:11 2023, max compression
+gzip compressed data, was "sedi-0.6.tar", last modified: Sat Jul 29 13:26:04 2023, max compression
```

## Comparing `sedi-0.5.tar` & `sedi-0.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 13:15:11.868432 sedi-0.5/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2023-07-29 13:15:11.868432 sedi-0.5/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6383 2023-07-29 13:15:03.000000 sedi-0.5/provision.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 13:15:11.868432 sedi-0.5/sedi.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2023-07-29 13:15:11.000000 sedi-0.5/sedi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      164 2023-07-29 13:15:11.000000 sedi-0.5/sedi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-29 13:15:11.000000 sedi-0.5/sedi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2023-07-29 13:15:11.000000 sedi-0.5/sedi.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-07-29 13:15:11.000000 sedi-0.5/sedi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-29 13:15:11.868432 sedi-0.5/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      341 2023-07-29 13:15:03.000000 sedi-0.5/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 13:26:04.960028 sedi-0.6/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2023-07-29 13:26:04.960028 sedi-0.6/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6383 2023-07-29 13:25:54.000000 sedi-0.6/provision.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2493 2023-07-29 13:25:54.000000 sedi-0.6/sed.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-29 13:26:04.960028 sedi-0.6/sedi.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2023-07-29 13:26:04.000000 sedi-0.6/sedi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      171 2023-07-29 13:26:04.000000 sedi-0.6/sedi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-29 13:26:04.000000 sedi-0.6/sedi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2023-07-29 13:26:04.000000 sedi-0.6/sedi.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2023-07-29 13:26:04.000000 sedi-0.6/sedi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-29 13:26:04.960028 sedi-0.6/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2023-07-29 13:25:54.000000 sedi-0.6/setup.py
```

### Comparing `sedi-0.5/provision.py` & `sedi-0.6/provision.py`

 * *Files identical despite different names*

