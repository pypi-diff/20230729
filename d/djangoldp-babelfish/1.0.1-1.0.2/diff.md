# Comparing `tmp/djangoldp_babelfish-1.0.1.tar.gz` & `tmp/djangoldp_babelfish-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_babelfish-1.0.1.tar", last modified: Sat Jul 29 09:04:49 2023, max compression
+gzip compressed data, was "djangoldp_babelfish-1.0.2.tar", last modified: Sat Jul 29 09:46:57 2023, max compression
```

## Comparing `djangoldp_babelfish-1.0.1.tar` & `djangoldp_babelfish-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      335 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/djangoldp_babelfish/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-29 09:04:46.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/djangoldp_babelfish/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/djangoldp_babelfish/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/management/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3132 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/
--rw-r--r--   0 root         (0) root         (0)      335 2023-07-29 09:04:49.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      671 2023-07-29 09:04:49.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 09:04:49.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-29 09:04:49.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-29 09:04:49.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      335 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/djangoldp_babelfish/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-29 09:46:54.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/djangoldp_babelfish/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/djangoldp_babelfish/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/management/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      335 2023-07-29 09:46:57.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      671 2023-07-29 09:46:57.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 09:46:57.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-29 09:46:57.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-29 09:46:57.000000 djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-07-29 09:46:57.126579 djangoldp_babelfish-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 09:46:38.000000 djangoldp_babelfish-1.0.2/setup.py
```

### Comparing `djangoldp_babelfish-1.0.1/README.md` & `djangoldp_babelfish-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/0001_initial.py` & `djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py` & `djangoldp_babelfish-1.0.2/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.1/djangoldp_babelfish/models.py` & `djangoldp_babelfish-1.0.2/djangoldp_babelfish/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.1/djangoldp_babelfish/views.py` & `djangoldp_babelfish-1.0.2/djangoldp_babelfish/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/SOURCES.txt` & `djangoldp_babelfish-1.0.2/djangoldp_babelfish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.1/setup.cfg` & `djangoldp_babelfish-1.0.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 author_email = benoit@startinblox.com
 description = Djangoldp babelfish package which provides integration with the Babelfish API
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp~=0.5
+	djangoldp~=3.0
+	djangoldp_account~=3.0
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
 
 [semantic_release]
 version_source = tag
```

