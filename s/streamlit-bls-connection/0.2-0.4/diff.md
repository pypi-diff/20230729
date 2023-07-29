# Comparing `tmp/streamlit_bls_connection-0.2.tar.gz` & `tmp/streamlit_bls_connection-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_bls_connection-0.2.tar", last modified: Sat Jul 29 03:51:55 2023, max compression
+gzip compressed data, was "streamlit_bls_connection-0.4.tar", last modified: Sat Jul 29 04:19:49 2023, max compression
```

## Comparing `streamlit_bls_connection-0.2.tar` & `streamlit_bls_connection-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 03:51:55.170299 streamlit_bls_connection-0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-29 02:22:35.000000 streamlit_bls_connection-0.2/LICENSE
--rw-rw-rw-   0        0        0      225 2023-07-29 03:51:55.170299 streamlit_bls_connection-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-07-29 03:47:40.000000 streamlit_bls_connection-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 03:51:55.170299 streamlit_bls_connection-0.2/setup.cfg
--rw-rw-rw-   0        0        0      486 2023-07-29 03:48:17.000000 streamlit_bls_connection-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:51:55.163291 streamlit_bls_connection-0.2/streamlit_bls_connection.egg-info/
--rw-rw-rw-   0        0        0      225 2023-07-29 03:51:55.000000 streamlit_bls_connection-0.2/streamlit_bls_connection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-07-29 03:51:55.000000 streamlit_bls_connection-0.2/streamlit_bls_connection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 03:51:55.000000 streamlit_bls_connection-0.2/streamlit_bls_connection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-29 03:51:55.000000 streamlit_bls_connection-0.2/streamlit_bls_connection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-29 03:51:55.000000 streamlit_bls_connection-0.2/streamlit_bls_connection.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-29 03:51:55.167295 streamlit_bls_connection-0.2/streamlit_connection_package/
--rw-rw-rw-   0        0        0       41 2023-07-29 01:24:58.000000 streamlit_bls_connection-0.2/streamlit_connection_package/__init__.py
--rw-rw-rw-   0        0        0     3645 2023-07-25 22:28:07.000000 streamlit_bls_connection-0.2/streamlit_connection_package/bls_connection.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:19:49.108293 streamlit_bls_connection-0.4/
+-rw-rw-rw-   0        0        0     1090 2023-07-29 02:22:35.000000 streamlit_bls_connection-0.4/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-07-29 04:19:49.107773 streamlit_bls_connection-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-07-29 03:47:40.000000 streamlit_bls_connection-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 04:19:49.108293 streamlit_bls_connection-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      486 2023-07-29 04:18:15.000000 streamlit_bls_connection-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:19:49.097912 streamlit_bls_connection-0.4/streamlit_bls_connection/
+-rw-rw-rw-   0        0        0       41 2023-07-29 01:24:58.000000 streamlit_bls_connection-0.4/streamlit_bls_connection/__init__.py
+-rw-rw-rw-   0        0        0     3645 2023-07-25 22:28:07.000000 streamlit_bls_connection-0.4/streamlit_bls_connection/streamlit_bls_connection.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:19:49.106671 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-07-29 04:19:49.000000 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-07-29 04:19:49.000000 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 04:19:49.000000 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-29 04:19:49.000000 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-29 04:19:49.000000 streamlit_bls_connection-0.4/streamlit_bls_connection.egg-info/top_level.txt
```

### Comparing `streamlit_bls_connection-0.2/LICENSE` & `streamlit_bls_connection-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_bls_connection-0.2/README.md` & `streamlit_bls_connection-0.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_bls_connection-0.2/streamlit_connection_package/bls_connection.py` & `streamlit_bls_connection-0.4/streamlit_bls_connection/streamlit_bls_connection.py`

 * *Files identical despite different names*

