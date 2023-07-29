# Comparing `tmp/tagpatch-0.1.0.tar.gz` & `tmp/tagpatch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagpatch-0.1.0.tar", last modified: Sat Jul 29 09:14:25 2023, max compression
+gzip compressed data, was "tagpatch-0.1.1.tar", last modified: Sat Jul 29 09:33:55 2023, max compression
```

## Comparing `tagpatch-0.1.0.tar` & `tagpatch-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:14:25.023777 tagpatch-0.1.0/
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1081 2023-07-08 13:19:47.000000 tagpatch-0.1.0/LICENSE
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1383 2023-07-29 09:14:25.023777 tagpatch-0.1.0/PKG-INFO
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1108 2023-07-29 08:56:37.000000 tagpatch-0.1.0/README.md
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)      470 2023-07-28 10:18:18.000000 tagpatch-0.1.0/pyproject.toml
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)      144 2023-07-29 09:14:25.024777 tagpatch-0.1.0/setup.cfg
-drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:14:25.021777 tagpatch-0.1.0/tagpatch/
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 08:54:16.000000 tagpatch-0.1.0/tagpatch/__init__.py
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     2124 2023-07-29 08:54:18.000000 tagpatch-0.1.0/tagpatch/__main__.py
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1189 2023-07-29 08:54:20.000000 tagpatch-0.1.0/tagpatch/options.py
-drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:14:25.023777 tagpatch-0.1.0/tagpatch/patches/
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 08:54:09.000000 tagpatch-0.1.0/tagpatch/patches/__init__.py
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     2813 2023-07-29 08:54:12.000000 tagpatch-0.1.0/tagpatch/patches/artist_name.py
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     2840 2023-07-29 08:54:13.000000 tagpatch-0.1.0/tagpatch/patches/embed_lrc.py
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)      860 2023-07-29 08:54:15.000000 tagpatch-0.1.0/tagpatch/patches/patch.py
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)       90 2023-07-29 08:54:21.000000 tagpatch-0.1.0/tagpatch/types.py
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     2754 2023-07-29 08:54:23.000000 tagpatch-0.1.0/tagpatch/utils.py
-drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:14:25.022777 tagpatch-0.1.0/tagpatch.egg-info/
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1383 2023-07-29 09:14:25.000000 tagpatch-0.1.0/tagpatch.egg-info/PKG-INFO
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)      511 2023-07-29 09:14:25.000000 tagpatch-0.1.0/tagpatch.egg-info/SOURCES.txt
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)        1 2023-07-29 09:14:25.000000 tagpatch-0.1.0/tagpatch.egg-info/dependency_links.txt
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)       52 2023-07-29 09:14:25.000000 tagpatch-0.1.0/tagpatch.egg-info/entry_points.txt
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)       62 2023-07-29 09:14:25.000000 tagpatch-0.1.0/tagpatch.egg-info/requires.txt
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)       15 2023-07-29 09:14:25.000000 tagpatch-0.1.0/tagpatch.egg-info/top_level.txt
-drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:14:25.023777 tagpatch-0.1.0/tests/
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)        0 2023-07-28 05:34:28.000000 tagpatch-0.1.0/tests/__init__.py
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     2118 2023-07-29 08:54:31.000000 tagpatch-0.1.0/tests/test_patches.py
--rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1731 2023-07-29 08:54:51.000000 tagpatch-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:33:55.931042 tagpatch-0.1.1/
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1081 2023-07-08 13:19:47.000000 tagpatch-0.1.1/LICENSE
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)       37 2023-07-29 09:26:59.000000 tagpatch-0.1.1/MANIFEST.in
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1392 2023-07-29 09:33:55.931042 tagpatch-0.1.1/PKG-INFO
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1108 2023-07-29 08:56:37.000000 tagpatch-0.1.1/README.md
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)      480 2023-07-29 09:32:44.000000 tagpatch-0.1.1/pyproject.toml
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)      172 2023-07-29 09:33:55.931042 tagpatch-0.1.1/setup.cfg
+drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:33:55.926041 tagpatch-0.1.1/tagpatch/
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 08:54:16.000000 tagpatch-0.1.1/tagpatch/__init__.py
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     2124 2023-07-29 08:54:18.000000 tagpatch-0.1.1/tagpatch/__main__.py
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1189 2023-07-29 08:54:20.000000 tagpatch-0.1.1/tagpatch/options.py
+drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:33:55.928042 tagpatch-0.1.1/tagpatch/patches/
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 08:54:09.000000 tagpatch-0.1.1/tagpatch/patches/__init__.py
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     2813 2023-07-29 08:54:12.000000 tagpatch-0.1.1/tagpatch/patches/artist_name.py
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     2840 2023-07-29 08:54:13.000000 tagpatch-0.1.1/tagpatch/patches/embed_lrc.py
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)      860 2023-07-29 08:54:15.000000 tagpatch-0.1.1/tagpatch/patches/patch.py
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)       90 2023-07-29 08:54:21.000000 tagpatch-0.1.1/tagpatch/types.py
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     2754 2023-07-29 08:54:23.000000 tagpatch-0.1.1/tagpatch/utils.py
+drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:33:55.927041 tagpatch-0.1.1/tagpatch.egg-info/
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1392 2023-07-29 09:33:55.000000 tagpatch-0.1.1/tagpatch.egg-info/PKG-INFO
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)      604 2023-07-29 09:33:55.000000 tagpatch-0.1.1/tagpatch.egg-info/SOURCES.txt
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)        1 2023-07-29 09:33:55.000000 tagpatch-0.1.1/tagpatch.egg-info/dependency_links.txt
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)       52 2023-07-29 09:33:55.000000 tagpatch-0.1.1/tagpatch.egg-info/entry_points.txt
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)       62 2023-07-29 09:33:55.000000 tagpatch-0.1.1/tagpatch.egg-info/requires.txt
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)       15 2023-07-29 09:33:55.000000 tagpatch-0.1.1/tagpatch.egg-info/top_level.txt
+drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:33:55.928042 tagpatch-0.1.1/tests/
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)        0 2023-07-28 05:34:28.000000 tagpatch-0.1.1/tests/__init__.py
+drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:33:55.924042 tagpatch-0.1.1/tests/data/
+drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:33:55.929041 tagpatch-0.1.1/tests/data/song1/
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)      172 2023-07-28 05:54:20.000000 tagpatch-0.1.1/tests/data/song1/ATTRIBUTION.txt
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)  3329994 2023-07-28 05:53:34.000000 tagpatch-0.1.1/tests/data/song1/test.mp3
+drwxr-xr-x   0 icewreck  (1000) icewreck  (1000)        0 2023-07-29 09:33:55.931042 tagpatch-0.1.1/tests/output/
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)        0 2023-07-28 06:02:00.000000 tagpatch-0.1.1/tests/output/.gitkeep
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     2118 2023-07-29 08:54:31.000000 tagpatch-0.1.1/tests/test_patches.py
+-rw-r--r--   0 icewreck  (1000) icewreck  (1000)     1731 2023-07-29 08:54:51.000000 tagpatch-0.1.1/tests/test_utils.py
```

### Comparing `tagpatch-0.1.0/LICENSE` & `tagpatch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tagpatch-0.1.0/PKG-INFO` & `tagpatch-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tagpatch
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tool which applies common patches to music tags
-Author-email: Anchit Bajaj <ab@abifog.com>
+Author-email: Anchit Bajaj <python.pypi@abifog.com>
 License: MIT
 Keywords: music,tag
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tagpatch
```

### Comparing `tagpatch-0.1.0/README.md` & `tagpatch-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tagpatch-0.1.0/tagpatch/__main__.py` & `tagpatch-0.1.1/tagpatch/__main__.py`

 * *Files identical despite different names*

### Comparing `tagpatch-0.1.0/tagpatch/options.py` & `tagpatch-0.1.1/tagpatch/options.py`

 * *Files identical despite different names*

### Comparing `tagpatch-0.1.0/tagpatch/patches/artist_name.py` & `tagpatch-0.1.1/tagpatch/patches/artist_name.py`

 * *Files identical despite different names*

### Comparing `tagpatch-0.1.0/tagpatch/patches/embed_lrc.py` & `tagpatch-0.1.1/tagpatch/patches/embed_lrc.py`

 * *Files identical despite different names*

### Comparing `tagpatch-0.1.0/tagpatch/patches/patch.py` & `tagpatch-0.1.1/tagpatch/patches/patch.py`

 * *Files identical despite different names*

### Comparing `tagpatch-0.1.0/tagpatch/utils.py` & `tagpatch-0.1.1/tagpatch/utils.py`

 * *Files identical despite different names*

### Comparing `tagpatch-0.1.0/tagpatch.egg-info/PKG-INFO` & `tagpatch-0.1.1/tagpatch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tagpatch
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tool which applies common patches to music tags
-Author-email: Anchit Bajaj <ab@abifog.com>
+Author-email: Anchit Bajaj <python.pypi@abifog.com>
 License: MIT
 Keywords: music,tag
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tagpatch
```

### Comparing `tagpatch-0.1.0/tests/test_patches.py` & `tagpatch-0.1.1/tests/test_patches.py`

 * *Files identical despite different names*

### Comparing `tagpatch-0.1.0/tests/test_utils.py` & `tagpatch-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

