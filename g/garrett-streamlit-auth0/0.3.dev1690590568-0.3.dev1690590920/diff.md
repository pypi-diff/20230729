# Comparing `tmp/garrett-streamlit-auth0-0.3.dev1690590568.tar.gz` & `tmp/garrett-streamlit-auth0-0.3.dev1690590920.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garrett-streamlit-auth0-0.3.dev1690590568.tar", last modified: Sat Jul 29 00:29:28 2023, max compression
+gzip compressed data, was "garrett-streamlit-auth0-0.3.dev1690590920.tar", last modified: Sat Jul 29 00:35:20 2023, max compression
```

## Comparing `garrett-streamlit-auth0-0.3.dev1690590568.tar` & `garrett-streamlit-auth0-0.3.dev1690590920.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:29:28.925599 garrett-streamlit-auth0-0.3.dev1690590568/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-29 00:29:16.000000 garrett-streamlit-auth0-0.3.dev1690590568/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-29 00:29:16.000000 garrett-streamlit-auth0-0.3.dev1690590568/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-29 00:29:28.925599 garrett-streamlit-auth0-0.3.dev1690590568/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-29 00:29:16.000000 garrett-streamlit-auth0-0.3.dev1690590568/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:29:28.921599 garrett-streamlit-auth0-0.3.dev1690590568/auth0_component/
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-29 00:29:16.000000 garrett-streamlit-auth0-0.3.dev1690590568/auth0_component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:29:28.921599 garrett-streamlit-auth0-0.3.dev1690590568/auth0_component/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:29:28.921599 garrett-streamlit-auth0-0.3.dev1690590568/auth0_component/frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:29:28.925599 garrett-streamlit-auth0-0.3.dev1690590568/auth0_component/frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-29 00:29:28.000000 garrett-streamlit-auth0-0.3.dev1690590568/auth0_component/frontend/dist/assets/index.90c573b3.css
--rw-r--r--   0 runner    (1001) docker     (123)   331693 2023-07-29 00:29:28.000000 garrett-streamlit-auth0-0.3.dev1690590568/auth0_component/frontend/dist/assets/index.b724162b.js
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-29 00:29:28.000000 garrett-streamlit-auth0-0.3.dev1690590568/auth0_component/frontend/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:29:28.925599 garrett-streamlit-auth0-0.3.dev1690590568/garrett_streamlit_auth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-29 00:29:28.000000 garrett-streamlit-auth0-0.3.dev1690590568/garrett_streamlit_auth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-29 00:29:28.000000 garrett-streamlit-auth0-0.3.dev1690590568/garrett_streamlit_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:29:28.000000 garrett-streamlit-auth0-0.3.dev1690590568/garrett_streamlit_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 00:29:28.000000 garrett-streamlit-auth0-0.3.dev1690590568/garrett_streamlit_auth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 00:29:28.000000 garrett-streamlit-auth0-0.3.dev1690590568/garrett_streamlit_auth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-29 00:29:16.000000 garrett-streamlit-auth0-0.3.dev1690590568/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:29:28.925599 garrett-streamlit-auth0-0.3.dev1690590568/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-29 00:29:16.000000 garrett-streamlit-auth0-0.3.dev1690590568/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:20.490458 garrett-streamlit-auth0-0.3.dev1690590920/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-29 00:34:58.000000 garrett-streamlit-auth0-0.3.dev1690590920/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-29 00:34:58.000000 garrett-streamlit-auth0-0.3.dev1690590920/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-29 00:35:20.490458 garrett-streamlit-auth0-0.3.dev1690590920/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-29 00:34:58.000000 garrett-streamlit-auth0-0.3.dev1690590920/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:20.490458 garrett-streamlit-auth0-0.3.dev1690590920/auth0_component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-29 00:34:58.000000 garrett-streamlit-auth0-0.3.dev1690590920/auth0_component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:20.490458 garrett-streamlit-auth0-0.3.dev1690590920/auth0_component/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:20.490458 garrett-streamlit-auth0-0.3.dev1690590920/auth0_component/frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:20.490458 garrett-streamlit-auth0-0.3.dev1690590920/auth0_component/frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-29 00:35:20.000000 garrett-streamlit-auth0-0.3.dev1690590920/auth0_component/frontend/dist/assets/index.90c573b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)   331693 2023-07-29 00:35:20.000000 garrett-streamlit-auth0-0.3.dev1690590920/auth0_component/frontend/dist/assets/index.b724162b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-29 00:35:20.000000 garrett-streamlit-auth0-0.3.dev1690590920/auth0_component/frontend/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:20.490458 garrett-streamlit-auth0-0.3.dev1690590920/garrett_streamlit_auth0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-29 00:35:20.000000 garrett-streamlit-auth0-0.3.dev1690590920/garrett_streamlit_auth0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-29 00:35:20.000000 garrett-streamlit-auth0-0.3.dev1690590920/garrett_streamlit_auth0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:35:20.000000 garrett-streamlit-auth0-0.3.dev1690590920/garrett_streamlit_auth0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 00:35:20.000000 garrett-streamlit-auth0-0.3.dev1690590920/garrett_streamlit_auth0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 00:35:20.000000 garrett-streamlit-auth0-0.3.dev1690590920/garrett_streamlit_auth0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-29 00:34:58.000000 garrett-streamlit-auth0-0.3.dev1690590920/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:35:20.494458 garrett-streamlit-auth0-0.3.dev1690590920/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-29 00:34:58.000000 garrett-streamlit-auth0-0.3.dev1690590920/setup.py
```

### Comparing `garrett-streamlit-auth0-0.3.dev1690590568/LICENSE` & `garrett-streamlit-auth0-0.3.dev1690590920/LICENSE`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.dev1690590568/README.md` & `garrett-streamlit-auth0-0.3.dev1690590920/README.md`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.dev1690590568/auth0_component/__init__.py` & `garrett-streamlit-auth0-0.3.dev1690590920/auth0_component/__init__.py`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.dev1690590568/auth0_component/frontend/dist/assets/index.b724162b.js` & `garrett-streamlit-auth0-0.3.dev1690590920/auth0_component/frontend/dist/assets/index.b724162b.js`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.dev1690590568/setup.py` & `garrett-streamlit-auth0-0.3.dev1690590920/setup.py`

 * *Files identical despite different names*

