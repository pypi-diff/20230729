# Comparing `tmp/garrett-streamlit-auth0-0.3.dev1690586794.tar.gz` & `tmp/garrett-streamlit-auth0-0.3.dev1690588875.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garrett-streamlit-auth0-0.3.dev1690586794.tar", last modified: Fri Jul 28 23:26:34 2023, max compression
+gzip compressed data, was "garrett-streamlit-auth0-0.3.dev1690588875.tar", last modified: Sat Jul 29 00:01:15 2023, max compression
```

## Comparing `garrett-streamlit-auth0-0.3.dev1690586794.tar` & `garrett-streamlit-auth0-0.3.dev1690588875.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:26:34.171357 garrett-streamlit-auth0-0.3.dev1690586794/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-28 23:26:22.000000 garrett-streamlit-auth0-0.3.dev1690586794/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-28 23:26:22.000000 garrett-streamlit-auth0-0.3.dev1690586794/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 23:26:34.171357 garrett-streamlit-auth0-0.3.dev1690586794/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-28 23:26:22.000000 garrett-streamlit-auth0-0.3.dev1690586794/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:26:34.167357 garrett-streamlit-auth0-0.3.dev1690586794/auth0_component/
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-28 23:26:22.000000 garrett-streamlit-auth0-0.3.dev1690586794/auth0_component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:26:34.167357 garrett-streamlit-auth0-0.3.dev1690586794/auth0_component/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:26:34.167357 garrett-streamlit-auth0-0.3.dev1690586794/auth0_component/frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:26:34.167357 garrett-streamlit-auth0-0.3.dev1690586794/auth0_component/frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-28 23:26:33.000000 garrett-streamlit-auth0-0.3.dev1690586794/auth0_component/frontend/dist/assets/index.90c573b3.css
--rw-r--r--   0 runner    (1001) docker     (123)   331693 2023-07-28 23:26:33.000000 garrett-streamlit-auth0-0.3.dev1690586794/auth0_component/frontend/dist/assets/index.b724162b.js
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-28 23:26:33.000000 garrett-streamlit-auth0-0.3.dev1690586794/auth0_component/frontend/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:26:34.167357 garrett-streamlit-auth0-0.3.dev1690586794/garrett_streamlit_auth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 23:26:34.000000 garrett-streamlit-auth0-0.3.dev1690586794/garrett_streamlit_auth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-28 23:26:34.000000 garrett-streamlit-auth0-0.3.dev1690586794/garrett_streamlit_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:26:34.000000 garrett-streamlit-auth0-0.3.dev1690586794/garrett_streamlit_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 23:26:34.000000 garrett-streamlit-auth0-0.3.dev1690586794/garrett_streamlit_auth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 23:26:34.000000 garrett-streamlit-auth0-0.3.dev1690586794/garrett_streamlit_auth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 23:26:22.000000 garrett-streamlit-auth0-0.3.dev1690586794/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:26:34.171357 garrett-streamlit-auth0-0.3.dev1690586794/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-28 23:26:22.000000 garrett-streamlit-auth0-0.3.dev1690586794/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:01:15.204975 garrett-streamlit-auth0-0.3.dev1690588875/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-29 00:01:00.000000 garrett-streamlit-auth0-0.3.dev1690588875/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-29 00:01:00.000000 garrett-streamlit-auth0-0.3.dev1690588875/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-29 00:01:15.204975 garrett-streamlit-auth0-0.3.dev1690588875/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-29 00:01:00.000000 garrett-streamlit-auth0-0.3.dev1690588875/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:01:15.200975 garrett-streamlit-auth0-0.3.dev1690588875/auth0_component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-29 00:01:00.000000 garrett-streamlit-auth0-0.3.dev1690588875/auth0_component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:01:15.192974 garrett-streamlit-auth0-0.3.dev1690588875/auth0_component/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:01:15.200975 garrett-streamlit-auth0-0.3.dev1690588875/auth0_component/frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:01:15.200975 garrett-streamlit-auth0-0.3.dev1690588875/auth0_component/frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-29 00:01:14.000000 garrett-streamlit-auth0-0.3.dev1690588875/auth0_component/frontend/dist/assets/index.90c573b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)   331693 2023-07-29 00:01:14.000000 garrett-streamlit-auth0-0.3.dev1690588875/auth0_component/frontend/dist/assets/index.b724162b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-29 00:01:14.000000 garrett-streamlit-auth0-0.3.dev1690588875/auth0_component/frontend/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:01:15.204975 garrett-streamlit-auth0-0.3.dev1690588875/garrett_streamlit_auth0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-29 00:01:15.000000 garrett-streamlit-auth0-0.3.dev1690588875/garrett_streamlit_auth0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-29 00:01:15.000000 garrett-streamlit-auth0-0.3.dev1690588875/garrett_streamlit_auth0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:01:15.000000 garrett-streamlit-auth0-0.3.dev1690588875/garrett_streamlit_auth0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 00:01:15.000000 garrett-streamlit-auth0-0.3.dev1690588875/garrett_streamlit_auth0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 00:01:15.000000 garrett-streamlit-auth0-0.3.dev1690588875/garrett_streamlit_auth0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-29 00:01:00.000000 garrett-streamlit-auth0-0.3.dev1690588875/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:01:15.204975 garrett-streamlit-auth0-0.3.dev1690588875/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-29 00:01:00.000000 garrett-streamlit-auth0-0.3.dev1690588875/setup.py
```

### Comparing `garrett-streamlit-auth0-0.3.dev1690586794/LICENSE` & `garrett-streamlit-auth0-0.3.dev1690588875/LICENSE`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.dev1690586794/README.md` & `garrett-streamlit-auth0-0.3.dev1690588875/README.md`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.dev1690586794/auth0_component/__init__.py` & `garrett-streamlit-auth0-0.3.dev1690588875/auth0_component/__init__.py`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.dev1690586794/auth0_component/frontend/dist/assets/index.b724162b.js` & `garrett-streamlit-auth0-0.3.dev1690588875/auth0_component/frontend/dist/assets/index.b724162b.js`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.dev1690586794/setup.py` & `garrett-streamlit-auth0-0.3.dev1690588875/setup.py`

 * *Files identical despite different names*

