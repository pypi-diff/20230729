# Comparing `tmp/djangoldp_event-2.0.5.tar.gz` & `tmp/djangoldp_event-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_event-2.0.5.tar", last modified: Thu Oct 13 09:43:58 2022, max compression
+gzip compressed data, was "djangoldp_event-3.0.0.tar", last modified: Sat Jul 29 09:32:51 2023, max compression
```

## Comparing `djangoldp_event-2.0.5.tar` & `djangoldp_event-3.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/
--rw-rw-rw-   0 root         (0) root         (0)      236 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      292 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/djangoldp_event.egg-info/
--rw-r--r--   0 root         (0) root         (0)      292 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/djangoldp_event.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/djangoldp_event.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1543 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/djangoldp_event.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/djangoldp_event.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       61 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/djangoldp_event.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/djangoldp_event/
--rw-rw-rw-   0 root         (0) root         (0)      425 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/views.py
--rw-rw-rw-   0 root         (0) root         (0)     3399 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/models.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/djangoldp_event/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/djangoldp_event/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      493 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/management/commands/mock_example.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2022-10-13 09:43:56.000000 djangoldp_event-2.0.5/djangoldp_event/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 09:43:58.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      509 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0003_auto_20200202_1644.py
--rw-rw-rw-   0 root         (0) root         (0)     1454 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0016_auto_20210527_1612.py
--rw-rw-rw-   0 root         (0) root         (0)     3506 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0010_auto_20200812_1459.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0009_auto_20200812_1446.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0007_merge_20200812_0928.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0005_auto_20200617_1458.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0004_auto_20200426_1603.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0015_event_visible.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0017_auto_20221012_1503.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0006_auto_20200709_1411.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0004_auto_20200202_2110.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0008_merge_20200812_1009.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0013_auto_20210525_1018.py
--rw-rw-rw-   0 root         (0) root         (0)     2255 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0014_auto_20210525_1022.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0002_auto_20200202_1639.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0011_auto_20200923_1017.py
--rw-rw-rw-   0 root         (0) root         (0)      639 2022-10-13 09:43:41.000000 djangoldp_event-2.0.5/djangoldp_event/migrations/0012_event_author.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-29 09:32:51.385101 djangoldp_event-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/djangoldp_event/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-29 09:32:48.000000 djangoldp_event-3.0.0/djangoldp_event/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/djangoldp_event/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/djangoldp_event/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/management/commands/mock_example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/djangoldp_event/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     3506 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0002_auto_20200202_1639.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0003_auto_20200202_1644.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0004_auto_20200202_2110.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0004_auto_20200426_1603.py
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0005_auto_20200617_1458.py
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0006_auto_20200709_1411.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0007_merge_20200812_0928.py
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0008_merge_20200812_1009.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0009_auto_20200812_1446.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0010_auto_20200812_1459.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0011_auto_20200923_1017.py
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0012_event_author.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0013_auto_20210525_1018.py
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0014_auto_20210525_1022.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0015_event_visible.py
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0016_auto_20210527_1612.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/0017_auto_20221012_1503.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3399 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/djangoldp_event/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:32:51.381101 djangoldp_event-3.0.0/djangoldp_event.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-29 09:32:51.000000 djangoldp_event-3.0.0/djangoldp_event.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-07-29 09:32:51.000000 djangoldp_event-3.0.0/djangoldp_event.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 09:32:51.000000 djangoldp_event-3.0.0/djangoldp_event.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-29 09:32:51.000000 djangoldp_event-3.0.0/djangoldp_event.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-29 09:32:51.000000 djangoldp_event-3.0.0/djangoldp_event.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-07-29 09:32:51.385101 djangoldp_event-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 09:32:32.000000 djangoldp_event-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_event-2.0.5/setup.cfg` & `djangoldp_event-3.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = djangoldp_event
 version = attr: djangoldp_event.__version__
-url = http://git.startinblox.fr/startinblox/applications/etuc/djangoldp-event
+url = https://git.startinblox.com/djangoldp-packages/djangoldp-event
 author = Startin'blox
-author_email = nicolas@happy-dev.fr
+author_email = contact@startinblox.com
 description = djangoldp event package
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp>=1.0.0
-	djangoldp_circle
+	djangoldp~=3.0
+	djangoldp_circle~=3.0
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
 
 [semantic_release]
 version_source = tag
```

### Comparing `djangoldp_event-2.0.5/djangoldp_event.egg-info/SOURCES.txt` & `djangoldp_event-3.0.0/djangoldp_event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/models.py` & `djangoldp_event-3.0.0/djangoldp_event/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0016_auto_20210527_1612.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0016_auto_20210527_1612.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0001_initial.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0010_auto_20200812_1459.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0010_auto_20200812_1459.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0009_auto_20200812_1446.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0009_auto_20200812_1446.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0005_auto_20200617_1458.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0005_auto_20200617_1458.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0006_auto_20200709_1411.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0006_auto_20200709_1411.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0004_auto_20200202_2110.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0004_auto_20200202_2110.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0013_auto_20210525_1018.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0013_auto_20210525_1018.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0014_auto_20210525_1022.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0014_auto_20210525_1022.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0002_auto_20200202_1639.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0002_auto_20200202_1639.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0011_auto_20200923_1017.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0011_auto_20200923_1017.py`

 * *Files identical despite different names*

### Comparing `djangoldp_event-2.0.5/djangoldp_event/migrations/0012_event_author.py` & `djangoldp_event-3.0.0/djangoldp_event/migrations/0012_event_author.py`

 * *Files identical despite different names*

