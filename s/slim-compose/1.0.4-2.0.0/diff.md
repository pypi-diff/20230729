# Comparing `tmp/slim-compose-1.0.4.tar.gz` & `tmp/slim_compose-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slim-compose-1.0.4.tar", last modified: Thu May 18 09:28:43 2023, max compression
+gzip compressed data, was "slim_compose-2.0.0.tar", last modified: Sat Jul 29 12:35:27 2023, max compression
```

## Comparing `slim-compose-1.0.4.tar` & `slim_compose-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,10 @@
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-05-18 09:28:43.112415 slim-compose-1.0.4/
--rw-r--r--   0 foobar    (1000) foobar    (1000)     1056 2023-04-20 02:33:29.000000 slim-compose-1.0.4/LICENSE
--rw-r--r--   0 foobar    (1000) foobar    (1000)     2183 2023-05-18 09:28:43.112415 slim-compose-1.0.4/PKG-INFO
--rw-r--r--   0 foobar    (1000) foobar    (1000)      472 2023-04-20 06:49:18.000000 slim-compose-1.0.4/README.md
--rw-r--r--   0 foobar    (1000) foobar    (1000)      553 2023-05-18 09:23:54.000000 slim-compose-1.0.4/pyproject.toml
--rw-r--r--   0 foobar    (1000) foobar    (1000)       38 2023-05-18 09:28:43.112415 slim-compose-1.0.4/setup.cfg
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-05-18 09:28:43.112415 slim-compose-1.0.4/src/
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-05-18 09:28:43.112415 slim-compose-1.0.4/src/slim_compose.egg-info/
--rw-r--r--   0 foobar    (1000) foobar    (1000)     2183 2023-05-18 09:28:43.000000 slim-compose-1.0.4/src/slim_compose.egg-info/PKG-INFO
--rw-r--r--   0 foobar    (1000) foobar    (1000)      255 2023-05-18 09:28:43.000000 slim-compose-1.0.4/src/slim_compose.egg-info/SOURCES.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)        1 2023-05-18 09:28:43.000000 slim-compose-1.0.4/src/slim_compose.egg-info/dependency_links.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)       51 2023-05-18 09:28:43.000000 slim-compose-1.0.4/src/slim_compose.egg-info/entry_points.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)       13 2023-05-18 09:28:43.000000 slim-compose-1.0.4/src/slim_compose.egg-info/top_level.txt
--rwxr-xr-x   0 foobar    (1000) foobar    (1000)    13464 2023-05-18 09:28:24.000000 slim-compose-1.0.4/src/slim_compose.py
+-rw-r--r--   0        0        0     1061 2023-07-29 12:23:00.466444 slim_compose-2.0.0/LICENSE
+-rw-r--r--   0        0        0      510 2023-07-29 12:11:33.418423 slim_compose-2.0.0/README.md
+-rw-r--r--   0        0        0      720 2023-07-29 12:35:27.466715 slim_compose-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 12:11:33.450423 slim_compose-2.0.0/src/slim_compose/__init__.py
+-rw-r--r--   0        0        0     4774 2023-07-29 12:11:33.454423 slim_compose-2.0.0/src/slim_compose/args.py
+-rw-r--r--   0        0        0    10117 2023-07-29 12:11:33.474423 slim_compose-2.0.0/src/slim_compose/main.py
+-rw-r--r--   0        0        0     2943 2023-07-29 12:11:33.494423 slim_compose-2.0.0/src/slim_compose/utils.py
+-rw-r--r--   0        0        0        0 2023-07-29 12:11:33.506423 slim_compose-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      222 2023-07-29 12:11:33.510423 slim_compose-2.0.0/tests/test.py
+-rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 slim_compose-2.0.0/PKG-INFO
```

### Comparing `slim-compose-1.0.4/LICENSE` & `slim_compose-2.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023
+Copyright (c) 2023 brin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

