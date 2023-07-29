# Comparing `tmp/napatrackmater-3.9.0.tar.gz` & `tmp/napatrackmater-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-3.9.0.tar", last modified: Sat Jul 29 15:03:27 2023, max compression
+gzip compressed data, was "napatrackmater-3.9.1.tar", last modified: Sat Jul 29 15:22:41 2023, max compression
```

## Comparing `napatrackmater-3.9.0.tar` & `napatrackmater-3.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:03:27.454446 napatrackmater-3.9.0/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 15:03:27.454108 napatrackmater-3.9.0/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:03:27.452114 napatrackmater-3.9.0/napatrackmater/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)   114228 2023-07-29 15:02:11.000000 napatrackmater-3.9.0/napatrackmater/Trackmate.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/Trackvector.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/clustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/fate_mapping.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/pretrained.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 15:02:18.000000 napatrackmater-3.9.0/napatrackmater/version.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:03:27.453537 napatrackmater-3.9.0/napatrackmater.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 15:03:27.454534 napatrackmater-3.9.0/setup.cfg
--rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/setup.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:22:41.328906 napatrackmater-3.9.1/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 15:22:41.328796 napatrackmater-3.9.1/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:22:41.327789 napatrackmater-3.9.1/napatrackmater/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)   114228 2023-07-29 15:21:02.000000 napatrackmater-3.9.1/napatrackmater/Trackmate.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/napatrackmater/Trackvector.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/napatrackmater/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/napatrackmater/clustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/napatrackmater/fate_mapping.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/napatrackmater/pretrained.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 15:21:08.000000 napatrackmater-3.9.1/napatrackmater/version.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:22:41.328634 napatrackmater-3.9.1/napatrackmater.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 15:22:41.000000 napatrackmater-3.9.1/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 15:22:41.000000 napatrackmater-3.9.1/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 15:22:41.000000 napatrackmater-3.9.1/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 15:22:41.000000 napatrackmater-3.9.1/napatrackmater.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 15:22:41.000000 napatrackmater-3.9.1/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 15:22:41.000000 napatrackmater-3.9.1/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 15:22:41.328939 napatrackmater-3.9.1/setup.cfg
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-3.9.1/setup.py
```

### Comparing `napatrackmater-3.9.0/LICENSE` & `napatrackmater-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/PKG-INFO` & `napatrackmater-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.9.0
+Version: 3.9.1
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.9.0/README.md` & `napatrackmater-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.9.1/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.9.1/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/napatrackmater/Trackmate.py` & `napatrackmater-3.9.1/napatrackmater/Trackmate.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,32 +475,32 @@
 00001da0: 2020 2020 2020 2073 656c 662e 7370 6565         self.spee
 00001db0: 645f 6b65 7920 3d20 7365 6c66 2e74 7261  d_key = self.tra
 00001dc0: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
 00001dd0: 735f 6b65 7973 5b22 7370 6565 6422 5d0d  s_keys["speed"].
 00001de0: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
 00001df0: 7370 6c61 6365 6d65 6e74 5f6b 6579 203d  splacement_key =
 00001e00: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00001e10: 7973 6973 5f65 6467 6573 5f6b 6579 735b  ysis_edges_keys[
+00001e10: 7973 6973 5f74 7261 636b 5f6b 6579 735b  ysis_track_keys[
 00001e20: 2264 6973 706c 6163 656d 656e 7422 5d0d  "displacement"].
 00001e30: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
 00001e40: 7461 6c5f 7472 6163 6b5f 6469 7374 616e  tal_track_distan
 00001e50: 6365 5f6b 6579 203d 2073 656c 662e 7472  ce_key = self.tr
-00001e60: 6163 6b5f 616e 616c 7973 6973 5f65 6467  ack_analysis_edg
-00001e70: 6573 5f6b 6579 735b 2274 6f74 616c 5f74  es_keys["total_t
+00001e60: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
+00001e70: 636b 5f6b 6579 735b 2274 6f74 616c 5f74  ck_keys["total_t
 00001e80: 7261 636b 5f64 6973 7461 6e63 6522 5d0d  rack_distance"].
 00001e90: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
 00001ea0: 785f 6469 7374 616e 6365 5f74 7261 7665  x_distance_trave
 00001eb0: 6c65 645f 6b65 7920 3d20 7365 6c66 2e74  led_key = self.t
-00001ec0: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
-00001ed0: 6765 735f 6b65 7973 5b22 6d61 785f 7472  ges_keys["max_tr
+00001ec0: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
+00001ed0: 6163 6b5f 6b65 7973 5b22 6d61 785f 7472  ack_keys["max_tr
 00001ee0: 6163 6b5f 6469 7374 616e 6365 225d 0d0a  ack_distance"]..
 00001ef0: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
 00001f00: 636b 5f64 7572 6174 696f 6e5f 6b65 7920  ck_duration_key 
 00001f10: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
-00001f20: 6c79 7369 735f 6564 6765 735f 6b65 7973  lysis_edges_keys
+00001f20: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
 00001f30: 5b22 7472 6163 6b5f 6475 7261 7469 6f6e  ["track_duration
 00001f40: 225d 0d0a 2020 2020 2020 2020 0d0a 2020  "]..        ..  
 00001f50: 2020 2020 2020 7365 6c66 2e65 6467 655f        self.edge_
 00001f60: 7469 6d65 5f6b 6579 203d 2073 656c 662e  time_key = self.
 00001f70: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
 00001f80: 6467 6573 5f6b 6579 735b 2265 6467 655f  dges_keys["edge_
 00001f90: 7469 6d65 225d 0d0a 2020 2020 2020 2020  time"]..
```

### Comparing `napatrackmater-3.9.0/napatrackmater/Trackvector.py` & `napatrackmater-3.9.1/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/napatrackmater/__init__.py` & `napatrackmater-3.9.1/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/napatrackmater/clustering.py` & `napatrackmater-3.9.1/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.9.1/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/napatrackmater/fate_mapping.py` & `napatrackmater-3.9.1/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/napatrackmater/pretrained.py` & `napatrackmater-3.9.1/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.9.1/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.9.0
+Version: 3.9.1
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.9.0/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.9.1/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.0/setup.py` & `napatrackmater-3.9.1/setup.py`

 * *Files identical despite different names*

