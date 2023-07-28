# Comparing `tmp/naruno_tests-0.59.0.tar.gz` & `tmp/naruno_tests-0.60.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_tests-0.59.0.tar", last modified: Thu Jun 29 00:20:11 2023, max compression
+gzip compressed data, was "naruno_tests-0.60.0.tar", last modified: Fri Jul 28 22:57:38 2023, max compression
```

## Comparing `naruno_tests-0.59.0.tar` & `naruno_tests-0.60.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:11.430738 naruno_tests-0.59.0/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-29 00:20:11.430738 naruno_tests-0.59.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:11.430738 naruno_tests-0.59.0/naruno_tests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-29 00:20:11.000000 naruno_tests-0.59.0/naruno_tests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 00:20:11.000000 naruno_tests-0.59.0/naruno_tests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:20:11.000000 naruno_tests-0.59.0/naruno_tests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:20:11.000000 naruno_tests-0.59.0/naruno_tests.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 00:20:11.000000 naruno_tests-0.59.0/naruno_tests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:20:11.000000 naruno_tests-0.59.0/naruno_tests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 00:20:11.430738 naruno_tests-0.59.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-29 00:19:51.000000 naruno_tests-0.59.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:38.071781 naruno_tests-0.60.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-28 22:57:38.071781 naruno_tests-0.60.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:38.071781 naruno_tests-0.60.0/naruno_tests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-28 22:57:38.000000 naruno_tests-0.60.0/naruno_tests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-28 22:57:38.000000 naruno_tests-0.60.0/naruno_tests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:57:38.000000 naruno_tests-0.60.0/naruno_tests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:57:38.000000 naruno_tests-0.60.0/naruno_tests.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 22:57:38.000000 naruno_tests-0.60.0/naruno_tests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:57:38.000000 naruno_tests-0.60.0/naruno_tests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:57:38.071781 naruno_tests-0.60.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 22:57:19.000000 naruno_tests-0.60.0/setup.py
```

