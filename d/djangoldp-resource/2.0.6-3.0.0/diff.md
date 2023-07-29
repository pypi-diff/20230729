# Comparing `tmp/djangoldp_resource-2.0.6.tar.gz` & `tmp/djangoldp_resource-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_resource-2.0.6.tar", last modified: Wed Mar 15 23:06:31 2023, max compression
+gzip compressed data, was "djangoldp_resource-3.0.0.tar", last modified: Sat Jul 29 09:38:09 2023, max compression
```

## Comparing `djangoldp_resource-2.0.6.tar` & `djangoldp_resource-3.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/djangoldp_resource.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/djangoldp_resource.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/djangoldp_resource.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1420 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/djangoldp_resource.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/djangoldp_resource.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/djangoldp_resource.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      300 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/djangoldp_resource/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/views.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/models.py
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-03-15 23:06:29.000000 djangoldp_resource-2.0.6/djangoldp_resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      690 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:06:31.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0013_auto_20221012_1503.py
--rw-rw-rw-   0 root         (0) root         (0)     2661 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0002_auto_20200426_1902.py
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0009_auto_20200812_1459.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0004_merge_20200616_1011.py
--rw-rw-rw-   0 root         (0) root         (0)     1279 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0007_auto_20200709_1411.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0012_auto_20210525_1022.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0006_auto_20200617_1458.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0011_auto_20210525_1018.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0003_auto_20200616_0957.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0008_auto_20200812_1446.py
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0005_merge_20200616_1030.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0010_auto_20200923_1017.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0003_resource_conversations.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0002_resource_user.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-03-15 23:06:14.000000 djangoldp_resource-2.0.6/djangoldp_resource/migrations/0014_auto_20221027_0958.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:38:09.357727 djangoldp_resource-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-29 09:38:09.357727 djangoldp_resource-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:38:09.353727 djangoldp_resource-3.0.0/djangoldp_resource/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-29 09:38:06.000000 djangoldp_resource-3.0.0/djangoldp_resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:38:09.357727 djangoldp_resource-3.0.0/djangoldp_resource/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2661 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0002_auto_20200426_1902.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0002_resource_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0003_auto_20200616_0957.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0003_resource_conversations.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0004_merge_20200616_1011.py
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0005_merge_20200616_1030.py
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0006_auto_20200617_1458.py
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0007_auto_20200709_1411.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0008_auto_20200812_1446.py
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0009_auto_20200812_1459.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0010_auto_20200923_1017.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0011_auto_20210525_1018.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0012_auto_20210525_1022.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0013_auto_20221012_1503.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/0014_auto_20221027_0958.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/djangoldp_resource/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 09:38:09.357727 djangoldp_resource-3.0.0/djangoldp_resource.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-29 09:38:09.000000 djangoldp_resource-3.0.0/djangoldp_resource.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-07-29 09:38:09.000000 djangoldp_resource-3.0.0/djangoldp_resource.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 09:38:09.000000 djangoldp_resource-3.0.0/djangoldp_resource.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-07-29 09:38:09.000000 djangoldp_resource-3.0.0/djangoldp_resource.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-29 09:38:09.000000 djangoldp_resource-3.0.0/djangoldp_resource.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-29 09:38:09.357727 djangoldp_resource-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-29 09:37:49.000000 djangoldp_resource-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource.egg-info/SOURCES.txt` & `djangoldp_resource-3.0.0/djangoldp_resource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/setup.cfg` & `djangoldp_resource-3.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [metadata]
 name = djangoldp_resource
 version = attr: djangoldp_resource.__version__
-url = http://git.startinblox.fr/djangoldp-packages/djangoldp-resource
+url = https://git.startinblox.com/djangoldp-packages/djangoldp-resource
 author = Startin'blox
-author_email = marjolaine@nantes.happy-dev.fr
+author_email = Marjolaine@startinblox.com
 description = djangoldp resource package
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp>=1.0.0
-	djangoldp_conversation
-	djangoldp_circle
+	djangoldp~=3.0
+	djangoldp_conversation~=3.0
+	djangoldp_circle~=3.0
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
 
 [semantic_release]
 version_source = tag
```

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/models.py` & `djangoldp_resource-3.0.0/djangoldp_resource/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/filters.py` & `djangoldp_resource-3.0.0/djangoldp_resource/filters.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0001_initial.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0002_auto_20200426_1902.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0002_auto_20200426_1902.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0009_auto_20200812_1459.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0009_auto_20200812_1459.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0007_auto_20200709_1411.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0007_auto_20200709_1411.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0012_auto_20210525_1022.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0012_auto_20210525_1022.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0006_auto_20200617_1458.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0006_auto_20200617_1458.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0011_auto_20210525_1018.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0011_auto_20210525_1018.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0003_auto_20200616_0957.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0003_auto_20200616_0957.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0008_auto_20200812_1446.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0008_auto_20200812_1446.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0010_auto_20200923_1017.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0010_auto_20200923_1017.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0003_resource_conversations.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0003_resource_conversations.py`

 * *Files identical despite different names*

### Comparing `djangoldp_resource-2.0.6/djangoldp_resource/migrations/0002_resource_user.py` & `djangoldp_resource-3.0.0/djangoldp_resource/migrations/0002_resource_user.py`

 * *Files identical despite different names*

