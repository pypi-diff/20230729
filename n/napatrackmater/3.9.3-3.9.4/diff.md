# Comparing `tmp/napatrackmater-3.9.3.tar.gz` & `tmp/napatrackmater-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-3.9.3.tar", last modified: Sat Jul 29 16:04:00 2023, max compression
+gzip compressed data, was "napatrackmater-3.9.4.tar", last modified: Sat Jul 29 16:18:32 2023, max compression
```

## Comparing `napatrackmater-3.9.3.tar` & `napatrackmater-3.9.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:04:00.646534 napatrackmater-3.9.3/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 16:04:00.646434 napatrackmater-3.9.3/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:04:00.645413 napatrackmater-3.9.3/napatrackmater/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)   114170 2023-07-29 16:02:33.000000 napatrackmater-3.9.3/napatrackmater/Trackmate.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/Trackvector.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/clustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/fate_mapping.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/pretrained.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 16:02:40.000000 napatrackmater-3.9.3/napatrackmater/version.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:04:00.646270 napatrackmater-3.9.3/napatrackmater.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 16:04:00.646569 napatrackmater-3.9.3/setup.cfg
--rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/setup.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:18:32.719372 napatrackmater-3.9.4/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 16:18:32.719272 napatrackmater-3.9.4/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:18:32.718373 napatrackmater-3.9.4/napatrackmater/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)   114112 2023-07-29 16:17:26.000000 napatrackmater-3.9.4/napatrackmater/Trackmate.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/napatrackmater/Trackvector.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/napatrackmater/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/napatrackmater/clustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/napatrackmater/fate_mapping.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/napatrackmater/pretrained.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 16:17:29.000000 napatrackmater-3.9.4/napatrackmater/version.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:18:32.719130 napatrackmater-3.9.4/napatrackmater.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 16:18:32.000000 napatrackmater-3.9.4/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 16:18:32.000000 napatrackmater-3.9.4/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 16:18:32.000000 napatrackmater-3.9.4/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 16:18:32.000000 napatrackmater-3.9.4/napatrackmater.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 16:18:32.000000 napatrackmater-3.9.4/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 16:18:32.000000 napatrackmater-3.9.4/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 16:18:32.719403 napatrackmater-3.9.4/setup.cfg
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-3.9.4/setup.py
```

### Comparing `napatrackmater-3.9.3/LICENSE` & `napatrackmater-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/PKG-INFO` & `napatrackmater-3.9.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.9.3
+Version: 3.9.4
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.9.3/README.md` & `napatrackmater-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.9.4/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.9.4/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/napatrackmater/Trackmate.py` & `napatrackmater-3.9.4/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -6971,166 +6971,162 @@
 0001b3a0: 6964 203d 2074 7261 636b 5f61 6e61 6c79  id = track_analy
 0001b3b0: 7369 735f 7370 6f74 5f6b 6579 735b 2274  sis_spot_keys["t
 0001b3c0: 7261 636b 5f69 6422 5d0d 0a20 2020 2054  rack_id"]..    T
 0001b3d0: 6964 203d 2074 7261 636b 5f64 6174 6173  id = track_datas
 0001b3e0: 6574 5b74 7261 636b 5f69 645d 2e61 7374  et[track_id].ast
 0001b3f0: 7970 6528 2266 6c6f 6174 2229 0d0a 0d0a  ype("float")....
 0001b400: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
-0001b410: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
-0001b420: 7d0d 0a20 2020 2041 6c6c 5472 6163 6b56  }..    AllTrackV
-0001b430: 616c 7565 735b 7472 6163 6b5f 6964 5d5b  alues[track_id][
-0001b440: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
-0001b450: 786e 616d 655d 203d 2054 6964 0d0a 0d0a  xname] = Tid....
-0001b460: 2020 2020 666f 7220 286b 2c20 7629 2069      for (k, v) i
-0001b470: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
-0001b480: 5f74 7261 636b 5f6b 6579 732e 6974 656d  _track_keys.item
-0001b490: 7328 293a 0d0a 2020 2020 2020 2020 7820  s():..        x 
-0001b4a0: 3d20 7472 6163 6b5f 6461 7461 7365 745b  = track_dataset[
-0001b4b0: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
-0001b4c0: 2229 0d0a 2020 2020 2020 2020 6d69 6e76  ")..        minv
-0001b4d0: 616c 203d 206d 696e 2878 290d 0a20 2020  al = min(x)..   
-0001b4e0: 2020 2020 206d 6178 7661 6c20 3d20 6d61       maxval = ma
-0001b4f0: 7828 7829 0d0a 0d0a 2020 2020 2020 2020  x(x)....        
-0001b500: 6966 206d 696e 7661 6c20 3e20 3020 616e  if minval > 0 an
-0001b510: 6420 6d61 7876 616c 203c 3d20 313a 0d0a  d maxval <= 1:..
-0001b520: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-0001b530: 7820 2b20 310d 0a0d 0a20 2020 2020 2020  x + 1....       
-0001b540: 2041 6c6c 5472 6163 6b56 616c 7565 735b   AllTrackValues[
-0001b550: 7472 6163 6b5f 6964 5d5b 6b5d 203d 2072  track_id][k] = r
-0001b560: 6f75 6e64 2878 2c20 3329 0d0a 0d0a 2020  ound(x, 3)....  
-0001b570: 2020 5472 6163 6b41 7474 7269 6275 7465    TrackAttribute
-0001b580: 6964 7320 3d20 5b54 7261 636b 4174 7472  ids = [TrackAttr
-0001b590: 6962 7574 6542 6f78 6e61 6d65 5d20 2b20  ibuteBoxname] + 
-0001b5a0: 6c69 7374 2874 7261 636b 5f61 6e61 6c79  list(track_analy
-0001b5b0: 7369 735f 7472 6163 6b5f 6b65 7973 2e6b  sis_track_keys.k
-0001b5c0: 6579 7328 2929 0d0a 0d0a 2020 2020 7265  eys())....    re
-0001b5d0: 7475 726e 2054 7261 636b 4174 7472 6962  turn TrackAttrib
-0001b5e0: 7574 6569 6473 2c20 416c 6c54 7261 636b  uteids, AllTrack
-0001b5f0: 5661 6c75 6573 0d0a 2020 2020 0d0a 6465  Values..    ..de
-0001b600: 6620 6765 745f 6564 6765 735f 6461 7461  f get_edges_data
-0001b610: 7365 7428 6564 6765 735f 6461 7461 7365  set(edges_datase
-0001b620: 742c 2065 6467 6573 5f64 6174 6173 6574  t, edges_dataset
-0001b630: 5f69 6e64 6578 2c20 7472 6163 6b5f 616e  _index, track_an
-0001b640: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001b650: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
-0001b660: 5f65 6467 6573 5f6b 6579 7329 3a0d 0a0d  _edges_keys):...
-0001b670: 0a20 2020 2020 2020 2041 6c6c 4564 6765  .        AllEdge
-0001b680: 7356 616c 7565 7320 3d20 7b7d 0d0a 2020  sValues = {}..  
-0001b690: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
-0001b6a0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001b6b0: 7370 6f74 5f6b 6579 735b 2274 7261 636b  spot_keys["track
-0001b6c0: 5f69 6422 5d0d 0a20 2020 2020 2020 2054  _id"]..        T
-0001b6d0: 6964 203d 2065 6467 6573 5f64 6174 6173  id = edges_datas
-0001b6e0: 6574 5b74 7261 636b 5f69 645d 2e61 7374  et[track_id].ast
-0001b6f0: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
-0001b700: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-0001b710: 6e70 2e77 6865 7265 2854 6964 203d 3d20  np.where(Tid == 
-0001b720: 3029 0d0a 2020 2020 2020 2020 6d61 7874  0)..        maxt
-0001b730: 7261 636b 5f69 6420 3d20 6d61 7828 5469  rack_id = max(Ti
-0001b740: 6429 0d0a 2020 2020 2020 2020 636f 6e64  d)..        cond
-0001b750: 6974 696f 6e5f 696e 6469 6365 7320 3d20  ition_indices = 
-0001b760: 6564 6765 735f 6461 7461 7365 745f 696e  edges_dataset_in
-0001b770: 6465 785b 696e 6469 6365 735d 0d0a 2020  dex[indices]..  
-0001b780: 2020 2020 2020 5469 645b 636f 6e64 6974        Tid[condit
-0001b790: 696f 6e5f 696e 6469 6365 735d 203d 206d  ion_indices] = m
-0001b7a0: 6178 7472 6163 6b5f 6964 202b 2031 0d0a  axtrack_id + 1..
-0001b7b0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
-0001b7c0: 5661 6c75 6573 5b74 7261 636b 5f69 645d  Values[track_id]
-0001b7d0: 203d 2054 6964 0d0a 0d0a 2020 2020 2020   = Tid....      
-0001b7e0: 2020 666f 7220 6b20 696e 2074 7261 636b    for k in track
-0001b7f0: 5f61 6e61 6c79 7369 735f 6564 6765 735f  _analysis_edges_
-0001b800: 6b65 7973 2e76 616c 7565 7328 293a 0d0a  keys.values():..
-0001b810: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001b820: 206b 2021 3d20 7472 6163 6b5f 6964 3a0d   k != track_id:.
-0001b830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b840: 2078 203d 2065 6467 6573 5f64 6174 6173   x = edges_datas
-0001b850: 6574 5b6b 5d2e 6173 7479 7065 2822 666c  et[k].astype("fl
-0001b860: 6f61 7422 290d 0a0d 0a20 2020 2020 2020  oat")....       
-0001b870: 2020 2020 2020 2020 2041 6c6c 4564 6765           AllEdge
-0001b880: 7356 616c 7565 735b 6b5d 203d 2078 2020  sValues[k] = x  
-0001b890: 200d 0a20 2020 2020 2020 2020 0d0a 2020   ..         ..  
-0001b8a0: 2020 2020 2020 7265 7475 726e 2041 6c6c        return All
-0001b8b0: 4564 6765 7356 616c 7565 7320 2020 0d0a  EdgesValues   ..
-0001b8c0: 2020 2020 0d0a 2020 2020 2020 200d 0a20      ..       .. 
-0001b8d0: 2020 200d 0a64 6566 2073 6361 6c65 5f76     ..def scale_v
-0001b8e0: 616c 7565 2878 2c20 7363 616c 6520 3d20  alue(x, scale = 
-0001b8f0: 3235 3520 2a20 3235 3529 3a0d 0a0d 0a0d  255 * 255):.....
-0001b900: 0a20 2020 2020 7265 7475 726e 2078 202a  .     return x *
-0001b910: 2073 6361 6c65 2020 200d 0a20 2020 200d   scale   ..    .
-0001b920: 0a0d 0a0d 0a64 6566 2070 726f 625f 7369  .....def prob_si
-0001b930: 676d 6f69 6428 7829 3a0d 0a20 2020 2072  gmoid(x):..    r
-0001b940: 6574 7572 6e20 3120 2d20 6d61 7468 2e65  eturn 1 - math.e
-0001b950: 7870 282d 7829 0d0a 0d0a 0d0a 6465 6620  xp(-x)......def 
-0001b960: 616e 6775 6c61 725f 6368 616e 6765 2876  angular_change(v
-0001b970: 6563 5f30 2c20 7665 635f 3129 3a0d 0a20  ec_0, vec_1):.. 
-0001b980: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001b990: 2076 6563 5f30 203d 2076 6563 5f30 202f   vec_0 = vec_0 /
-0001b9a0: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
-0001b9b0: 7665 635f 3029 0d0a 2020 2020 2020 2020  vec_0)..        
-0001b9c0: 7665 635f 3120 3d20 7665 635f 3120 2f20  vec_1 = vec_1 / 
-0001b9d0: 6e70 2e6c 696e 616c 672e 6e6f 726d 2876  np.linalg.norm(v
-0001b9e0: 6563 5f31 290d 0a20 2020 2020 2020 2061  ec_1)..        a
-0001b9f0: 6e67 6c65 203d 206e 702e 6172 6363 6f73  ngle = np.arccos
-0001ba00: 286e 702e 636c 6970 286e 702e 646f 7428  (np.clip(np.dot(
-0001ba10: 7665 635f 302c 2076 6563 5f31 292c 202d  vec_0, vec_1), -
-0001ba20: 312e 302c 2031 2e30 2929 0d0a 2020 2020  1.0, 1.0))..    
-0001ba30: 2020 2020 616e 676c 6520 3d20 616e 676c      angle = angl
-0001ba40: 6520 2a20 3138 3020 2f20 6e70 2e70 690d  e * 180 / np.pi.
-0001ba50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001ba60: 616e 676c 650d 0a20 2020 2020 0d0a 0d0a  angle..     ....
-0001ba70: 6465 6620 6576 616c 5f62 6f6f 6c28 7661  def eval_bool(va
-0001ba80: 6c75 6529 3a0d 0a20 2020 2020 2020 2020  lue):..         
-0001ba90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0001baa0: 2020 2069 6620 7661 6c75 6520 203d 3d20     if value  == 
-0001bab0: 2754 7275 6527 3a20 0d0a 2020 2020 2020  'True': ..      
-0001bac0: 2020 2020 2020 2020 2020 6469 765f 6b65            div_ke
-0001bad0: 7920 3d20 5472 7565 0d0a 2020 2020 2020  y = True..      
-0001bae0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0001baf0: 2020 2020 2020 2020 2064 6976 5f6b 6579           div_key
-0001bb00: 203d 2046 616c 7365 200d 0a0d 0a20 2020   = False ....   
-0001bb10: 2020 2020 2072 6574 7572 6e20 6469 765f       return div_
-0001bb20: 6b65 7920 2020 2020 2020 2020 2020 2020  key             
-0001bb30: 2020 200d 0a0d 0a64 6566 2063 6865 636b     ....def check
-0001bb40: 5f61 6e64 5f75 7064 6174 655f 6d61 736b  _and_update_mask
-0001bb50: 286d 6173 6b2c 696d 6167 6529 3a0d 0a20  (mask,image):.. 
-0001bb60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001bb70: 6966 206c 656e 286d 6173 6b2e 7368 6170  if len(mask.shap
-0001bb80: 6529 203c 206c 656e 2869 6d61 6765 2e73  e) < len(image.s
-0001bb90: 6861 7065 293a 0d0a 2020 2020 2020 2020  hape):..        
-0001bba0: 2020 2020 7570 6461 7465 5f6d 6173 6b20      update_mask 
-0001bbb0: 3d20 6e70 2e7a 6572 6f73 280d 0a20 2020  = np.zeros(..   
-0001bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbd0: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
+0001b410: 6573 5b74 7261 636b 5f69 645d 203d 2054  es[track_id] = T
+0001b420: 6964 0d0a 0d0a 2020 2020 666f 7220 286b  id....    for (k
+0001b430: 2c20 7629 2069 6e20 7472 6163 6b5f 616e  , v) in track_an
+0001b440: 616c 7973 6973 5f74 7261 636b 5f6b 6579  alysis_track_key
+0001b450: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
+0001b460: 2020 2020 7820 3d20 7472 6163 6b5f 6461      x = track_da
+0001b470: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
+0001b480: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+0001b490: 2020 6d69 6e76 616c 203d 206d 696e 2878    minval = min(x
+0001b4a0: 290d 0a20 2020 2020 2020 206d 6178 7661  )..        maxva
+0001b4b0: 6c20 3d20 6d61 7828 7829 0d0a 0d0a 2020  l = max(x)....  
+0001b4c0: 2020 2020 2020 6966 206d 696e 7661 6c20        if minval 
+0001b4d0: 3e20 3020 616e 6420 6d61 7876 616c 203c  > 0 and maxval <
+0001b4e0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+0001b4f0: 2020 7820 3d20 7820 2b20 310d 0a0d 0a20    x = x + 1.... 
+0001b500: 2020 2020 2020 2041 6c6c 5472 6163 6b56         AllTrackV
+0001b510: 616c 7565 735b 7472 6163 6b5f 6964 5d5b  alues[track_id][
+0001b520: 6b5d 203d 2072 6f75 6e64 2878 2c20 3329  k] = round(x, 3)
+0001b530: 0d0a 0d0a 2020 2020 5472 6163 6b41 7474  ....    TrackAtt
+0001b540: 7269 6275 7465 6964 7320 3d20 5b54 7261  ributeids = [Tra
+0001b550: 636b 4174 7472 6962 7574 6542 6f78 6e61  ckAttributeBoxna
+0001b560: 6d65 5d20 2b20 6c69 7374 2874 7261 636b  me] + list(track
+0001b570: 5f61 6e61 6c79 7369 735f 7472 6163 6b5f  _analysis_track_
+0001b580: 6b65 7973 2e6b 6579 7328 2929 0d0a 0d0a  keys.keys())....
+0001b590: 2020 2020 7265 7475 726e 2054 7261 636b      return Track
+0001b5a0: 4174 7472 6962 7574 6569 6473 2c20 416c  Attributeids, Al
+0001b5b0: 6c54 7261 636b 5661 6c75 6573 0d0a 2020  lTrackValues..  
+0001b5c0: 2020 0d0a 6465 6620 6765 745f 6564 6765    ..def get_edge
+0001b5d0: 735f 6461 7461 7365 7428 6564 6765 735f  s_dataset(edges_
+0001b5e0: 6461 7461 7365 742c 2065 6467 6573 5f64  dataset, edges_d
+0001b5f0: 6174 6173 6574 5f69 6e64 6578 2c20 7472  ataset_index, tr
+0001b600: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+0001b610: 745f 6b65 7973 2c20 7472 6163 6b5f 616e  t_keys, track_an
+0001b620: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
+0001b630: 7329 3a0d 0a0d 0a20 2020 2020 2020 2041  s):....        A
+0001b640: 6c6c 4564 6765 7356 616c 7565 7320 3d20  llEdgesValues = 
+0001b650: 7b7d 0d0a 2020 2020 2020 2020 7472 6163  {}..        trac
+0001b660: 6b5f 6964 203d 2074 7261 636b 5f61 6e61  k_id = track_ana
+0001b670: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+0001b680: 2274 7261 636b 5f69 6422 5d0d 0a20 2020  "track_id"]..   
+0001b690: 2020 2020 2054 6964 203d 2065 6467 6573       Tid = edges
+0001b6a0: 5f64 6174 6173 6574 5b74 7261 636b 5f69  _dataset[track_i
+0001b6b0: 645d 2e61 7374 7970 6528 2266 6c6f 6174  d].astype("float
+0001b6c0: 2229 0d0a 2020 2020 2020 2020 696e 6469  ")..        indi
+0001b6d0: 6365 7320 3d20 6e70 2e77 6865 7265 2854  ces = np.where(T
+0001b6e0: 6964 203d 3d20 3029 0d0a 2020 2020 2020  id == 0)..      
+0001b6f0: 2020 6d61 7874 7261 636b 5f69 6420 3d20    maxtrack_id = 
+0001b700: 6d61 7828 5469 6429 0d0a 2020 2020 2020  max(Tid)..      
+0001b710: 2020 636f 6e64 6974 696f 6e5f 696e 6469    condition_indi
+0001b720: 6365 7320 3d20 6564 6765 735f 6461 7461  ces = edges_data
+0001b730: 7365 745f 696e 6465 785b 696e 6469 6365  set_index[indice
+0001b740: 735d 0d0a 2020 2020 2020 2020 5469 645b  s]..        Tid[
+0001b750: 636f 6e64 6974 696f 6e5f 696e 6469 6365  condition_indice
+0001b760: 735d 203d 206d 6178 7472 6163 6b5f 6964  s] = maxtrack_id
+0001b770: 202b 2031 0d0a 2020 2020 2020 2020 416c   + 1..        Al
+0001b780: 6c45 6467 6573 5661 6c75 6573 5b74 7261  lEdgesValues[tra
+0001b790: 636b 5f69 645d 203d 2054 6964 0d0a 0d0a  ck_id] = Tid....
+0001b7a0: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
+0001b7b0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001b7c0: 6564 6765 735f 6b65 7973 2e76 616c 7565  edges_keys.value
+0001b7d0: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
+0001b7e0: 2020 2020 6966 206b 2021 3d20 7472 6163      if k != trac
+0001b7f0: 6b5f 6964 3a0d 0a20 2020 2020 2020 2020  k_id:..         
+0001b800: 2020 2020 2020 2078 203d 2065 6467 6573         x = edges
+0001b810: 5f64 6174 6173 6574 5b6b 5d2e 6173 7479  _dataset[k].asty
+0001b820: 7065 2822 666c 6f61 7422 290d 0a0d 0a20  pe("float").... 
+0001b830: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0001b840: 6c6c 4564 6765 7356 616c 7565 735b 6b5d  llEdgesValues[k]
+0001b850: 203d 2078 2020 200d 0a20 2020 2020 2020   = x   ..       
+0001b860: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
+0001b870: 726e 2041 6c6c 4564 6765 7356 616c 7565  rn AllEdgesValue
+0001b880: 7320 2020 0d0a 2020 2020 0d0a 2020 2020  s   ..    ..    
+0001b890: 2020 200d 0a20 2020 200d 0a64 6566 2073     ..    ..def s
+0001b8a0: 6361 6c65 5f76 616c 7565 2878 2c20 7363  cale_value(x, sc
+0001b8b0: 616c 6520 3d20 3235 3520 2a20 3235 3529  ale = 255 * 255)
+0001b8c0: 3a0d 0a0d 0a0d 0a20 2020 2020 7265 7475  :......     retu
+0001b8d0: 726e 2078 202a 2073 6361 6c65 2020 200d  rn x * scale   .
+0001b8e0: 0a20 2020 200d 0a0d 0a0d 0a64 6566 2070  .    ......def p
+0001b8f0: 726f 625f 7369 676d 6f69 6428 7829 3a0d  rob_sigmoid(x):.
+0001b900: 0a20 2020 2072 6574 7572 6e20 3120 2d20  .    return 1 - 
+0001b910: 6d61 7468 2e65 7870 282d 7829 0d0a 0d0a  math.exp(-x)....
+0001b920: 0d0a 6465 6620 616e 6775 6c61 725f 6368  ..def angular_ch
+0001b930: 616e 6765 2876 6563 5f30 2c20 7665 635f  ange(vec_0, vec_
+0001b940: 3129 3a0d 0a20 2020 2020 2020 200d 0a20  1):..        .. 
+0001b950: 2020 2020 2020 2076 6563 5f30 203d 2076         vec_0 = v
+0001b960: 6563 5f30 202f 206e 702e 6c69 6e61 6c67  ec_0 / np.linalg
+0001b970: 2e6e 6f72 6d28 7665 635f 3029 0d0a 2020  .norm(vec_0)..  
+0001b980: 2020 2020 2020 7665 635f 3120 3d20 7665        vec_1 = ve
+0001b990: 635f 3120 2f20 6e70 2e6c 696e 616c 672e  c_1 / np.linalg.
+0001b9a0: 6e6f 726d 2876 6563 5f31 290d 0a20 2020  norm(vec_1)..   
+0001b9b0: 2020 2020 2061 6e67 6c65 203d 206e 702e       angle = np.
+0001b9c0: 6172 6363 6f73 286e 702e 636c 6970 286e  arccos(np.clip(n
+0001b9d0: 702e 646f 7428 7665 635f 302c 2076 6563  p.dot(vec_0, vec
+0001b9e0: 5f31 292c 202d 312e 302c 2031 2e30 2929  _1), -1.0, 1.0))
+0001b9f0: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
+0001ba00: 3d20 616e 676c 6520 2a20 3138 3020 2f20  = angle * 180 / 
+0001ba10: 6e70 2e70 690d 0a20 2020 2020 2020 2072  np.pi..        r
+0001ba20: 6574 7572 6e20 616e 676c 650d 0a20 2020  eturn angle..   
+0001ba30: 2020 0d0a 0d0a 6465 6620 6576 616c 5f62    ....def eval_b
+0001ba40: 6f6f 6c28 7661 6c75 6529 3a0d 0a20 2020  ool(value):..   
+0001ba50: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0001ba60: 0a20 2020 2020 2020 2069 6620 7661 6c75  .        if valu
+0001ba70: 6520 203d 3d20 2754 7275 6527 3a20 0d0a  e  == 'True': ..
+0001ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba90: 6469 765f 6b65 7920 3d20 5472 7565 0d0a  div_key = True..
+0001baa0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0001bab0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001bac0: 6976 5f6b 6579 203d 2046 616c 7365 200d  iv_key = False .
+0001bad0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+0001bae0: 6e20 6469 765f 6b65 7920 2020 2020 2020  n div_key       
+0001baf0: 2020 2020 2020 2020 200d 0a0d 0a64 6566           ....def
+0001bb00: 2063 6865 636b 5f61 6e64 5f75 7064 6174   check_and_updat
+0001bb10: 655f 6d61 736b 286d 6173 6b2c 696d 6167  e_mask(mask,imag
+0001bb20: 6529 3a0d 0a20 2020 2020 2020 0d0a 2020  e):..       ..  
+0001bb30: 2020 2020 2020 6966 206c 656e 286d 6173        if len(mas
+0001bb40: 6b2e 7368 6170 6529 203c 206c 656e 2869  k.shape) < len(i
+0001bb50: 6d61 6765 2e73 6861 7065 293a 0d0a 2020  mage.shape):..  
+0001bb60: 2020 2020 2020 2020 2020 7570 6461 7465            update
+0001bb70: 5f6d 6173 6b20 3d20 6e70 2e7a 6572 6f73  _mask = np.zeros
+0001bb80: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001bb90: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0001bba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbc0: 2020 696d 6167 652e 7368 6170 655b 305d    image.shape[0]
+0001bbd0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 0001bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbf0: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-0001bc00: 652e 7368 6170 655b 305d 2c0d 0a20 2020  e.shape[0],..   
+0001bbf0: 2020 2069 6d61 6765 2e73 6861 7065 5b31     image.shape[1
+0001bc00: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
 0001bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc20: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-0001bc30: 6765 2e73 6861 7065 5b31 5d2c 0d0a 2020  ge.shape[1],..  
+0001bc20: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
+0001bc30: 325d 2c0d 0a20 2020 2020 2020 2020 2020  2],..           
 0001bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc50: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0001bc60: 6167 652e 7368 6170 655b 325d 2c0d 0a20  age.shape[2],.. 
+0001bc50: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
+0001bc60: 5b33 5d2c 0d0a 2020 2020 2020 2020 2020  [3],..          
 0001bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001bc90: 6d61 6765 2e73 6861 7065 5b33 5d2c 0d0a  mage.shape[3],..
-0001bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcb0: 2020 2020 2020 2020 2020 2020 5d2c 2064              ], d
-0001bcc0: 7479 7065 3d22 7569 6e74 3822 0d0a 2020  type="uint8"..  
-0001bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bce0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001bcf0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+0001bc80: 2020 5d2c 2064 7479 7065 3d22 7569 6e74    ], dtype="uint
+0001bc90: 3822 0d0a 2020 2020 2020 2020 2020 2020  8"..            
+0001bca0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+0001bcb0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0001bcc0: 2069 6e20 7261 6e67 6528 302c 2075 7064   in range(0, upd
+0001bcd0: 6174 655f 6d61 736b 2e73 6861 7065 5b30  ate_mask.shape[0
+0001bce0: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
+0001bcf0: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
 0001bd00: 6e67 6528 302c 2075 7064 6174 655f 6d61  nge(0, update_ma
-0001bd10: 736b 2e73 6861 7065 5b30 5d29 3a0d 0a20  sk.shape[0]):.. 
-0001bd20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001bd30: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-0001bd40: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
-0001bd50: 7065 5b31 5d29 3a0d 0a0d 0a20 2020 2020  pe[1]):....     
-0001bd60: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0001bd70: 7064 6174 655f 6d61 736b 5b69 2c20 6a2c  pdate_mask[i, j,
-0001bd80: 203a 2c20 3a5d 203d 206d 6173 6b5b 692c   :, :] = mask[i,
-0001bd90: 203a 2c20 3a5d 0d0a 2020 2020 2020 2020   :, :]..        
-0001bda0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0001bdb0: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
-0001bdc0: 736b 203d 206d 6173 6b0d 0a0d 0a20 2020  sk = mask....   
-0001bdd0: 2020 2020 2072 6574 7572 6e20 7570 6461       return upda
-0001bde0: 7465 5f6d 6173 6b20 2020 2020 2020 200d  te_mask        .
-0001bdf0: 0a20 2020 2020 2020 0d0a                 .       ..
+0001bd10: 736b 2e73 6861 7065 5b31 5d29 3a0d 0a0d  sk.shape[1]):...
+0001bd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bd30: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
+0001bd40: 5b69 2c20 6a2c 203a 2c20 3a5d 203d 206d  [i, j, :, :] = m
+0001bd50: 6173 6b5b 692c 203a 2c20 3a5d 0d0a 2020  ask[i, :, :]..  
+0001bd60: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0001bd70: 2020 2020 2020 2020 2020 2020 2075 7064               upd
+0001bd80: 6174 655f 6d61 736b 203d 206d 6173 6b0d  ate_mask = mask.
+0001bd90: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+0001bda0: 6e20 7570 6461 7465 5f6d 6173 6b20 2020  n update_mask   
+0001bdb0: 2020 2020 200d 0a20 2020 2020 2020 0d0a       ..       ..
```

### Comparing `napatrackmater-3.9.3/napatrackmater/Trackvector.py` & `napatrackmater-3.9.4/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/napatrackmater/__init__.py` & `napatrackmater-3.9.4/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/napatrackmater/clustering.py` & `napatrackmater-3.9.4/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.9.4/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/napatrackmater/fate_mapping.py` & `napatrackmater-3.9.4/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/napatrackmater/pretrained.py` & `napatrackmater-3.9.4/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.9.4/napatrackmater.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.9.3
+Version: 3.9.4
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.9.3/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.9.4/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.3/setup.py` & `napatrackmater-3.9.4/setup.py`

 * *Files identical despite different names*

