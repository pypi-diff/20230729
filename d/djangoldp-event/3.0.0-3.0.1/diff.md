# Comparing `tmp/djangoldp_event-3.0.0.tar.gz` & `tmp/djangoldp_event-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_event-3.0.0.tar", last modified: Sat Jul 29 09:32:51 2023, max compression
+gzip compressed data, was "djangoldp_event-3.0.1.tar", last modified: Sat Jul 29 09:57:20 2023, max compression
```

## Comparing `djangoldp_event-3.0.0.tar` & `djangoldp_event-3.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/
--rw-r--r--   0 root         (0) root         (0)      258 2023-07-29 09:32:51.385101 djangoldp_event-3.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/djangoldp_event/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-29 09:32:48.000000 djangoldp_event-3.0.0/djangoldp_event/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/djangoldp_event/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/djangoldp_event/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/management/commands/mock_example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/djangoldp_event/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3506 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0002_auto_20200202_1639.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0003_auto_20200202_1644.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0004_auto_20200202_2110.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0004_auto_20200426_1603.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0005_auto_20200617_1458.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0006_auto_20200709_1411.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0007_merge_20200812_0928.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0008_merge_20200812_1009.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0009_auto_20200812_1446.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0010_auto_20200812_1459.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0011_auto_20200923_1017.py
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0012_event_author.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0013_auto_20210525_1018.py
--rw-rw-rw-   0 root         (0) root         (0)     2255 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0014_auto_20210525_1022.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0015_event_visible.py
--rw-rw-rw-   0 root         (0) root         (0)     1454 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0016_auto_20210527_1612.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0017_auto_20221012_1503.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3399 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/models.py
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/djangoldp_event.egg-info/
--rw-r--r--   0 root         (0) root         (0)      258 2023-07-29 09:32:51.000000 djangoldp_event-3.0.0/djangoldp_event.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1543 2023-07-29 09:32:51.000000 djangoldp_event-3.0.0/djangoldp_event.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 09:32:51.000000 djangoldp_event-3.0.0/djangoldp_event.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-29 09:32:51.000000 djangoldp_event-3.0.0/djangoldp_event.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-29 09:32:51.000000 djangoldp_event-3.0.0/djangoldp_event.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-07-29 09:32:51.385101 djangoldp_event-3.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:57:20.971160 djangoldp_event-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-29 09:57:20.971160 djangoldp_event-3.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:57:20.967160 djangoldp_event-3.0.1/djangoldp_event/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-29 09:57:18.000000 djangoldp_event-3.0.1/djangoldp_event/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:57:20.967160 djangoldp_event-3.0.1/djangoldp_event/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:57:20.967160 djangoldp_event-3.0.1/djangoldp_event/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/management/commands/mock_example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:57:20.971160 djangoldp_event-3.0.1/djangoldp_event/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     3506 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0002_auto_20200202_1639.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0003_auto_20200202_1644.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0004_auto_20200202_2110.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0004_auto_20200426_1603.py
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0005_auto_20200617_1458.py
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0006_auto_20200709_1411.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0007_merge_20200812_0928.py
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0008_merge_20200812_1009.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0009_auto_20200812_1446.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0010_auto_20200812_1459.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0011_auto_20200923_1017.py
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0012_event_author.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0013_auto_20210525_1018.py
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0014_auto_20210525_1022.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0015_event_visible.py
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0016_auto_20210527_1612.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/0017_auto_20221012_1503.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3399 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/djangoldp_event/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:57:20.967160 djangoldp_event-3.0.1/djangoldp_event.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-29 09:57:20.000000 djangoldp_event-3.0.1/djangoldp_event.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-07-29 09:57:20.000000 djangoldp_event-3.0.1/djangoldp_event.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 09:57:20.000000 djangoldp_event-3.0.1/djangoldp_event.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-29 09:57:20.000000 djangoldp_event-3.0.1/djangoldp_event.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-29 09:57:20.000000 djangoldp_event-3.0.1/djangoldp_event.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-07-29 09:57:20.971160 djangoldp_event-3.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 09:57:02.000000 djangoldp_event-3.0.1/setup.py
```

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0001_initial.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0002_auto_20200202_1639.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0002_auto_20200202_1639.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0004_auto_20200202_2110.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0004_auto_20200202_2110.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0005_auto_20200617_1458.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0005_auto_20200617_1458.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0006_auto_20200709_1411.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0006_auto_20200709_1411.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0009_auto_20200812_1446.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0009_auto_20200812_1446.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0010_auto_20200812_1459.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0010_auto_20200812_1459.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0011_auto_20200923_1017.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0011_auto_20200923_1017.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0012_event_author.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0012_event_author.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0013_auto_20210525_1018.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0013_auto_20210525_1018.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0014_auto_20210525_1022.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0014_auto_20210525_1022.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/migrations/0016_auto_20210527_1612.py` & `djangoldp_event-3.0.1/djangoldp_event/migrations/0016_auto_20210527_1612.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event/models.py` & `djangoldp_event-3.0.1/djangoldp_event/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/djangoldp_event.egg-info/SOURCES.txt` & `djangoldp_event-3.0.1/djangoldp_event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_event-3.0.0/setup.cfg` & `djangoldp_event-3.0.1/setup.cfg`

 * *Files identical despite different names*

