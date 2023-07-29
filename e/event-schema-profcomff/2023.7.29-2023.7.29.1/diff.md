# Comparing `tmp/event_schema_profcomff-2023.7.29.tar.gz` & `tmp/event_schema_profcomff-2023.7.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_schema_profcomff-2023.7.29.tar", last modified: Sat Jul 29 13:08:37 2023, max compression
+gzip compressed data, was "event_schema_profcomff-2023.7.29.1.tar", last modified: Sat Jul 29 13:19:01 2023, max compression
```

## Comparing `event_schema_profcomff-2023.7.29.tar` & `event_schema_profcomff-2023.7.29.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:08:37.602416 event_schema_profcomff-2023.7.29/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-29 13:08:24.000000 event_schema_profcomff-2023.7.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-29 13:08:37.602416 event_schema_profcomff-2023.7.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-29 13:08:24.000000 event_schema_profcomff-2023.7.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:08:37.602416 event_schema_profcomff-2023.7.29/event_schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:08:24.000000 event_schema_profcomff-2023.7.29/event_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:08:37.602416 event_schema_profcomff-2023.7.29/event_schema/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-29 13:08:24.000000 event_schema_profcomff-2023.7.29/event_schema/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-29 13:08:24.000000 event_schema_profcomff-2023.7.29/event_schema/auth/user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-29 13:08:24.000000 event_schema_profcomff-2023.7.29/event_schema/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:08:37.602416 event_schema_profcomff-2023.7.29/event_schema_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-29 13:08:37.000000 event_schema_profcomff-2023.7.29/event_schema_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-29 13:08:37.000000 event_schema_profcomff-2023.7.29/event_schema_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:08:37.000000 event_schema_profcomff-2023.7.29/event_schema_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 13:08:37.000000 event_schema_profcomff-2023.7.29/event_schema_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 13:08:37.000000 event_schema_profcomff-2023.7.29/event_schema_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 13:08:37.602416 event_schema_profcomff-2023.7.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-29 13:08:24.000000 event_schema_profcomff-2023.7.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/event_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/event_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/event_schema/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/event_schema/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/event_schema/auth/user_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/event_schema/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-29 13:19:01.000000 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-29 13:19:01.000000 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:19:01.000000 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 13:19:01.000000 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 13:19:01.000000 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/setup.py
```

### Comparing `event_schema_profcomff-2023.7.29/LICENSE` & `event_schema_profcomff-2023.7.29.1/LICENSE`

 * *Files identical despite different names*

