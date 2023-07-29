# Comparing `tmp/djangoldp_babelfish-1.0.0.tar.gz` & `tmp/djangoldp_babelfish-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_babelfish-1.0.0.tar", last modified: Sat Jul 29 09:01:57 2023, max compression
+gzip compressed data, was "djangoldp_babelfish-1.0.1.tar", last modified: Sat Jul 29 09:04:49 2023, max compression
```

## Comparing `djangoldp_babelfish-1.0.0.tar` & `djangoldp_babelfish-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/
--rw-rw-rw-   0 root         (0) root         (0)     3132 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/views.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/models.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-29 09:01:54.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-29 09:01:36.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
--rw-r--r--   0 root         (0) root         (0)      363 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/
--rw-r--r--   0 root         (0) root         (0)      363 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      671 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-29 09:01:57.000000 djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      335 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/djangoldp_babelfish/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-29 09:04:46.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/djangoldp_babelfish/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/djangoldp_babelfish/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/management/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      335 2023-07-29 09:04:49.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      671 2023-07-29 09:04:49.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 09:04:49.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-29 09:04:49.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-29 09:04:49.000000 djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-29 09:04:49.267139 djangoldp_babelfish-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 09:04:30.000000 djangoldp_babelfish-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_babelfish-1.0.0/README.md` & `djangoldp_babelfish-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.0/setup.cfg` & `djangoldp_babelfish-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.0/djangoldp_babelfish/views.py` & `djangoldp_babelfish-1.0.1/djangoldp_babelfish/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.0/djangoldp_babelfish/models.py` & `djangoldp_babelfish-1.0.1/djangoldp_babelfish/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/0001_initial.py` & `djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.0/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py` & `djangoldp_babelfish-1.0.1/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.0/djangoldp_babelfish.egg-info/SOURCES.txt` & `djangoldp_babelfish-1.0.1/djangoldp_babelfish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

