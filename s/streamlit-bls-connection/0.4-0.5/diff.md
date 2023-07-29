# Comparing `tmp/streamlit_bls_connection-0.4.tar.gz` & `tmp/streamlit_bls_connection-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_bls_connection-0.4.tar", last modified: Sat Jul 29 04:19:49 2023, max compression
+gzip compressed data, was "streamlit_bls_connection-0.5.tar", last modified: Sat Jul 29 16:44:38 2023, max compression
```

## Comparing `streamlit_bls_connection-0.4.tar` & `streamlit_bls_connection-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 04:19:49.108293 streamlit_bls_connection-0.4/
--rw-rw-rw-   0        0        0     1090 2023-07-29 02:22:35.000000 streamlit_bls_connection-0.4/LICENSE
--rw-rw-rw-   0        0        0      225 2023-07-29 04:19:49.107773 streamlit_bls_connection-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-07-29 03:47:40.000000 streamlit_bls_connection-0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 04:19:49.108293 streamlit_bls_connection-0.4/setup.cfg
--rw-rw-rw-   0        0        0      486 2023-07-29 04:18:15.000000 streamlit_bls_connection-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 04:19:49.097912 streamlit_bls_connection-0.4/streamlit_bls_connection/
--rw-rw-rw-   0        0        0       41 2023-07-29 01:24:58.000000 streamlit_bls_connection-0.4/streamlit_bls_connection/__init__.py
--rw-rw-rw-   0        0        0     3645 2023-07-25 22:28:07.000000 streamlit_bls_connection-0.4/streamlit_bls_connection/streamlit_bls_connection.py
-drwxrwxrwx   0        0        0        0 2023-07-29 04:19:49.106671 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/
--rw-rw-rw-   0        0        0      225 2023-07-29 04:19:49.000000 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-07-29 04:19:49.000000 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 04:19:49.000000 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-29 04:19:49.000000 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-29 04:19:49.000000 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 16:44:38.947064 streamlit_bls_connection-0.5/
+-rw-rw-rw-   0        0        0     1089 2023-07-29 16:30:01.000000 streamlit_bls_connection-0.5/LICENSE
+-rw-rw-rw-   0        0        0      763 2023-07-29 16:44:38.947064 streamlit_bls_connection-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-07-29 03:47:40.000000 streamlit_bls_connection-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 16:44:38.947064 streamlit_bls_connection-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1094 2023-07-29 16:44:28.000000 streamlit_bls_connection-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:44:38.893945 streamlit_bls_connection-0.5/streamlit_bls_connection/
+-rw-rw-rw-   0        0        0       65 2023-07-29 16:22:24.000000 streamlit_bls_connection-0.5/streamlit_bls_connection/__init__.py
+-rw-rw-rw-   0        0        0     3645 2023-07-25 22:28:07.000000 streamlit_bls_connection-0.5/streamlit_bls_connection/bls_connection.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:44:38.945575 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/
+-rw-rw-rw-   0        0        0      763 2023-07-29 16:44:38.000000 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-07-29 16:44:38.000000 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:44:38.000000 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-29 16:44:38.000000 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-29 16:44:38.000000 streamlit_bls_connection-0.5/streamlit_bls_connection.egg-info/top_level.txt
```

### Comparing `streamlit_bls_connection-0.4/LICENSE` & `streamlit_bls_connection-0.5/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Tony Hollaar
+Copyright (c) 2023 tony hollaar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `streamlit_bls_connection-0.4/README.md` & `streamlit_bls_connection-0.5/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_bls_connection-0.4/streamlit_bls_connection/streamlit_bls_connection.py` & `streamlit_bls_connection-0.5/streamlit_bls_connection/bls_connection.py`

 * *Files identical despite different names*

